# Comparing `tmp/oblv_ctl-0.3.1.tar.gz` & `tmp/oblv_ctl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oblv_ctl-0.3.1.tar", max compression
+gzip compressed data, was "oblv_ctl-0.4.1.tar", max compression
```

## Comparing `oblv_ctl-0.3.1.tar` & `oblv_ctl-0.4.1.tar`

### file list

```diff
@@ -1,99 +1,147 @@
--rw-r--r--   0        0        0    11558 2023-01-05 11:33:47.193634 oblv_ctl-0.3.1/LICENSE
--rw-r--r--   0        0        0       94 2023-05-04 07:16:41.170094 oblv_ctl-0.3.1/oblv_ctl/__init__.py
--rw-r--r--   0        0        0       48 2023-05-02 04:48:50.842284 oblv_ctl-0.3.1/oblv_ctl/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.843282 oblv_ctl-0.3.1/oblv_ctl/api/account/__init__.py
--rw-r--r--   0        0        0     5146 2023-05-02 04:48:50.843282 oblv_ctl-0.3.1/oblv_ctl/api/account/get_user_accounts_account_get.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.843282 oblv_ctl-0.3.1/oblv_ctl/api/auth/__init__.py
--rw-r--r--   0        0        0     5029 2023-05-02 04:48:50.844282 oblv_ctl-0.3.1/oblv_ctl/api/auth/authenticate_key_login_apikey_post.py
--rw-r--r--   0        0        0     5004 2023-05-02 04:48:50.844282 oblv_ctl-0.3.1/oblv_ctl/api/auth/logout_session_logout_delete.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.844282 oblv_ctl-0.3.1/oblv_ctl/api/deployment/__init__.py
--rw-r--r--   0        0        0     5735 2023-05-02 04:48:50.845281 oblv_ctl-0.3.1/oblv_ctl/api/deployment/create_new_deployment_deployment_post.py
--rw-r--r--   0        0        0     5233 2023-05-02 04:48:50.846280 oblv_ctl-0.3.1/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py
--rw-r--r--   0        0        0     8308 2023-05-02 04:48:50.846280 oblv_ctl-0.3.1/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py
--rw-r--r--   0        0        0     6874 2023-05-02 04:48:50.846280 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_available_deployments_deployment_available_get.py
--rw-r--r--   0        0        0     5302 2023-05-02 04:48:50.847281 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py
--rw-r--r--   0        0        0     5623 2023-05-02 04:48:50.847281 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_roles_deployment_roles_get.py
--rw-r--r--   0        0        0     3227 2023-05-02 04:48:50.848284 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_supported_regions_deployment_supported_regions_get.py
--rw-r--r--   0        0        0     6724 2023-05-02 04:48:50.848284 oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_user_owned_deployments_deployment_owned_get.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.849283 oblv_ctl-0.3.1/oblv_ctl/api/notification/__init__.py
--rw-r--r--   0        0        0     5145 2023-05-02 04:48:50.849283 oblv_ctl-0.3.1/oblv_ctl/api/notification/get_all_notifications_notification_get.py
--rw-r--r--   0        0        0     5110 2023-05-02 04:48:50.850283 oblv_ctl-0.3.1/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py
--rw-r--r--   0        0        0     4484 2023-05-02 04:48:50.850283 oblv_ctl-0.3.1/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py
--rw-r--r--   0        0        0     4954 2023-05-02 04:48:50.851281 oblv_ctl-0.3.1/oblv_ctl/api/notification/mark_notification_read_notification_notification_id_delete.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.851281 oblv_ctl-0.3.1/oblv_ctl/api/repo/__init__.py
--rw-r--r--   0        0        0     5202 2023-05-02 04:48:50.852280 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_all_repos_repo_linked_get.py
--rw-r--r--   0        0        0     6198 2023-05-02 04:48:50.852280 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py
--rw-r--r--   0        0        0     7756 2023-05-02 04:48:50.852280 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py
--rw-r--r--   0        0        0     6065 2023-05-02 04:48:50.853281 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_id_get.py
--rw-r--r--   0        0        0     6245 2023-05-02 04:48:50.853281 oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py
--rw-r--r--   0        0        0     5907 2023-05-02 04:48:50.854282 oblv_ctl-0.3.1/oblv_ctl/api/repo/search_repo_from_vcs_repo_search_get.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.854282 oblv_ctl-0.3.1/oblv_ctl/api/service/__init__.py
--rw-r--r--   0        0        0     8037 2023-05-02 04:48:50.854282 oblv_ctl-0.3.1/oblv_ctl/api/service/add_repo_service_repo_service_post.py
--rw-r--r--   0        0        0     7266 2023-05-02 04:48:50.855280 oblv_ctl-0.3.1/oblv_ctl/api/service/delete_repo_services_repo_service_delete.py
--rw-r--r--   0        0        0     7513 2023-05-02 04:48:50.855280 oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py
--rw-r--r--   0        0        0     8367 2023-05-02 04:48:50.856281 oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_services_repo_service_get.py
--rw-r--r--   0        0        0     7166 2023-05-02 04:48:50.856281 oblv_ctl-0.3.1/oblv_ctl/api/service/get_user_services_service_get.py
--rw-r--r--   0        0        0     8539 2023-05-02 04:48:50.857280 oblv_ctl-0.3.1/oblv_ctl/api/service/update_repo_service_repo_service_put.py
--rw-r--r--   0        0        0     8369 2023-05-02 04:48:50.857280 oblv_ctl-0.3.1/oblv_ctl/api/service/validate_repo_service_repo_service_validate_get.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.857280 oblv_ctl-0.3.1/oblv_ctl/api/user/__init__.py
--rw-r--r--   0        0        0     4991 2023-05-02 04:48:50.858280 oblv_ctl-0.3.1/oblv_ctl/api/user/add_user_public_shared_key_user_psk_put.py
--rw-r--r--   0        0        0     4913 2023-05-02 04:48:50.858280 oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py
--rw-r--r--   0        0        0     4874 2023-05-02 04:48:50.859281 oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_profile_view_user_profile_get.py
--rw-r--r--   0        0        0     4888 2023-05-02 04:48:50.859281 oblv_ctl-0.3.1/oblv_ctl/api/user/get_user_public_shared_key_user_psk_get.py
--rw-r--r--   0        0        0     5013 2023-05-02 04:48:50.859281 oblv_ctl-0.3.1/oblv_ctl/api/user/update_user_name_user_name_put.py
--rw-r--r--   0        0        0     5150 2023-05-02 04:48:50.860280 oblv_ctl-0.3.1/oblv_ctl/api/user/update_user_password_user_password_put.py
--rw-r--r--   0        0        0      389 2023-05-02 05:12:33.359116 oblv_ctl-0.3.1/oblv_ctl/auth.py
--rw-r--r--   0        0        0        0 2023-05-02 04:48:50.864283 oblv_ctl-0.3.1/oblv_ctl/cli/__init__.py
--rw-r--r--   0        0        0     4910 2023-05-04 10:47:47.198954 oblv_ctl-0.3.1/oblv_ctl/cli/deployment.py
--rw-r--r--   0        0        0     2873 2023-05-04 10:47:47.198954 oblv_ctl-0.3.1/oblv_ctl/cli/main.py
--rw-r--r--   0        0        0     4079 2023-05-04 10:47:47.194954 oblv_ctl-0.3.1/oblv_ctl/cli/service.py
--rw-r--r--   0        0        0     1775 2023-05-04 10:47:47.198954 oblv_ctl-0.3.1/oblv_ctl/cli/utils.py
--rw-r--r--   0        0        0     1885 2023-05-02 04:48:50.878886 oblv_ctl-0.3.1/oblv_ctl/client.py
--rw-r--r--   0        0        0       30 2023-05-02 04:48:50.879888 oblv_ctl-0.3.1/oblv_ctl/config.py
--rw-r--r--   0        0        0     4219 2023-05-04 09:07:09.223713 oblv_ctl-0.3.1/oblv_ctl/exceptions.py
--rw-r--r--   0        0        0     1573 2023-05-02 04:48:50.880884 oblv_ctl-0.3.1/oblv_ctl/models/__init__.py
--rw-r--r--   0        0        0     2611 2023-05-02 04:48:50.881916 oblv_ctl-0.3.1/oblv_ctl/models/access_history.py
--rw-r--r--   0        0        0     2326 2023-05-02 04:48:50.881916 oblv_ctl-0.3.1/oblv_ctl/models/account.py
--rw-r--r--   0        0        0     1533 2023-05-02 04:48:50.881916 oblv_ctl-0.3.1/oblv_ctl/models/api_key.py
--rw-r--r--   0        0        0     1979 2023-05-02 04:48:50.882919 oblv_ctl-0.3.1/oblv_ctl/models/available_deployment.py
--rw-r--r--   0        0        0     2395 2023-05-02 04:48:50.883916 oblv_ctl-0.3.1/oblv_ctl/models/available_deployment_list.py
--rw-r--r--   0        0        0     1975 2023-05-02 04:48:50.883916 oblv_ctl-0.3.1/oblv_ctl/models/build_args_schema.py
--rw-r--r--   0        0        0     4051 2023-05-02 04:48:50.883916 oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_input.py
--rw-r--r--   0        0        0     2108 2023-05-02 04:48:50.884917 oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_response.py
--rw-r--r--   0        0        0    10161 2023-05-02 04:48:50.884917 oblv_ctl-0.3.1/oblv_ctl/models/deployment_complete.py
--rw-r--r--   0        0        0     2342 2023-05-02 04:48:50.885915 oblv_ctl-0.3.1/oblv_ctl/models/deployment_list.py
--rw-r--r--   0        0        0     8783 2023-05-02 04:48:50.885915 oblv_ctl-0.3.1/oblv_ctl/models/deployment_response.py
--rw-r--r--   0        0        0     2251 2023-05-02 04:48:50.885915 oblv_ctl-0.3.1/oblv_ctl/models/http_validation_error.py
--rw-r--r--   0        0        0     3419 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/instance.py
--rw-r--r--   0        0        0     1704 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/message_model.py
--rw-r--r--   0        0        0     1656 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/name_input.py
--rw-r--r--   0        0        0     3066 2023-05-02 04:48:50.886916 oblv_ctl-0.3.1/oblv_ctl/models/notification_response.py
--rw-r--r--   0        0        0     1980 2023-05-02 04:48:50.887915 oblv_ctl-0.3.1/oblv_ctl/models/oblv_auth_response.py
--rw-r--r--   0        0        0     1585 2023-05-02 04:48:50.887915 oblv_ctl-0.3.1/oblv_ctl/models/psk.py
--rw-r--r--   0        0        0     2172 2023-05-02 04:48:50.887915 oblv_ctl-0.3.1/oblv_ctl/models/ref_response.py
--rw-r--r--   0        0        0     4997 2023-05-02 04:48:50.888915 oblv_ctl-0.3.1/oblv_ctl/models/repo.py
--rw-r--r--   0        0        0     2338 2023-05-02 04:48:50.888915 oblv_ctl-0.3.1/oblv_ctl/models/repo_all_response.py
--rw-r--r--   0        0        0     2319 2023-05-02 04:48:50.889915 oblv_ctl-0.3.1/oblv_ctl/models/repo_service_list.py
--rw-r--r--   0        0        0     5571 2023-05-02 04:48:50.889915 oblv_ctl-0.3.1/oblv_ctl/models/repo_services.py
--rw-r--r--   0        0        0     2100 2023-05-02 04:48:50.890916 oblv_ctl-0.3.1/oblv_ctl/models/role_response.py
--rw-r--r--   0        0        0     1407 2023-05-02 04:48:50.890916 oblv_ctl-0.3.1/oblv_ctl/models/service_content_response.py
--rw-r--r--   0        0        0     2432 2023-05-02 04:48:50.890916 oblv_ctl-0.3.1/oblv_ctl/models/service_validation_response.py
--rw-r--r--   0        0        0     1395 2023-05-02 04:48:50.891916 oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_add_input.py
--rw-r--r--   0        0        0     1410 2023-05-02 04:48:50.891916 oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_update_input.py
--rw-r--r--   0        0        0     2682 2023-05-02 04:48:50.892915 oblv_ctl-0.3.1/oblv_ctl/models/shared_users.py
--rw-r--r--   0        0        0     1374 2023-05-02 04:48:50.892915 oblv_ctl-0.3.1/oblv_ctl/models/supported_regions.py
--rw-r--r--   0        0        0     3177 2023-05-02 04:48:50.892915 oblv_ctl-0.3.1/oblv_ctl/models/user_credit_utilization.py
--rw-r--r--   0        0        0     1870 2023-05-02 04:48:50.893915 oblv_ctl-0.3.1/oblv_ctl/models/user_password_input.py
--rw-r--r--   0        0        0     2688 2023-05-02 04:48:50.893915 oblv_ctl-0.3.1/oblv_ctl/models/user_profile_response.py
--rw-r--r--   0        0        0     2291 2023-05-02 04:48:50.893915 oblv_ctl-0.3.1/oblv_ctl/models/user_service_list.py
--rw-r--r--   0        0        0     3444 2023-05-02 04:48:50.894916 oblv_ctl-0.3.1/oblv_ctl/models/user_services.py
--rw-r--r--   0        0        0     2544 2023-05-02 04:48:50.894916 oblv_ctl-0.3.1/oblv_ctl/models/validated_service.py
--rw-r--r--   0        0        0     1903 2023-05-02 04:48:50.895916 oblv_ctl-0.3.1/oblv_ctl/models/validation_error.py
--rw-r--r--   0        0        0     2731 2023-05-02 04:48:50.895916 oblv_ctl-0.3.1/oblv_ctl/models/vcs_repo_response.py
--rw-r--r--   0        0        0    21623 2023-05-04 10:26:44.709977 oblv_ctl-0.3.1/oblv_ctl/oblv_client.py
--rw-r--r--   0        0        0       25 2023-05-02 04:48:50.900915 oblv_ctl-0.3.1/oblv_ctl/py.typed
--rw-r--r--   0        0        0      982 2023-05-02 04:48:50.901917 oblv_ctl-0.3.1/oblv_ctl/types.py
--rw-r--r--   0        0        0     1283 2023-05-02 04:48:50.901917 oblv_ctl-0.3.1/oblv_ctl/utils.py
--rw-r--r--   0        0        0      750 2023-05-04 10:15:25.127725 oblv_ctl-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6661 2023-05-02 05:12:37.943952 oblv_ctl-0.3.1/README.md
--rw-r--r--   0        0        0     7459 1970-01-01 00:00:00.000000 oblv_ctl-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-01-05 11:33:47.193634 oblv_ctl-0.4.1/LICENSE
+-rw-r--r--   0        0        0       94 2023-06-15 10:31:33.248468 oblv_ctl-0.4.1/oblv_ctl/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-09 07:31:18.220909 oblv_ctl-0.4.1/oblv_ctl/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.225674 oblv_ctl-0.4.1/oblv_ctl/api/account/__init__.py
+-rw-r--r--   0        0        0     6614 2023-06-15 10:30:41.292812 oblv_ctl-0.4.1/oblv_ctl/api/account/get_user_accounts_account_get.py
+-rw-r--r--   0        0        0     6075 2023-06-15 10:30:41.299508 oblv_ctl-0.4.1/oblv_ctl/api/account/get_user_accounts_user_account_get.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:30:41.302060 oblv_ctl-0.4.1/oblv_ctl/api/additional/__init__.py
+-rw-r--r--   0        0        0     2036 2023-06-15 10:30:41.309059 oblv_ctl-0.4.1/oblv_ctl/api/additional/get_sample_service_content_sample_service_get.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.243756 oblv_ctl-0.4.1/oblv_ctl/api/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-06-15 10:30:41.315288 oblv_ctl-0.4.1/oblv_ctl/api/auth/authenticate_key_login_apikey_post.py
+-rw-r--r--   0        0        0     5876 2023-06-15 10:30:41.321751 oblv_ctl-0.4.1/oblv_ctl/api/auth/logout_session_logout_delete.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.261875 oblv_ctl-0.4.1/oblv_ctl/api/deployment/__init__.py
+-rw-r--r--   0        0        0     6142 2023-06-15 10:30:41.327362 oblv_ctl-0.4.1/oblv_ctl/api/deployment/add_deployment_tag_deployment_deployment_id_tag_post.py
+-rw-r--r--   0        0        0     6607 2023-06-15 10:30:41.334009 oblv_ctl-0.4.1/oblv_ctl/api/deployment/create_new_deployment_deployment_post.py
+-rw-r--r--   0        0        0     6614 2023-06-15 10:30:41.340557 oblv_ctl-0.4.1/oblv_ctl/api/deployment/create_new_deployment_deployment_static_post.py
+-rw-r--r--   0        0        0     6105 2023-06-15 10:30:41.347155 oblv_ctl-0.4.1/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py
+-rw-r--r--   0        0        0     9555 2023-06-15 10:30:41.355338 oblv_ctl-0.4.1/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py
+-rw-r--r--   0        0        0     7746 2023-06-15 10:30:41.361765 oblv_ctl-0.4.1/oblv_ctl/api/deployment/get_available_deployments_deployment_available_get.py
+-rw-r--r--   0        0        0     6169 2023-06-15 10:30:41.367351 oblv_ctl-0.4.1/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py
+-rw-r--r--   0        0        0     6515 2023-06-15 10:30:41.374406 oblv_ctl-0.4.1/oblv_ctl/api/deployment/get_deployment_roles_deployment_roles_get.py
+-rw-r--r--   0        0        0     3511 2023-06-15 10:30:41.381506 oblv_ctl-0.4.1/oblv_ctl/api/deployment/get_supported_regions_deployment_supported_regions_get.py
+-rw-r--r--   0        0        0     7702 2023-06-15 10:30:41.393648 oblv_ctl-0.4.1/oblv_ctl/api/deployment/get_user_owned_deployments_deployment_owned_get.py
+-rw-r--r--   0        0        0     6164 2023-06-15 10:30:41.400271 oblv_ctl-0.4.1/oblv_ctl/api/deployment/remove_deployment_tag_deployment_deployment_id_tag_delete.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.327579 oblv_ctl-0.4.1/oblv_ctl/api/notification/__init__.py
+-rw-r--r--   0        0        0     6037 2023-06-15 10:30:41.408327 oblv_ctl-0.4.1/oblv_ctl/api/notification/get_all_notifications_notification_get.py
+-rw-r--r--   0        0        0     5982 2023-06-15 10:30:41.415713 oblv_ctl-0.4.1/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py
+-rw-r--r--   0        0        0     5351 2023-06-15 10:30:41.425050 oblv_ctl-0.4.1/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py
+-rw-r--r--   0        0        0     5821 2023-06-15 10:30:41.434622 oblv_ctl-0.4.1/oblv_ctl/api/notification/mark_notification_read_notification_notification_id_delete.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.356530 oblv_ctl-0.4.1/oblv_ctl/api/repo/__init__.py
+-rw-r--r--   0        0        0     6756 2023-06-15 10:30:41.444743 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_all_repos_repo_linked_get.py
+-rw-r--r--   0        0        0     6181 2023-06-15 10:30:41.452345 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_all_repos_user_repo_linked_get.py
+-rw-r--r--   0        0        0    10465 2023-06-15 10:30:41.458786 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_dynamic_services_repo_service_dynamic_get.py
+-rw-r--r--   0        0        0     7065 2023-06-15 10:30:41.466341 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py
+-rw-r--r--   0        0        0     7663 2023-06-15 10:30:41.473706 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py
+-rw-r--r--   0        0        0     8155 2023-06-15 10:30:41.481759 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py
+-rw-r--r--   0        0        0    10984 2023-06-15 10:30:41.488804 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_static_services_repo_service_static_get.py
+-rw-r--r--   0        0        0     7492 2023-06-15 10:30:41.497130 oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_user_repo_repo_owner_repo_name_get.py
+-rw-r--r--   0        0        0     6815 2023-06-15 10:30:41.505238 oblv_ctl-0.4.1/oblv_ctl/api/repo/search_repo_from_vcs_repo_search_get.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.398532 oblv_ctl-0.4.1/oblv_ctl/api/service/__init__.py
+-rw-r--r--   0        0        0    10182 2023-06-15 10:30:41.512796 oblv_ctl-0.4.1/oblv_ctl/api/service/add_update_repo_dynamic_service_service_dynamic_put.py
+-rw-r--r--   0        0        0     5957 2023-06-15 10:30:41.519533 oblv_ctl-0.4.1/oblv_ctl/api/service/create_static_service_service_static_post.py
+-rw-r--r--   0        0        0     9450 2023-06-15 10:30:41.527981 oblv_ctl-0.4.1/oblv_ctl/api/service/delete_dynamic_service_repo_service_delete.py
+-rw-r--r--   0        0        0     8605 2023-06-15 10:30:41.535704 oblv_ctl-0.4.1/oblv_ctl/api/service/delete_dynamic_service_service_dynamic_delete.py
+-rw-r--r--   0        0        0     5866 2023-06-15 10:30:41.542977 oblv_ctl-0.4.1/oblv_ctl/api/service/delete_static_service_service_static_delete.py
+-rw-r--r--   0        0        0     6036 2023-06-15 10:30:41.554409 oblv_ctl-0.4.1/oblv_ctl/api/service/get_docker_image_service_static_docker_get.py
+-rw-r--r--   0        0        0     8814 2023-06-15 10:30:41.561886 oblv_ctl-0.4.1/oblv_ctl/api/service/get_dynamic_service_service_dynamic_get.py
+-rw-r--r--   0        0        0    10761 2023-06-15 10:30:41.571005 oblv_ctl-0.4.1/oblv_ctl/api/service/get_marketplace_services_service_marketplace_get.py
+-rw-r--r--   0        0        0    10929 2023-06-15 10:30:41.580556 oblv_ctl-0.4.1/oblv_ctl/api/service/get_repo_dynamic_services_repo_service_get.py
+-rw-r--r--   0        0        0     9425 2023-06-15 10:30:41.589694 oblv_ctl-0.4.1/oblv_ctl/api/service/get_service_yaml_content_repo_service_data_get.py
+-rw-r--r--   0        0        0     5941 2023-06-15 10:30:41.597730 oblv_ctl-0.4.1/oblv_ctl/api/service/get_static_service_build_logs_service_static_logs_get.py
+-rw-r--r--   0        0        0     6149 2023-06-15 10:30:41.607319 oblv_ctl-0.4.1/oblv_ctl/api/service/get_static_service_service_static_get.py
+-rw-r--r--   0        0        0     9811 2023-06-15 10:30:41.615080 oblv_ctl-0.4.1/oblv_ctl/api/service/get_user_dynamic_services_service_get.py
+-rw-r--r--   0        0        0     9564 2023-06-15 10:30:41.624817 oblv_ctl-0.4.1/oblv_ctl/api/service/get_user_dynamic_services_user_service_dynamic_get.py
+-rw-r--r--   0        0        0    10616 2023-06-15 10:30:41.633713 oblv_ctl-0.4.1/oblv_ctl/api/service/get_user_static_services_user_service_static_get.py
+-rw-r--r--   0        0        0    10463 2023-06-15 10:30:41.649261 oblv_ctl-0.4.1/oblv_ctl/api/service/old_add_repo_service_repo_service_post.py
+-rw-r--r--   0        0        0    10940 2023-06-15 10:30:41.656204 oblv_ctl-0.4.1/oblv_ctl/api/service/old_update_repo_service_repo_service_put.py
+-rw-r--r--   0        0        0    10600 2023-06-15 10:30:41.664477 oblv_ctl-0.4.1/oblv_ctl/api/service/old_validate_repo_dynamic_service_repo_service_validate_get.py
+-rw-r--r--   0        0        0     5919 2023-06-15 10:30:41.670220 oblv_ctl-0.4.1/oblv_ctl/api/service/remove_service_from_marketplace_service_marketplace_delete.py
+-rw-r--r--   0        0        0     5983 2023-06-15 10:30:41.679024 oblv_ctl-0.4.1/oblv_ctl/api/service/request_marketplace_addition_service_marketplace_request_put.py
+-rw-r--r--   0        0        0     6577 2023-06-15 10:30:41.686304 oblv_ctl-0.4.1/oblv_ctl/api/service/update_static_service_description_service_static_description_put.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.450397 oblv_ctl-0.4.1/oblv_ctl/api/user/__init__.py
+-rw-r--r--   0        0        0     5905 2023-06-15 10:30:41.695124 oblv_ctl-0.4.1/oblv_ctl/api/user/add_user_public_shared_key_user_psk_put.py
+-rw-r--r--   0        0        0     5812 2023-06-15 10:30:41.704430 oblv_ctl-0.4.1/oblv_ctl/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py
+-rw-r--r--   0        0        0     5773 2023-06-15 10:30:41.711530 oblv_ctl-0.4.1/oblv_ctl/api/user/get_user_profile_view_user_profile_get.py
+-rw-r--r--   0        0        0     5858 2023-06-15 10:30:41.718355 oblv_ctl-0.4.1/oblv_ctl/api/user/get_user_public_shared_key_user_psk_get.py
+-rw-r--r--   0        0        0     5912 2023-06-15 10:30:41.724408 oblv_ctl-0.4.1/oblv_ctl/api/user/update_user_name_user_name_put.py
+-rw-r--r--   0        0        0     6073 2023-06-15 10:30:41.730742 oblv_ctl-0.4.1/oblv_ctl/api/user/update_user_password_user_password_put.py
+-rw-r--r--   0        0        0      389 2023-06-09 07:31:18.488721 oblv_ctl-0.4.1/oblv_ctl/auth.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:31:18.489720 oblv_ctl-0.4.1/oblv_ctl/cli/__init__.py
+-rw-r--r--   0        0        0     7663 2023-06-15 10:30:41.738242 oblv_ctl-0.4.1/oblv_ctl/cli/deployment.py
+-rw-r--r--   0        0        0     3123 2023-06-15 10:30:41.744584 oblv_ctl-0.4.1/oblv_ctl/cli/main.py
+-rw-r--r--   0        0        0     2296 2023-06-15 10:30:41.750044 oblv_ctl-0.4.1/oblv_ctl/cli/marketplace.py
+-rw-r--r--   0        0        0     4079 2023-06-09 07:31:18.511066 oblv_ctl-0.4.1/oblv_ctl/cli/service.py
+-rw-r--r--   0        0        0     3787 2023-06-15 10:30:41.757460 oblv_ctl-0.4.1/oblv_ctl/cli/static_service.py
+-rw-r--r--   0        0        0     1835 2023-06-15 10:30:41.765099 oblv_ctl-0.4.1/oblv_ctl/cli/utils.py
+-rw-r--r--   0        0        0     1885 2023-06-15 10:30:41.772316 oblv_ctl-0.4.1/oblv_ctl/client.py
+-rw-r--r--   0        0        0       30 2023-06-15 10:30:07.623308 oblv_ctl-0.4.1/oblv_ctl/config.py
+-rw-r--r--   0        0        0     3351 2023-06-15 10:30:41.779382 oblv_ctl-0.4.1/oblv_ctl/exceptions.py
+-rw-r--r--   0        0        0     5329 2023-06-15 10:30:41.785975 oblv_ctl-0.4.1/oblv_ctl/models/__init__.py
+-rw-r--r--   0        0        0     2649 2023-06-15 10:30:41.792939 oblv_ctl-0.4.1/oblv_ctl/models/access_history.py
+-rw-r--r--   0        0        0     2326 2023-06-09 07:31:18.548369 oblv_ctl-0.4.1/oblv_ctl/models/account.py
+-rw-r--r--   0        0        0     1533 2023-06-09 07:31:18.549392 oblv_ctl-0.4.1/oblv_ctl/models/api_key.py
+-rw-r--r--   0        0        0     1979 2023-06-15 10:30:41.799944 oblv_ctl-0.4.1/oblv_ctl/models/available_deployment.py
+-rw-r--r--   0        0        0     2397 2023-06-15 10:30:41.805315 oblv_ctl-0.4.1/oblv_ctl/models/available_deployment_list.py
+-rw-r--r--   0        0        0     1975 2023-06-09 07:31:18.560005 oblv_ctl-0.4.1/oblv_ctl/models/build_args_schema.py
+-rw-r--r--   0        0        0     4049 2023-06-15 10:30:41.812451 oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_input.py
+-rw-r--r--   0        0        0      167 2023-06-15 10:30:41.816994 oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_input_account_type.py
+-rw-r--r--   0        0        0      180 2023-06-15 10:30:41.823536 oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_input_ref_type.py
+-rw-r--r--   0        0        0      265 2023-06-15 10:30:41.828386 oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_input_region_name.py
+-rw-r--r--   0        0        0      191 2023-06-15 10:30:41.834146 oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_input_visibility.py
+-rw-r--r--   0        0        0     2108 2023-06-09 07:31:18.576142 oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_response.py
+-rw-r--r--   0        0        0    10446 2023-06-15 10:30:41.840437 oblv_ctl-0.4.1/oblv_ctl/models/deployment_complete.py
+-rw-r--r--   0        0        0     2344 2023-06-15 10:30:41.849183 oblv_ctl-0.4.1/oblv_ctl/models/deployment_list.py
+-rw-r--r--   0        0        0     8710 2023-06-15 10:30:41.856313 oblv_ctl-0.4.1/oblv_ctl/models/deployment_response.py
+-rw-r--r--   0        0        0     2534 2023-06-15 10:30:41.863305 oblv_ctl-0.4.1/oblv_ctl/models/dynamic_service.py
+-rw-r--r--   0        0        0     1413 2023-06-15 10:30:41.871897 oblv_ctl-0.4.1/oblv_ctl/models/dynamic_service_yaml_input.py
+-rw-r--r--   0        0        0     2245 2023-06-15 10:30:41.880948 oblv_ctl-0.4.1/oblv_ctl/models/http_validation_error.py
+-rw-r--r--   0        0        0     3419 2023-06-09 07:31:18.603069 oblv_ctl-0.4.1/oblv_ctl/models/instance.py
+-rw-r--r--   0        0        0     3973 2023-06-15 10:30:41.889073 oblv_ctl-0.4.1/oblv_ctl/models/market_place_service.py
+-rw-r--r--   0        0        0     1704 2023-06-09 07:31:18.609292 oblv_ctl-0.4.1/oblv_ctl/models/message_model.py
+-rw-r--r--   0        0        0     1575 2023-06-15 10:30:41.899154 oblv_ctl-0.4.1/oblv_ctl/models/name_input.py
+-rw-r--r--   0        0        0     3066 2023-06-09 07:31:18.614823 oblv_ctl-0.4.1/oblv_ctl/models/notification_response.py
+-rw-r--r--   0        0        0     1980 2023-06-09 07:31:18.615818 oblv_ctl-0.4.1/oblv_ctl/models/oblv_auth_response.py
+-rw-r--r--   0        0        0     1490 2023-06-15 10:30:41.905692 oblv_ctl-0.4.1/oblv_ctl/models/old_add_repo_service_repo_service_post_data.py
+-rw-r--r--   0        0        0     1500 2023-06-15 10:30:41.913114 oblv_ctl-0.4.1/oblv_ctl/models/old_update_repo_service_repo_service_put_data.py
+-rw-r--r--   0        0        0     1610 2023-06-15 10:30:41.920392 oblv_ctl-0.4.1/oblv_ctl/models/psk.py
+-rw-r--r--   0        0        0     2172 2023-06-09 07:31:18.627240 oblv_ctl-0.4.1/oblv_ctl/models/ref_response.py
+-rw-r--r--   0        0        0     4997 2023-06-09 07:31:18.628762 oblv_ctl-0.4.1/oblv_ctl/models/repo.py
+-rw-r--r--   0        0        0     2338 2023-06-09 07:31:18.633536 oblv_ctl-0.4.1/oblv_ctl/models/repo_all_response.py
+-rw-r--r--   0        0        0     2542 2023-06-15 10:30:41.929372 oblv_ctl-0.4.1/oblv_ctl/models/repo_dynamic_service.py
+-rw-r--r--   0        0        0     4953 2023-06-15 10:30:41.936935 oblv_ctl-0.4.1/oblv_ctl/models/repo_static_service.py
+-rw-r--r--   0        0        0     1428 2023-06-15 10:30:41.944605 oblv_ctl-0.4.1/oblv_ctl/models/repo_static_service_arguments.py
+-rw-r--r--   0        0        0     2100 2023-06-09 07:31:18.642760 oblv_ctl-0.4.1/oblv_ctl/models/role_response.py
+-rw-r--r--   0        0        0      204 2023-06-15 10:30:41.951573 oblv_ctl-0.4.1/oblv_ctl/models/service_filter_type.py
+-rw-r--r--   0        0        0     2472 2023-06-15 10:30:41.960141 oblv_ctl-0.4.1/oblv_ctl/models/service_list_market_place_service.py
+-rw-r--r--   0        0        0     1811 2023-06-15 10:30:41.966715 oblv_ctl-0.4.1/oblv_ctl/models/service_list_repo_dynamic_service.py
+-rw-r--r--   0        0        0     1802 2023-06-15 10:30:41.974018 oblv_ctl-0.4.1/oblv_ctl/models/service_list_repo_static_service.py
+-rw-r--r--   0        0        0     2414 2023-06-15 10:30:41.981560 oblv_ctl-0.4.1/oblv_ctl/models/service_validation_response.py
+-rw-r--r--   0        0        0     1385 2023-06-15 10:30:41.988799 oblv_ctl-0.4.1/oblv_ctl/models/service_yaml_content.py
+-rw-r--r--   0        0        0     2682 2023-06-09 07:31:18.664364 oblv_ctl-0.4.1/oblv_ctl/models/shared_users.py
+-rw-r--r--   0        0        0     5241 2023-06-15 10:30:41.994918 oblv_ctl-0.4.1/oblv_ctl/models/static_deployment_input.py
+-rw-r--r--   0        0        0      322 2023-06-15 10:30:42.002984 oblv_ctl-0.4.1/oblv_ctl/models/static_deployment_input_infra_reqs.py
+-rw-r--r--   0        0        0      265 2023-06-15 10:30:42.010264 oblv_ctl-0.4.1/oblv_ctl/models/static_deployment_input_region_name.py
+-rw-r--r--   0        0        0     1428 2023-06-15 10:30:42.018276 oblv_ctl-0.4.1/oblv_ctl/models/static_deployment_input_users.py
+-rw-r--r--   0        0        0     4872 2023-06-15 10:30:42.026721 oblv_ctl-0.4.1/oblv_ctl/models/static_service.py
+-rw-r--r--   0        0        0     1405 2023-06-15 10:30:42.033774 oblv_ctl-0.4.1/oblv_ctl/models/static_service_arguments.py
+-rw-r--r--   0        0        0     3446 2023-06-15 10:30:42.040907 oblv_ctl-0.4.1/oblv_ctl/models/static_service_input.py
+-rw-r--r--   0        0        0     1527 2023-06-15 10:30:42.049052 oblv_ctl-0.4.1/oblv_ctl/models/static_service_input_arguments.py
+-rw-r--r--   0        0        0     1372 2023-06-15 10:30:42.055616 oblv_ctl-0.4.1/oblv_ctl/models/supported_regions.py
+-rw-r--r--   0        0        0     3177 2023-06-09 07:31:18.694361 oblv_ctl-0.4.1/oblv_ctl/models/user_credit_utilization.py
+-rw-r--r--   0        0        0     2814 2023-06-15 10:30:42.064038 oblv_ctl-0.4.1/oblv_ctl/models/user_dynamic_service.py
+-rw-r--r--   0        0        0     2093 2023-06-15 10:30:42.070745 oblv_ctl-0.4.1/oblv_ctl/models/user_password_input.py
+-rw-r--r--   0        0        0     2688 2023-06-09 07:31:18.704139 oblv_ctl-0.4.1/oblv_ctl/models/user_profile_response.py
+-rw-r--r--   0        0        0     2991 2023-06-15 10:30:42.077861 oblv_ctl-0.4.1/oblv_ctl/models/user_service_list_user_dynamic_service.py
+-rw-r--r--   0        0        0     2981 2023-06-15 10:30:42.084213 oblv_ctl-0.4.1/oblv_ctl/models/user_service_list_user_static_service.py
+-rw-r--r--   0        0        0     4793 2023-06-15 10:30:42.091177 oblv_ctl-0.4.1/oblv_ctl/models/user_static_service.py
+-rw-r--r--   0        0        0     1428 2023-06-15 10:30:42.098757 oblv_ctl-0.4.1/oblv_ctl/models/user_static_service_arguments.py
+-rw-r--r--   0        0        0     1441 2023-06-15 10:30:42.104788 oblv_ctl-0.4.1/oblv_ctl/models/user_static_service_yaml_details.py
+-rw-r--r--   0        0        0     2335 2023-06-15 10:30:42.112205 oblv_ctl-0.4.1/oblv_ctl/models/validation_error.py
+-rw-r--r--   0        0        0     2725 2023-06-15 10:30:42.120339 oblv_ctl-0.4.1/oblv_ctl/models/vcs_repo_response.py
+-rw-r--r--   0        0        0    29287 2023-06-15 10:30:42.128599 oblv_ctl-0.4.1/oblv_ctl/oblv_client.py
+-rw-r--r--   0        0        0       25 2023-06-09 07:31:18.739038 oblv_ctl-0.4.1/oblv_ctl/py.typed
+-rw-r--r--   0        0        0      982 2023-06-09 07:31:18.740568 oblv_ctl-0.4.1/oblv_ctl/types.py
+-rw-r--r--   0        0        0     1283 2023-06-09 07:31:18.742585 oblv_ctl-0.4.1/oblv_ctl/utils.py
+-rw-r--r--   0        0        0      750 2023-06-15 10:31:33.248468 oblv_ctl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8151 2023-06-15 10:30:41.280327 oblv_ctl-0.4.1/README.md
+-rw-r--r--   0        0        0     8908 1970-01-01 00:00:00.000000 oblv_ctl-0.4.1/PKG-INFO
```

### Comparing `oblv_ctl-0.3.1/LICENSE` & `oblv_ctl-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/auth/authenticate_key_login_apikey_post.py` & `oblv_ctl-0.4.1/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
-from ...client import Client
-from ...exceptions import AuthenticationError, BadRequestError, HTTPClientError, ParamValidationError
-from ...models.api_key import APIKey
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.oblv_auth_response import OblvAuthResponse
-from ...types import Response
+from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
-    client: Client,
-    json_body: APIKey,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/login/apikey".format(client.base_url)
+    url = "{}/notification".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
-        "method": "post",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
     if response.status_code == 200:
