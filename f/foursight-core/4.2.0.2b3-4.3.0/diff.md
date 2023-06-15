# Comparing `tmp/foursight_core-4.2.0.2b3.tar.gz` & `tmp/foursight_core-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.2.0.2b3.tar", max compression
+gzip compressed data, was "foursight_core-4.3.0.tar", max compression
```

## Comparing `foursight_core-4.2.0.2b3.tar` & `foursight_core-4.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-06-15 19:53:07.709405 foursight_core-4.2.0.2b3/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/app.py
--rw-r--r--   0        0        0   105128 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     5539 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5408 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    81026 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    34216 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-06-15 19:53:07.717404 foursight_core-4.2.0.2b3/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-06-15 19:53:07.721404 foursight_core-4.2.0.2b3/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-06-15 19:53:07.721404 foursight_core-4.2.0.2b3/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-06-15 19:53:07.721404 foursight_core-4.2.0.2b3/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-06-15 19:53:07.721404 foursight_core-4.2.0.2b3/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1936472 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-06-15 19:53:07.729405 foursight_core-4.2.0.2b3/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1633 2023-06-15 19:53:07.733404 foursight_core-4.2.0.2b3/pyproject.toml
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 foursight_core-4.2.0.2b3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-15 20:06:13.726802 foursight_core-4.3.0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/app.py
+-rw-r--r--   0        0        0   105128 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     5539 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5408 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    81026 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1936472 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1604 2023-06-15 20:06:13.750802 foursight_core-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 foursight_core-4.3.0/PKG-INFO
```

### Comparing `foursight_core-4.2.0.2b3/LICENSE.txt` & `foursight_core-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/abstract_connection.py` & `foursight_core-4.3.0/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/app_utils.py` & `foursight_core-4.3.0/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/buckets.py` & `foursight_core-4.3.0/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/check_schema.py` & `foursight_core-4.3.0/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/check_utils.py` & `foursight_core-4.3.0/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.3.0/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.3.0/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/ecs_checks.py` & `foursight_core-4.3.0/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.3.0/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.3.0/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.3.0/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/scaling_checks.py` & `foursight_core-4.3.0/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/checks/test_checks.py` & `foursight_core-4.3.0/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/decorators.py` & `foursight_core-4.3.0/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/deploy.py` & `foursight_core-4.3.0/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/environment.py` & `foursight_core-4.3.0/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/es_connection.py` & `foursight_core-4.3.0/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/exceptions.py` & `foursight_core-4.3.0/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/fs_connection.py` & `foursight_core-4.3.0/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/identity.py` & `foursight_core-4.3.0/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/mapping.json` & `foursight_core-4.3.0/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/package.py` & `foursight_core-4.3.0/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/auth.py` & `foursight_core-4.3.0/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/auth0_config.py` & `foursight_core-4.3.0/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/aws_network.py` & `foursight_core-4.3.0/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/aws_s3.py` & `foursight_core-4.3.0/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.3.0/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/checks.py` & `foursight_core-4.3.0/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/cognito.py` & `foursight_core-4.3.0/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.3.0/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.3.0/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.3.0/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/encryption.py` & `foursight_core-4.3.0/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/envs.py` & `foursight_core-4.3.0/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/gac.py` & `foursight_core-4.3.0/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.3.0/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/misc_utils.py` & `foursight_core-4.3.0/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.3.0/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/react_api.py` & `foursight_core-4.3.0/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/react_api_base.py` & `foursight_core-4.3.0/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.3.0/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/react_routes.py` & `foursight_core-4.3.0/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/react_ui.py` & `foursight_core-4.3.0/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.3.0/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/ui/index.html` & `foursight_core-4.3.0/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.3.0/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.3.0/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/route_prefixes.py` & `foursight_core-4.3.0/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/routes.py` & `foursight_core-4.3.0/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/run_result.py` & `foursight_core-4.3.0/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/s3_connection.py` & `foursight_core-4.3.0/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/schedule_decorator.py` & `foursight_core-4.3.0/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.3.0/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.3.0/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/sqs_utils.py` & `foursight_core-4.3.0/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/stage.py` & `foursight_core-4.3.0/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/base.html` & `foursight_core-4.3.0/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/header.html` & `foursight_core-4.3.0/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/history.html` & `foursight_core-4.3.0/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/info.html` & `foursight_core-4.3.0/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/unused.html` & `foursight_core-4.3.0/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/user.html` & `foursight_core-4.3.0/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/users.html` & `foursight_core-4.3.0/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/view_checks.html` & `foursight_core-4.3.0/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/foursight_core/templates/view_groups.html` & `foursight_core-4.3.0/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.2.0.2b3/pyproject.toml` & `foursight_core-4.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.2.0.2b3"  # TODO: To become 4.3.0
+version = "4.3.0"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.2.0.2b3/PKG-INFO` & `foursight_core-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.2.0.2b3
+Version: 4.3.0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

