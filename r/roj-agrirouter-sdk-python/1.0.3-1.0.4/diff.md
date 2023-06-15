# Comparing `tmp/roj-agrirouter-sdk-python-1.0.3.tar.gz` & `tmp/roj-agrirouter-sdk-python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roj-agrirouter-sdk-python-1.0.3.tar", last modified: Wed May 31 10:27:12 2023, max compression
+gzip compressed data, was "roj-agrirouter-sdk-python-1.0.4.tar", last modified: Thu Jun 15 10:25:06 2023, max compression
```

## Comparing `roj-agrirouter-sdk-python-1.0.3.tar` & `roj-agrirouter-sdk-python-1.0.4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.509207 roj-agrirouter-sdk-python-1.0.3/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      977 2023-05-31 10:27:12.509207 roj-agrirouter-sdk-python-1.0.3/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.493207 roj-agrirouter-sdk-python-1.0.3/agrirouter/
--rw-rw-r--   0 user      (1000) user      (1000)     1084 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1356 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/auth.py
--rw-rw-r--   0 user      (1000) user      (1000)     3233 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/dto.py
--rw-rw-r--   0 user      (1000) user      (1000)      303 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/enums.py
--rw-rw-r--   0 user      (1000) user      (1000)      198 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1235 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)     3073 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/response.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/constants/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/constants/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/constants/media_types.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      508 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/environmental_services.py
--rw-rw-r--   0 user      (1000) user      (1000)     2578 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/environments.py
--rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1363 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/keys.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/cloud_provider_integration/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/cloud_provider_integration/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/commons/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/commons/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3522 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/commons/chunk_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     7512 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/commons/message_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/account/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/account/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4230 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.497207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/efdi/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/efdi/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)   306464 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/endpoint/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/endpoint/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9282 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     5278 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/feed/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/feed/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/gps/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/gps/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    14065 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     9916 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/request_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/account/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/account/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10371 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/endpoint/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/endpoint/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5137 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/feed/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/feed/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    37035 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)    12586 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     9214 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/response_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/settings/dh_settings_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.501207 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     7442 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/builders.py
--rw-rw-r--   0 user      (1000) user      (1000)      571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/certification.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.505207 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/clients/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/clients/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)       30 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/clients/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)     2725 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/clients/http.py
--rw-rw-r--   0 user      (1000) user      (1000)     5185 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/clients/mqtt.py
--rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/decode.py
--rw-rw-r--   0 user      (1000) user      (1000)     2438 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/encode.py
--rw-rw-r--   0 user      (1000) user      (1000)     1053 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/enums.py
--rw-rw-r--   0 user      (1000) user      (1000)      441 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/messages.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.505207 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/parameters/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/parameters/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3200 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/parameters/dto.py
--rw-rw-r--   0 user      (1000) user      (1000)    18534 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/parameters/service.py
--rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     1571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/result.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.505207 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2986 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     3153 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/commons.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.505207 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/http/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/http/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      757 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/http/outbox.py
--rw-rw-r--   0 user      (1000) user      (1000)    14297 2023-05-31 09:35:37.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/messaging.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.505207 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6174 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/dto.py
--rw-rw-r--   0 user      (1000) user      (1000)      169 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/enums.py
--rw-rw-r--   0 user      (1000) user      (1000)      894 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/headers.py
--rw-rw-r--   0 user      (1000) user      (1000)     2375 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/onboarding.py
--rw-rw-r--   0 user      (1000) user      (1000)     1653 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)     1140 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     2115 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/request_body.py
--rw-rw-r--   0 user      (1000) user      (1000)     6710 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     1015 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/signature.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.509207 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      801 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/headers.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)      995 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/request.py
--rw-rw-r--   0 user      (1000) user      (1000)      860 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/request_body.py
--rw-rw-r--   0 user      (1000) user      (1000)      428 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     1725 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/revoking.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.509207 roj-agrirouter-sdk-python-1.0.3/agrirouter/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1936 2023-05-31 09:35:47.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/utils/type_url.py
--rw-rw-r--   0 user      (1000) user      (1000)      202 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/utils/utc_time_util.py
--rw-rw-r--   0 user      (1000) user      (1000)       59 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/agrirouter/utils/uuid_util.py
--rw-rw-r--   0 user      (1000) user      (1000)       90 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.3/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 10:27:12.509207 roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      977 2023-05-31 10:27:12.000000 roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     4370 2023-05-31 10:27:12.000000 roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 10:27:12.000000 roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      171 2023-05-31 10:27:12.000000 roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       11 2023-05-31 10:27:12.000000 roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 10:27:12.509207 roj-agrirouter-sdk-python-1.0.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1450 2023-05-31 10:22:39.000000 roj-agrirouter-sdk-python-1.0.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.522493 roj-agrirouter-sdk-python-1.0.4/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      997 2023-06-15 10:25:06.522493 roj-agrirouter-sdk-python-1.0.4/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/
+-rw-rw-r--   0 user      (1000) user      (1000)     1084 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1356 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/auth.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3233 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/dto.py
+-rw-rw-r--   0 user      (1000) user      (1000)      303 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/enums.py
+-rw-rw-r--   0 user      (1000) user      (1000)      198 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1235 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3087 2023-06-15 10:00:14.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/response.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/constants/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/constants/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/constants/media_types.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      508 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/environmental_services.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2578 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/environments.py
+-rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1363 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/keys.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/cloud_provider_integration/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/cloud_provider_integration/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/commons/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/commons/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3522 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/commons/chunk_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7512 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/commons/message_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/account/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/account/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4230 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.510493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/efdi/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/efdi/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)   306464 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/endpoint/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/endpoint/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9282 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5278 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/feed/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/feed/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/gps/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/gps/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    14065 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9916 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/request_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/account/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/account/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10371 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/endpoint/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/endpoint/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5137 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/feed/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/feed/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    37035 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12586 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9214 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/response_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/settings/dh_settings_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7442 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/builders.py
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/certification.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.514493 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/clients/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/clients/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       30 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/clients/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2725 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/clients/http.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5185 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/clients/mqtt.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/decode.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2438 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/encode.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1053 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/enums.py
+-rw-rw-r--   0 user      (1000) user      (1000)      441 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/messages.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.518493 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/parameters/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/parameters/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3200 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/parameters/dto.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18534 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/parameters/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/result.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.518493 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2986 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3153 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/commons.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.518493 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/http/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/http/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      757 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/http/outbox.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14297 2023-05-31 09:35:37.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/messaging.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.518493 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6174 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/dto.py
+-rw-rw-r--   0 user      (1000) user      (1000)      169 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/enums.py
+-rw-rw-r--   0 user      (1000) user      (1000)      894 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/headers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2376 2023-06-15 10:01:14.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/onboarding.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1653 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1151 2023-06-15 10:01:38.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2115 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/request_body.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6710 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1035 2023-06-15 10:01:01.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/signature.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.518493 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      801 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/headers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1006 2023-06-15 10:02:01.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)      860 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/request_body.py
+-rw-rw-r--   0 user      (1000) user      (1000)      428 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1734 2023-06-15 10:02:19.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/revoking.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.518493 roj-agrirouter-sdk-python-1.0.4/agrirouter/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1936 2023-05-31 09:35:47.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/utils/type_url.py
+-rw-rw-r--   0 user      (1000) user      (1000)      202 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/utils/utc_time_util.py
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/agrirouter/utils/uuid_util.py
+-rw-rw-r--   0 user      (1000) user      (1000)       90 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.4/pyproject.toml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-15 10:25:06.522493 roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      997 2023-06-15 10:25:06.000000 roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     4370 2023-06-15 10:25:06.000000 roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-15 10:25:06.000000 roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      122 2023-06-15 10:25:06.000000 roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       11 2023-06-15 10:25:06.000000 roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-15 10:25:06.522493 roj-agrirouter-sdk-python-1.0.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1388 2023-06-15 10:16:45.000000 roj-agrirouter-sdk-python-1.0.4/setup.py
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/LICENSE` & `roj-agrirouter-sdk-python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/PKG-INFO` & `roj-agrirouter-sdk-python-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roj-agrirouter-sdk-python
-Version: 1.0.3
-Summary: Agrirouter SDK Python patched by ROJ for experimental test.
+Version: 1.0.4
+Summary: Agrirouter SDK Python patched by ROJ for experimental test to run on App mobile
 Home-page: https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Author: Stefano Gurrieri
 Author-email: stefano.gurrieri@vandewiele.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Project-URL: Source, https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Classifier: Intended Audience :: Developers
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/__init__.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/__init__.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/auth.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/auth.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/dto.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/dto.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/parameters.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/parameters.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/auth/response.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/auth/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import base64
 import json
 from typing import Union
 from urllib.parse import unquote
 
