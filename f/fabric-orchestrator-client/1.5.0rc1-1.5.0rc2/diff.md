# Comparing `tmp/fabric-orchestrator-client-1.5.0rc1.tar.gz` & `tmp/fabric-orchestrator-client-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.5.0rc1.tar", last modified: Thu May 11 17:40:36 2023, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.5.0rc2.tar", last modified: Fri May 12 13:46:59 2023, max compression
```

## Comparing `fabric-orchestrator-client-1.5.0rc1.tar` & `fabric-orchestrator-client-1.5.0rc2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      793 2023-05-11 17:37:01.210207 fabric-orchestrator-client-1.5.0rc1/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 17:37:01.210355 fabric-orchestrator-client-1.5.0rc1/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-05-11 17:37:01.210524 fabric-orchestrator-client-1.5.0rc1/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 17:37:01.210626 fabric-orchestrator-client-1.5.0rc1/.travis.yml
--rw-r--r--   0        0        0      770 2023-05-11 17:37:01.210729 fabric-orchestrator-client-1.5.0rc1/CODEGEN.md
--rw-r--r--   0        0        0     1071 2023-05-11 17:37:01.210862 fabric-orchestrator-client-1.5.0rc1/LICENSE
--rw-r--r--   0        0        0       59 2023-05-11 17:37:01.210963 fabric-orchestrator-client-1.5.0rc1/MANIFEST.in
--rw-r--r--   0        0        0     9238 2023-05-11 17:37:01.211113 fabric-orchestrator-client-1.5.0rc1/README.md
--rw-r--r--   0        0        0     4263 2023-05-11 17:37:01.211350 fabric-orchestrator-client-1.5.0rc1/docs/ResourcesApi.md
--rw-r--r--   0        0        0    17437 2023-05-11 17:37:01.211531 fabric-orchestrator-client-1.5.0rc1/docs/SlicesApi.md
--rw-r--r--   0        0        0     3740 2023-05-11 17:37:01.211677 fabric-orchestrator-client-1.5.0rc1/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2023-05-11 17:37:01.211789 fabric-orchestrator-client-1.5.0rc1/docs/Success.md
--rw-r--r--   0        0        0      352 2023-05-11 17:37:01.211912 fabric-orchestrator-client-1.5.0rc1/docs/Version.md
--rw-r--r--   0        0        0       25 2023-05-11 17:39:42.925010 fabric-orchestrator-client-1.5.0rc1/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:37:01.212158 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    18242 2023-05-11 17:37:01.212367 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3004 2023-05-11 17:37:01.212646 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      397 2023-05-11 17:37:01.212849 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0     9597 2023-05-11 17:37:01.213024 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    37827 2023-05-11 17:37:01.213284 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     8826 2023-05-11 17:37:01.213492 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2023-05-11 17:37:01.213724 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25128 2023-05-11 17:37:01.213944 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2023-05-11 17:37:01.214372 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     2496 2023-05-11 17:37:01.214654 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3055 2023-05-11 17:37:01.214908 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2023-05-11 17:37:01.215233 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     8496 2023-05-11 17:37:01.215453 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3435 2023-05-11 17:37:01.215578 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2023-05-11 17:37:01.215680 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0    10903 2023-05-11 17:37:01.215821 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2023-05-11 17:37:01.216181 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2023-05-11 17:37:01.216373 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2023-05-11 17:37:01.216668 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2023-05-11 17:37:01.216937 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2023-05-11 17:37:01.217164 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2023-05-11 17:37:01.217341 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2023-05-11 17:37:01.217534 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2023-05-11 17:37:01.217713 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2023-05-11 17:37:01.217919 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2023-05-11 17:37:01.218148 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2023-05-11 17:37:01.218431 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2023-05-11 17:37:01.218623 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2023-05-11 17:37:01.218944 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2023-05-11 17:37:01.219262 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2023-05-11 17:37:01.219487 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2023-05-11 17:37:01.219669 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2023-05-11 17:37:01.219920 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12988 2023-05-11 17:37:01.220174 fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 17:37:01.220383 fabric-orchestrator-client-1.5.0rc1/git_push.sh
--rw-r--r--   0        0        0     1027 2023-05-11 17:39:30.700751 fabric-orchestrator-client-1.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 17:37:01.221004 fabric-orchestrator-client-1.5.0rc1/test/__init__.py
--rw-r--r--   0        0        0      896 2023-05-11 17:37:01.221224 fabric-orchestrator-client-1.5.0rc1/test/test_resource.py
--rw-r--r--   0        0        0      950 2023-05-11 17:37:01.221397 fabric-orchestrator-client-1.5.0rc1/test/test_resources.py
--rw-r--r--   0        0        0     1206 2023-05-11 17:37:01.221693 fabric-orchestrator-client-1.5.0rc1/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2023-05-11 17:37:01.221929 fabric-orchestrator-client-1.5.0rc1/test/test_slice.py
--rw-r--r--   0        0        0      930 2023-05-11 17:37:01.222101 fabric-orchestrator-client-1.5.0rc1/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222270 fabric-orchestrator-client-1.5.0rc1/test/test_slices.py
--rw-r--r--   0        0        0     2018 2023-05-11 17:37:01.222442 fabric-orchestrator-client-1.5.0rc1/test/test_slices_api.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222608 fabric-orchestrator-client-1.5.0rc1/test/test_sliver.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.222785 fabric-orchestrator-client-1.5.0rc1/test/test_slivers.py
--rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223106 fabric-orchestrator-client-1.5.0rc1/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223296 fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2023-05-11 17:37:01.223607 fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2023-05-11 17:37:01.223847 fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.224081 fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2023-05-11 17:37:01.224292 fabric-orchestrator-client-1.5.0rc1/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2023-05-11 17:37:01.224535 fabric-orchestrator-client-1.5.0rc1/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2023-05-11 17:37:01.224771 fabric-orchestrator-client-1.5.0rc1/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2023-05-11 17:37:01.225030 fabric-orchestrator-client-1.5.0rc1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2023-05-11 17:37:01.225269 fabric-orchestrator-client-1.5.0rc1/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2023-05-11 17:37:01.225554 fabric-orchestrator-client-1.5.0rc1/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.225840 fabric-orchestrator-client-1.5.0rc1/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2023-05-11 17:37:01.226137 fabric-orchestrator-client-1.5.0rc1/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2023-05-11 17:37:01.226327 fabric-orchestrator-client-1.5.0rc1/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2023-05-11 17:37:01.226547 fabric-orchestrator-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.226964 fabric-orchestrator-client-1.5.0rc1/test/test_version.py
--rw-r--r--   0        0        0      814 2023-05-11 17:37:01.227150 fabric-orchestrator-client-1.5.0rc1/test/test_version_api.py
--rw-r--r--   0        0        0      922 2023-05-11 17:37:01.227332 fabric-orchestrator-client-1.5.0rc1/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 17:37:01.227515 fabric-orchestrator-client-1.5.0rc1/tox.ini
--rw-r--r--   0        0        0    10193 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      793 2023-05-11 17:37:01.210207 fabric-orchestrator-client-1.5.0rc2/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 17:37:01.210355 fabric-orchestrator-client-1.5.0rc2/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-05-11 17:37:01.210524 fabric-orchestrator-client-1.5.0rc2/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 17:37:01.210626 fabric-orchestrator-client-1.5.0rc2/.travis.yml
+-rw-r--r--   0        0        0      770 2023-05-11 17:37:01.210729 fabric-orchestrator-client-1.5.0rc2/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2023-05-11 17:37:01.210862 fabric-orchestrator-client-1.5.0rc2/LICENSE
+-rw-r--r--   0        0        0       59 2023-05-11 17:37:01.210963 fabric-orchestrator-client-1.5.0rc2/MANIFEST.in
+-rw-r--r--   0        0        0     9238 2023-05-11 17:37:01.211113 fabric-orchestrator-client-1.5.0rc2/README.md
+-rw-r--r--   0        0        0     4263 2023-05-11 17:37:01.211350 fabric-orchestrator-client-1.5.0rc2/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    17437 2023-05-11 17:37:01.211531 fabric-orchestrator-client-1.5.0rc2/docs/SlicesApi.md
+-rw-r--r--   0        0        0     3740 2023-05-11 17:37:01.211677 fabric-orchestrator-client-1.5.0rc2/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2023-05-11 17:37:01.211789 fabric-orchestrator-client-1.5.0rc2/docs/Success.md
+-rw-r--r--   0        0        0      352 2023-05-11 17:37:01.211912 fabric-orchestrator-client-1.5.0rc2/docs/Version.md
+-rw-r--r--   0        0        0       25 2023-05-12 13:46:55.675728 fabric-orchestrator-client-1.5.0rc2/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:37:01.212158 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    18242 2023-05-11 17:37:01.212367 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3004 2023-05-11 17:37:01.212646 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-11 17:37:01.212849 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     9597 2023-05-11 17:37:01.213024 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    37827 2023-05-11 17:37:01.213284 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     8826 2023-05-11 17:37:01.213492 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2023-05-11 17:37:01.213724 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25128 2023-05-11 17:37:01.213944 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2023-05-11 17:37:01.214372 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2496 2023-05-11 17:37:01.214654 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3055 2023-05-11 17:37:01.214908 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2023-05-11 17:37:01.215233 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     8496 2023-05-11 17:37:01.215453 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3435 2023-05-11 17:37:01.215578 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2023-05-11 17:37:01.215680 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0    10903 2023-05-11 17:37:01.215821 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2023-05-11 17:37:01.216181 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2023-05-11 17:37:01.216373 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2023-05-11 17:37:01.216668 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2023-05-11 17:37:01.216937 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2023-05-11 17:37:01.217164 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2023-05-11 17:37:01.217341 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2023-05-11 17:37:01.217534 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2023-05-11 17:37:01.217713 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2023-05-11 17:37:01.217919 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2023-05-11 17:37:01.218148 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2023-05-11 17:37:01.218431 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2023-05-11 17:37:01.218623 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2023-05-11 17:37:01.218944 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2023-05-11 17:37:01.219262 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2023-05-11 17:37:01.219487 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2023-05-11 17:37:01.219669 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2023-05-11 17:37:01.219920 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12988 2023-05-11 17:37:01.220174 fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 17:37:01.220383 fabric-orchestrator-client-1.5.0rc2/git_push.sh
+-rw-r--r--   0        0        0     1026 2023-05-12 13:46:49.514872 fabric-orchestrator-client-1.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 17:37:01.221004 fabric-orchestrator-client-1.5.0rc2/test/__init__.py
+-rw-r--r--   0        0        0      896 2023-05-11 17:37:01.221224 fabric-orchestrator-client-1.5.0rc2/test/test_resource.py
+-rw-r--r--   0        0        0      950 2023-05-11 17:37:01.221397 fabric-orchestrator-client-1.5.0rc2/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2023-05-11 17:37:01.221693 fabric-orchestrator-client-1.5.0rc2/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2023-05-11 17:37:01.221929 fabric-orchestrator-client-1.5.0rc2/test/test_slice.py
+-rw-r--r--   0        0        0      930 2023-05-11 17:37:01.222101 fabric-orchestrator-client-1.5.0rc2/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222270 fabric-orchestrator-client-1.5.0rc2/test/test_slices.py
+-rw-r--r--   0        0        0     2018 2023-05-11 17:37:01.222442 fabric-orchestrator-client-1.5.0rc2/test/test_slices_api.py
+-rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222608 fabric-orchestrator-client-1.5.0rc2/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2023-05-11 17:37:01.222785 fabric-orchestrator-client-1.5.0rc2/test/test_slivers.py
+-rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223106 fabric-orchestrator-client-1.5.0rc2/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223296 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2023-05-11 17:37:01.223607 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2023-05-11 17:37:01.223847 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2023-05-11 17:37:01.224081 fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2023-05-11 17:37:01.224292 fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2023-05-11 17:37:01.224535 fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2023-05-11 17:37:01.224771 fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2023-05-11 17:37:01.225030 fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2023-05-11 17:37:01.225269 fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2023-05-11 17:37:01.225554 fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2023-05-11 17:37:01.225840 fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2023-05-11 17:37:01.226137 fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2023-05-11 17:37:01.226327 fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2023-05-11 17:37:01.226547 fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2023-05-11 17:37:01.226964 fabric-orchestrator-client-1.5.0rc2/test/test_version.py
+-rw-r--r--   0        0        0      814 2023-05-11 17:37:01.227150 fabric-orchestrator-client-1.5.0rc2/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2023-05-11 17:37:01.227332 fabric-orchestrator-client-1.5.0rc2/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 17:37:01.227515 fabric-orchestrator-client-1.5.0rc2/tox.ini
+-rw-r--r--   0        0        0    10192 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.5.0rc2/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.5.0rc1/.gitignore` & `fabric-orchestrator-client-1.5.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.5.0rc2/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/CODEGEN.md` & `fabric-orchestrator-client-1.5.0rc2/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/LICENSE` & `fabric-orchestrator-client-1.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/README.md` & `fabric-orchestrator-client-1.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.5.0rc2/docs/ResourcesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/docs/SlicesApi.md` & `fabric-orchestrator-client-1.5.0rc2/docs/SlicesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/docs/SliversApi.md` & `fabric-orchestrator-client-1.5.0rc2/docs/SliversApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.5.0rc2/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/git_push.sh` & `fabric-orchestrator-client-1.5.0rc2/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/pyproject.toml` & `fabric-orchestrator-client-1.5.0rc2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 requires-python = '>=3.9'
 dependencies = [
     "certifi >= 14.05.14",
     "six >= 1.10",
     "python_dateutil >= 2.5.3",
     "requests>=2.28.1",
-    "fabric-fim==1.5.0rc1",
+    "fabric-fim==1.5.0b4",
     ]
 
 [project.optional-dependencies]
 test = ["coverage>=4.0.3",
         "nose>=1.3.7",
         "pluggy>=0.3.1",
         "py>=1.4.31",
```

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_resource.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_resources.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_resources_api.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_slice.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_slice_details.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_slices.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_slices_api.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_sliver.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_slivers.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_slivers_api.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_version.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_version_api.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/test/test_version_data.py` & `fabric-orchestrator-client-1.5.0rc2/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.0rc1/PKG-INFO` & `fabric-orchestrator-client-1.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: Fabric Orchestrator API
 Keywords: Swagger,Fabric Orchestrator API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: certifi >= 14.05.14
 Requires-Dist: six >= 1.10
 Requires-Dist: python_dateutil >= 2.5.3
 Requires-Dist: requests>=2.28.1
-Requires-Dist: fabric-fim==1.5.0rc1
+Requires-Dist: fabric-fim==1.5.0b4
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/OrchestratorClient
```