-        response_200 = OblvAuthResponse.from_dict(response.json())
-
+        response_200 = cast(str, response.json())
         return response_200
-    if response.status_code == 401:
-        raise AuthenticationError()
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
         response_422 = HTTPValidationError.from_dict(response.json())
         if response_422.detail[0].type.__contains__("regex"):
             report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, str]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Client,
-    json_body: APIKey,
-) -> Response[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]:
-    """Authenticate With Apikey
-
-     API to validate user's credentials using their **apikey**. This apikey is to be generated from the
-    Console UI and then used for authentication.
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
 
     Args:
-        json_body (APIKey):
+        oblivious_user_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]
+        Union[HTTPValidationError, MessageModel, str]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
-    client: Client,
-    json_body: APIKey,
-) -> Optional[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]:
-    """Authenticate With Apikey
-
-     API to validate user's credentials using their **apikey**. This apikey is to be generated from the
-    Console UI and then used for authentication.
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
 
     Args:
-        json_body (APIKey):
+        oblivious_user_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]
+        Union[HTTPValidationError, MessageModel, str]
     """
 
     return sync_detailed(
         client=client,
-        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Client,
-    json_body: APIKey,
-) -> Response[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]:
-    """Authenticate With Apikey
-
-     API to validate user's credentials using their **apikey**. This apikey is to be generated from the
-    Console UI and then used for authentication.
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
 
     Args:
-        json_body (APIKey):
+        oblivious_user_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]
+        Union[HTTPValidationError, MessageModel, str]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
-    client: Client,
-    json_body: APIKey,
-) -> Optional[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]:
-    """Authenticate With Apikey
-
-     API to validate user's credentials using their **apikey**. This apikey is to be generated from the
-    Console UI and then used for authentication.
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
 
     Args:
-        json_body (APIKey):
+        oblivious_user_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, OblvAuthResponse]]
+        Union[HTTPValidationError, MessageModel, str]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            json_body=json_body,
+            oblivious_user_id=oblivious_user_id,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/auth/logout_session_logout_delete.py` & `oblv_ctl-0.4.1/oblv_ctl/api/user/update_user_name_user_name_put.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,38 +2,43 @@
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
+from ...models.name_input import NameInput
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
+    json_body: NameInput,
     oblivious_user_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/logout".format(client.base_url)
+    url = "{}/user/name".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "delete",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
         "params": params,
     }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
         response_200 = MessageModel.from_dict(response.json())
@@ -64,108 +69,132 @@
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
+    json_body: NameInput,
     oblivious_user_id: str,
 ) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
+    """Update Name
 
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
+     API to update the name.
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        json_body (NameInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
+    json_body: NameInput,
     oblivious_user_id: str,
 ) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
+    """Update Name
 
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
+     API to update the name.
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        json_body (NameInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
+        json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
+    json_body: NameInput,
     oblivious_user_id: str,
 ) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
+    """Update Name
 
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
+     API to update the name.
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        json_body (NameInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
+    json_body: NameInput,
     oblivious_user_id: str,
 ) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
+    """Update Name
 
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
+     API to update the name.
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        json_body (NameInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
+            json_body=json_body,
             oblivious_user_id=oblivious_user_id,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/deployment/create_new_deployment_deployment_post.py` & `oblv_ctl-0.4.1/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,54 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.create_deployment_input import CreateDeploymentInput
-from ...models.create_deployment_response import CreateDeploymentResponse
+from ...models.deployment_response import DeploymentResponse
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
     oblivious_user_id: str,
+    deployment_id: str,
 ) -> Dict[str, Any]:
     url = "{}/deployment".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+    params["deployment_id"] = deployment_id
 
-    json_json_body = json_body.to_dict()
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
         "params": params,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
+) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == 201:
-        response_201 = CreateDeploymentResponse.from_dict(response.json())
+        response_200 = DeploymentResponse.from_dict(response.json())
 
-        return response_201
+        return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -65,128 +60,144 @@
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
+) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
     oblivious_user_id: str,
-) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
+    deployment_id: str,
+) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
 
-     API to create a new deployment.
+     API to fetch a deployment's details.
 
     Args:
         oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
+        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[DeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
         oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
     oblivious_user_id: str,
-) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
+    deployment_id: str,
+) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
 
-     API to create a new deployment.
+     API to fetch a deployment's details.
 
     Args:
         oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
+        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[DeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
-        json_body=json_body,
         oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
     oblivious_user_id: str,
-) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
+    deployment_id: str,
+) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
 
-     API to create a new deployment.
+     API to fetch a deployment's details.
 
     Args:
         oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
+        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[DeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
         oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
     oblivious_user_id: str,
-) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
+    deployment_id: str,
+) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
 
-     API to create a new deployment.
+     API to fetch a deployment's details.
 
     Args:
         oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
+        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[DeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            json_body=json_body,
             oblivious_user_id=oblivious_user_id,
+            deployment_id=deployment_id,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py` & `oblv_ctl-0.4.1/oblv_ctl/api/deployment/delete_deployment_deployment_delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -81,16 +81,20 @@
 
      API to initiate termination of a deployment.
 
     Args:
         oblivious_user_id (str):
         deployment_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
         deployment_id=deployment_id,
     )
@@ -113,16 +117,20 @@
 
      API to initiate termination of a deployment.
 
     Args:
         oblivious_user_id (str):
         deployment_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
         oblivious_user_id=oblivious_user_id,
         deployment_id=deployment_id,
     ).parsed
@@ -138,16 +146,20 @@
 
      API to initiate termination of a deployment.
 
     Args:
         oblivious_user_id (str):
         deployment_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
         deployment_id=deployment_id,
     )
@@ -168,16 +180,20 @@
 
      API to initiate termination of a deployment.
 
     Args:
         oblivious_user_id (str):
         deployment_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             oblivious_user_id=oblivious_user_id,
             deployment_id=deployment_id,
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/deployment/generate_build_args_deployment_arguments_get.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
         response_200 = BuildArgsSchema.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
@@ -74,17 +72,15 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, BuildArgsSchema, HTTPValidationError, MessageModel]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
@@ -106,20 +102,25 @@
 
     Note - A service could have different build args schema depending on the service's commit history.
 
     Args:
         oblivious_user_id (str):
         owner (str):
         repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        ref (str): Service Ref
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+        Union[BuildArgsSchema, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
         owner=owner,
         repo=repo,
@@ -153,20 +154,25 @@
 
     Note - A service could have different build args schema depending on the service's commit history.
 
     Args:
         oblivious_user_id (str):
         owner (str):
         repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        ref (str): Service Ref
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+        Union[BuildArgsSchema, HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
         oblivious_user_id=oblivious_user_id,
         owner=owner,
         repo=repo,
@@ -193,20 +199,25 @@
 
     Note - A service could have different build args schema depending on the service's commit history.
 
     Args:
         oblivious_user_id (str):
         owner (str):
         repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        ref (str): Service Ref
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+        Union[BuildArgsSchema, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
         owner=owner,
         repo=repo,
@@ -238,20 +249,25 @@
 
     Note - A service could have different build args schema depending on the service's commit history.
 
     Args:
         oblivious_user_id (str):
         owner (str):
         repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        ref (str): Service Ref
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+        Union[BuildArgsSchema, HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             oblivious_user_id=oblivious_user_id,
             owner=owner,
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_available_deployments_deployment_available_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/repo/get_all_repos_user_repo_linked_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.available_deployment_list import AvailableDeploymentList
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...types import UNSET, Response, Unset
+from ...models.repo_all_response import RepoAllResponse
+from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
 ) -> Dict[str, Any]:
-    url = "{}/deployment/available".format(client.base_url)
+    url = "{}/user/repo/linked".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["page"] = page
-
-    params["per_page"] = per_page
-
-    params["search_term"] = search_term
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+) -> Optional[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
     if response.status_code == 200:
-        response_200 = AvailableDeploymentList.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = RepoAllResponse.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
 
         return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -66,152 +65,132 @@
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+) -> Response[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
+) -> Response[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to fetch all the deployments the user can connect to.
+     API to fetch user's repo without services
 
     Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
+) -> Optional[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to fetch all the deployments the user can connect to.
+     API to fetch user's repo without services
 
     Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     return sync_detailed(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
+) -> Response[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to fetch all the deployments the user can connect to.
+     API to fetch user's repo without services
 
     Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
+) -> Optional[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to fetch all the deployments the user can connect to.
+     API to fetch user's repo without services
 
     Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             oblivious_user_id=oblivious_user_id,
-            page=page,
-            per_page=per_page,
-            search_term=search_term,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_info_deployment_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,51 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.deployment_response import DeploymentResponse
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
+    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/deployment".format(client.base_url)
+    url = "{}/notification/{notification_id}".format(client.base_url, notification_id=notification_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["deployment_id"] = deployment_id
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, DeploymentResponse, HTTPValidationError, MessageModel]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
     if response.status_code == 200:
-        response_200 = DeploymentResponse.from_dict(response.json())
-
+        response_200 = cast(str, response.json())
         return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -58,130 +55,136 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
+) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
 
     Args:
+        notification_id (str):
         oblivious_user_id (str):
-        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, str]
     """
 
     kwargs = _get_kwargs(
+        notification_id=notification_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
 
     Args:
+        notification_id (str):
         oblivious_user_id (str):
-        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, str]
     """
 
     return sync_detailed(
+        notification_id=notification_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
     ).parsed
 
 
 async def asyncio_detailed(
+    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
+) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
 
     Args:
+        notification_id (str):
         oblivious_user_id (str):
-        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, str]
     """
 
     kwargs = _get_kwargs(
+        notification_id=notification_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
 
     Args:
+        notification_id (str):
         oblivious_user_id (str):
-        deployment_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, str]
     """
 
     return (
         await asyncio_detailed(
+            notification_id=notification_id,
             client=client,
             oblivious_user_id=oblivious_user_id,
-            deployment_id=deployment_id,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_deployment_roles_deployment_roles_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/user/get_user_profile_view_user_profile_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,196 +1,188 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.role_response import RoleResponse
+from ...models.user_profile_response import UserProfileResponse
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/deployment/roles".format(client.base_url)
+    url = "{}/user/profile".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["deployment_id"] = deployment_id
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+) -> Optional[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
     if response.status_code == 200:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = RoleResponse.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = UserProfileResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 501:
-        response_501 = MessageModel.from_dict(response.json())
-
-        return response_501
     if response.status_code == 422:
         response_422 = HTTPValidationError.from_dict(response.json())
         if response_422.detail[0].type.__contains__("regex"):
             report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
+) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
 
-     API to get a deployment's roles.
+     API to fetch user's profile details
 
     Args:
-        oblivious_user_id (str):
-        deployment_id (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+        Union[HTTPValidationError, MessageModel, UserProfileResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
+) -> Optional[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
 
-     API to get a deployment's roles.
+     API to fetch user's profile details
 
     Args:
-        oblivious_user_id (str):
-        deployment_id (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+        Union[HTTPValidationError, MessageModel, UserProfileResponse]
     """
 
     return sync_detailed(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
+) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
 
-     API to get a deployment's roles.
+     API to fetch user's profile details
 
     Args:
-        oblivious_user_id (str):
-        deployment_id (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+        Union[HTTPValidationError, MessageModel, UserProfileResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
+) -> Optional[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
 
-     API to get a deployment's roles.
+     API to fetch user's profile details
 
     Args:
-        oblivious_user_id (str):
-        deployment_id (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+        Union[HTTPValidationError, MessageModel, UserProfileResponse]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             oblivious_user_id=oblivious_user_id,
-            deployment_id=deployment_id,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/deployment/get_user_owned_deployments_deployment_owned_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/deployment/add_deployment_tag_deployment_deployment_id_tag_post.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,50 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.deployment_list import DeploymentList
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...types import UNSET, Response, Unset
+from ...types import UNSET, Response
 
 
 def _get_kwargs(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
+    tag: str,
 ) -> Dict[str, Any]:
-    url = "{}/deployment/owned".format(client.base_url)
+    url = "{}/deployment/{deployment_id}/tag".format(client.base_url, deployment_id=deployment_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["page"] = page
-
-    params["per_page"] = per_page
-
-    params["search_term"] = search_term
+    params["tag"] = tag
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = DeploymentList.from_dict(response.json())
+        response_200 = MessageModel.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
@@ -64,154 +56,156 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
+    tag: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Add Deployment Tag
 
-     API to fetch a user's owned deployments.
+     API to add a tag to deployment.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
+        deployment_id=deployment_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
+        tag=tag,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
+    tag: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Add Deployment Tag
 
-     API to fetch a user's owned deployments.
+     API to add a tag to deployment.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
+        deployment_id=deployment_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
+        tag=tag,
     ).parsed
 
 
 async def asyncio_detailed(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
+    tag: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Add Deployment Tag
 
-     API to fetch a user's owned deployments.
+     API to add a tag to deployment.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
+        deployment_id=deployment_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
+        tag=tag,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
+    tag: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Add Deployment Tag
 
-     API to fetch a user's owned deployments.
+     API to add a tag to deployment.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
+            deployment_id=deployment_id,
             client=client,
             oblivious_user_id=oblivious_user_id,
-            page=page,
-            per_page=per_page,
-            search_term=search_term,
+            tag=tag,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/notification/get_all_notifications_notification_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/service/get_docker_image_service_static_docker_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-from typing import Any, Dict, List, Optional, Union, cast
+from io import BytesIO
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.notification_response import NotificationResponse
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
+    service: str,
 ) -> Dict[str, Any]:
-    url = "{}/notification".format(client.base_url)
+    url = "{}/service/static/docker".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
+    params["service"] = service
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[str, HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = NotificationResponse.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = response.json()
 
         return response_200
-    if response.status_code == 204:
-        response_204 = cast(Any, None)
-        return response_204
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -63,110 +56,144 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[str, HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
+    service: str,
+) -> Response[Union[str, HTTPValidationError, MessageModel]]:
+    """Get static service docker image
+
+     To fetch docker image of the static service
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+        Union[str, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
+        service=service,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
+    service: str,
+) -> Optional[Union[str, HTTPValidationError, MessageModel]]:
+    """Get static service docker image
+
+     To fetch docker image of the static service
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+        Union[str, HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
         oblivious_user_id=oblivious_user_id,
+        service=service,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
+    service: str,
+) -> Response[Union[str, HTTPValidationError, MessageModel]]:
+    """Get static service docker image
+
+     To fetch docker image of the static service
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+        Union[str, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
+        service=service,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
+    service: str,
+) -> Optional[Union[str, HTTPValidationError, MessageModel]]:
+    """Get static service docker image
+
+     To fetch docker image of the static service
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+        Union[str, HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             oblivious_user_id=oblivious_user_id,
+            service=service,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/notification/get_notification_details_notification_notification_id_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/service/delete_static_service_service_static_delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
-    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
+    service: str,
 ) -> Dict[str, Any]:
-    url = "{}/notification/{notification_id}".format(client.base_url, notification_id=notification_id)
+    url = "{}/service/static".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
+    params["service"] = service
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = cast(str, response.json())
+        response_200 = MessageModel.from_dict(response.json())
+
         return response_200
-    if response.status_code == 204:
-        response_204 = cast(Any, None)
-        return response_204
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -55,120 +55,144 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
+    service: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Delete static service
+
+     Delete a static service.
 
     Args:
-        notification_id (str):
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
-        notification_id=notification_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
+        service=service,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
+    service: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Delete static service
+
+     Delete a static service.
 
     Args:
-        notification_id (str):
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
-        notification_id=notification_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
+        service=service,
     ).parsed
 
 
 async def asyncio_detailed(
-    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
+    service: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Delete static service
+
+     Delete a static service.
 
     Args:
-        notification_id (str):
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
-        notification_id=notification_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
+        service=service,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    notification_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
+    service: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Delete static service
+
+     Delete a static service.
 
     Args:
-        notification_id (str):
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
+        service (str): Service name or id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
-            notification_id=notification_id,
             client=client,
             oblivious_user_id=oblivious_user_id,
+            service=service,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/notification/mark_all_notification_read_notification_delete.py` & `oblv_ctl-0.4.1/oblv_ctl/api/deployment/remove_deployment_tag_deployment_deployment_id_tag_delete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
+    tag: str,
 ) -> Dict[str, Any]:
-    url = "{}/notification".format(client.base_url)
+    url = "{}/deployment/{deployment_id}/tag".format(client.base_url, deployment_id=deployment_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
+    params["tag"] = tag
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = cast(str, response.json())
+        response_200 = MessageModel.from_dict(response.json())
+
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
@@ -51,108 +56,156 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
+    tag: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Remove Deployment Tag
+
+     API to remove a deployment's tag.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
+        deployment_id=deployment_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
+        tag=tag,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
+    tag: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Remove Deployment Tag
+
+     API to remove a deployment's tag.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
+        deployment_id=deployment_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
+        tag=tag,
     ).parsed
 
 
 async def asyncio_detailed(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
+    tag: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Remove Deployment Tag
+
+     API to remove a deployment's tag.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
+        deployment_id=deployment_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
+        tag=tag,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    deployment_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
+    tag: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Remove Deployment Tag
+
+     API to remove a deployment's tag.
 
     Args:
+        deployment_id (str):
         oblivious_user_id (str):
+        tag (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
+            deployment_id=deployment_id,
             client=client,
             oblivious_user_id=oblivious_user_id,
+            tag=tag,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_from_vcs_repo_get.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, VCSRepoResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, VCSRepoResponse]]:
     if response.status_code == 200:
         response_200 = VCSRepoResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
@@ -84,16 +84,20 @@
     any organization they are member of).
 
     Args:
         oblivious_user_id (str):
         page (Union[Unset, None, int]):  Default: 1.
         per_page (Union[Unset, None, int]):  Default: 10.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
+        Union[HTTPValidationError, VCSRepoResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
         page=page,
         per_page=per_page,
@@ -120,16 +124,20 @@
     any organization they are member of).
 
     Args:
         oblivious_user_id (str):
         page (Union[Unset, None, int]):  Default: 1.
         per_page (Union[Unset, None, int]):  Default: 10.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
+        Union[HTTPValidationError, VCSRepoResponse]
     """
 
     return sync_detailed(
         client=client,
         oblivious_user_id=oblivious_user_id,
         page=page,
         per_page=per_page,
@@ -149,16 +157,20 @@
     any organization they are member of).
 
     Args:
         oblivious_user_id (str):
         page (Union[Unset, None, int]):  Default: 1.
         per_page (Union[Unset, None, int]):  Default: 10.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
+        Union[HTTPValidationError, VCSRepoResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
         page=page,
         per_page=per_page,
@@ -183,16 +195,20 @@
     any organization they are member of).
 
     Args:
         oblivious_user_id (str):
         page (Union[Unset, None, int]):  Default: 1.
         per_page (Union[Unset, None, int]):  Default: 10.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
+        Union[HTTPValidationError, VCSRepoResponse]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             oblivious_user_id=oblivious_user_id,
             page=page,
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,57 +2,51 @@
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.ref_response import RefResponse
+from ...models.repo import Repo
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
+    repo_owner: str,
+    repo_name: str,
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
+    account_type: Union[Unset, None, str] = "github",
 ) -> Dict[str, Any]:
-    url = "{}/repo/refs".format(client.base_url)
+    url = "{}/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_owner=repo_owner, repo_name=repo_name)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["account_type"] = account_type
-
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["repo_owner"] = repo_owner
-
-    params["repo_name"] = repo_name
+    params["account_type"] = account_type
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RefResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
     if response.status_code == 200:
-        response_200 = RefResponse.from_dict(response.json())
+        response_200 = Repo.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
@@ -64,178 +58,176 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    repo_owner: str,
+    repo_name: str,
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
 
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
+     API to fetch user's repo information. This API is deprecated and will not be supported from upcoming
+    releases. Kindly use GET /user/repo/{repo_owner}/{repo_name} for getting user's repo information.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     kwargs = _get_kwargs(
-        client=client,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    repo_owner: str,
+    repo_name: str,
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
 
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
+     API to fetch user's repo information. This API is deprecated and will not be supported from upcoming
+    releases. Kindly use GET /user/repo/{repo_owner}/{repo_name} for getting user's repo information.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     return sync_detailed(
-        client=client,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
     ).parsed
 
 
 async def asyncio_detailed(
+    repo_owner: str,
+    repo_name: str,
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
 
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
+     API to fetch user's repo information. This API is deprecated and will not be supported from upcoming
+    releases. Kindly use GET /user/repo/{repo_owner}/{repo_name} for getting user's repo information.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     kwargs = _get_kwargs(
-        client=client,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    repo_owner: str,
+    repo_name: str,
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
 
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
+     API to fetch user's repo information. This API is deprecated and will not be supported from upcoming
+    releases. Kindly use GET /user/repo/{repo_owner}/{repo_name} for getting user's repo information.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     return (
         await asyncio_detailed(
-            client=client,
-            account_type=account_type,
-            oblivious_user_id=oblivious_user_id,
             repo_owner=repo_owner,
             repo_name=repo_name,
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            account_type=account_type,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_id_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/account/get_user_accounts_user_account_get.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,59 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.account import Account
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.repo_services import RepoServices
-from ...types import UNSET, Response, Unset
+from ...types import UNSET, Response
 
 
 def _get_kwargs(
-    repo_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
 ) -> Dict[str, Any]:
-    url = "{}/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_id=repo_id)
+    url = "{}/user/account".format(client.base_url)
+
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["account_type"] = account_type
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+) -> Optional[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
     if response.status_code == 200:
-        response_200 = RepoServices.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = Account.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
 
         return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -60,140 +65,132 @@
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+) -> Response[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    repo_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
+) -> Response[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's linked VCS accounts
 
     Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     kwargs = _get_kwargs(
-        repo_id=repo_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    repo_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
+) -> Optional[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's linked VCS accounts
 
     Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     return sync_detailed(
-        repo_id=repo_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
     ).parsed
 
 
 async def asyncio_detailed(
-    repo_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
+) -> Response[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's linked VCS accounts
 
     Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     kwargs = _get_kwargs(
-        repo_id=repo_id,
         client=client,
         oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    repo_id: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
+) -> Optional[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's linked VCS accounts
 
     Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     return (
         await asyncio_detailed(
-            repo_id=repo_id,
             client=client,
             oblivious_user_id=oblivious_user_id,
-            account_type=account_type,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/repo/get_repo_repo_repo_owner_repo_name_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_user_repo_repo_owner_repo_name_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     repo_owner: str,
     repo_name: str,
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
     account_type: Union[Unset, None, str] = "github",
 ) -> Dict[str, Any]:
-    url = "{}/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_owner=repo_owner, repo_name=repo_name)
+    url = "{}/user/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_owner=repo_owner, repo_name=repo_name)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
@@ -39,14 +39,15 @@
         "params": params,
     }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
     if response.status_code == 200:
         response_200 = Repo.from_dict(response.json())
+
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
@@ -76,24 +77,29 @@
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
     account_type: Union[Unset, None, str] = "github",
 ) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
     """Get User Repo
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's repo information
 
     Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     kwargs = _get_kwargs(
         repo_owner=repo_owner,
         repo_name=repo_name,
         client=client,
         oblivious_user_id=oblivious_user_id,
@@ -114,24 +120,29 @@
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
     account_type: Union[Unset, None, str] = "github",
 ) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
     """Get User Repo
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's repo information
 
     Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     return sync_detailed(
         repo_owner=repo_owner,
         repo_name=repo_name,
         client=client,
         oblivious_user_id=oblivious_user_id,
@@ -145,24 +156,29 @@
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
     account_type: Union[Unset, None, str] = "github",
 ) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
     """Get User Repo
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's repo information
 
     Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     kwargs = _get_kwargs(
         repo_owner=repo_owner,
         repo_name=repo_name,
         client=client,
         oblivious_user_id=oblivious_user_id,
@@ -181,24 +197,29 @@
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
     account_type: Union[Unset, None, str] = "github",
 ) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
     """Get User Repo
 
-     API to fetch user's repo with services created for every repo.
+     API to fetch user's repo information
 
     Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        oblivious_user_id (str): User id
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
+        Union[HTTPValidationError, MessageModel, Repo]
     """
 
     return (
         await asyncio_detailed(
             repo_owner=repo_owner,
             repo_name=repo_name,
             client=client,
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/repo/search_repo_from_vcs_repo_search_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/account/get_user_accounts_account_get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.account import Account
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.repo import Repo
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    search_string: str,
 ) -> Dict[str, Any]:
-    url = "{}/repo/search".format(client.base_url)
+    url = "{}/account".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["search_string"] = search_string
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
     if response.status_code == 200:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
-            response_200_item = Repo.from_dict(response_200_item_data)
+            response_200_item = Account.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
     if response.status_code == 204:
         response_204 = cast(Any, None)
         return response_204
@@ -64,132 +63,138 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    search_string: str,
-) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
+) -> Response[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
+     API to fetch user's linked VCS accounts. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/account for list of user's accounts
 
     Args:
-        oblivious_user_id (str):
-        search_string (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        search_string=search_string,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    search_string: str,
-) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
+) -> Optional[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
+     API to fetch user's linked VCS accounts. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/account for list of user's accounts
 
     Args:
-        oblivious_user_id (str):
-        search_string (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     return sync_detailed(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        search_string=search_string,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    search_string: str,
-) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
+) -> Response[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
+     API to fetch user's linked VCS accounts. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/account for list of user's accounts
 
     Args:
-        oblivious_user_id (str):
-        search_string (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         oblivious_user_id=oblivious_user_id,
-        search_string=search_string,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     oblivious_user_id: str,
-    search_string: str,
-) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
+) -> Optional[Union[Any, HTTPValidationError, List["Account"], MessageModel]]:
+    """Get User Accounts
 
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
+     API to fetch user's linked VCS accounts. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/account for list of user's accounts
 
     Args:
-        oblivious_user_id (str):
-        search_string (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+        Union[Any, HTTPValidationError, List['Account'], MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             oblivious_user_id=oblivious_user_id,
-            search_string=search_string,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/service/add_repo_service_repo_service_post.py` & `oblv_ctl-0.4.1/oblv_ctl/api/repo/get_repo_refs_repo_refs_get.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,68 +2,55 @@
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.service_validation_response import ServiceValidationResponse
-from ...models.service_yaml_add_input import ServiceYamlAddInput
+from ...models.ref_response import RefResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
 ) -> Dict[str, Any]:
-    url = "{}/repo/service".format(client.base_url)
+    url = "{}/repo/refs".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["ref"] = ref
-
-    params["ref_type"] = ref_type
-
     params["account_type"] = account_type
 
     params["oblivious_user_id"] = oblivious_user_id
 
     params["repo_owner"] = repo_owner
 
     params["repo_name"] = repo_name
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
         "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
     if response.status_code == 200:
-        response_200 = ServiceValidationResponse.from_dict(response.json())
+        response_200 = RefResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
@@ -75,58 +62,52 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
+) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
 
-     API to create a service after validation.
+     API to fetch the repository refs (branches and tags).
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, RefResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
         account_type=account_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
     )
 
     response = httpx.request(
@@ -136,84 +117,76 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
+) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
 
-     API to create a service after validation.
+     API to fetch the repository refs (branches and tags).
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, RefResponse]
     """
 
     return sync_detailed(
         client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
         account_type=account_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
+) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
 
-     API to create a service after validation.
+     API to fetch the repository refs (branches and tags).
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, RefResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
         account_type=account_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -221,44 +194,40 @@
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
+) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
 
-     API to create a service after validation.
+     API to fetch the repository refs (branches and tags).
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, RefResponse]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            json_body=json_body,
-            ref=ref,
-            ref_type=ref_type,
             account_type=account_type,
             oblivious_user_id=oblivious_user_id,
             repo_owner=repo_owner,
             repo_name=repo_name,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/service/delete_repo_services_repo_service_delete.py` & `oblv_ctl-0.4.1/oblv_ctl/api/repo/get_all_repos_repo_linked_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...types import UNSET, Response, Unset
+from ...models.repo_all_response import RepoAllResponse
+from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
 ) -> Dict[str, Any]:
-    url = "{}/repo/service".format(client.base_url)
+    url = "{}/repo/linked".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["ref"] = ref
-
-    params["ref_type"] = ref_type
-
-    params["account_type"] = account_type
-
     params["oblivious_user_id"] = oblivious_user_id
 
-    params["repo_owner"] = repo_owner
-
-    params["repo_name"] = repo_name
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
     if response.status_code == 200:
-        response_200 = MessageModel.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = RepoAllResponse.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
 
         return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -67,176 +63,138 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Delete Repo Service
+) -> Response[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to delete a service. It does not delete the existing deployments created from this service.
+     API to fetch user's repo without services. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/repo/linked for list of user's linked repos.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
         oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Delete Repo Service
+) -> Optional[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to delete a service. It does not delete the existing deployments created from this service.
+     API to fetch user's repo without services. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/repo/linked for list of user's linked repos.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     return sync_detailed(
         client=client,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
         oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Delete Repo Service
+) -> Response[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to delete a service. It does not delete the existing deployments created from this service.
+     API to fetch user's repo without services. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/repo/linked for list of user's linked repos.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
         oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Delete Repo Service
+) -> Optional[Union[Any, HTTPValidationError, List["RepoAllResponse"], MessageModel]]:
+    """Get User Repos
 
-     API to delete a service. It does not delete the existing deployments created from this service.
+     API to fetch user's repo without services. This API is deprecated and will not be supported from
+    upcoming releases. Kindly use GET /user/repo/linked for list of user's linked repos.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[Any, HTTPValidationError, List['RepoAllResponse'], MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            ref=ref,
-            ref_type=ref_type,
-            account_type=account_type,
             oblivious_user_id=oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/service/delete_dynamic_service_service_dynamic_delete.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,63 +2,60 @@
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.service_content_response import ServiceContentResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    account_type: Union[Unset, None, str] = "github",
-    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
 ) -> Dict[str, Any]:
-    url = "{}/repo/service/yaml".format(client.base_url)
+    url = "{}/service/dynamic".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["ref"] = ref
-
-    params["account_type"] = account_type
-
-    params["ref_type"] = ref_type
-
     params["oblivious_user_id"] = oblivious_user_id
 
     params["repo_owner"] = repo_owner
 
     params["repo_name"] = repo_name
 
+    params["account_type"] = account_type
+
+    params["ref"] = ref
+
+    params["ref_type"] = ref_type
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = ServiceContentResponse.from_dict(response.json())
+        response_200 = MessageModel.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
@@ -70,178 +67,196 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    account_type: Union[Unset, None, str] = "github",
-    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]:
-    """Get Repo Service Yaml
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Delete dynamic service
 
-     API to fetch the service.yaml content as object for the given service.
+     Delete a dynamic service.
 
     Args:
-        ref (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        ref=ref,
-        account_type=account_type,
-        ref_type=ref_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        account_type=account_type,
+        ref=ref,
+        ref_type=ref_type,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    account_type: Union[Unset, None, str] = "github",
-    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]:
-    """Get Repo Service Yaml
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Delete dynamic service
 
-     API to fetch the service.yaml content as object for the given service.
+     Delete a dynamic service.
 
     Args:
-        ref (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
-        ref=ref,
-        account_type=account_type,
-        ref_type=ref_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        account_type=account_type,
+        ref=ref,
+        ref_type=ref_type,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    account_type: Union[Unset, None, str] = "github",
-    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]:
-    """Get Repo Service Yaml
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Delete dynamic service
 
-     API to fetch the service.yaml content as object for the given service.
+     Delete a dynamic service.
 
     Args:
-        ref (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        ref=ref,
-        account_type=account_type,
-        ref_type=ref_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        account_type=account_type,
+        ref=ref,
+        ref_type=ref_type,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    account_type: Union[Unset, None, str] = "github",
-    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]:
-    """Get Repo Service Yaml
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Delete dynamic service
 
-     API to fetch the service.yaml content as object for the given service.
+     Delete a dynamic service.
 
     Args:
-        ref (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceContentResponse]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            ref=ref,
-            account_type=account_type,
-            ref_type=ref_type,
             oblivious_user_id=oblivious_user_id,
             repo_owner=repo_owner,
             repo_name=repo_name,
+            account_type=account_type,
+            ref=ref,
+            ref_type=ref_type,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/service/get_repo_services_repo_service_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/service/get_user_dynamic_services_user_service_dynamic_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,43 @@
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.repo_service_list import RepoServiceList
+from ...models.user_service_list_user_dynamic_service import UserServiceListUserDynamicService
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
     page: Union[Unset, None, int] = 1,
     per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
     get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
 ) -> Dict[str, Any]:
-    url = "{}/repo/service".format(client.base_url)
+    url = "{}/user/service/dynamic".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["account_type"] = account_type
+    params["oblivious_user_id"] = oblivious_user_id
 
     params["page"] = page
 
     params["per_page"] = per_page
 
-    params["get_all"] = get_all
-
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["repo_owner"] = repo_owner
+    params["search_term"] = search_term
 
-    params["repo_name"] = repo_name
+    params["get_all"] = get_all
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
@@ -51,19 +45,22 @@
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]:
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]]:
     if response.status_code == 200:
-        response_200 = RepoServiceList.from_dict(response.json())
+        response_200 = UserServiceListUserDynamicService.from_dict(response.json())
 
         return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -75,192 +72,192 @@
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]:
+) -> Response[Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
     page: Union[Unset, None, int] = 1,
     per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
     get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
+) -> Response[Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]]:
+    """Get user dynamic services
 
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
+     To fetch all dynamic services owned by the user. These are equivalent to the services in the
+    previous version.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        page (Union[Unset, None, int]): Requested page Default: 1.
+        per_page (Union[Unset, None, int]): Responses per page Default: 10.
+        search_term (Union[Unset, None, str]): Search keyword for resources to be filtered with
+            Default: ''.
+        get_all (Union[Unset, None, bool]): Get all responses. Precedence over *page* and
+            *per_page* parameters
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
         page=page,
         per_page=per_page,
+        search_term=search_term,
         get_all=get_all,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
     page: Union[Unset, None, int] = 1,
     per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
     get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]]:
+    """Get user dynamic services
 
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
+     To fetch all dynamic services owned by the user. These are equivalent to the services in the
+    previous version.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        page (Union[Unset, None, int]): Requested page Default: 1.
+        per_page (Union[Unset, None, int]): Responses per page Default: 10.
+        search_term (Union[Unset, None, str]): Search keyword for resources to be filtered with
+            Default: ''.
+        get_all (Union[Unset, None, bool]): Get all responses. Precedence over *page* and
+            *per_page* parameters
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]
     """
 
     return sync_detailed(
         client=client,
-        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
         page=page,
         per_page=per_page,
+        search_term=search_term,
         get_all=get_all,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
     page: Union[Unset, None, int] = 1,
     per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
     get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
+) -> Response[Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]]:
+    """Get user dynamic services
 
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
+     To fetch all dynamic services owned by the user. These are equivalent to the services in the
+    previous version.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        page (Union[Unset, None, int]): Requested page Default: 1.
+        per_page (Union[Unset, None, int]): Responses per page Default: 10.
+        search_term (Union[Unset, None, str]): Search keyword for resources to be filtered with
+            Default: ''.
+        get_all (Union[Unset, None, bool]): Get all responses. Precedence over *page* and
+            *per_page* parameters
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
         page=page,
         per_page=per_page,
+        search_term=search_term,
         get_all=get_all,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
     page: Union[Unset, None, int] = 1,
     per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
     get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]]:
+    """Get user dynamic services
 
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
+     To fetch all dynamic services owned by the user. These are equivalent to the services in the
+    previous version.
 
     Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        page (Union[Unset, None, int]): Requested page Default: 1.
+        per_page (Union[Unset, None, int]): Responses per page Default: 10.
+        search_term (Union[Unset, None, str]): Search keyword for resources to be filtered with
+            Default: ''.
+        get_all (Union[Unset, None, bool]): Get all responses. Precedence over *page* and
+            *per_page* parameters
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+        Union[Any, HTTPValidationError, MessageModel, UserServiceListUserDynamicService]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            account_type=account_type,
+            oblivious_user_id=oblivious_user_id,
             page=page,
             per_page=per_page,
+            search_term=search_term,
             get_all=get_all,
-            oblivious_user_id=oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/service/update_repo_service_repo_service_put.py` & `oblv_ctl-0.4.1/oblv_ctl/api/service/get_service_yaml_content_repo_service_data_get.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,67 +2,63 @@
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.service_validation_response import ServiceValidationResponse
-from ...models.service_yaml_update_input import ServiceYamlUpdateInput
+from ...models.service_yaml_content import ServiceYamlContent
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
     ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
+    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
 ) -> Dict[str, Any]:
-    url = "{}/repo/service".format(client.base_url)
+    url = "{}/repo/service/data".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["ref"] = ref
 
-    params["ref_type"] = ref_type
-
     params["account_type"] = account_type
 
+    params["ref_type"] = ref_type
+
     params["oblivious_user_id"] = oblivious_user_id
+
     params["repo_owner"] = repo_owner
 
     params["repo_name"] = repo_name
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "put",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
         "params": params,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+) -> Optional[Union[HTTPValidationError, MessageModel, ServiceYamlContent]]:
     if response.status_code == 200:
-        response_200 = ServiceValidationResponse.from_dict(response.json())
+        response_200 = ServiceYamlContent.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
@@ -76,58 +72,60 @@
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+) -> Response[Union[HTTPValidationError, MessageModel, ServiceYamlContent]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
     ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
+    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
+) -> Response[Union[HTTPValidationError, MessageModel, ServiceYamlContent]]:
+    """Get Service Yaml Content without service
 
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
+     API to fetch the service.yaml content as object for the given ref. The ref need not be a service. It
+    returns the sample service, if service.yaml not found.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
+        ref (str): Service Ref
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceYamlContent]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
         ref=ref,
-        ref_type=ref_type,
         account_type=account_type,
+        ref_type=ref_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
@@ -136,132 +134,138 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
     ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
+    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
+) -> Optional[Union[HTTPValidationError, MessageModel, ServiceYamlContent]]:
+    """Get Service Yaml Content without service
 
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
+     API to fetch the service.yaml content as object for the given ref. The ref need not be a service. It
+    returns the sample service, if service.yaml not found.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
+        ref (str): Service Ref
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceYamlContent]
     """
 
     return sync_detailed(
         client=client,
-        json_body=json_body,
         ref=ref,
-        ref_type=ref_type,
         account_type=account_type,
+        ref_type=ref_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
     ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
+    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
+) -> Response[Union[HTTPValidationError, MessageModel, ServiceYamlContent]]:
+    """Get Service Yaml Content without service
 
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
+     API to fetch the service.yaml content as object for the given ref. The ref need not be a service. It
+    returns the sample service, if service.yaml not found.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
+        ref (str): Service Ref
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceYamlContent]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
         ref=ref,
-        ref_type=ref_type,
         account_type=account_type,
+        ref_type=ref_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
     ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
     account_type: Union[Unset, None, str] = "github",
+    ref_type: Union[Unset, None, str] = "branch",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
+) -> Optional[Union[HTTPValidationError, MessageModel, ServiceYamlContent]]:
+    """Get Service Yaml Content without service
 
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
+     API to fetch the service.yaml content as object for the given ref. The ref need not be a service. It
+    returns the sample service, if service.yaml not found.
 
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
+        ref (str): Service Ref
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceYamlContent]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            json_body=json_body,
             ref=ref,
-            ref_type=ref_type,
             account_type=account_type,
+            ref_type=ref_type,
             oblivious_user_id=oblivious_user_id,
             repo_owner=repo_owner,
             repo_name=repo_name,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/service/validate_repo_service_repo_service_validate_get.py` & `oblv_ctl-0.4.1/oblv_ctl/api/service/old_validate_repo_dynamic_service_repo_service_validate_get.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,54 +9,54 @@
 from ...models.service_validation_response import ServiceValidationResponse
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
 ) -> Dict[str, Any]:
     url = "{}/repo/service/validate".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["ref"] = ref
-
-    params["ref_type"] = ref_type
-
-    params["account_type"] = account_type
-
     params["oblivious_user_id"] = oblivious_user_id
 
     params["repo_owner"] = repo_owner
 
     params["repo_name"] = repo_name
 
+    params["account_type"] = account_type
+
+    params["ref"] = ref
+
+    params["ref_type"] = ref_type
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
     if response.status_code == 200:
         response_200 = ServiceValidationResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
@@ -84,180 +84,212 @@
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
 ) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
     """Validate Repo Service
 
      API to validate a service with supported service schema. The checks include
 
     - Presence of service.yaml in ./oblivious folder.
     - Presence of Dockerfile in ./oblivious folder.
     - Content of service.yaml must be valid with respect to supported service schema.
 
+    This API is deprecated and will not be supported from upcoming releases. Kindly use **PUT
+    /service/dynamic** for adding/updating dynamic services
+
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceValidationResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        account_type=account_type,
+        ref=ref,
+        ref_type=ref_type,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
 ) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
     """Validate Repo Service
 
      API to validate a service with supported service schema. The checks include
 
     - Presence of service.yaml in ./oblivious folder.
     - Presence of Dockerfile in ./oblivious folder.
     - Content of service.yaml must be valid with respect to supported service schema.
 
+    This API is deprecated and will not be supported from upcoming releases. Kindly use **PUT
+    /service/dynamic** for adding/updating dynamic services
+
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceValidationResponse]
     """
 
     return sync_detailed(
         client=client,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        account_type=account_type,
+        ref=ref,
+        ref_type=ref_type,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
 ) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
     """Validate Repo Service
 
      API to validate a service with supported service schema. The checks include
 
     - Presence of service.yaml in ./oblivious folder.
     - Presence of Dockerfile in ./oblivious folder.
     - Content of service.yaml must be valid with respect to supported service schema.
 
+    This API is deprecated and will not be supported from upcoming releases. Kindly use **PUT
+    /service/dynamic** for adding/updating dynamic services
+
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceValidationResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
         oblivious_user_id=oblivious_user_id,
         repo_owner=repo_owner,
         repo_name=repo_name,
+        account_type=account_type,
+        ref=ref,
+        ref_type=ref_type,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
     oblivious_user_id: str,
     repo_owner: str,
     repo_name: str,
+    account_type: Union[Unset, None, str] = "github",
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
 ) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
     """Validate Repo Service
 
      API to validate a service with supported service schema. The checks include
 
     - Presence of service.yaml in ./oblivious folder.
     - Presence of Dockerfile in ./oblivious folder.
     - Content of service.yaml must be valid with respect to supported service schema.
 
+    This API is deprecated and will not be supported from upcoming releases. Kindly use **PUT
+    /service/dynamic** for adding/updating dynamic services
+
     Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
+        oblivious_user_id (str): User id
+        repo_owner (str): Repository owner for service
+        repo_name (str): Repository name for service
+        account_type (Union[Unset, None, str]): VCS type. Only supported input is github Default:
+            'github'.
+        ref (str): The reference tree of the repo
+        ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag Default: 'branch'.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        Union[HTTPValidationError, MessageModel, ServiceValidationResponse]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            ref=ref,
-            ref_type=ref_type,
-            account_type=account_type,
             oblivious_user_id=oblivious_user_id,
             repo_owner=repo_owner,
             repo_name=repo_name,
+            account_type=account_type,
+            ref=ref,
+            ref_type=ref_type,
         )
     ).parsed
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/user/add_user_public_shared_key_user_psk_put.py` & `oblv_ctl-0.4.1/oblv_ctl/api/deployment/create_new_deployment_deployment_static_post.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.create_deployment_response import CreateDeploymentResponse
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_model import MessageModel
-from ...models.psk import PSK
+from ...models.static_deployment_input import StaticDeploymentInput
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    json_body: PSK,
+    json_body: StaticDeploymentInput,
     oblivious_user_id: str,
 ) -> Dict[str, Any]:
-    url = "{}/user/psk".format(client.base_url)
+    url = "{}/deployment/static".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["oblivious_user_id"] = oblivious_user_id
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "put",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, PSK]]:
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = response.json()
-
+        response_200 = cast(Any, response.json())
         return response_200
+    if response.status_code == 201:
+        response_201 = CreateDeploymentResponse.from_dict(response.json())
+
+        return response_201
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
         raise HTTPClientError(request_id=response_500_request_id)
     if response.status_code == 422:
@@ -57,39 +63,45 @@
         report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
         raise ParamValidationError(report=report)
     if response.status_code == 403:
         raise UnauthorizedTokenError()
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: PSK,
+    json_body: StaticDeploymentInput,
     oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
+) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Create Deployment
 
-     API to update user's psk
+     API to create a new deployment.
 
     Args:
         oblivious_user_id (str):
-        json_body (PSK):
+        json_body (StaticDeploymentInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
+        Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     )
@@ -101,52 +113,60 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    json_body: PSK,
+    json_body: StaticDeploymentInput,
     oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
+) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Create Deployment
 
-     API to update user's psk
+     API to create a new deployment.
 
     Args:
         oblivious_user_id (str):
-        json_body (PSK):
+        json_body (StaticDeploymentInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
+        Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: PSK,
+    json_body: StaticDeploymentInput,
     oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
+) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Create Deployment
 
-     API to update user's psk
+     API to create a new deployment.
 
     Args:
         oblivious_user_id (str):
-        json_body (PSK):
+        json_body (StaticDeploymentInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
+        Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     )
@@ -156,27 +176,31 @@
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    json_body: PSK,
+    json_body: StaticDeploymentInput,
     oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
+) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Create Deployment
 
-     API to update user's psk
+     API to create a new deployment.
 
     Args:
         oblivious_user_id (str):
-        json_body (PSK):
+        json_body (StaticDeploymentInput):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
+        Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
             oblivious_user_id=oblivious_user_id,
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/api/user/update_user_password_user_password_put.py` & `oblv_ctl-0.4.1/oblv_ctl/api/user/update_user_password_user_password_put.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
     if response.status_code == 200:
-        response_200 = response.json()
+        response_200 = MessageModel.from_dict(response.json())
 
         return response_200
     if response.status_code == 400:
         response_400_message = response.json()["message"]
         raise BadRequestError(message=response_400_message)
     if response.status_code == 500:
         response_500_request_id = response.headers["apigw-requestid"]
@@ -77,19 +77,23 @@
     oblivious_user_id: str,
 ) -> Response[Union[HTTPValidationError, MessageModel]]:
     """Update User's Password
 
      API to update user's password
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
         json_body (UserPasswordInput):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     )
@@ -109,19 +113,23 @@
     oblivious_user_id: str,
 ) -> Optional[Union[HTTPValidationError, MessageModel]]:
     """Update User's Password
 
      API to update user's password
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
         json_body (UserPasswordInput):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     ).parsed
@@ -134,19 +142,23 @@
     oblivious_user_id: str,
 ) -> Response[Union[HTTPValidationError, MessageModel]]:
     """Update User's Password
 
      API to update user's password
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
         json_body (UserPasswordInput):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         oblivious_user_id=oblivious_user_id,
     )
@@ -164,19 +176,23 @@
     oblivious_user_id: str,
 ) -> Optional[Union[HTTPValidationError, MessageModel]]:
     """Update User's Password
 
      API to update user's password
 
     Args:
-        oblivious_user_id (str):
+        oblivious_user_id (str): User id
         json_body (UserPasswordInput):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
+        Union[HTTPValidationError, MessageModel]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
             oblivious_user_id=oblivious_user_id,
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/cli/main.py` & `oblv_ctl-0.4.1/oblv_ctl/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import typer
 from rich.text import Text
 
 from oblv_ctl import __version__, authenticate
 