-from cryptography.exceptions import InvalidSignature
+#from cryptography.exceptions import InvalidSignature
 
 from agrirouter.auth.dto import AuthorizationToken, AuthorizationResultUrl
-from agrirouter.onboarding.signature import verify_signature
+#from agrirouter.onboarding.signature import verify_signature
 
 
 class AuthResponse:
     SIGNATURE_KEY = "signature"
     STATE_KEY = "state"
     TOKEN_KEY = "token"
     ERROR_KEY = "error"
@@ -30,36 +30,36 @@
     def is_valid(self):
         if not self._was_verified:
             raise PermissionError("The response was not verified yet. Please verify first. "
                                   "You can access is_valid only after verifying")
 
         return self._is_valid
 
-    def verify(self, public_key) -> None:
+#    def verify(self, public_key) -> None:
         """
         Validates signature according to docs:
         https://docs.my-agrirouter.com/agrirouter-interface-documentation/latest/integration/authorization.html#analyse-result
 
         If signature is not valid, all actions with AuthResponse instance
          will fail with BadAuthResponse
 
         :return:
         """
-        encoded_data = self.state + self.token
-        unquoted_signature = unquote(self.signature)
-        encoded_signature = base64.b64decode(unquoted_signature.encode("utf-8"))
-
-        self._is_valid = True
-        try:
-            verify_signature(encoded_data, encoded_signature, public_key)
-        except InvalidSignature:
-            print("Response is invalid: invalid signature.")
-            self._is_valid = False
-        finally:
-            self._was_verified = True
+#        encoded_data = self.state + self.token
+#        unquoted_signature = unquote(self.signature)
+#        encoded_signature = base64.b64decode(unquoted_signature.encode("utf-8"))
+
+#        self._is_valid = True
+#        try:
+#            verify_signature(encoded_data, encoded_signature, public_key)
+#        except InvalidSignature:
+#            print("Response is invalid: invalid signature.")
+#            self._is_valid = False
+#        finally:
+#            self._was_verified = True
 
     @staticmethod
     def decode_token(token: Union[str, bytes]) -> AuthorizationToken:
         if type(token) == str:
             token = token.encode("utf-8")
         base_64_decoded_token = base64.b64decode(token)
         decoded_token = base_64_decoded_token.decode("utf-8")
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/environments.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/environments.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/environments/keys.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/environments/keys.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/commons/chunk_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/commons/chunk_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/commons/message_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/commons/message_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/request/request_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/request/request_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/messaging/response/response_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/messaging/response/response_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/generated/settings/dh_settings_pb2.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/generated/settings/dh_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/builders.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/builders.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/certification.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/certification.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/clients/http.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/clients/http.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/clients/mqtt.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/clients/mqtt.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/decode.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/decode.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/encode.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/encode.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/enums.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/enums.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/messages.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/messages.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/parameters/dto.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/parameters/dto.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/parameters/service.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/parameters/service.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/request.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/request.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/result.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/result.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/cloud.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/cloud.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/commons.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/commons.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/http/outbox.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/http/outbox.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/messaging/services/messaging.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/messaging/services/messaging.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/dto.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/dto.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/exceptions.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/exceptions.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/headers.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/headers.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/onboarding.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/onboarding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 from agrirouter.environments.environmental_services import EnvironmentalService
-from agrirouter.onboarding.exceptions import RequestNotSigned
+#from agrirouter.onboarding.exceptions import RequestNotSigned
 from agrirouter.onboarding.headers import SoftwareOnboardingHeader
 from agrirouter.onboarding.parameters import SoftwareOnboardingParameter
 from agrirouter.onboarding.request import SoftwareOnboardingRequest
 from agrirouter.onboarding.request_body import SoftwareOnboardingBody
 from agrirouter.onboarding.response import SoftwareVerifyOnboardingResponse, SoftwareOnboardingResponse
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/parameters.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/parameters.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/request.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from agrirouter.onboarding.headers import SoftwareOnboardingHeader
 from agrirouter.onboarding.request_body import SoftwareOnboardingBody
