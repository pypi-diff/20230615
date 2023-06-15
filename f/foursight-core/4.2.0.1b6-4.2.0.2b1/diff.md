# Comparing `tmp/foursight_core-4.2.0.1b6.tar.gz` & `tmp/foursight_core-4.2.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.2.0.1b6.tar", max compression
+gzip compressed data, was "foursight_core-4.2.0.2b1.tar", max compression
```

## Comparing `foursight_core-4.2.0.1b6.tar` & `foursight_core-4.2.0.2b1.tar`

### file list

```diff
@@ -1,77 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-06-08 17:29:21.521993 foursight_core-4.2.0.1b6/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-08 17:29:21.526873 foursight_core-4.2.0.1b6/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-08 17:29:21.526949 foursight_core-4.2.0.1b6/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-06-08 17:29:21.527000 foursight_core-4.2.0.1b6/foursight_core/app.py
--rw-r--r--   0        0        0   105128 2023-06-08 17:29:21.527440 foursight_core-4.2.0.1b6/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-06-08 17:29:21.527526 foursight_core-4.2.0.1b6/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-06-08 17:29:21.527588 foursight_core-4.2.0.1b6/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-06-08 17:29:21.527638 foursight_core-4.2.0.1b6/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-06-08 17:29:21.527760 foursight_core-4.2.0.1b6/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-06-08 17:29:21.527854 foursight_core-4.2.0.1b6/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4476 2023-06-08 17:29:21.527928 foursight_core-4.2.0.1b6/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-06-08 17:29:21.527988 foursight_core-4.2.0.1b6/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-06-08 17:29:21.528055 foursight_core-4.2.0.1b6/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-06-08 17:29:21.528131 foursight_core-4.2.0.1b6/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-06-08 17:29:21.528189 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-06-08 17:29:21.528252 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-06-08 17:29:21.528315 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-06-08 17:29:21.528380 foursight_core-4.2.0.1b6/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-06-08 17:29:21.528450 foursight_core-4.2.0.1b6/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-06-08 17:29:21.528510 foursight_core-4.2.0.1b6/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-06-08 17:29:21.528602 foursight_core-4.2.0.1b6/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-06-08 17:29:21.528695 foursight_core-4.2.0.1b6/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-06-08 17:29:21.528782 foursight_core-4.2.0.1b6/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-06-08 17:29:21.528862 foursight_core-4.2.0.1b6/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-06-08 17:29:21.529002 foursight_core-4.2.0.1b6/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5408 2023-06-09 17:22:22.577742 foursight_core-4.2.0.1b6/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-06-08 17:29:21.529157 foursight_core-4.2.0.1b6/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-06-08 17:29:21.529223 foursight_core-4.2.0.1b6/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-06-08 17:29:21.529277 foursight_core-4.2.0.1b6/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-06-08 17:29:21.529456 foursight_core-4.2.0.1b6/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-06-08 17:29:21.529548 foursight_core-4.2.0.1b6/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-06-08 17:29:21.529665 foursight_core-4.2.0.1b6/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-06-08 17:29:21.529880 foursight_core-4.2.0.1b6/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-06-08 17:29:21.529963 foursight_core-4.2.0.1b6/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-06-08 17:29:21.530084 foursight_core-4.2.0.1b6/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-06-08 17:29:21.530276 foursight_core-4.2.0.1b6/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-06-08 17:29:21.530400 foursight_core-4.2.0.1b6/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-06-08 17:29:21.530486 foursight_core-4.2.0.1b6/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-06-08 17:29:21.530563 foursight_core-4.2.0.1b6/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-06-08 17:29:21.530634 foursight_core-4.2.0.1b6/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-06-08 17:29:21.530710 foursight_core-4.2.0.1b6/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-06-08 17:29:21.530775 foursight_core-4.2.0.1b6/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-06-08 17:29:21.530838 foursight_core-4.2.0.1b6/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-06-08 17:29:21.530928 foursight_core-4.2.0.1b6/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-06-08 17:29:21.531018 foursight_core-4.2.0.1b6/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    80660 2023-06-09 17:22:22.578116 foursight_core-4.2.0.1b6/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-06-08 17:29:21.531406 foursight_core-4.2.0.1b6/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-06-08 17:29:21.531496 foursight_core-4.2.0.1b6/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    34216 2023-06-08 17:29:28.846377 foursight_core-4.2.0.1b6/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-06-08 17:29:21.531697 foursight_core-4.2.0.1b6/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-06-08 17:29:21.531762 foursight_core-4.2.0.1b6/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-06-08 17:29:21.531853 foursight_core-4.2.0.1b6/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-06-08 17:29:21.531916 foursight_core-4.2.0.1b6/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-06-08 17:29:21.531964 foursight_core-4.2.0.1b6/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-06-08 17:29:21.532567 foursight_core-4.2.0.1b6/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1935185 2023-06-09 17:22:22.585038 foursight_core-4.2.0.1b6/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-06-08 17:29:21.541812 foursight_core-4.2.0.1b6/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-06-08 17:29:21.541900 foursight_core-4.2.0.1b6/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-06-08 17:29:21.541974 foursight_core-4.2.0.1b6/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-06-08 17:29:21.542064 foursight_core-4.2.0.1b6/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-06-08 17:29:21.542130 foursight_core-4.2.0.1b6/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-06-08 17:29:21.542227 foursight_core-4.2.0.1b6/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-06-08 17:29:21.542277 foursight_core-4.2.0.1b6/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-06-08 17:29:21.542349 foursight_core-4.2.0.1b6/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-06-08 17:29:21.542414 foursight_core-4.2.0.1b6/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-06-08 17:29:21.542590 foursight_core-4.2.0.1b6/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-06-08 17:29:21.542697 foursight_core-4.2.0.1b6/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-06-08 17:29:21.542772 foursight_core-4.2.0.1b6/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-06-08 17:29:21.542860 foursight_core-4.2.0.1b6/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-06-08 17:29:21.542929 foursight_core-4.2.0.1b6/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-06-08 17:29:21.542988 foursight_core-4.2.0.1b6/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-06-08 17:29:21.543055 foursight_core-4.2.0.1b6/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-06-08 17:29:21.543139 foursight_core-4.2.0.1b6/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-06-08 17:29:21.543191 foursight_core-4.2.0.1b6/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1627 2023-06-09 17:22:22.585934 foursight_core-4.2.0.1b6/pyproject.toml
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b6/setup.py
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-15 13:43:17.505303 foursight_core-4.2.0.2b1/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-15 13:43:17.509303 foursight_core-4.2.0.2b1/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-15 13:43:17.509303 foursight_core-4.2.0.2b1/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-15 13:43:17.509303 foursight_core-4.2.0.2b1/foursight_core/app.py
+-rw-r--r--   0        0        0   105128 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     5222 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5408 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    81027 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-15 13:43:17.513303 foursight_core-4.2.0.2b1/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1936472 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-15 13:43:17.525303 foursight_core-4.2.0.2b1/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1633 2023-06-15 13:43:17.529303 foursight_core-4.2.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 foursight_core-4.2.0.2b1/PKG-INFO
```

### Comparing `foursight_core-4.2.0.1b6/LICENSE.txt` & `foursight_core-4.2.0.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/abstract_connection.py` & `foursight_core-4.2.0.2b1/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/app_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/buckets.py` & `foursight_core-4.2.0.2b1/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/check_schema.py` & `foursight_core-4.2.0.2b1/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/check_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/access_key_expiration_detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,24 +65,29 @@
         except Exception:
             continue  # user not found
         user_uuid = user['uuid']
         access_keys = search_metadata(f'/search/?type=AccessKey&description={kp_name}&user.uuid={user_uuid}'
                                       f'&sort=-date_created', key=connection.ff_keys)
         # generate new key
         access_key_req = {'user': user_uuid, 'description': kp_name}