-from . import deployment, service, utils
+from . import deployment, service, utils, static_service, marketplace
 
 app = typer.Typer(no_args_is_help=True, rich_markup_mode="markdown", help="""**Oblvious Controller v{}**   
 **Oblivious Software Ltd. <oblivious.ai>**  
 ======
   
 __Description__  
 
@@ -70,13 +70,14 @@
     except FileNotFoundError as e:
         utils.render_warning_message("Kindly login before performing this action")
     except Exception as e:
         if e.args[0]==utils.NO_CREDS_FOUND:
             utils.render_warning_message("Kindly login before performing this action")
     
 app.add_typer(service.app, name="service", help="Commands to interact with the services")
+app.add_typer(static_service.app, name="static-service", help="Commands to interact with the static services")
 app.add_typer(deployment.app, name="deployment", help="Commands to interact with the deployments")
-
+app.add_typer(marketplace.app, name="marketplace", help="Commands to interact with the marketplace services")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/cli/service.py` & `oblv_ctl-0.4.1/oblv_ctl/cli/service.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/cli/utils.py` & `oblv_ctl-0.4.1/oblv_ctl/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         client = OblvClient(oblivious_user_id=contents[0][1],token=contents[1][1])
     return client
 
 
 def render_output(object):
     if type(object)==list:
         console.print_json(data=[x.to_dict() for x in object])
+    elif type(object)==str:
+        console.print(object)
     else:
         console.print_json(data=object.to_dict())
         
 def render_success_message(message: str):
     print(
                 bcolors.GREEN
                 + "Success"
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/client.py` & `oblv_ctl-0.4.1/oblv_ctl/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 @attr.s(auto_attribs=True, repr=False)
 class Client:
     """A class for keeping track of data related to the API"""
         
     cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
     headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
-    timeout: float = attr.ib(20.0, kw_only=True)
+    timeout: float = attr.ib(50.0, kw_only=True)
     verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
     
     @property
     def base_url(self):
         return URL
 
     def get_headers(self) -> Dict[str, str]:
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/access_history.py` & `oblv_ctl-0.4.1/oblv_ctl/models/access_history.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 
 @attr.s(auto_attribs=True, repr=False)
 class AccessHistory:
     """
     Attributes:
         action (Union[Unset, str]):  Default: ''.
-        timestamp (Union[Unset, str]):  Default: ''.
+        timestamp (Union[Unset, str]):  Default: '21-05-2023 07:37:30'.
         oblivious_user_id (Union[Unset, str]):  Default: ''.
         role (Union[Unset, str]):
     """
 
     action: Union[Unset, str] = ""
-    timestamp: Union[Unset, str] = ""
+    timestamp: Union[Unset, str] = "21-05-2023 07:37:30"
     oblivious_user_id: Union[Unset, str] = ""
     role: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         action = self.action
         timestamp = self.timestamp
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/account.py` & `oblv_ctl-0.4.1/oblv_ctl/models/account.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/api_key.py` & `oblv_ctl-0.4.1/oblv_ctl/models/api_key.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/available_deployment.py` & `oblv_ctl-0.4.1/oblv_ctl/models/available_deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
-
 from .deployment_complete import DeploymentComplete
 
 T = TypeVar("T", bound="AvailableDeployment")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class AvailableDeployment:
     """
     Attributes:
         role (List[str]):
         deployment (DeploymentComplete):
     """
 
     role: List[str]
-    deployment: DeploymentComplete
+    deployment: "DeploymentComplete"
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         role = self.role
 
         deployment = self.deployment.to_dict()
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/available_deployment_list.py` & `oblv_ctl-0.4.1/oblv_ctl/models/available_deployment_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
-
 from .available_deployment import AvailableDeployment
 
 T = TypeVar("T", bound="AvailableDeploymentList")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class AvailableDeploymentList:
     """
     Attributes:
         total_pages (int):
-        deployments (List[AvailableDeployment]):
+        deployments (List['AvailableDeployment']):
     """
 
     total_pages: int
-    deployments: List[AvailableDeployment]
+    deployments: List["AvailableDeployment"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         total_pages = self.total_pages
         deployments = []
         for deployments_item_data in self.deployments:
             deployments_item = deployments_item_data.to_dict()
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/build_args_schema.py` & `oblv_ctl-0.4.1/oblv_ctl/models/build_args_schema.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_input.py` & `oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_input.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,8 @@
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
     def __str__(self):
         return json.dumps(self.to_dict(), indent=2)
 
     def __repr__(self):
-        return str(self)
+        return str(self)
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/create_deployment_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/create_deployment_response.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/deployment_complete.py` & `oblv_ctl-0.4.1/oblv_ctl/models/deployment_complete.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
-from ..models.access_history import AccessHistory
-from ..models.instance import Instance
-from ..models.shared_users import SharedUsers
 from ..types import UNSET, Unset
+from .instance import Instance
+from .shared_users import SharedUsers
+from .access_history import AccessHistory
 
 T = TypeVar("T", bound="DeploymentComplete")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class DeploymentComplete:
     """
@@ -31,16 +31,17 @@
         owner_login (Union[Unset, str]):  Default: ''.
         is_deleted (Union[Unset, bool]):
         instance (Union[Unset, Instance]):
         pcr_codes (Union[Unset, List[str]]):
         credit_utilization_per_hour (Union[Unset, float]):
         total_credits_used (Union[Unset, float]):
         build_args (Union[Unset, Any]):
-        shared_users (Union[Unset, List[SharedUsers]]):
-        history (Union[Unset, List[AccessHistory]]):
+        shared_users (Union[Unset, List['SharedUsers']]):
+        history (Union[Unset, List['AccessHistory']]):
+        service_id (str):
     """
 
     deployment_id: Union[Unset, str] = ""
     deployment_name: Union[Unset, str] = ""
     owner: Union[Unset, str] = ""
     repo_name: Union[Unset, str] = ""
     account_type: Union[Unset, str] = ""
@@ -50,21 +51,22 @@
     current_state: Union[Unset, str] = ""
     visibility: Union[Unset, str] = ""
     is_dev_env: Union[Unset, bool] = True
     creation_time: Union[Unset, str] = ""
     sha: Union[Unset, str] = ""
     owner_login: Union[Unset, str] = ""
     is_deleted: Union[Unset, bool] = False
-    instance: Union[Unset, Instance] = UNSET
+    instance: Union[Unset, "Instance"] = UNSET
     pcr_codes: Union[Unset, List[str]] = UNSET
     credit_utilization_per_hour: Union[Unset, float] = 0.0
     total_credits_used: Union[Unset, float] = 0.0
     build_args: Union[Unset, Any] = UNSET
-    shared_users: Union[Unset, List[SharedUsers]] = UNSET
-    history: Union[Unset, List[AccessHistory]] = UNSET
+    shared_users: Union[Unset, List["SharedUsers"]] = UNSET
+    history: Union[Unset, List["AccessHistory"]] = UNSET
+    service_id: Union[Unset, str] = ""
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         deployment_id = self.deployment_id
         deployment_name = self.deployment_name
         owner = self.owner
         repo_name = self.repo_name
@@ -105,14 +107,16 @@
         if not isinstance(self.history, Unset):
             history = []
             for history_item_data in self.history:
                 history_item = history_item_data.to_dict()
 
                 history.append(history_item)
 
+        service_id = self.service_id
+        
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if deployment_id is not UNSET:
             field_dict["deployment_id"] = deployment_id
         if deployment_name is not UNSET:
             field_dict["deployment_name"] = deployment_name
@@ -152,15 +156,16 @@
             field_dict["total_credits_used"] = total_credits_used
         if build_args is not UNSET:
             field_dict["build_args"] = build_args
         if shared_users is not UNSET:
             field_dict["shared_users"] = shared_users
         if history is not UNSET:
             field_dict["history"] = history
-
+        if service_id is not UNSET:
+            field_dict["service_id"] = service_id
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         deployment_id = d.pop("deployment_id", UNSET)
 
@@ -216,14 +221,16 @@
 
         history = []
         _history = d.pop("history", UNSET)
         for history_item_data in _history or []:
             history_item = AccessHistory.from_dict(history_item_data)
 
             history.append(history_item)
+            
+        service_id = d.pop("service_id", UNSET)
 
         deployment_complete = cls(
             deployment_id=deployment_id,
             deployment_name=deployment_name,
             owner=owner,
             repo_name=repo_name,
             account_type=account_type,
@@ -240,14 +247,15 @@
             instance=instance,
             pcr_codes=pcr_codes,
             credit_utilization_per_hour=credit_utilization_per_hour,
             total_credits_used=total_credits_used,
             build_args=build_args,
             shared_users=shared_users,
             history=history,
+            service_id=service_id
         )
 
         deployment_complete.additional_properties = d
         return deployment_complete
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/deployment_list.py` & `oblv_ctl-0.4.1/oblv_ctl/models/deployment_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
-
 from .deployment_complete import DeploymentComplete
 
 T = TypeVar("T", bound="DeploymentList")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class DeploymentList:
     """
     Attributes:
         total_pages (int):
-        deployments (List[DeploymentComplete]):
+        deployments (List['DeploymentComplete']):
     """
 
     total_pages: int
-    deployments: List[DeploymentComplete]
+    deployments: List["DeploymentComplete"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         total_pages = self.total_pages
         deployments = []
         for deployments_item_data in self.deployments:
             deployments_item = deployments_item_data.to_dict()
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/deployment_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/deployment_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
-from ..models.instance import Instance
-from ..models.shared_users import SharedUsers
 from ..types import UNSET, Unset
+from .instance import Instance
+from .shared_users import SharedUsers
 
 T = TypeVar("T", bound="DeploymentResponse")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class DeploymentResponse:
     """
@@ -28,15 +28,15 @@
         pcr_codes (Union[Unset, List[str]]):
         credit_utilization_per_hour (Union[Unset, float]):
         creation_time (Union[Unset, str]):  Default: ''.
         sha (Union[Unset, str]):  Default: ''.
         is_deleted (Union[Unset, bool]):
         build_args (Union[Unset, Any]):
         instance (Union[Unset, Instance]):
-        shared_users (Union[Unset, List[SharedUsers]]):
+        shared_users (Union[Unset, List['SharedUsers']]):
     """
 
     deployment_id: Union[Unset, str] = ""
     deployment_name: Union[Unset, str] = ""
     owner_login: Union[Unset, str] = ""
     repo_name: Union[Unset, str] = ""
     account_type: Union[Unset, str] = ""
@@ -46,18 +46,18 @@
     current_state: Union[Unset, str] = ""
     visibility: Union[Unset, str] = ""
     is_dev_env: Union[Unset, bool] = True
     pcr_codes: Union[Unset, List[str]] = UNSET
     credit_utilization_per_hour: Union[Unset, float] = 0.0
     creation_time: Union[Unset, str] = ""
     sha: Union[Unset, str] = ""
-    is_deleted: Union[Unset,bool] = UNSET
+    is_deleted: Union[Unset, bool] = False
     build_args: Union[Unset, Any] = UNSET
-    instance: Union[Unset, Instance] = UNSET
-    shared_users: Union[Unset, List[SharedUsers]] = UNSET
+    instance: Union[Unset, "Instance"] = UNSET
+    shared_users: Union[Unset, List["SharedUsers"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         deployment_id = self.deployment_id
         deployment_name = self.deployment_name
         owner_login = self.owner_login
         repo_name = self.repo_name
@@ -74,16 +74,15 @@
         pcr_codes: Union[Unset, List[str]] = UNSET
         if not isinstance(self.pcr_codes, Unset):
             pcr_codes = self.pcr_codes
 
         credit_utilization_per_hour = self.credit_utilization_per_hour
         creation_time = self.creation_time
         sha = self.sha
-        if not isinstance(self.is_deleted, Unset):
-            is_deleted = self.is_deleted
+        is_deleted = self.is_deleted
         build_args = self.build_args
         instance: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.instance, Unset):
             instance = self.instance.to_dict()
 
         shared_users: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.shared_users, Unset):
@@ -165,15 +164,15 @@
         pcr_codes = cast(List[str], d.pop("pcr_codes", UNSET))
 
         credit_utilization_per_hour = d.pop("credit_utilization_per_hour", UNSET)
 
         creation_time = d.pop("creation_time", UNSET)
 
         sha = d.pop("sha", UNSET)
-        
+
         is_deleted = d.pop("is_deleted", UNSET)
 
         build_args = d.pop("build_args", UNSET)
 
         _instance = d.pop("instance", UNSET)
         instance: Union[Unset, Instance]
         if isinstance(_instance, Unset):
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/http_validation_error.py` & `oblv_ctl-0.4.1/oblv_ctl/models/http_validation_error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
-
-from ..models.validation_error import ValidationError
+from .validation_error import ValidationError
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="HTTPValidationError")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class HTTPValidationError:
     """
     Attributes:
-        detail (Union[Unset, List[ValidationError]]):
+        detail (Union[Unset, List['ValidationError']]):
     """
 
-    detail: Union[Unset, List[ValidationError]] = UNSET
+    detail: Union[Unset, List["ValidationError"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         detail: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.detail, Unset):
             detail = []
             for detail_item_data in self.detail:
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/instance.py` & `oblv_ctl-0.4.1/oblv_ctl/models/instance.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/message_model.py` & `oblv_ctl-0.4.1/oblv_ctl/models/message_model.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/name_input.py` & `oblv_ctl-0.4.1/oblv_ctl/models/service_yaml_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,35 @@
 import json
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="NameInput")
+T = TypeVar("T", bound="ServiceYamlContent")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class NameInput:
-    """
-    Attributes:
-        name (Union[Unset, str]):  Default: ''.
-    """
+class ServiceYamlContent:
+    """ """
 
-    name: Union[Unset, str] = ""
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if name is not UNSET:
-            field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name", UNSET)
-
-        name_input = cls(
-            name=name,
-        )
+        service_yaml_content = cls()
 
-        name_input.additional_properties = d
-        return name_input
+        service_yaml_content.additional_properties = d
+        return service_yaml_content
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/notification_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/notification_response.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/oblv_auth_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/oblv_auth_response.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/psk.py` & `oblv_ctl-0.4.1/oblv_ctl/models/psk.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 T = TypeVar("T", bound="PSK")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class PSK:
     """
     Attributes:
-        public_key (str):
+        public_key (str): Publically shareable key
     """
 
     public_key: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         public_key = self.public_key
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/ref_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/ref_response.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/repo.py` & `oblv_ctl-0.4.1/oblv_ctl/models/repo.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/repo_all_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/repo_all_response.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/repo_service_list.py` & `oblv_ctl-0.4.1/oblv_ctl/models/name_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,49 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.validated_service import ValidatedService
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="RepoServiceList")
+T = TypeVar("T", bound="NameInput")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class RepoServiceList:
+class NameInput:
     """
     Attributes:
-        total_pages (int):
-        services (List[ValidatedService]):
+        name (str): Name of the user
     """
 
-    total_pages: int
-    services: List[ValidatedService]
+    name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        total_pages = self.total_pages
-        services = []
-        for services_item_data in self.services:
-            services_item = services_item_data.to_dict()
-
-            services.append(services_item)
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "total_pages": total_pages,
-                "services": services,
+                "name": name,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        total_pages = d.pop("total_pages")
+        name = d.pop("name")
 
-        services = []
-        _services = d.pop("services")
-        for services_item_data in _services:
-            services_item = ValidatedService.from_dict(services_item_data)
-
-            services.append(services_item)
-
-        repo_services_list = cls(
-            total_pages=total_pages,
-            services=services,
+        name_input = cls(
+            name=name,
         )
 
-        repo_services_list.additional_properties = d
-        return repo_services_list
+        name_input.additional_properties = d
+        return name_input
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/role_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/role_response.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/service_content_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/static_service_arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ServiceContentResponse")
+T = TypeVar("T", bound="StaticServiceArguments")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class ServiceContentResponse:
+class StaticServiceArguments:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        service_content_response = cls()
+        static_service_arguments = cls()
 
-        service_content_response.additional_properties = d
-        return service_content_response
+        static_service_arguments.additional_properties = d
+        return static_service_arguments
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/service_validation_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/service_list_market_place_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.validated_service import ValidatedService
 from ..types import UNSET, Unset
+from .market_place_service import MarketPlaceService
 
-T = TypeVar("T", bound="ServiceValidationResponse")
+T = TypeVar("T", bound="ServiceListMarketPlaceService")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class ServiceValidationResponse:
+class ServiceListMarketPlaceService:
     """
     Attributes:
-        message (Union[Unset, str]):  Default: ''.
-        service (Union[Unset, ValidatedService]):
+        total_pages (Union[Unset, int]):
+        services (Union[Unset, List['MarketPlaceService']]):
     """
 
-    message: Union[Unset, str] = ""
-    service: Union[Unset, ValidatedService] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    total_pages: Union[Unset, int] = 0
+    services: Union[Unset, List["MarketPlaceService"]] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
-        message = self.message
-        service: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.service, Unset):
-            service = self.service.to_dict()
+        total_pages = self.total_pages
+        services: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.services, Unset):
+            services = []
+            for services_item_data in self.services:
+                services_item = services_item_data.to_dict()
+
+                services.append(services_item)
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update({})
-        if message is not UNSET:
-            field_dict["message"] = message
-        if service is not UNSET:
-            field_dict["service"] = service
+        if total_pages is not UNSET:
+            field_dict["total_pages"] = total_pages
+        if services is not UNSET:
+            field_dict["services"] = services
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        message = d.pop("message", UNSET)
+        total_pages = d.pop("total_pages", UNSET)
 
-        _service = d.pop("service", UNSET)
-        service: Union[Unset, ValidatedService]
-        if isinstance(_service, Unset):
-            service = UNSET
-        else:
-            service = ValidatedService.from_dict(_service)
-
-        service_validation_response = cls(
-            message=message,
-            service=service,
+        services = []
+        _services = d.pop("services", UNSET)
+        for services_item_data in _services or []:
+            services_item = MarketPlaceService.from_dict(services_item_data)
+
+            services.append(services_item)
+
+        service_list_market_place_service = cls(
+            total_pages=total_pages,
+            services=services,
         )
 
-        service_validation_response.additional_properties = d
-        return service_validation_response
-
+        return service_list_market_place_service
+    
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
@@ -73,8 +74,8 @@
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
     def __str__(self):
         return json.dumps(self.to_dict(), indent=2)
 
     def __repr__(self):
-        return str(self)
+        return str(self)
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_add_input.py` & `oblv_ctl-0.4.1/oblv_ctl/models/supported_regions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ServiceYamlAddInput")
+T = TypeVar("T", bound="SupportedRegions")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class ServiceYamlAddInput:
+class SupportedRegions:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        service_yaml_add_input = cls()
+        supported_regions = cls()
 
-        service_yaml_add_input.additional_properties = d
-        return service_yaml_add_input
+        supported_regions.additional_properties = d
+        return supported_regions
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/service_yaml_update_input.py` & `oblv_ctl-0.4.1/oblv_ctl/models/old_add_repo_service_repo_service_post_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ServiceYamlUpdateInput")
+T = TypeVar("T", bound="OldAddRepoServiceRepoServicePostData")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class ServiceYamlUpdateInput:
+class OldAddRepoServiceRepoServicePostData:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        service_yaml_update_input = cls()
+        old_add_repo_service_repo_service_post_data = cls()
 
-        service_yaml_update_input.additional_properties = d
-        return service_yaml_update_input
+        old_add_repo_service_repo_service_post_data.additional_properties = d
+        return old_add_repo_service_repo_service_post_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/shared_users.py` & `oblv_ctl-0.4.1/oblv_ctl/models/shared_users.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/supported_regions.py` & `oblv_ctl-0.4.1/oblv_ctl/models/static_deployment_input_users.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SupportedRegions")
+T = TypeVar("T", bound="StaticDeploymentInputUsers")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class SupportedRegions:
+class StaticDeploymentInputUsers:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        supported_regions = cls()
+        static_deployment_input_users = cls()
 
-        supported_regions.additional_properties = d
-        return supported_regions
+        static_deployment_input_users.additional_properties = d
+        return static_deployment_input_users
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/user_credit_utilization.py` & `oblv_ctl-0.4.1/oblv_ctl/models/user_credit_utilization.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/user_password_input.py` & `oblv_ctl-0.4.1/oblv_ctl/models/user_password_input.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 T = TypeVar("T", bound="UserPasswordInput")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class UserPasswordInput:
     """
     Attributes:
-        old_password (str):
-        password (str):
+        old_password (str): Old password of user
+        password (str): New password for user. It must contain a capital letter, a small letter, a digit, and a special
+            character. Allowed special characters are - '#', '?', '!', '@', '$', '%', '^', '&', '*', '-'
     """
 
     old_password: str
     password: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/user_profile_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/user_profile_response.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/user_service_list.py` & `oblv_ctl-0.4.1/oblv_ctl/models/service_validation_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 import json
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from .user_services import UserServices
 from ..types import UNSET, Unset
+from .dynamic_service import DynamicService
 
-T = TypeVar("T", bound="UserServiceList")
+T = TypeVar("T", bound="ServiceValidationResponse")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class UserServiceList:
+class ServiceValidationResponse:
     """
     Attributes:
-        total_pages (int):
-        services (List[UserServices]):
+        message (Union[Unset, str]):  Default: ''.
+        service (Union[Unset, DynamicService]):
     """
 
-    total_pages: int
-    services: List[UserServices]
+    message: Union[Unset, str] = ""
+    service: Union[Unset, "DynamicService"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        total_pages = self.total_pages
-        services = []
-        for services_item_data in self.services:
-            services_item = services_item_data.to_dict()
-
-            services.append(services_item)
+        message = self.message
+        service: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.service, Unset):
+            service = self.service.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "total_pages": total_pages,
-                "services": services,
-            }
-        )
+        field_dict.update({})
+        if message is not UNSET:
+            field_dict["message"] = message
+        if service is not UNSET:
+            field_dict["service"] = service
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        total_pages = d.pop("total_pages")
+        message = d.pop("message", UNSET)
 
-        services = []
-        _services = d.pop("services")
-        for services_item_data in _services:
-            services_item = UserServices.from_dict(services_item_data)
-
-            services.append(services_item)
-
-        user_services_list = cls(
-            total_pages=total_pages,
-            services=services,
+        _service = d.pop("service", UNSET)
+        service: Union[Unset, DynamicService]
+        if isinstance(_service, Unset):
+            service = UNSET
+        else:
+            service = DynamicService.from_dict(_service)
+
+        service_validation_response = cls(
+            message=message,
+            service=service,
         )
 
-        user_services_list.additional_properties = d
-        return user_services_list
+        service_validation_response.additional_properties = d
+        return service_validation_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/user_services.py` & `oblv_ctl-0.4.1/oblv_ctl/models/repo_dynamic_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,73 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UserServices")
+T = TypeVar("T", bound="RepoDynamicService")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class UserServices:
+class RepoDynamicService:
     """
     Attributes:
-        repo_name (Union[Unset, str]):  Default: ''.
-        repo_owner (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: ''.
         ref (Union[Unset, str]):  Default: ''.
         service_validated (Union[Unset, bool]):
         sha (Union[Unset, str]):  Default: ''.
         type (Union[Unset, str]):  Default: ''.
     """
 
-    repo_name: Union[Unset, str] = ""
-    repo_owner: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = ""
     ref: Union[Unset, str] = ""
     service_validated: Union[Unset, bool] = False
     sha: Union[Unset, str] = ""
     type: Union[Unset, str] = ""
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        repo_name = self.repo_name
-        repo_owner = self.repo_owner
-        account_type = self.account_type
         ref = self.ref
         service_validated = self.service_validated
         sha = self.sha
         type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if repo_name is not UNSET:
-            field_dict["repo_name"] = repo_name
-        if repo_owner is not UNSET:
-            field_dict["repo_owner"] = repo_owner
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
         if ref is not UNSET:
             field_dict["ref"] = ref
         if service_validated is not UNSET:
             field_dict["service_validated"] = service_validated
         if sha is not UNSET:
             field_dict["sha"] = sha
         if type is not UNSET:
             field_dict["type"] = type
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        repo_name = d.pop("repo_name", UNSET)
-
-        repo_owner = d.pop("repo_owner", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
         ref = d.pop("ref", UNSET)
 
         service_validated = d.pop("service_validated", UNSET)
 
         sha = d.pop("sha", UNSET)
 
         type = d.pop("type", UNSET)
 
-        user_services = cls(
-            repo_name=repo_name,
-            repo_owner=repo_owner,
-            account_type=account_type,
+        repo_dynamic_service = cls(
             ref=ref,
             service_validated=service_validated,
             sha=sha,
             type=type,
         )
 
-        user_services.additional_properties = d
-        return user_services
+        repo_dynamic_service.additional_properties = d
+        return repo_dynamic_service
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/validated_service.py` & `oblv_ctl-0.4.1/oblv_ctl/models/dynamic_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ValidatedService")
+T = TypeVar("T", bound="DynamicService")
 
 
 @attr.s(auto_attribs=True, repr=False)
-class ValidatedService:
+class DynamicService:
     """
     Attributes:
         ref (Union[Unset, str]):  Default: ''.
         service_validated (Union[Unset, bool]):  Default: True.
         sha (Union[Unset, str]):  Default: ''.
         type (Union[Unset, str]):  Default: ''.
     """
@@ -51,23 +51,23 @@
 
         service_validated = d.pop("service_validated", UNSET)
 
         sha = d.pop("sha", UNSET)
 
         type = d.pop("type", UNSET)
 
-        validated_service = cls(
+        dynamic_service = cls(
             ref=ref,
             service_validated=service_validated,
             sha=sha,
             type=type,
         )
 
-        validated_service.additional_properties = d
-        return validated_service
+        dynamic_service.additional_properties = d
+        return dynamic_service
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/validation_error.py` & `oblv_ctl-0.4.1/oblv_ctl/models/validation_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import json
-from typing import Any, Dict, List, Type, TypeVar, cast
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 T = TypeVar("T", bound="ValidationError")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class ValidationError:
     """
     Attributes:
-        loc (List[str]):
+        loc (List[Union[int, str]]):
         msg (str):
         type (str):
     """
 
-    loc: List[str]
+    loc: List[Union[int, str]]
     msg: str
     type: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        loc = self.loc
+        loc = []
+        for loc_item_data in self.loc:
+            loc_item: Union[int, str]
+
+            loc_item = loc_item_data
+
+            loc.append(loc_item)
 
         msg = self.msg
         type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
@@ -37,15 +43,24 @@
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        loc = cast(List[str], d.pop("loc"))
+        loc = []
+        _loc = d.pop("loc")
+        for loc_item_data in _loc:
+
+            def _parse_loc_item(data: object) -> Union[int, str]:
+                return cast(Union[int, str], data)
+
+            loc_item = _parse_loc_item(loc_item_data)
+
+            loc.append(loc_item)
 
         msg = d.pop("msg")
 
         type = d.pop("type")
 
         validation_error = cls(
             loc=loc,
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/models/vcs_repo_response.py` & `oblv_ctl-0.4.1/oblv_ctl/models/vcs_repo_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import json
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
-
-from ..models.repo import Repo
+from .repo import Repo
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="VCSRepoResponse")
 
 
 @attr.s(auto_attribs=True, repr=False)
 class VCSRepoResponse:
     """
     Attributes:
-        repos (Union[Unset, List[Repo]]):
+        repos (Union[Unset, List['Repo']]):
         total_pages (Union[Unset, int]):
         message (Union[Unset, str]):  Default: ''.
     """
 
-    repos: Union[Unset, List[Repo]] = UNSET
+    repos: Union[Unset, List["Repo"]] = UNSET
     total_pages: Union[Unset, int] = 0
     message: Union[Unset, str] = ""
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         repos: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.repos, Unset):
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/oblv_client.py` & `oblv_ctl-0.4.1/oblv_ctl/oblv_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,165 +1,189 @@
-import requests
+"""OblvClient
+
+Python Client for calling open APIs supported by Oblivious
+
+"""
 import sys
+import requests
 from jsonschema import validate
 from jsonschema.exceptions import ValidationError
+from oblv_ctl.exceptions import BadRequestError
 from oblv_ctl.models.name_input import NameInput
-from .api.account import get_user_accounts_account_get
-from .api.auth import logout_session_logout_delete
-from .api.deployment import (
+from oblv_ctl.api.account import get_user_accounts_user_account_get
+from oblv_ctl.api.auth import logout_session_logout_delete
+from oblv_ctl.api.deployment import (
     create_new_deployment_deployment_post,
     delete_deployment_deployment_delete,
     generate_build_args_deployment_arguments_get,
     get_available_deployments_deployment_available_get,
     get_deployment_info_deployment_get,
     get_deployment_roles_deployment_roles_get,
     get_supported_regions_deployment_supported_regions_get,
     get_user_owned_deployments_deployment_owned_get,
+    create_new_deployment_deployment_static_post
 )
-from .api.repo import (
+from oblv_ctl.api.repo import (
     get_all_repos_repo_linked_get,
     get_repo_from_vcs_repo_get,
     get_repo_refs_repo_refs_get,
     get_repo_repo_repo_owner_repo_name_get,
     search_repo_from_vcs_repo_search_get,
 )
-from .api.service import (
-    add_repo_service_repo_service_post,
-    delete_repo_services_repo_service_delete,
-    get_repo_service_yaml_form_content_repo_service_yaml_get,
-    get_repo_services_repo_service_get,
-    get_user_services_service_get,
-    update_repo_service_repo_service_put,
-    validate_repo_service_repo_service_validate_get,
+from oblv_ctl.api.service import (
+    add_update_repo_dynamic_service_service_dynamic_put,
+    delete_dynamic_service_service_dynamic_delete,
+    get_repo_dynamic_services_repo_service_get,
+    get_user_dynamic_services_user_service_dynamic_get,
+    get_service_yaml_content_repo_service_data_get,
+    create_static_service_service_static_post,
+    get_static_service_service_static_get,
+    get_user_static_services_user_service_static_get,
+    get_marketplace_services_service_marketplace_get,
+    request_marketplace_addition_service_marketplace_request_put,
+    delete_static_service_service_static_delete,
+    get_static_service_build_logs_service_static_logs_get,
+    get_docker_image_service_static_docker_get,
+    remove_service_from_marketplace_service_marketplace_delete
 )
-from .api.user import (
+from oblv_ctl.api.user import (
     add_user_public_shared_key_user_psk_put,
     get_user_deployment_credit_usage_user_credit_usage_get,
     get_user_profile_view_user_profile_get,
     get_user_public_shared_key_user_psk_get,
     update_user_name_user_name_put,
     update_user_password_user_password_put,
 )
-from .client import AuthenticatedClient
-from .config import URL
-from .exceptions import BadYamlData
-from .models import (
+from oblv_ctl.client import AuthenticatedClient
+from oblv_ctl.config import URL
+from oblv_ctl.exceptions import BadYamlData
+from oblv_ctl.models import (
     PSK,
     CreateDeploymentInput,
-    ServiceYamlAddInput,
-    ServiceYamlUpdateInput,
     UserPasswordInput,
+    DynamicServiceYamlInput,
+    StaticServiceInput,
+    StaticDeploymentInput
 )
 from .utils import bcolors
 
 
-class OblvClient(AuthenticatedClient):
-    def _method_wrapper(function):
+def _method_wrapper(function):
+        """
+        A wrapper method for exception logging
+        """
+
         def wrap(*args, **kwargs):
+            """Method to call the requested method in try-catch block"""
+
             try:
                 return function(*args, **kwargs)
-            except Exception as e:
-                reason = e.__str__()
+            except Exception as exception:
                 print(
-                bcolors.RED
-                + bcolors.BOLD
-                + "Exception"
-                + bcolors.BLACK
-                + bcolors.ENDC
-                + f": {e}",
-                file=sys.stderr,
-            )
-                raise Exception(reason)
+                    bcolors.RED
+                    + bcolors.BOLD
+                    + "Exception"
+                    + bcolors.BLACK
+                    + bcolors.ENDC
+                    + f": {str(exception)}",
+                    file=sys.stderr,
+                )
+                raise exception
 
         return wrap
 
+class OblvClient(AuthenticatedClient):
+    """
+    Client for making API calls to Oblivious
+    """
+
     @_method_wrapper
     def logout(self):
         """Logout Session
 
-         This API invalidates the user's token. After a successul response, the user will not be able to use
-        the auth token provided in the auth APIs.
+        This API invalidates the user's token.
+
+        After a successul response, the user will not be able to use the auth token provided in the auth APIs.
 
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
+            None
         """
         try:
             logout_session_logout_delete.sync(
                 client=self, oblivious_user_id=self.oblivious_user_id
             )
-        except Exception as e:
-            raise e
+        except Exception as exception:
+            raise exception
         finally:
             self.token = ""
             self.oblivious_user_id = ""
 
     ###### Account Method ######
 
     @_method_wrapper
     def accounts(self):
         """Get User Accounts
          API to fetch user's linked VCS accounts
         Returns:
-            Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
+            List[Account]
         """
-        return get_user_accounts_account_get.sync(
+        return get_user_accounts_user_account_get.sync(
             client=self, oblivious_user_id=self.oblivious_user_id
         )
 
     ############################
 
     ####### User Methods #######
     @_method_wrapper
     def psk(self):
         """Get User PSK
          API to fetch user's psk
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, str]]
+            str
         """
         return get_user_public_shared_key_user_psk_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             user_id=self.oblivious_user_id,
         )
 
     @_method_wrapper
     def credit_usage(self):
         """Get User Credit Usage
          API to fetch user's credit usage
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, UserCreditUtilization]]
+            UserCreditUtilization
         """
         return get_user_deployment_credit_usage_user_credit_usage_get.sync(
             client=self, oblivious_user_id=self.oblivious_user_id
         )
 
     @_method_wrapper
     def set_psk(self, public_key):
         """Update user's publically shareable key
         API to update user's publically shareable key
         Args:
             public_key (str): Public Key to be shared
         Returns:
-            Response[Union[None, HTTPValidationError, MessageModel]]
-            None is returned if successful
+            None
         """
 
-        input = PSK(public_key)
+        json_body = PSK(public_key)
         return add_user_public_shared_key_user_psk_put.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id, json_body=input
+            client=self, oblivious_user_id=self.oblivious_user_id, json_body=json_body
         )
 
     @_method_wrapper
     def update_name(self, name):
         """Update Name
         API to update the name.
         Args:
             name (str): User Name
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
+            None
         """
         update_user_name_user_name_put.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             json_body=NameInput(name),
         )
 
@@ -167,28 +191,27 @@
     def update_password(self, old_pass, new_pass):
         """Update User's Password
          API to update user's password
         Args:
             old_pass (str): Old Password
             new_pass (str): New Password
         Returns:
-            Response[Union[None, HTTPValidationError, MessageModel]]
-                None is returned if successful
+            None
         """
-        input = UserPasswordInput(old_password=old_pass, password=new_pass)
+        json_body = UserPasswordInput(old_password=old_pass, password=new_pass)
         update_user_password_user_password_put.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id, json_body=input
+            client=self, oblivious_user_id=self.oblivious_user_id, json_body=json_body
         )
 
     @_method_wrapper
     def user_profile(self):
         """Get User Profile
          API to fetch user's profile details
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, UserProfileResponse]]
+            UserProfileResponse
         """
         return get_user_profile_view_user_profile_get.sync(
             client=self, oblivious_user_id=self.oblivious_user_id
         )
 
     ############################
 
@@ -197,57 +220,56 @@
     def get_repo(self, owner, name):
         """Get User Repo
          API to fetch user's repo information
         Args:
             owner (str): Repo Owner
             name (str): Repo Name
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, Repo]]
+            Repo
         """
         return get_repo_repo_repo_owner_repo_name_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             repo_owner=owner,
             repo_name=name,
         )
 
     @_method_wrapper
     def search_repo(self, keyword):
         """Add Repo Service With Yaml
-         API to search a repository in VCS, on which the user has access (via their own account, or by any
-        organization they are member of).
+         API to search a repository in VCS, on which the user has access.
         Args:
             keyword (str): Search Keyword
         Returns:
-            Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+            List[Repo]
         """
         return search_repo_from_vcs_repo_search_get.sync(
             client=self, oblivious_user_id=self.oblivious_user_id, search_string=keyword
         )
 
     @_method_wrapper
     def linked_repos(self):
         """Get User Repos
          API to fetch user's repo without services
         Returns:
-            Response[Union[Any, HTTPValidationError, List[RepoAllResponse], MessageModel]]
+            List[RepoAllResponse]
         """
         return get_all_repos_repo_linked_get.sync(
             client=self, oblivious_user_id=self.oblivious_user_id
         )
 
     @_method_wrapper
     def repo_refs(self, owner, name):
         """Get Repo Refs
          API to fetch the repository refs (branches and tags).
         Args:
             owner (str): Repo Owner
             name (str): Repo Name
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, RefResponse]]
+            RefResponse
         """
         return get_repo_refs_repo_refs_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             repo_owner=owner,
             repo_name=name,
         )
@@ -257,15 +279,15 @@
         """Get Repos From VCS
          API to get all the repositories from VCS, on which the user has access (via their own account, or by
         any organization they are member of).
         Args:
             page (int):  Page (Default 1)
             per_page (int):  Repositiories Per Page (Default 10)
         Returns:
-            Response[Union[Any, HTTPValidationError, VCSRepoResponse]]
+            VCSRepoResponse
         """
         return get_repo_from_vcs_repo_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             page=page,
             per_page=per_page,
         )
@@ -276,85 +298,94 @@
     @_method_wrapper
     def add_service(
         self,
         repo_owner: str,
         repo_name: str,
         ref: str,
         ref_type: str = "branch",
-        data: dict = {},
+        data: dict = None,
     ):
         """Add Repo Service
          API to create a service after validation.
         Args:
             repo_owner (str): Repo's Owner Name
             repo_name (str): Repo Name
             ref (str): Service Ref
             ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
             data (dict): Service Yaml Content in dictionary format. If provided, service.yaml file will be created/updated based on its existence.
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
+            ServiceValidationResponse
         """
-        if data != {}:
+        if data:
             try:
-                req = requests.get(URL + "/service_schema")
+                req = requests.get(URL + "/service_schema", timeout=self.timeout)
                 if req.status_code != 200:
-                    raise Exception("Failed to validate service yaml data")
+                    raise BadRequestError("Failed to validate service yaml data")
                 validate(data, req.json())
-            except ValidationError as e:
-                raise BadYamlData(e.message)
-            except Exception as e:
-                raise e
-        input = ServiceYamlAddInput.from_dict(data)
-        return add_repo_service_repo_service_post.sync(
+            except ValidationError as exception:
+                raise BadYamlData(exception.message) from exception
+            except Exception as exception:
+                raise exception
+        json_body = DynamicServiceYamlInput.from_dict(data)
+        return add_update_repo_dynamic_service_service_dynamic_put.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             ref=ref,
             ref_type=ref_type,
             repo_owner=repo_owner,
             repo_name=repo_name,
-            json_body=input,
+            json_body=json_body,
         )
 
     @_method_wrapper
     def remove_service(
         self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
     ):
         """Delete Repo Service
          API to delete a service. It does not delete the existing deployments created from this service.
         Args:
             repo_owner (str): Repo's Owner Name
             repo_name (str): Repo Name
             ref (str): Service Ref
             ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
+            None
         """
-        return delete_repo_services_repo_service_delete.sync(
+        delete_dynamic_service_service_dynamic_delete.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             ref=ref,
             ref_type=ref_type,
             repo_name=repo_name,
             repo_owner=repo_owner,
         )
 
     @_method_wrapper
     def service_content(
         self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
     ):
-        """Get Repo Service Yaml
-         API to fetch the service.yaml content as object for the given service.
+        """Get Service Yaml Content
+
+         API to fetch the service.yaml content as object for the given ref. The ref need not be a service. It
+        returns the sample service, if service.yaml not found.
+
         Args:
-            repo_id (Union[Unset, str]): Repo Id
             ref (str): Service Ref
-            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
+            ref_type (Union[Unset, None, str]): Whether the ref is a branch or tag. Default: 'branch'.
+            repo_owner (str): Repository owner for service
+            repo_name (str): Repository name for service
+
+        Raises:
+            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            httpx.TimeoutException: If the request takes longer than Client.timeout.
+
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceContentResponse]]
+            ServiceYamlContent
         """
-        return get_repo_service_yaml_form_content_repo_service_yaml_get.sync(
+        return get_service_yaml_content_repo_service_data_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             repo_owner=repo_owner,
             repo_name=repo_name,
             ref=ref,
             ref_type=ref_type,
         )
@@ -365,22 +396,33 @@
         repo_owner: str,
         repo_name: str,
         page: int = 1,
         per_page: int = 10,
         get_all: bool = False,
     ):
         """Get Repo Services
-         API to fetch all the services available for the given repository. This API is valid only for linked
-        repositories.
+
+         Fetch all the services available for the given repository.
+
         Args:
-            repo_id (str): Repo Id
+            page (Union[Unset, None, int]): Requested page Default: 1.
+            per_page (Union[Unset, None, int]): Responses per page Default: 10.
+            get_all (Union[Unset, None, bool]): Get all responses. Precedence over *page* and
+                *per_page* parameters
+            repo_owner (str): Repository owner for service
+            repo_name (str): Repository name for service
+
+        Raises:
+            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            httpx.TimeoutException: If the request takes longer than Client.timeout.
+
         Returns:
-            Response[Union[Any, HTTPValidationError, List[ValidatedService], MessageModel]]
+            ServiceListRepoDynamicService
         """