-from agrirouter.onboarding.signature import create_signature, verify_signature
+#from agrirouter.onboarding.signature import create_signature, verify_signature
 
 
 class SoftwareOnboardingRequest:
     def __init__(self, header: SoftwareOnboardingHeader, body: SoftwareOnboardingBody, url: str):
         self.header = header
         self.body = body
         self.url = url
@@ -17,19 +17,19 @@
 
     def get_header(self):
         return self.header.get_header()
 
     def get_body_content(self):
         return self.body.json().replace("\n", "")
 
-    def sign(self, private_key, public_key):
-        body = self.get_body_content()
-        signature = create_signature(body, private_key)
-        verify_signature(body, bytes.fromhex(signature), public_key)
-        self.header.sign(signature)
-
-    @property
-    def is_signed(self):
-        header_has_signature = self.get_header().get("X-Agrirouter-Signature", None)
-        if header_has_signature:
-            return True
-        return False
+#    def sign(self, private_key, public_key):
+#        body = self.get_body_content()
+#        signature = create_signature(body, private_key)
+#        verify_signature(body, bytes.fromhex(signature), public_key)
+#        self.header.sign(signature)
+
+#   @property
+#    def is_signed(self):
+#        header_has_signature = self.get_header().get("X-Agrirouter-Signature", None)
+#        if header_has_signature:
+#            return True
+#        return False
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/request_body.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/request_body.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/response.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/response.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/onboarding/signature.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/onboarding/signature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from cryptography.hazmat.primitives.serialization import load_pem_public_key, load_pem_private_key
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.asymmetric import padding
+#from cryptography.hazmat.primitives.serialization import load_pem_public_key, load_pem_private_key
+#from cryptography.hazmat.primitives import hashes
+#from cryptography.hazmat.primitives.asymmetric import padding
 
 
 SIGNATURE_ALGORITHM = "SHA256withRSA"
 
 
 def to_hex(sign: bytes):
     return sign.hex()
 
 