-        access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)['@graph'][0]
-        s3_obj = {'secret': access_key_res['secret_access_key'],
-                  'key': access_key_res['access_key_id'],
-                  'server': s3.url}
+        # 2020-06-13/dmichaels: The actual result returned by the portal for this POST is not what
+        # seems to be expected; the access_key_id and secret_access_key are not within the @graph
+        # array; but handle both cases just in case; maybe that as an older (or newer) API.
+        # access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)['@graph'][0]
+        access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)
+        access_key_id = access_key_res['access_key_id'] if 'access_key_id' in access_key_res else None
+        secret_access_key = access_key_res['secret_access_key'] if 'secret_access_key' in access_key_res else None
+        if not access_key_id:
+            access_key_id = access_key_res['@graph'][0]['access_key_id']
+        if not secret_access_key:
+            secret_access_key = access_key_res['@graph'][0]['secret_access_key']
+        s3_obj = {'secret': secret_access_key, 'key': access_key_id, 'server': s3.url}
         s3.s3_put_secret(json.dumps(s3_obj), kp_name)
         full_output['successfully_generated'].append(email)
         # clear out old keys after generating new one
         for access_key in access_keys:  # note this search result was computed before the new key was added
             if access_key['status'] != 'deleted':
                 patch_metadata(patch_item={'status': 'deleted'}, obj_id=access_key['uuid'], key=connection.ff_keys)
 
     action.full_output = full_output
     action.status = 'DONE'
     return action