-        return get_repo_services_repo_service_get.sync(
+        return get_repo_dynamic_services_repo_service_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             repo_owner=repo_owner,
             repo_name=repo_name,
             page=page,
             per_page=per_page,
             get_all=get_all,
@@ -399,17 +441,17 @@
         Args:
             page (int):  Page (Default 1)
             per_page (str): services per page (Default 10)
             search_keyword (str): Search Keyword and is applied on repo full name (Default "")
             get_all (bool): To fetch all services at once (Default False)
 
         Returns:
-            Response[Union[Any, HTTPValidationError, List[UserServices], MessageModel]]
+            UserServiceListUserDynamicService
         """
-        return get_user_services_service_get.sync(
+        return get_user_dynamic_services_user_service_dynamic_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             page=page,
             per_page=per_page,
             get_all=get_all,
             search_term=search_keyword,
         )
@@ -417,47 +459,47 @@
     @_method_wrapper
     def update_service(
         self,
         repo_owner: str,
         repo_name: str,
         ref,
         ref_type: str = "branch",
-        data: dict = {},
+        data: dict = None,
     ):
         """Update Repo Service With Yaml
          API to update a service, along with updating the service.yaml file. After updating the service.yaml file, the service is validate as well (for missing Dockerfile).
         Args:
             repo_owner (str): Repo's Owner Name
             repo_name (str): Repo Name
             ref (str): Service Ref
             ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
             data (dict): Service Yaml Content in dictionary format. If provided, service.yaml file will be created/updated based on its existence.
 
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
+            ServiceValidationResponse
         """
-        if data != {}:
+        if data:
             try:
-                req = requests.get(URL + "/service_schema")
+                req = requests.get(URL + "/service_schema", timeout=self.timeout)
                 if req.status_code != 200:
-                    raise Exception("Failed to validate service yaml data")
+                    raise BadRequestError("Failed to validate service yaml data")
                 validate(data, req.json())
-            except ValidationError as e:
-                raise BadYamlData(e.message)
-            except Exception as e:
-                raise e
-        input = ServiceYamlUpdateInput.from_dict(data)
-        return update_repo_service_repo_service_put.sync(
+            except ValidationError as exception:
+                raise BadYamlData(exception.message) from exception
+            except Exception as exception:
+                raise exception
+        json_body = DynamicServiceYamlInput.from_dict(data)
+        return add_update_repo_dynamic_service_service_dynamic_put.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             ref=ref,
             ref_type=ref_type,
             repo_owner=repo_owner,
             repo_name=repo_name,
-            json_body=input,
+            json_body=json_body,
         )
 
     @_method_wrapper
     def revalidate_service(
         self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
     ):
         """Validate Repo Service
@@ -467,136 +509,351 @@
         - Content of service.yaml must be valid with respect to supported service schema.
         Args:
             repo_owner (str): Repo's Owner Name
             repo_name (str): Repo Name
             ref (str): Service Ref
             ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
+            ServiceValidationResponse
         """
-        return validate_repo_service_repo_service_validate_get.sync(
+        json_body = DynamicServiceYamlInput.from_dict({})
+        return add_update_repo_dynamic_service_service_dynamic_put.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
+            ref=ref,
+            ref_type=ref_type,
             repo_owner=repo_owner,
             repo_name=repo_name,
+            json_body=json_body,
+        )
+
+    @_method_wrapper
+    def add_static_service(
+        self,
+        name: str,
+        description: str,
+        repo_owner: str,
+        repo_name: str,
+        ref: str,
+        arguments: dict = None,
+    ) -> None:
+        """Add Static Service
+        Create a new static/pre-built service.
+
+        Args:
+            repo_owner (str): Repo's Owner Name
+            repo_name (str): Repo Name
+            name (str): Service name. The name should start with an alphabet and can only contain numbers, alphabets, '_',
+            '-'
+            description (str): Service description
+            ref (str): The commit sha or the ref from which the service is to be created.
+            arguments (Union[Unset, StaticServiceInputArguments]): The arguments for docker build. From your service.yaml,
+                the arguments added under "build_args".
+        """
+        if arguments is None:
+            arguments = {}
+        json_body = StaticServiceInput(
+            name=name,
+            description=description,
+            repo_full_name="/".join([repo_owner, repo_name]),
             ref=ref,
-            ref_type=ref_type,
+            arguments=arguments,
+        )
+        result = create_static_service_service_static_post.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            json_body=json_body,
+        )
+        print(result)
+
+    @_method_wrapper
+    def user_static_services(
+        self,
+        page: int = 1,
+        per_page: int = 10,
+        get_all: bool = False,
+        search_keyword: str = "",
+    ):
+        """Get User Services
+         API to fetch user's services
+        Args:
+            page (int):  Page (Default 1)
+            per_page (str): services per page (Default 10)
+            search_keyword (str): Search Keyword and is applied on repo full name (Default "")
+            get_all (bool): To fetch all services at once (Default False)
+
+        Returns:
+            UserServiceListUserStaticService
+        """
+        return get_user_static_services_user_service_static_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            page=page,
+            per_page=per_page,
+            get_all=get_all,
+            search_term=search_keyword,
+        )
+
+    @_method_wrapper
+    def get_static_service(self, service: str):
+        """Get User Services
+         API to fetch user's services
+        Args:
+            oblivious_user_id (str): User id
+            service (str): Service name or id
+
+        Returns:
+            StaticService
+        """
+        return get_static_service_service_static_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, service=service
+        )
+
+    @_method_wrapper
+    def delete_static_service(self, service: str):
+        """Get User Services
+         API to fetch user's services
+        Args:
+            oblivious_user_id (str): User id
+            service (str): Service name or id
+
+        Returns:
+            None
+        """
+        delete_static_service_service_static_delete.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, service=service
+        )
+
+    @_method_wrapper
+    def marketplace_services(
+        self,
+        page: int = 1,
+        per_page: int = 10,
+        get_all: bool = False,
+        name_filter: str = "",
+        repo_filter: str = "",
+    ):
+        """Get marketplace services
+
+         To get all the marketplace services. These are the static services publically available for
+        everyone's use.
+
+        Args:
+            page (Union[Unset, None, int]): Requested page Default: 1.
+            per_page (Union[Unset, None, int]): Responses per page Default: 10.
+            get_all (Union[Unset, None, bool]): Get all responses. Precedence over *page* and
+                *per_page* parameters
+            name_filter (Union[Unset, None, str]): Name filter for services Default: ''.
+            repo_filter (Union[Unset, None, str]): Repo filter for services Default: ''.
+
+        Returns:
+           ServiceListMarketPlaceService
+        """
+
+        return get_marketplace_services_service_marketplace_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            page=page,
+            per_page=per_page,
+            get_all=get_all,
+            name_filter=name_filter,
+            repo_filter=repo_filter,
+        )
+
+    @_method_wrapper
+    def add_service_to_marketplace(self, service: str):
+        """Request to move a static service to marketplace
+
+         Request a static service to be made available in the marketplace.
+
+        Args:
+            service (str): Service name or id
+
+        Returns:
+            None
+        """
+        request_marketplace_addition_service_marketplace_request_put.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, service=service
+        )
+
+    @_method_wrapper
+    def remove_service_from_marketplace(self, service: str):
+        """Remove from Marketplace
+
+        Remove a service from marketplace.
+
+        Args:
+            service (str): Service name or id
+
+        Returns:
+            None
+        """
+        remove_service_from_marketplace_service_marketplace_delete.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, service=service
+        )
+    
+    @_method_wrapper
+    def get_static_service_docker_logs(self, service: str):
+        """Get Build Logs
+
+        Get build logs for static service build
+
+        Args:
+            service (str): Service name or id
+
+        Returns:
+            str
+        """
+        return get_static_service_build_logs_service_static_logs_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, service=service
+        )
+
+    @_method_wrapper
+    def get_docker_image_url(self, service: str):
+        """Get static service docker image download url
+
+        To fetch download url of docker image for the static service. 
+        
+        Use this pre-signed url to download the docker image or directly load to docker.
+        
+        To load the image directly to docker execute the command -
+        "wget <url> | docker load"
+
+        Args:
+            service (str): Service name or id
+
+        Returns:
+            str
+        """
+        return get_docker_image_service_static_docker_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, service=service
         )
 
     ############################
 
     #### Deployment Methods ####
 
     @_method_wrapper
     def deployment_info(self, deployment_id):
         """Get Deployment
          API to fetch a deployment's details.
         Args:
             deployment_id (str): Deployment Id
         Returns:
-            Response[Union[Any, DeploymentResponse, HTTPValidationError, MessageModel]]
+            DeploymentResponse
         """
         return get_deployment_info_deployment_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             deployment_id=deployment_id,
         )
 
     @_method_wrapper
     def create_deployment(self, deployment: CreateDeploymentInput):
         """Create Deployment
          API to create a new deployment.
         Args:
             deployment (CreateDeploymentInput): Deployment Details Input
         Returns:
-            Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
+            CreateDeploymentResponse
         """
         return create_new_deployment_deployment_post.sync(
             client=self, oblivious_user_id=self.oblivious_user_id, json_body=deployment
         )
 
     @_method_wrapper
+    def create_static_service_deployment(self, deployment: StaticDeploymentInput):
+        """Create Deployment
+         API to create a new deployment from static service.
+        Args:
+            deployment (StaticDeploymentInput): Deployment Details Input
+        Returns:
+            CreateDeploymentResponse
+        """
+        return create_new_deployment_deployment_static_post.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, json_body=deployment
+        )
+
+
+    @_method_wrapper
     def remove_deployment(self, deployment_id):
         """Delete Deployment
          API to initiate termination of a deployment.
         Args:
             deployment_id (str): Deployment Id
         Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
+            MessageModel
         """
         return delete_deployment_deployment_delete.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             deployment_id=deployment_id,
         )
 
     @_method_wrapper
-    def generate_deployment_build_args(
-        self, owner: str, repo: str, ref: str, ref_type: str = "branch"
-    ):
+    def generate_deployment_build_args(self, owner: str, repo: str, ref: str):
         """Get Build Deployment Arguments
         API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
         at which point it was generated. This is to be passed to the create deployment API.
         Note - A service could have different build args schema depending on the service's commit history.
         Args:
             owner (str): Repo Owner
             repo (str): Repo Name
             ref (str): Service Ref
-            ref_type (str): Ref Type branch/tag (Default 'branch')
         Returns:
-            Response[Union[Any, BuildArgsSchema, HTTPValidationError, MessageModel]]
+            BuildArgsSchema
         """
         return generate_build_args_deployment_arguments_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             repo=repo,
             owner=owner,
             ref=ref,
         )
 
     @_method_wrapper
     def available_deployments(self):
         """Get Available Deployments
          API to fetch all the deployments the user can connect to.
         Returns:
-            Response[Union[Any, HTTPValidationError, List[DeploymentComplete], MessageModel]]
+            List[DeploymentComplete]
         """
         return get_available_deployments_deployment_available_get.sync(
             client=self, oblivious_user_id=self.oblivious_user_id
         )
 
     @_method_wrapper
     def deployment_roles(self, deployment_id):
         """Get Deployment Roles
          API to get a deployment's roles.
         Args:
             deployment_id (str): Deployment Id
         Returns:
-            Response[Union[Any, HTTPValidationError, List[RoleResponse], MessageModel]]
+            List[RoleResponse]
         """
         return get_deployment_roles_deployment_roles_get.sync(
             client=self,
             oblivious_user_id=self.oblivious_user_id,
             deployment_id=deployment_id,
         )
 
     @_method_wrapper
     def supported_aws_regions(self):
         """Deployment Supported Regions
          API to fetch a deployment's details.
         Returns:
-            Response[Union[Any, MessageModel]]
+            dict
         """
         return get_supported_regions_deployment_supported_regions_get.sync(client=self)
 
     @_method_wrapper
     def deployments(self):
         """Get Owned Deployments
          API to fetch a user's owned deployments.
         Returns:
-            Response[Union[Any, HTTPValidationError, List[DeploymentResponse], MessageModel]]
+            List[DeploymentResponse]
         """
         return get_user_owned_deployments_deployment_owned_get.sync(
             client=self, oblivious_user_id=self.oblivious_user_id
         )
 
     ############################
```

### Comparing `oblv_ctl-0.3.1/oblv_ctl/types.py` & `oblv_ctl-0.4.1/oblv_ctl/types.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/oblv_ctl/utils.py` & `oblv_ctl-0.4.1/oblv_ctl/utils.py`

 * *Files identical despite different names*

### Comparing `oblv_ctl-0.3.1/pyproject.toml` & `oblv_ctl-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 58.0.4", "wheel >= 0.37.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "oblv-ctl"
-version = "0.3.1"
+version = "0.4.1"
 description = "A client library for accessing Oblivious APIs"
 authors = ["Oblivious Support <support@oblivious.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/ObliviousAI/oblv-ctl"
 homepage = "https://github.com/ObliviousAI/oblv-ctl/tree/master/README.md"
 keywords = ["Oblivious", "python", "package"]
```

### Comparing `oblv_ctl-0.3.1/README.md` & `oblv_ctl-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 client = authenticate(apikey=*your_key_here*)
 ```
 
 
 Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
 
 
+The deployments can be created in two ways - using a pre-built static service or dynamically deploying the code.
 
+# Dynamic Service Deployment
 ### 1 Create a service
 
 A service refers to a branch/tag of your repository that needs to be
 deployed. For your first service. you can use the repository
 [ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
 Execute the below command to create the service.
 
@@ -170,14 +172,15 @@
 ```
 
 
 On successful request, enclave creation is initiated, and it returns an
 id for the deployment, which can be later used to track the status and
 connection details for the enclave.
 
+### 3 Enclave Information
 To check the state of the deployment, run
 
 ``` {.python}
 client.deployment_info(response.deployment_id).current_state
 ```
 
 > 'CFT Initiated'
@@ -207,7 +210,46 @@
 
 ``` {.python}
 client.deployment_info(response.deployment_id).pcr_codes
 ```
 
 >['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
 'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+
+
+# Static Service Deployment
+In this type of deployment, services are prebuilt and kept ahead of time. You can either create you static service first and then go ahead for deployment, or you could simply use a service available in marketplace.
+
+### 1 Create a service
+Execute the below command to create a static service.
+
+```python
+oblv_client.add_static_service(
+    name="first deployment",
+    description="First Static Service creation",
+    repo_owner="ObliviousAI",
+    repo_name="FastAPI-Enclave-Services",
+    ref="60d7c177be25cc9758520580f78f7d6b135b17c8",
+    arguments={}
+)
+```
+
+
+### 2 Enclave Creation
+Execute the below command to create deployment from static service. 
+
+```python
+from oblv_ctl.models import StaticDeploymentInput
+obj = StaticDeploymentInput(
+    service="<service_id>",
+    deployment_name="first_static_deployment",
+    region_name="us-east-1",
+    is_dev_env=True,
+    runtime_args="somthing",
+    users = {"somerole": [{"user_name": "<your name>", "public key": "<your public key>"}]},
+    infra_reqs="m5.xlarge",
+    marketplace=False
+)
+oblv_client.create_static_service_deployment(obj)
+```
+
+The next steps for getting deployment information and the pcr codes are same for both the service types and can be found [here](#3-enclave-information).
```

### Comparing `oblv_ctl-0.3.1/PKG-INFO` & `oblv_ctl-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oblv-ctl
-Version: 0.3.1
+Version: 0.4.1
 Summary: A client library for accessing Oblivious APIs
 Home-page: https://github.com/ObliviousAI/oblv-ctl/tree/master/README.md
 License: Apache-2.0
 Keywords: Oblivious,python,package
 Author: Oblivious Support
 Author-email: support@oblivious.ai
 Requires-Python: >=3.7,<4.0
@@ -40,15 +40,17 @@
 client = authenticate(apikey=*your_key_here*)
 ```
 
 
 Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
 
 
+The deployments can be created in two ways - using a pre-built static service or dynamically deploying the code.
 
+# Dynamic Service Deployment
 ### 1 Create a service
 
 A service refers to a branch/tag of your repository that needs to be
 deployed. For your first service. you can use the repository
 [ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
 Execute the below command to create the service.
 
@@ -196,14 +198,15 @@
 ```
 
 
 On successful request, enclave creation is initiated, and it returns an
 id for the deployment, which can be later used to track the status and
 connection details for the enclave.
 
+### 3 Enclave Information
 To check the state of the deployment, run
 
 ``` {.python}
 client.deployment_info(response.deployment_id).current_state
 ```
 
 > 'CFT Initiated'
@@ -234,7 +237,45 @@
 ``` {.python}
 client.deployment_info(response.deployment_id).pcr_codes
 ```
 
 >['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
 'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
 
+
+# Static Service Deployment
+In this type of deployment, services are prebuilt and kept ahead of time. You can either create you static service first and then go ahead for deployment, or you could simply use a service available in marketplace.
+
+### 1 Create a service
+Execute the below command to create a static service.
+
+```python
+oblv_client.add_static_service(
+    name="first deployment",
+    description="First Static Service creation",
+    repo_owner="ObliviousAI",
+    repo_name="FastAPI-Enclave-Services",
+    ref="60d7c177be25cc9758520580f78f7d6b135b17c8",
+    arguments={}
+)
+```
+
+
+### 2 Enclave Creation
+Execute the below command to create deployment from static service. 
+
+```python
+from oblv_ctl.models import StaticDeploymentInput
+obj = StaticDeploymentInput(
+    service="<service_id>",
+    deployment_name="first_static_deployment",
+    region_name="us-east-1",
+    is_dev_env=True,
+    runtime_args="somthing",
+    users = {"somerole": [{"user_name": "<your name>", "public key": "<your public key>"}]},
+    infra_reqs="m5.xlarge",
+    marketplace=False
+)
+oblv_client.create_static_service_deployment(obj)
+```
+
+The next steps for getting deployment information and the pcr codes are same for both the service types and can be found [here](#3-enclave-information).
```