-def create_signature(request_body: str, private_key: str) -> str:
-    private_key_bytes = bytearray(private_key.encode('utf-8'))
-    private_key_data = load_pem_private_key(private_key_bytes, None)
-    signature = private_key_data.sign(
-        request_body.encode("utf-8"),
-        padding.PKCS1v15(),
-        hashes.SHA256()
-    )
-
-    return to_hex(signature)
-
-
-def verify_signature(request_body: str, signature: bytes, public_key: str) -> None:
-    public_key_bytes = bytearray(public_key.encode('utf-8'))
-    public_key_data = load_pem_public_key(public_key_bytes)
-    public_key_data.verify(
-        signature,
-        request_body.encode('utf-8'),
-        padding.PKCS1v15(),
-        hashes.SHA256()
-    )
+#def create_signature(request_body: str, private_key: str) -> str:
+#    private_key_bytes = bytearray(private_key.encode('utf-8'))
+#    private_key_data = load_pem_private_key(private_key_bytes, None)
+#    signature = private_key_data.sign(
+#        request_body.encode("utf-8"),
+#        padding.PKCS1v15(),
+#        hashes.SHA256()
+#    )
+#    return to_hex(signature)
+
+
+#def verify_signature(request_body: str, signature: bytes, public_key: str) -> None:
+#    public_key_bytes = bytearray(public_key.encode('utf-8'))
+#    public_key_data = load_pem_public_key(public_key_bytes)
+#    public_key_data.verify(
+#        signature,
+#        request_body.encode('utf-8'),
+#        padding.PKCS1v15(),
+#        hashes.SHA256()
+#    )
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/headers.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/headers.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/parameters.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/parameters.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/request.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from agrirouter.onboarding.signature import create_signature
+#from agrirouter.onboarding.signature import create_signature
 from agrirouter.revoking.headers import RevokingHeader
 from agrirouter.revoking.request_body import RevokingBody
 
 
 class RevokingRequest:
     def __init__(self, header: RevokingHeader, body: RevokingBody, url: str):
         self.header = header
@@ -17,18 +17,18 @@
 
     def get_header(self):
         return self.header.get_header()
 
     def get_body_content(self):
         return self.body.json().replace("\n", "")
 