-
-
-
```

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/ecs_checks.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/scaling_checks.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/checks/test_checks.py` & `foursight_core-4.2.0.2b1/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/decorators.py` & `foursight_core-4.2.0.2b1/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/deploy.py` & `foursight_core-4.2.0.2b1/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/environment.py` & `foursight_core-4.2.0.2b1/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/es_connection.py` & `foursight_core-4.2.0.2b1/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/exceptions.py` & `foursight_core-4.2.0.2b1/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/fs_connection.py` & `foursight_core-4.2.0.2b1/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/identity.py` & `foursight_core-4.2.0.2b1/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/mapping.json` & `foursight_core-4.2.0.2b1/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/package.py` & `foursight_core-4.2.0.2b1/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/auth.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/auth0_config.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/aws_network.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/aws_s3.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/checks.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/cognito.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/encryption.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/envs.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/gac.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/misc_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/react_api.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/react_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,22 @@
         user_schema_properties = user_schema.get("properties") if user_schema else None
         user_schema_status = user_schema_properties.get("status") if user_schema_properties else None
         user_schema_status_enum = user_schema_status.get("enum") if user_schema_status else None
         if not user_schema_status_enum:
             return []
         return [{"id": status, "name": status, "title": status.title()} for status in user_schema_status_enum]
 
+    @classmethod
+    def _is_test_name(cls, name):
+        return isinstance(name, str) and name.startswith("test_x")
+
+    @classmethod
+    def _is_test_name_item(cls, item, property_name = "name"):
+        return isinstance(item, dict) and cls._is_test_name(item.get(property_name))
+
     def react_serve_static_file(self, env: str, paths: list) -> Response:
         """
         Called from react_routes for static endpoints: /{env}/{path}/{etc}
         Serves static UI related (JavaScript, CSS, HTML) files.
         Note that this in an UNPROTECTED route.
         """
         return self._react_ui.serve_static_file(env, paths)
@@ -1136,15 +1144,16 @@
         Called from react_routes for endpoint: GET /{env}/checks_validation
         Returns information about any problems with the checks setup.
         """
         ignored(request, env)
         response = {}
         checks_actions_registry = self._checks.get_registry()
         actions_with_no_associated_check = [item for _, item in checks_actions_registry.items()
-                                            if item.get("kind") == "action" and not item.get("checks")]
+                                            if item.get("kind") == "action" and not item.get("checks")
+                                            and not self._is_test_name_item(item)]
         if actions_with_no_associated_check:
             response["actions_with_no_associated_check"] = actions_with_no_associated_check
         return self.create_success_response(response)
 
     def reactapi_lambdas(self, request: dict, env: str) -> Response:
         """
         Called from react_routes for endpoint: GET /{env}/lambdas
```

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/react_api_base.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/react_routes.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/react_ui.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/ui/index.html` & `foursight_core-4.2.0.2b1/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.2.0.2b1/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.2.0.2b1/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.a8bddaf8.js.LICENSE.txt */
+/*! For license information please see main.b90e06b3.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -49323,19 +49323,23 @@
                                         })
                                     })]
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Creation Date:"
-                                }), (0, Kr.jsxs)("td", {
+                                }), (0, Kr.jsx)("td", {
                                     style: i,
-                                    children: [r.created_at, "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)("small", {
-                                        children: Pr.Ago(r.created_at, !0, !1)
-                                    })]
+                                    children: r.created_at ? (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: [r.created_at, "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)("small", {
+                                            children: Pr.Ago(r.created_at, !0, !1)
+                                        })]
+                                    }) : (0, Kr.jsx)(Kr.Fragment, {
+                                        children: "Not available"
+                                    })
                                 })]
                             }), (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Expiration Date:"
                                 }), (0, Kr.jsxs)("td", {
                                     style: i,
@@ -49349,16 +49353,18 @@
                                                 children: Pr.Ago(r.expires_at, !0, !1)
                                             })]
                                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                                             children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)("small", {
                                                 children: Pr.FromNow(r.expires_at, !0, !1)
                                             })]
                                         })
-                                    }) : (0, Kr.jsx)(Kr.Fragment, {
-                                        children: "None"
+                                    }) : (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: ["Not available", r.probably_expired ? (0, Kr.jsx)(Kr.Fragment, {
+                                            children: "\xa0(probably expired)"
+                                        }) : (0, Kr.jsx)(Kr.Fragment, {})]
                                     })]
                                 })]
                             }), r.exception && (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: s,
                                     children: "Details:"
                                 }), (0, Kr.jsx)("td", {
@@ -54588,14 +54594,15 @@
                                     children: Fr.X
                                 })
                             }), s.length > 0 ? (0, Kr.jsx)("div", {
                                 style: {
                                     marginTop: "4pt"
                                 },
                                 children: s.map((function(t) {
+                                    var n, r;
                                     return (0, Kr.jsx)("table", {
                                         children: (0, Kr.jsx)("tbody", {
                                             children: (0, Kr.jsxs)("tr", {
                                                 children: [(0, Kr.jsx)("td", {
                                                     style: {
                                                         verticalAlign: "top",
                                                         paddingTop: "4pt",
@@ -54657,25 +54664,59 @@
                                                                 height: "18"
                                                             })
                                                         }), (0, Kr.jsx)(Mi, {
                                                             id: "tooltip-search-".concat(t.name),
                                                             text: "Click to view source code for this check (in new tab).",
                                                             position: "bottom"
                                                         })]
-                                                    }), (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                                        className: "pointer",
-                                                        onClick: function() {
-                                                            return e.toggleShowGroup(e.findGroup(t.group), e.environ, e.groupList)
-                                                        },
-                                                        children: (0, Kr.jsx)("i", {
-                                                            children: t.group
-                                                        })
-                                                    }), " (", (0, Kr.jsx)("small", {
-                                                        children: t.name
-                                                    }), ")"]
+                                                    }), (0, Kr.jsx)("br", {}), (0, Kr.jsxs)("small", {
+                                                        children: [(0, Kr.jsx)("i", {
+                                                            children: "Group"
+                                                        }), ":\xa0", (0, Kr.jsx)("span", {
+                                                            className: "pointer",
+                                                            onClick: function() {
+                                                                return e.toggleShowGroup(e.findGroup(t.group), e.environ, e.groupList)
+                                                            },
+                                                            children: t.group.replace(/ checks$/i, "")
+                                                        }), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("i", {
+                                                            children: "Function:"
+                                                        }), "\xa0", t.registered_github_url ? (0, Kr.jsx)(Kr.Fragment, {
+                                                            children: (0, Kr.jsx)("a", {
+                                                                rel: "noreferrer",
+                                                                target: "_blank",
+                                                                href: t.registered_github_url,
+                                                                children: (0, Kr.jsxs)("span", {
+                                                                    style: {
+                                                                        color: "darkblue"
+                                                                    },
+                                                                    children: [t.module, (0, Kr.jsx)("b", {
+                                                                        style: {
+                                                                            marginLeft: "2px",
+                                                                            marginRight: "2px"
+                                                                        },
+                                                                        children: "."
+                                                                    }), t.name]
+                                                                })
+                                                            })
+                                                        }) : (0, Kr.jsxs)(Kr.Fragment, {
+                                                            children: [t.module, (0, Kr.jsx)("b", {
+                                                                style: {
+                                                                    marginLeft: "2px",
+                                                                    marginRight: "2px"
+                                                                },
+                                                                children: "."
+                                                            }), t.name]
+                                                        }), 1 == (null === (n = Object.keys(null === t || void 0 === t ? void 0 : t.schedule)) || void 0 === n ? void 0 : n.length) && (0, Kr.jsxs)(Kr.Fragment, {
+                                                            children: [(0, Kr.jsx)("br", {}), (0, Kr.jsxs)("small", {
+                                                                children: [(0, Kr.jsx)("i", {
+                                                                    children: "Schedule:"
+                                                                }), " ", null === (r = t.schedule[Object.keys(t.schedule)[0]]) || void 0 === r ? void 0 : r.cron_description]
+                                                            })]
+                                                        })]
+                                                    })]
                                                 })]
                                             })
                                         })
                                     }, t.name)
                                 }))
                             }) : (0, Kr.jsx)(Kr.Fragment, {
                                 children: (0, Kr.jsx)("div", {
@@ -57962,16 +58003,23 @@
                             style: {
                                 color: "inherit"
                             },
                             children: "View"
                         })]
                     });
                     if (null !== (r = t.data) && void 0 !== r && r.invalid) return (0, Kr.jsxs)(ms, {
-                        children: [(0, Kr.jsxs)("b", {
-                            children: ["Warning: Access key for associated Portal ", t.data.expired ? "has expired" : "is invalid"]
+                        children: [(0, Kr.jsx)(Mi, {
+                            id: "alert-access-key-invalid",
+                            position: "bottom",
+                            text: "Portal access key: ".concat(t.data.key)
+                        }), (0, Kr.jsxs)("b", {
+                            children: ["Alert: ", (0, Kr.jsx)("span", {
+                                id: "alert-access-key-invalid",
+                                children: "Access key"
+                            }), " for associated Portal ", t.data.expired ? "has expired" : t.data.probably_expired ? "has probably expired" : "is invalid"]
                         }), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                             to: kr.Path("/portal_access_key"),
                             style: {
                                 color: "inherit"
                             },
                             children: "View"
                         })]
```

### Comparing `foursight_core-4.2.0.1b6/foursight_core/route_prefixes.py` & `foursight_core-4.2.0.2b1/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/routes.py` & `foursight_core-4.2.0.2b1/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/run_result.py` & `foursight_core-4.2.0.2b1/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/s3_connection.py` & `foursight_core-4.2.0.2b1/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/schedule_decorator.py` & `foursight_core-4.2.0.2b1/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.2.0.2b1/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.2.0.2b1/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/sqs_utils.py` & `foursight_core-4.2.0.2b1/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/stage.py` & `foursight_core-4.2.0.2b1/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/base.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/header.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/history.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/info.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/unused.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/user.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/users.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/view_checks.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/foursight_core/templates/view_groups.html` & `foursight_core-4.2.0.2b1/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.1b6/pyproject.toml` & `foursight_core-4.2.0.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.2.0.1b6"  # to become 4.2.0
+version = "4.2.0.2b1"  # TODO: To become 4.3.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.2.0.1b6/PKG-INFO` & `foursight_core-4.2.0.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.2.0.1b6
+Version: 4.2.0.2b1
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