-    def sign(self, private_key):
-        body = self.get_body_content()
-        signature = create_signature(body, private_key)
-        self.header.sign(signature)
-
-    @property
-    def is_signed(self) -> bool:
-        header_has_signature = self.get_header().get("X-Agrirouter-Signature", None)
-        if header_has_signature:
-            return True
-        return False
+#    def sign(self, private_key):
+#        body = self.get_body_content()
+#        signature = create_signature(body, private_key)
+#        self.header.sign(signature)
+
+#    @property
+#    def is_signed(self) -> bool:
+#        header_has_signature = self.get_header().get("X-Agrirouter-Signature", None)
+#        if header_has_signature:
+#            return True
+#        return False
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/request_body.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/request_body.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/revoking/revoking.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/revoking/revoking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 from agrirouter.environments.environmental_services import EnvironmentalService
-from agrirouter.onboarding.exceptions import RequestNotSigned
+#from agrirouter.onboarding.exceptions import RequestNotSigned
 from agrirouter.revoking.headers import RevokingHeader
 from agrirouter.revoking.parameters import RevokingParameter
 from agrirouter.revoking.request import RevokingRequest
 from agrirouter.revoking.request_body import RevokingBody
 from agrirouter.revoking.response import RevokingResponse
 
 
@@ -23,21 +23,21 @@
         header_params = params.get_header_params()
         request_header = RevokingHeader(**header_params)
 
         return RevokingRequest(header=request_header, body=request_body, url=url)
 
     def _perform_request(self, params: RevokingParameter, url: str) -> requests.Response:
         request = self._create_request(params, url)
-        request.sign(self._private_key)
-        if request.is_signed:
-            return requests.delete(
-                url=request.get_url(),
-                json=request.get_data(),
-                headers=request.get_header()
-            )
-        raise RequestNotSigned
+#        request.sign(self._private_key)
+#        if request.is_signed:
+#            return requests.delete(
+#                url=request.get_url(),
+#                json=request.get_data(),
+#                headers=request.get_header()
+#            )
+#        raise RequestNotSigned
 
     def revoke(self, params: RevokingParameter) -> RevokingResponse:
         url = self._environment.get_revoke_url()
         http_response = self._perform_request(params=params, url=url)
 
         return RevokingResponse(http_response)
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/agrirouter/utils/type_url.py` & `roj-agrirouter-sdk-python-1.0.4/agrirouter/utils/type_url.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/PKG-INFO` & `roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roj-agrirouter-sdk-python
-Version: 1.0.3
-Summary: Agrirouter SDK Python patched by ROJ for experimental test.
+Version: 1.0.4
+Summary: Agrirouter SDK Python patched by ROJ for experimental test to run on App mobile
 Home-page: https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Author: Stefano Gurrieri
 Author-email: stefano.gurrieri@vandewiele.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Project-URL: Source, https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Classifier: Intended Audience :: Developers
```

### Comparing `roj-agrirouter-sdk-python-1.0.3/roj_agrirouter_sdk_python.egg-info/SOURCES.txt` & `roj-agrirouter-sdk-python-1.0.4/roj_agrirouter_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.3/setup.py` & `roj-agrirouter-sdk-python-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from setuptools import setup, find_packages
 
 setup(
     name='roj-agrirouter-sdk-python',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),	
     include_package_data=True,
     python_requires=">= 3.6",
     url='https://github.com/ROJ-ITALY/agrirouter-sdk-python',
     license='Apache-2.0',
     author='Stefano Gurrieri',
     author_email='stefano.gurrieri@vandewiele.com',
-    description="""Agrirouter SDK Python patched by ROJ for experimental test.""",
+    description="""Agrirouter SDK Python patched by ROJ for experimental test to run on App mobile""",
     classifiers=[
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     install_requires=[
         'certifi~=2021.5.30',
-        'cffi~=1.14.6',
         'charset-normalizer~=2.0.6',
-        'cryptography~=3.4.8',
         'idna~=3.2',
-        'pycparser~=2.20',
         'requests~=2.26.0',
         'urllib3~=1.26.7',
         'paho-mqtt~=1.5.1',
         'protobuf~=3.18.0'
     ],
     project_urls={
         'Documentation': 'https://github.com/ROJ-ITALY/agrirouter-sdk-python',
```

