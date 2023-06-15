# Comparing `tmp/twilio-8.2.2.tar.gz` & `tmp/twilio-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilio-8.2.2.tar", last modified: Thu Jun  1 10:43:35 2023, max compression
+gzip compressed data, was "twilio-8.3.0.tar", last modified: Thu Jun 15 07:43:44 2023, max compression
```

## Comparing `twilio-8.2.2.tar` & `twilio-8.3.0.tar`

### file list

```diff
@@ -1,855 +1,855 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.694253 twilio-8.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-01 10:43:19.000000 twilio-8.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-01 10:43:19.000000 twilio-8.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 10:43:19.000000 twilio-8.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-01 10:43:35.694253 twilio-8.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-01 10:43:19.000000 twilio-8.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 10:43:35.694253 twilio-8.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-06-01 10:43:19.000000 twilio-8.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.554252 twilio-8.2.2/twilio/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/instance_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/instance_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/obsolete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/values.py
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/http/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/http/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/http/validation_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/jwt/access_token/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/jwt/access_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/jwt/access_token/grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/jwt/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/jwt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/jwt/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/jwt/taskrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/jwt/taskrouter/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/jwt/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/jwt/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/request_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.558252 twilio-8.2.2/twilio/rest/
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.562252 twilio-8.2.2/twilio/rest/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/AccountsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.562252 twilio-8.2.2/twilio/rest/accounts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/v1/auth_token_promotion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.562252 twilio-8.2.2/twilio/rest/accounts/v1/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/v1/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/v1/credential/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/v1/credential/public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/accounts/v1/secondary_auth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.562252 twilio-8.2.2/twilio/rest/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/ApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.562252 twilio-8.2.2/twilio/rest/api/v2010/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.566252 twilio-8.2.2/twilio/rest/api/v2010/account/
--rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.566252 twilio-8.2.2/twilio/rest/api/v2010/account/address/
--rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/address/dependent_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/authorized_connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.566252 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/
--rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/national.py
--rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.570252 twilio-8.2.2/twilio/rest/api/v2010/account/call/
--rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/feedback_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/siprec.py
--rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/user_defined_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.570252 twilio-8.2.2/twilio/rest/api/v2010/account/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75225 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/conference/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/conference/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.570252 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/message/
--rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/message/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/message/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/new_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/new_signing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/outgoing_caller_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/queue/
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/queue/member.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/recording/
--rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/recording/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/recording/add_on_result/
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/recording/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/signing_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/sip/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/sip/credential_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/credential_list/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.574252 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.578252 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.578252 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.578252 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.578252 twilio-8.2.2/twilio/rest/api/v2010/account/sip/ip_access_control_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/transcription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.578252 twilio-8.2.2/twilio/rest/api/v2010/account/usage/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.582252 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/all_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/last_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/this_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/today.py
--rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/yearly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/yesterday.py
--rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/usage/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/api/v2010/account/validation_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.582252 twilio-8.2.2/twilio/rest/autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/AutopilotBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.582252 twilio-8.2.2/twilio/rest/autopilot/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.582252 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.582252 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.582252 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/assistant/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/autopilot/v1/restore_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.586252 twilio-8.2.2/twilio/rest/bulkexports/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/BulkexportsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.586252 twilio-8.2.2/twilio/rest/bulkexports/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.586252 twilio-8.2.2/twilio/rest/bulkexports/v1/export/
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/v1/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/v1/export/day.py
--rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/v1/export/export_custom_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/v1/export/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/bulkexports/v1/export_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.586252 twilio-8.2.2/twilio/rest/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.586252 twilio-8.2.2/twilio/rest/chat/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.590252 twilio-8.2.2/twilio/rest/chat/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.590252 twilio-8.2.2/twilio/rest/chat/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.590252 twilio-8.2.2/twilio/rest/chat/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.590252 twilio-8.2.2/twilio/rest/chat/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.590252 twilio-8.2.2/twilio/rest/chat/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.594252 twilio-8.2.2/twilio/rest/chat/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.594252 twilio-8.2.2/twilio/rest/chat/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.594252 twilio-8.2.2/twilio/rest/chat/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/chat/v3/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.594252 twilio-8.2.2/twilio/rest/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/content/ContentBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.594252 twilio-8.2.2/twilio/rest/content/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/content/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.594252 twilio-8.2.2/twilio/rest/content/v1/content/
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/content/v1/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/content/v1/content/approval_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/content/v1/content_and_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/content/v1/legacy_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.594252 twilio-8.2.2/twilio/rest/conversations/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/ConversationsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.598252 twilio-8.2.2/twilio/rest/conversations/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37619 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/address_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.598252 twilio-8.2.2/twilio/rest/conversations/v1/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.598252 twilio-8.2.2/twilio/rest/conversations/v1/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    42957 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.598252 twilio-8.2.2/twilio/rest/conversations/v1/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.598252 twilio-8.2.2/twilio/rest/conversations/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.598252 twilio-8.2.2/twilio/rest/conversations/v1/service/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/configuration/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.598252 twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/conversations/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/service/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/conversations/v1/user/
--rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/conversations/v1/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/EventsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/events/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/event_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/events/v1/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/schema/schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/events/v1/sink/
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/sink/sink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/sink/sink_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/events/v1/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/subscription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/events/v1/subscription/subscribed_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.602253 twilio-8.2.2/twilio/rest/flex_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/FlexApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.606253 twilio-8.2.2/twilio/rest/flex_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/assessments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/flex_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_assessments_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_questionnaires.py
--rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_questionnaires_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_questionnaires_question.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_settings_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/insights_user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.606253 twilio-8.2.2/twilio/rest/flex_api/v1/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/interaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.606253 twilio-8.2.2/twilio/rest/flex_api/v1/interaction/interaction_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v1/web_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/flex_api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/flex_api/v2/web_channels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/frontline_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/frontline_api/FrontlineApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/frontline_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/frontline_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/frontline_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/frontline_api/v1/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/insights/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/InsightsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/insights/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/insights/v1/call/
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/call/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/call/call_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/call/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    31969 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/call_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/insights/v1/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/conference/conference_participant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.610252 twilio-8.2.2/twilio/rest/insights/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/room/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/room/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/insights/v1/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.614252 twilio-8.2.2/twilio/rest/ip_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/IpMessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.614252 twilio-8.2.2/twilio/rest/ip_messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.614252 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.614252 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.614252 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.614252 twilio-8.2.2/twilio/rest/ip_messaging/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.614252 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/ip_messaging/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/lookups/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/lookups/LookupsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/lookups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/lookups/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/lookups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/lookups/v1/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/lookups/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/lookups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/lookups/v2/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/media/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/media/MediaBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/media/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/media/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/media/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/media/v1/media_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/media/v1/media_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/media/v1/player_streamer/
--rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/media/v1/player_streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/media/v1/player_streamer/playback_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.618253 twilio-8.2.2/twilio/rest/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/MessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.622253 twilio-8.2.2/twilio/rest/messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.622253 twilio-8.2.2/twilio/rest/messaging/v1/brand_registration/
--rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/brand_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/deactivations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/domain_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/domain_config_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/external_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/linkshortening_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.622253 twilio-8.2.2/twilio/rest/messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/service/alpha_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/service/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/service/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/service/us_app_to_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/messaging/v1/usecase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/microvisor/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/MicrovisorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/microvisor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/account_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/account_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/microvisor/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/app/app_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/microvisor/v1/device/
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/device/device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/microvisor/v1/device/device_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/monitor/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/monitor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/monitor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/monitor/v1/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/monitor/v1/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/notify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/notify/NotifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.626253 twilio-8.2.2/twilio/rest/notify/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/notify/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/notify/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.630253 twilio-8.2.2/twilio/rest/notify/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/notify/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/notify/v1/service/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/notify/v1/service/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.630253 twilio-8.2.2/twilio/rest/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/NumbersBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.630253 twilio-8.2.2/twilio/rest/numbers/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v1/bulk_eligibility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.630253 twilio-8.2.2/twilio/rest/numbers/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.630253 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.630253 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.634253 twilio-8.2.2/twilio/rest/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/OauthBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.634253 twilio-8.2.2/twilio/rest/oauth/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/v1/device_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/v1/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/v1/openid_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/v1/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/oauth/v1/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.634253 twilio-8.2.2/twilio/rest/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/PreviewBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.634253 twilio-8.2.2/twilio/rest/preview/deployed_devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/deployed_devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.634253 twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.634253 twilio-8.2.2/twilio/rest/preview/hosted_numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/hosted_numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/hosted_numbers/authorization_document/
--rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/hosted_numbers/hosted_number_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/marketplace/available_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/marketplace/available_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/marketplace/installed_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/marketplace/installed_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/sync/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/sync/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/sync/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.638253 twilio-8.2.2/twilio/rest/preview/understand/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.642253 twilio-8.2.2/twilio/rest/preview/understand/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.642253 twilio-8.2.2/twilio/rest/preview/understand/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.642253 twilio-8.2.2/twilio/rest/preview/understand/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/understand/assistant/task/task_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.642253 twilio-8.2.2/twilio/rest/preview/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/wireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/wireless/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/wireless/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.642253 twilio-8.2.2/twilio/rest/preview/wireless/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/wireless/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/preview/wireless/sim/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.642253 twilio-8.2.2/twilio/rest/pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/PricingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/pricing/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/pricing/v1/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/messaging/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/pricing/v1/phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/phone_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/phone_number/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/pricing/v1/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v1/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/pricing/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v2/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v2/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/pricing/v2/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v2/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v2/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/pricing/v2/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/ProxyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/proxy/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.646253 twilio-8.2.2/twilio/rest/proxy/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/service/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/proxy/v1/service/session/
--rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/service/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/service/session/interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/proxy/v1/service/session/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/service/session/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/proxy/v1/service/short_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/routes/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/routes/RoutesBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/routes/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/routes/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/routes/v2/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/routes/v2/sip_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/routes/v2/trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/ServerlessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/serverless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/serverless/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/serverless/v1/service/asset/
--rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/asset/asset_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.650253 twilio-8.2.2/twilio/rest/serverless/v1/service/build/
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/build/build_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/serverless/v1/service/environment/
--rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/environment/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/environment/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/environment/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/serverless/v1/service/function/
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/function/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/serverless/v1/service/function/function_version/
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/function/function_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/StudioBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/v1/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/
--rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/engagement_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/step/
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/step/step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/v1/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/v1/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.654253 twilio-8.2.2/twilio/rest/studio/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.658253 twilio-8.2.2/twilio/rest/studio/v2/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.658253 twilio-8.2.2/twilio/rest/studio/v2/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.658253 twilio-8.2.2/twilio/rest/studio/v2/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow/flow_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow/flow_test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/studio/v2/flow_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.658253 twilio-8.2.2/twilio/rest/supersim/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/SupersimBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.658253 twilio-8.2.2/twilio/rest/supersim/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/esim_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    35221 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/fleet.py
--rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/ip_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.658253 twilio-8.2.2/twilio/rest/supersim/v1/network_access_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/network_access_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/settings_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/supersim/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/sim/billing_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/sim/sim_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/sms_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/supersim/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/SyncBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/sync/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/sync/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/sync/v1/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/sync/v1/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/sync/v1/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/sync/v1/service/sync_stream/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/sync/v1/service/sync_stream/stream_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/TaskrouterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.662253 twilio-8.2.2/twilio/rest/taskrouter/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.666253 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.666253 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task/
--rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.666253 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/
--rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.670253 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/
--rw-r--r--   0 runner    (1001) docker     (123)    43462 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.670253 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.670253 twilio-8.2.2/twilio/rest/trunking/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/TrunkingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.670253 twilio-8.2.2/twilio/rest/trunking/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.670253 twilio-8.2.2/twilio/rest/trunking/v1/trunk/
--rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/v1/trunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/v1/trunk/credential_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/v1/trunk/origination_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/v1/trunk/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trunking/v1/trunk/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.670253 twilio-8.2.2/twilio/rest/trusthub/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/TrusthubBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.674253 twilio-8.2.2/twilio/rest/trusthub/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.674253 twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.674253 twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/
--rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.674253 twilio-8.2.2/twilio/rest/verify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/VerifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.678253 twilio-8.2.2/twilio/rest/verify/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/safelist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.678253 twilio-8.2.2/twilio/rest/verify/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.678253 twilio-8.2.2/twilio/rest/verify/v2/service/entity/
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.678253 twilio-8.2.2/twilio/rest/verify/v2/service/entity/challenge/
--rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/entity/challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/entity/challenge/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/entity/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/entity/new_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/messaging_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.678253 twilio-8.2.2/twilio/rest/verify/v2/service/rate_limit/
--rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/rate_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/rate_limit/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/verification_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/service/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/verification_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/verify/v2/verification_attempts_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.682253 twilio-8.2.2/twilio/rest/video/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/VideoBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.682253 twilio-8.2.2/twilio/rest/video/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/composition_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/composition_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/recording_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.682253 twilio-8.2.2/twilio/rest/video/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.682253 twilio-8.2.2/twilio/rest/video/v1/room/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/participant/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/participant/published_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/participant/subscribe_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/participant/subscribed_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/recording_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/video/v1/room/room_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.682253 twilio-8.2.2/twilio/rest/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/VoiceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.686253 twilio-8.2.2/twilio/rest/voice/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/archived_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/byoc_trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.686253 twilio-8.2.2/twilio/rest/voice/v1/connection_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/connection_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.690253 twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.690253 twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/country/
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/ip_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/voice/v1/source_ip_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.690253 twilio-8.2.2/twilio/rest/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/WirelessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.690253 twilio-8.2.2/twilio/rest/wireless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/v1/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/v1/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.694253 twilio-8.2.2/twilio/rest/wireless/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/v1/sim/data_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/v1/sim/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/rest/wireless/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.694253 twilio-8.2.2/twilio/twiml/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/twiml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/twiml/fax_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/twiml/messaging_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-06-01 10:43:19.000000 twilio-8.2.2/twilio/twiml/voice_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:43:35.554252 twilio-8.2.2/twilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-01 10:43:35.000000 twilio-8.2.2/twilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30474 2023-06-01 10:43:35.000000 twilio-8.2.2/twilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:43:35.000000 twilio-8.2.2/twilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 10:43:35.000000 twilio-8.2.2/twilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 10:43:35.000000 twilio-8.2.2/twilio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.189010 twilio-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-15 07:43:30.000000 twilio-8.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-15 07:43:30.000000 twilio-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 07:43:30.000000 twilio-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-15 07:43:44.189010 twilio-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-15 07:43:30.000000 twilio-8.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 07:43:44.189010 twilio-8.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-06-15 07:43:30.000000 twilio-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.016999 twilio-8.3.0/twilio/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.020999 twilio-8.3.0/twilio/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/instance_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/instance_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/http/async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/http/validation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/jwt/access_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/jwt/access_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/jwt/access_token/grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/jwt/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/jwt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/jwt/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/jwt/taskrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/jwt/taskrouter/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/jwt/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/jwt/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/request_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.024999 twilio-8.3.0/twilio/rest/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/AccountsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.028999 twilio-8.3.0/twilio/rest/accounts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/v1/auth_token_promotion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.028999 twilio-8.3.0/twilio/rest/accounts/v1/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/v1/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/v1/credential/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/v1/credential/public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/accounts/v1/secondary_auth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.028999 twilio-8.3.0/twilio/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/ApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.028999 twilio-8.3.0/twilio/rest/api/v2010/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.033000 twilio-8.3.0/twilio/rest/api/v2010/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.033000 twilio-8.3.0/twilio/rest/api/v2010/account/address/
+-rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/authorized_connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.037000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/
+-rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.041000 twilio-8.3.0/twilio/rest/api/v2010/account/call/
+-rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/feedback_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/siprec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/user_defined_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.041000 twilio-8.3.0/twilio/rest/api/v2010/account/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75225 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/conference/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/conference/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.041000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.041000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.041000 twilio-8.3.0/twilio/rest/api/v2010/account/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/message/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/message/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/new_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/new_signing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.045000 twilio-8.3.0/twilio/rest/api/v2010/account/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/queue/member.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.045000 twilio-8.3.0/twilio/rest/api/v2010/account/recording/
+-rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/recording/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.045000 twilio-8.3.0/twilio/rest/api/v2010/account/recording/add_on_result/
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/recording/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/signing_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.045000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.045000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/credential_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.045000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.045000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.049001 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.049001 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.049001 twilio-8.3.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/transcription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.049001 twilio-8.3.0/twilio/rest/api/v2010/account/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.053001 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/all_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/last_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/this_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/today.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/yearly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/usage/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/api/v2010/account/validation_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.053001 twilio-8.3.0/twilio/rest/autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/AutopilotBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.053001 twilio-8.3.0/twilio/rest/autopilot/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.053001 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.057001 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.057001 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/assistant/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/autopilot/v1/restore_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.057001 twilio-8.3.0/twilio/rest/bulkexports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/BulkexportsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.057001 twilio-8.3.0/twilio/rest/bulkexports/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.057001 twilio-8.3.0/twilio/rest/bulkexports/v1/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/v1/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/v1/export/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/v1/export/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/bulkexports/v1/export_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.061001 twilio-8.3.0/twilio/rest/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.061001 twilio-8.3.0/twilio/rest/chat/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.061001 twilio-8.3.0/twilio/rest/chat/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.061001 twilio-8.3.0/twilio/rest/chat/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.061001 twilio-8.3.0/twilio/rest/chat/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.061001 twilio-8.3.0/twilio/rest/chat/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.065002 twilio-8.3.0/twilio/rest/chat/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.065002 twilio-8.3.0/twilio/rest/chat/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.065002 twilio-8.3.0/twilio/rest/chat/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.065002 twilio-8.3.0/twilio/rest/chat/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/chat/v3/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.069002 twilio-8.3.0/twilio/rest/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/content/ContentBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.069002 twilio-8.3.0/twilio/rest/content/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/content/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.069002 twilio-8.3.0/twilio/rest/content/v1/content/
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/content/v1/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/content/v1/content/approval_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/content/v1/content_and_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/content/v1/legacy_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.069002 twilio-8.3.0/twilio/rest/conversations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/ConversationsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.069002 twilio-8.3.0/twilio/rest/conversations/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37619 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/address_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.073002 twilio-8.3.0/twilio/rest/conversations/v1/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.073002 twilio-8.3.0/twilio/rest/conversations/v1/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    42957 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.073002 twilio-8.3.0/twilio/rest/conversations/v1/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.073002 twilio-8.3.0/twilio/rest/conversations/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.073002 twilio-8.3.0/twilio/rest/conversations/v1/service/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/configuration/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.077003 twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.077003 twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.077003 twilio-8.3.0/twilio/rest/conversations/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/service/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.077003 twilio-8.3.0/twilio/rest/conversations/v1/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/conversations/v1/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.077003 twilio-8.3.0/twilio/rest/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/EventsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.077003 twilio-8.3.0/twilio/rest/events/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/event_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.077003 twilio-8.3.0/twilio/rest/events/v1/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/schema/schema_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.081003 twilio-8.3.0/twilio/rest/events/v1/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/sink/sink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/sink/sink_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.081003 twilio-8.3.0/twilio/rest/events/v1/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/events/v1/subscription/subscribed_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.081003 twilio-8.3.0/twilio/rest/flex_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/FlexApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.085003 twilio-8.3.0/twilio/rest/flex_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/flex_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_settings_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/insights_user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.085003 twilio-8.3.0/twilio/rest/flex_api/v1/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/interaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.085003 twilio-8.3.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v1/web_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.085003 twilio-8.3.0/twilio/rest/flex_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/flex_api/v2/web_channels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.089003 twilio-8.3.0/twilio/rest/frontline_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/frontline_api/FrontlineApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/frontline_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.089003 twilio-8.3.0/twilio/rest/frontline_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/frontline_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/frontline_api/v1/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.089003 twilio-8.3.0/twilio/rest/insights/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/InsightsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.089003 twilio-8.3.0/twilio/rest/insights/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.089003 twilio-8.3.0/twilio/rest/insights/v1/call/
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/call/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/call/call_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/call/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32001 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/call_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.089003 twilio-8.3.0/twilio/rest/insights/v1/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/conference/conference_participant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.093004 twilio-8.3.0/twilio/rest/insights/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/room/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/room/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/insights/v1/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.093004 twilio-8.3.0/twilio/rest/ip_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/IpMessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.093004 twilio-8.3.0/twilio/rest/ip_messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.093004 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.093004 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.093004 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.097004 twilio-8.3.0/twilio/rest/ip_messaging/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.097004 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.097004 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.097004 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.097004 twilio-8.3.0/twilio/rest/lookups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/lookups/LookupsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/lookups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.101004 twilio-8.3.0/twilio/rest/lookups/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/lookups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/lookups/v1/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.101004 twilio-8.3.0/twilio/rest/lookups/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/lookups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/lookups/v2/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.101004 twilio-8.3.0/twilio/rest/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/media/MediaBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.101004 twilio-8.3.0/twilio/rest/media/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/media/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/media/v1/media_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/media/v1/media_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.101004 twilio-8.3.0/twilio/rest/media/v1/player_streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/media/v1/player_streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/media/v1/player_streamer/playback_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.101004 twilio-8.3.0/twilio/rest/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/MessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.105004 twilio-8.3.0/twilio/rest/messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.105004 twilio-8.3.0/twilio/rest/messaging/v1/brand_registration/
+-rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/brand_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/deactivations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/domain_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/external_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.105004 twilio-8.3.0/twilio/rest/messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/service/alpha_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/service/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/service/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/service/us_app_to_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/messaging/v1/usecase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.105004 twilio-8.3.0/twilio/rest/microvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/MicrovisorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.109005 twilio-8.3.0/twilio/rest/microvisor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/account_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/account_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.109005 twilio-8.3.0/twilio/rest/microvisor/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/app/app_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.109005 twilio-8.3.0/twilio/rest/microvisor/v1/device/
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/device/device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/microvisor/v1/device/device_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.109005 twilio-8.3.0/twilio/rest/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/monitor/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.109005 twilio-8.3.0/twilio/rest/monitor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/monitor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/monitor/v1/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/monitor/v1/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.113005 twilio-8.3.0/twilio/rest/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/notify/NotifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.113005 twilio-8.3.0/twilio/rest/notify/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/notify/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/notify/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.113005 twilio-8.3.0/twilio/rest/notify/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/notify/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/notify/v1/service/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/notify/v1/service/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.113005 twilio-8.3.0/twilio/rest/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/NumbersBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.113005 twilio-8.3.0/twilio/rest/numbers/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v1/bulk_eligibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.113005 twilio-8.3.0/twilio/rest/numbers/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.117005 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.117005 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.117005 twilio-8.3.0/twilio/rest/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/OauthBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.117005 twilio-8.3.0/twilio/rest/oauth/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/v1/device_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/v1/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/v1/openid_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/v1/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/oauth/v1/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.121005 twilio-8.3.0/twilio/rest/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/PreviewBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.121005 twilio-8.3.0/twilio/rest/preview/deployed_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/deployed_devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.121005 twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.121005 twilio-8.3.0/twilio/rest/preview/hosted_numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/hosted_numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.121005 twilio-8.3.0/twilio/rest/preview/hosted_numbers/authorization_document/
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.121005 twilio-8.3.0/twilio/rest/preview/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.121005 twilio-8.3.0/twilio/rest/preview/marketplace/available_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.125006 twilio-8.3.0/twilio/rest/preview/marketplace/installed_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.125006 twilio-8.3.0/twilio/rest/preview/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.125006 twilio-8.3.0/twilio/rest/preview/sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.125006 twilio-8.3.0/twilio/rest/preview/sync/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.125006 twilio-8.3.0/twilio/rest/preview/sync/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.125006 twilio-8.3.0/twilio/rest/preview/sync/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.125006 twilio-8.3.0/twilio/rest/preview/understand/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.129006 twilio-8.3.0/twilio/rest/preview/understand/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.129006 twilio-8.3.0/twilio/rest/preview/understand/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.129006 twilio-8.3.0/twilio/rest/preview/understand/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/understand/assistant/task/task_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.129006 twilio-8.3.0/twilio/rest/preview/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/wireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/wireless/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/wireless/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/preview/wireless/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/wireless/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/preview/wireless/sim/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/PricingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/pricing/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/pricing/v1/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/messaging/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/pricing/v1/phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/phone_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/phone_number/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/pricing/v1/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v1/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/pricing/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v2/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v2/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.133006 twilio-8.3.0/twilio/rest/pricing/v2/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v2/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v2/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/pricing/v2/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.137006 twilio-8.3.0/twilio/rest/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/ProxyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.137006 twilio-8.3.0/twilio/rest/proxy/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.137006 twilio-8.3.0/twilio/rest/proxy/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/service/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.137006 twilio-8.3.0/twilio/rest/proxy/v1/service/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/service/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/service/session/interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.137006 twilio-8.3.0/twilio/rest/proxy/v1/service/session/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/proxy/v1/service/short_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.137006 twilio-8.3.0/twilio/rest/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/routes/RoutesBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/routes/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/routes/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/routes/v2/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/routes/v2/sip_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/routes/v2/trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/ServerlessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/serverless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/serverless/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/serverless/v1/service/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/asset/asset_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/serverless/v1/service/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/build/build_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/serverless/v1/service/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/environment/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/environment/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/environment/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.141007 twilio-8.3.0/twilio/rest/serverless/v1/service/function/
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/function/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/serverless/v1/service/function/function_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/StudioBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/v1/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/v1/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/v1/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.145007 twilio-8.3.0/twilio/rest/studio/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.149007 twilio-8.3.0/twilio/rest/studio/v2/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.149007 twilio-8.3.0/twilio/rest/studio/v2/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.149007 twilio-8.3.0/twilio/rest/studio/v2/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow/flow_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow/flow_test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/studio/v2/flow_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.149007 twilio-8.3.0/twilio/rest/supersim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/SupersimBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.149007 twilio-8.3.0/twilio/rest/supersim/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/esim_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35221 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/ip_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.153007 twilio-8.3.0/twilio/rest/supersim/v1/network_access_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/settings_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.153007 twilio-8.3.0/twilio/rest/supersim/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/sim/billing_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/sms_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/supersim/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.153007 twilio-8.3.0/twilio/rest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/SyncBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.153007 twilio-8.3.0/twilio/rest/sync/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.153007 twilio-8.3.0/twilio/rest/sync/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.153007 twilio-8.3.0/twilio/rest/sync/v1/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.153007 twilio-8.3.0/twilio/rest/sync/v1/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.157008 twilio-8.3.0/twilio/rest/sync/v1/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.157008 twilio-8.3.0/twilio/rest/sync/v1/service/sync_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.157008 twilio-8.3.0/twilio/rest/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/TaskrouterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.157008 twilio-8.3.0/twilio/rest/taskrouter/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.157008 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.161008 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.161008 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.165008 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)    43462 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.165008 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.165008 twilio-8.3.0/twilio/rest/trunking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/TrunkingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.165008 twilio-8.3.0/twilio/rest/trunking/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.165008 twilio-8.3.0/twilio/rest/trunking/v1/trunk/
+-rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/v1/trunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/v1/trunk/credential_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/v1/trunk/origination_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/v1/trunk/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trunking/v1/trunk/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.165008 twilio-8.3.0/twilio/rest/trusthub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/TrusthubBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.169008 twilio-8.3.0/twilio/rest/trusthub/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.169008 twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.169008 twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/
+-rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.173009 twilio-8.3.0/twilio/rest/verify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/VerifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.173009 twilio-8.3.0/twilio/rest/verify/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/safelist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.173009 twilio-8.3.0/twilio/rest/verify/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.177009 twilio-8.3.0/twilio/rest/verify/v2/service/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.177009 twilio-8.3.0/twilio/rest/verify/v2/service/entity/challenge/
+-rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/entity/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/entity/new_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/messaging_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.177009 twilio-8.3.0/twilio/rest/verify/v2/service/rate_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/verification_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/service/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/verification_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/verify/v2/verification_attempts_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.177009 twilio-8.3.0/twilio/rest/video/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/VideoBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.177009 twilio-8.3.0/twilio/rest/video/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/composition_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/composition_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/recording_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.181009 twilio-8.3.0/twilio/rest/video/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.181009 twilio-8.3.0/twilio/rest/video/v1/room/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/participant/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/participant/published_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/participant/subscribed_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/recording_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/video/v1/room/room_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.181009 twilio-8.3.0/twilio/rest/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/VoiceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.181009 twilio-8.3.0/twilio/rest/voice/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/archived_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/byoc_trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.181009 twilio-8.3.0/twilio/rest/voice/v1/connection_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/connection_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.185009 twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.185009 twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/country/
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/ip_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/voice/v1/source_ip_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.185009 twilio-8.3.0/twilio/rest/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/WirelessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.185009 twilio-8.3.0/twilio/rest/wireless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/v1/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/v1/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.185009 twilio-8.3.0/twilio/rest/wireless/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/v1/sim/data_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/v1/sim/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/rest/wireless/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.189010 twilio-8.3.0/twilio/twiml/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/twiml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/twiml/fax_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/twiml/messaging_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-06-15 07:43:30.000000 twilio-8.3.0/twilio/twiml/voice_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:43:44.020999 twilio-8.3.0/twilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-15 07:43:43.000000 twilio-8.3.0/twilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30474 2023-06-15 07:43:43.000000 twilio-8.3.0/twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:43:43.000000 twilio-8.3.0/twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 07:43:43.000000 twilio-8.3.0/twilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 07:43:43.000000 twilio-8.3.0/twilio.egg-info/top_level.txt
```

### Comparing `twilio-8.2.2/AUTHORS.md` & `twilio-8.3.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/LICENSE` & `twilio-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/PKG-INFO` & `twilio-8.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.2.2
+Version: 8.3.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.2.2/README.md` & `twilio-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/setup.py` & `twilio-8.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # python setup.py install
 #
 # You need to have the setuptools module installed. Try reading the setuptools
 # documentation: http://pypi.python.org/pypi/setuptools
 
 setup(
     name="twilio",
-    version="8.2.2",
+    version="8.3.0",
     description="Twilio API client and TwiML generator",
     author="Twilio",
     author_email="help@twilio.com",
     url="https://github.com/twilio/twilio-python/",
     keywords=["twilio", "twiml"],
     python_requires=">=3.7.0",
     install_requires=[
```

### Comparing `twilio-8.2.2/twilio/base/client_base.py` & `twilio-8.3.0/twilio/base/client_base.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/base/deserialize.py` & `twilio-8.3.0/twilio/base/deserialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/base/domain.py` & `twilio-8.3.0/twilio/base/domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/base/exceptions.py` & `twilio-8.3.0/twilio/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/base/obsolete.py` & `twilio-8.3.0/twilio/base/obsolete.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/base/page.py` & `twilio-8.3.0/twilio/base/page.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/base/serialize.py` & `twilio-8.3.0/twilio/base/serialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/base/version.py` & `twilio-8.3.0/twilio/base/version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/http/__init__.py` & `twilio-8.3.0/twilio/http/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/http/async_http_client.py` & `twilio-8.3.0/twilio/http/async_http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/http/http_client.py` & `twilio-8.3.0/twilio/http/http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/http/request.py` & `twilio-8.3.0/twilio/http/request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/http/response.py` & `twilio-8.3.0/twilio/http/response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/http/validation_client.py` & `twilio-8.3.0/twilio/http/validation_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/jwt/__init__.py` & `twilio-8.3.0/twilio/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/jwt/access_token/__init__.py` & `twilio-8.3.0/twilio/jwt/access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/jwt/access_token/grants.py` & `twilio-8.3.0/twilio/jwt/access_token/grants.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/jwt/client/__init__.py` & `twilio-8.3.0/twilio/jwt/client/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/jwt/taskrouter/__init__.py` & `twilio-8.3.0/twilio/jwt/taskrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/jwt/taskrouter/capabilities.py` & `twilio-8.3.0/twilio/jwt/taskrouter/capabilities.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/jwt/validation/__init__.py` & `twilio-8.3.0/twilio/jwt/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/request_validator.py` & `twilio-8.3.0/twilio/request_validator.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/__init__.py` & `twilio-8.3.0/twilio/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/AccountsBase.py` & `twilio-8.3.0/twilio/rest/accounts/AccountsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/__init__.py` & `twilio-8.3.0/twilio/rest/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/v1/__init__.py` & `twilio-8.3.0/twilio/rest/accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/v1/auth_token_promotion.py` & `twilio-8.3.0/twilio/rest/accounts/v1/auth_token_promotion.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/v1/credential/__init__.py` & `twilio-8.3.0/twilio/rest/accounts/v1/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/v1/credential/aws.py` & `twilio-8.3.0/twilio/rest/accounts/v1/credential/aws.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/v1/credential/public_key.py` & `twilio-8.3.0/twilio/rest/accounts/v1/credential/public_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/accounts/v1/secondary_auth_token.py` & `twilio-8.3.0/twilio/rest/accounts/v1/secondary_auth_token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/ApiBase.py` & `twilio-8.3.0/twilio/rest/api/ApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/__init__.py` & `twilio-8.3.0/twilio/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/address/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/address/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/address/dependent_phone_number.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/application.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/application.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/authorized_connect_app.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/authorized_connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/local.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/national.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/available_phone_number_country/voip.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/balance.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/balance.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/event.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/feedback.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/feedback_summary.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/feedback_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/notification.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/payment.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/payment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/recording.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/siprec.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/siprec.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/stream.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/stream.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/user_defined_message.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/user_defined_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/conference/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/conference/participant.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/conference/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/conference/recording.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/conference/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/connect_app.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/local.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/key.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/message/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/message/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -482,20 +482,20 @@
         ] = values.unset,
         smart_encoded: Union[bool, object] = values.unset,
         persistent_action: Union[List[str], object] = values.unset,
         shorten_urls: Union[bool, object] = values.unset,
         schedule_type: Union["MessageInstance.ScheduleType", object] = values.unset,
         send_at: Union[datetime, object] = values.unset,
         send_as_mms: Union[bool, object] = values.unset,
-        content_sid: Union[str, object] = values.unset,
         content_variables: Union[str, object] = values.unset,
         from_: Union[str, object] = values.unset,
         messaging_service_sid: Union[str, object] = values.unset,
         body: Union[str, object] = values.unset,
         media_url: Union[List[str], object] = values.unset,
+        content_sid: Union[str, object] = values.unset,
     ) -> MessageInstance:
         """
         Create the MessageInstance
 
         :param to: The destination phone number in [E.164](https://www.twilio.com/docs/glossary/what-e164) format for SMS/MMS or [Channel user address](https://www.twilio.com/docs/sms/channels#channel-addresses) for other 3rd-party channels.
         :param status_callback: The URL we should call using the `status_callback_method` to send status information to your application. If specified, we POST these message status changes to the URL: `queued`, `failed`, `sent`, `delivered`, or `undelivered`. Twilio will POST its [standard request parameters](https://www.twilio.com/docs/sms/twiml#request-parameters) as well as some additional parameters including `MessageSid`, `MessageStatus`, and `ErrorCode`. If you include this parameter with the `messaging_service_sid`, we use this URL instead of the Status Callback URL of the [Messaging Service](https://www.twilio.com/docs/sms/services/api). URLs must contain a valid hostname and underscores are not allowed.
         :param application_sid: The SID of the application that should receive message status. We POST a `message_sid` parameter and a `message_status` parameter with a value of `sent` or `failed` to the [application](https://www.twilio.com/docs/usage/api/applications)'s `message_status_callback`. If a `status_callback` parameter is also passed, it will be ignored and the application's `message_status_callback` parameter will be used.
@@ -508,20 +508,20 @@
         :param address_retention:
         :param smart_encoded: Whether to detect Unicode characters that have a similar GSM-7 character and replace them. Can be: `true` or `false`.
         :param persistent_action: Rich actions for Channels Messages.
         :param shorten_urls: Determines the usage of Click Tracking. Setting it to `true` will instruct Twilio to replace all links in the Message with a shortened version based on the associated Domain Sid and track clicks on them. If this parameter is not set on an API call, we will use the value set on the Messaging Service. If this parameter is not set and the value is not configured on the Messaging Service used this will default to `false`.
         :param schedule_type:
         :param send_at: The time that Twilio will send the message. Must be in ISO 8601 format.
         :param send_as_mms: If set to True, Twilio will deliver the message as a single MMS message, regardless of the presence of media.
-        :param content_sid: The SID of the Content object returned at Content API content create time (https://www.twilio.com/docs/content-api/create-and-send-your-first-content-api-template#create-a-template). If this parameter is not specified, then the Content API will not be utilized.
         :param content_variables: Key-value pairs of variable names to substitution values, used alongside a content_sid. If not specified, Content API will default to the default variables defined at create time.
         :param from_: A Twilio phone number in [E.164](https://www.twilio.com/docs/glossary/what-e164) format, an [alphanumeric sender ID](https://www.twilio.com/docs/sms/send-messages#use-an-alphanumeric-sender-id), or a [Channel Endpoint address](https://www.twilio.com/docs/sms/channels#channel-addresses) that is enabled for the type of message you want to send. Phone numbers or [short codes](https://www.twilio.com/docs/sms/api/short-code) purchased from Twilio also work here. You cannot, for example, spoof messages from a private cell phone number. If you are using `messaging_service_sid`, this parameter must be empty.
         :param messaging_service_sid: The SID of the [Messaging Service](https://www.twilio.com/docs/sms/services#send-a-message-with-copilot) you want to associate with the Message. Set this parameter to use the [Messaging Service Settings and Copilot Features](https://www.twilio.com/console/sms/services) you have configured and leave the `from` parameter empty. When only this parameter is set, Twilio will use your enabled Copilot Features to select the `from` phone number for delivery.
         :param body: The text of the message you want to send. Can be up to 1,600 characters in length.
         :param media_url: The URL of the media to send with the message. The media can be of type `gif`, `png`, and `jpeg` and will be formatted correctly on the recipient's device. The media size limit is 5MB for supported file types (JPEG, PNG, GIF) and 500KB for [other types](https://www.twilio.com/docs/sms/accepted-mime-types) of accepted media. To send more than one image in the message body, provide multiple `media_url` parameters in the POST request. You can include up to 10 `media_url` parameters per message. You can send images in an SMS message in only the US and Canada.
+        :param content_sid: The SID of the Content object returned at Content API content create time (https://www.twilio.com/docs/content-api/create-and-send-your-first-content-api-template#create-a-template). If this parameter is not specified, then the Content API will not be utilized.
 
         :returns: The created MessageInstance
         """
         data = values.of(
             {
                 "To": to,
                 "StatusCallback": status_callback,
@@ -535,20 +535,20 @@
                 "AddressRetention": address_retention,
                 "SmartEncoded": smart_encoded,
                 "PersistentAction": serialize.map(persistent_action, lambda e: e),
                 "ShortenUrls": shorten_urls,
                 "ScheduleType": schedule_type,
                 "SendAt": serialize.iso8601_datetime(send_at),
                 "SendAsMms": send_as_mms,
-                "ContentSid": content_sid,
                 "ContentVariables": content_variables,
                 "From": from_,
                 "MessagingServiceSid": messaging_service_sid,
                 "Body": body,
                 "MediaUrl": serialize.map(media_url, lambda e: e),
+                "ContentSid": content_sid,
             }
         )
 
         payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
@@ -576,20 +576,20 @@
         ] = values.unset,
         smart_encoded: Union[bool, object] = values.unset,
         persistent_action: Union[List[str], object] = values.unset,
         shorten_urls: Union[bool, object] = values.unset,
         schedule_type: Union["MessageInstance.ScheduleType", object] = values.unset,
         send_at: Union[datetime, object] = values.unset,
         send_as_mms: Union[bool, object] = values.unset,
-        content_sid: Union[str, object] = values.unset,
         content_variables: Union[str, object] = values.unset,
         from_: Union[str, object] = values.unset,
         messaging_service_sid: Union[str, object] = values.unset,
         body: Union[str, object] = values.unset,
         media_url: Union[List[str], object] = values.unset,
+        content_sid: Union[str, object] = values.unset,
     ) -> MessageInstance:
         """
         Asynchronously create the MessageInstance
 
         :param to: The destination phone number in [E.164](https://www.twilio.com/docs/glossary/what-e164) format for SMS/MMS or [Channel user address](https://www.twilio.com/docs/sms/channels#channel-addresses) for other 3rd-party channels.
         :param status_callback: The URL we should call using the `status_callback_method` to send status information to your application. If specified, we POST these message status changes to the URL: `queued`, `failed`, `sent`, `delivered`, or `undelivered`. Twilio will POST its [standard request parameters](https://www.twilio.com/docs/sms/twiml#request-parameters) as well as some additional parameters including `MessageSid`, `MessageStatus`, and `ErrorCode`. If you include this parameter with the `messaging_service_sid`, we use this URL instead of the Status Callback URL of the [Messaging Service](https://www.twilio.com/docs/sms/services/api). URLs must contain a valid hostname and underscores are not allowed.
         :param application_sid: The SID of the application that should receive message status. We POST a `message_sid` parameter and a `message_status` parameter with a value of `sent` or `failed` to the [application](https://www.twilio.com/docs/usage/api/applications)'s `message_status_callback`. If a `status_callback` parameter is also passed, it will be ignored and the application's `message_status_callback` parameter will be used.
@@ -602,20 +602,20 @@
         :param address_retention:
         :param smart_encoded: Whether to detect Unicode characters that have a similar GSM-7 character and replace them. Can be: `true` or `false`.
         :param persistent_action: Rich actions for Channels Messages.
         :param shorten_urls: Determines the usage of Click Tracking. Setting it to `true` will instruct Twilio to replace all links in the Message with a shortened version based on the associated Domain Sid and track clicks on them. If this parameter is not set on an API call, we will use the value set on the Messaging Service. If this parameter is not set and the value is not configured on the Messaging Service used this will default to `false`.
         :param schedule_type:
         :param send_at: The time that Twilio will send the message. Must be in ISO 8601 format.
         :param send_as_mms: If set to True, Twilio will deliver the message as a single MMS message, regardless of the presence of media.
-        :param content_sid: The SID of the Content object returned at Content API content create time (https://www.twilio.com/docs/content-api/create-and-send-your-first-content-api-template#create-a-template). If this parameter is not specified, then the Content API will not be utilized.
         :param content_variables: Key-value pairs of variable names to substitution values, used alongside a content_sid. If not specified, Content API will default to the default variables defined at create time.
         :param from_: A Twilio phone number in [E.164](https://www.twilio.com/docs/glossary/what-e164) format, an [alphanumeric sender ID](https://www.twilio.com/docs/sms/send-messages#use-an-alphanumeric-sender-id), or a [Channel Endpoint address](https://www.twilio.com/docs/sms/channels#channel-addresses) that is enabled for the type of message you want to send. Phone numbers or [short codes](https://www.twilio.com/docs/sms/api/short-code) purchased from Twilio also work here. You cannot, for example, spoof messages from a private cell phone number. If you are using `messaging_service_sid`, this parameter must be empty.
         :param messaging_service_sid: The SID of the [Messaging Service](https://www.twilio.com/docs/sms/services#send-a-message-with-copilot) you want to associate with the Message. Set this parameter to use the [Messaging Service Settings and Copilot Features](https://www.twilio.com/console/sms/services) you have configured and leave the `from` parameter empty. When only this parameter is set, Twilio will use your enabled Copilot Features to select the `from` phone number for delivery.
         :param body: The text of the message you want to send. Can be up to 1,600 characters in length.
         :param media_url: The URL of the media to send with the message. The media can be of type `gif`, `png`, and `jpeg` and will be formatted correctly on the recipient's device. The media size limit is 5MB for supported file types (JPEG, PNG, GIF) and 500KB for [other types](https://www.twilio.com/docs/sms/accepted-mime-types) of accepted media. To send more than one image in the message body, provide multiple `media_url` parameters in the POST request. You can include up to 10 `media_url` parameters per message. You can send images in an SMS message in only the US and Canada.
+        :param content_sid: The SID of the Content object returned at Content API content create time (https://www.twilio.com/docs/content-api/create-and-send-your-first-content-api-template#create-a-template). If this parameter is not specified, then the Content API will not be utilized.
 
         :returns: The created MessageInstance
         """
         data = values.of(
             {
                 "To": to,
                 "StatusCallback": status_callback,
@@ -629,20 +629,20 @@
                 "AddressRetention": address_retention,
                 "SmartEncoded": smart_encoded,
                 "PersistentAction": serialize.map(persistent_action, lambda e: e),
                 "ShortenUrls": shorten_urls,
                 "ScheduleType": schedule_type,
                 "SendAt": serialize.iso8601_datetime(send_at),
                 "SendAsMms": send_as_mms,
-                "ContentSid": content_sid,
                 "ContentVariables": content_variables,
                 "From": from_,
                 "MessagingServiceSid": messaging_service_sid,
                 "Body": body,
                 "MediaUrl": serialize.map(media_url, lambda e: e),
+                "ContentSid": content_sid,
             }
         )
 
         payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
```

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/message/feedback.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/message/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/message/media.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/message/media.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/new_key.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/new_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/new_signing_key.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/new_signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/notification.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/outgoing_caller_id.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/outgoing_caller_id.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/queue/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/queue/member.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/queue/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/recording/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/recording/add_on_result/payload.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/recording/transcription.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/recording/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/short_code.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/signing_key.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/credential_list/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/credential_list/credential.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/token.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/transcription.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/__init__.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/all_time.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/all_time.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/daily.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/daily.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/last_month.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/last_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/monthly.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/monthly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/this_month.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/this_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/today.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/today.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/yearly.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/yearly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/record/yesterday.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/record/yesterday.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/usage/trigger.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/usage/trigger.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/api/v2010/account/validation_request.py` & `twilio-8.3.0/twilio/rest/api/v2010/account/validation_request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/AutopilotBase.py` & `twilio-8.3.0/twilio/rest/autopilot/AutopilotBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/__init__.py` & `twilio-8.3.0/twilio/rest/autopilot/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/__init__.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/__init__.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/defaults.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/defaults.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/dialogue.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/field_type/__init__.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/field_type/field_value.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/model_build.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/query.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/style_sheet.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/__init__.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/field.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/sample.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/task_actions.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/task/task_statistics.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/assistant/webhook.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/assistant/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/autopilot/v1/restore_assistant.py` & `twilio-8.3.0/twilio/rest/autopilot/v1/restore_assistant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/BulkexportsBase.py` & `twilio-8.3.0/twilio/rest/bulkexports/BulkexportsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/__init__.py` & `twilio-8.3.0/twilio/rest/bulkexports/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/v1/__init__.py` & `twilio-8.3.0/twilio/rest/bulkexports/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/v1/export/__init__.py` & `twilio-8.3.0/twilio/rest/bulkexports/v1/export/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/v1/export/day.py` & `twilio-8.3.0/twilio/rest/bulkexports/v1/export/day.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/v1/export/export_custom_job.py` & `twilio-8.3.0/twilio/rest/bulkexports/v1/export/export_custom_job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/v1/export/job.py` & `twilio-8.3.0/twilio/rest/bulkexports/v1/export/job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/bulkexports/v1/export_configuration.py` & `twilio-8.3.0/twilio/rest/bulkexports/v1/export_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/ChatBase.py` & `twilio-8.3.0/twilio/rest/chat/ChatBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/__init__.py` & `twilio-8.3.0/twilio/rest/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/credential.py` & `twilio-8.3.0/twilio/rest/chat/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/channel/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/channel/invite.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/channel/member.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/channel/message.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/role.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/user/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v1/service/user/user_channel.py` & `twilio-8.3.0/twilio/rest/chat/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/credential.py` & `twilio-8.3.0/twilio/rest/chat/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/binding.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/channel/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/channel/invite.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/channel/member.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/channel/message.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/channel/webhook.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/role.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/user/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/user/user_binding.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v2/service/user/user_channel.py` & `twilio-8.3.0/twilio/rest/chat/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v3/__init__.py` & `twilio-8.3.0/twilio/rest/chat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/chat/v3/channel.py` & `twilio-8.3.0/twilio/rest/chat/v3/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/content/ContentBase.py` & `twilio-8.3.0/twilio/rest/content/ContentBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/content/__init__.py` & `twilio-8.3.0/twilio/rest/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/content/v1/__init__.py` & `twilio-8.3.0/twilio/rest/content/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/content/v1/content/__init__.py` & `twilio-8.3.0/twilio/rest/content/v1/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/content/v1/content/approval_fetch.py` & `twilio-8.3.0/twilio/rest/content/v1/content/approval_fetch.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/content/v1/content_and_approvals.py` & `twilio-8.3.0/twilio/rest/content/v1/content_and_approvals.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/content/v1/legacy_content.py` & `twilio-8.3.0/twilio/rest/content/v1/legacy_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/ConversationsBase.py` & `twilio-8.3.0/twilio/rest/conversations/ConversationsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/address_configuration.py` & `twilio-8.3.0/twilio/rest/conversations/v1/address_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/configuration/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/configuration/webhook.py` & `twilio-8.3.0/twilio/rest/conversations/v1/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/conversation/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/conversation/message/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py` & `twilio-8.3.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/conversation/participant.py` & `twilio-8.3.0/twilio/rest/conversations/v1/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/conversation/webhook.py` & `twilio-8.3.0/twilio/rest/conversations/v1/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/credential.py` & `twilio-8.3.0/twilio/rest/conversations/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/participant_conversation.py` & `twilio-8.3.0/twilio/rest/conversations/v1/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/role.py` & `twilio-8.3.0/twilio/rest/conversations/v1/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/binding.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/configuration/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/configuration/notification.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/configuration/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/configuration/webhook.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/message/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/participant.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/conversation/webhook.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/participant_conversation.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/role.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/user/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/service/user/user_conversation.py` & `twilio-8.3.0/twilio/rest/conversations/v1/service/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/user/__init__.py` & `twilio-8.3.0/twilio/rest/conversations/v1/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/conversations/v1/user/user_conversation.py` & `twilio-8.3.0/twilio/rest/conversations/v1/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/EventsBase.py` & `twilio-8.3.0/twilio/rest/events/EventsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/__init__.py` & `twilio-8.3.0/twilio/rest/events/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/__init__.py` & `twilio-8.3.0/twilio/rest/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/event_type.py` & `twilio-8.3.0/twilio/rest/events/v1/event_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/schema/__init__.py` & `twilio-8.3.0/twilio/rest/events/v1/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/schema/schema_version.py` & `twilio-8.3.0/twilio/rest/events/v1/schema/schema_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/sink/__init__.py` & `twilio-8.3.0/twilio/rest/events/v1/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/sink/sink_test.py` & `twilio-8.3.0/twilio/rest/events/v1/sink/sink_test.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/sink/sink_validate.py` & `twilio-8.3.0/twilio/rest/events/v1/sink/sink_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/subscription/__init__.py` & `twilio-8.3.0/twilio/rest/events/v1/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/events/v1/subscription/subscribed_event.py` & `twilio-8.3.0/twilio/rest/events/v1/subscription/subscribed_event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/FlexApiBase.py` & `twilio-8.3.0/twilio/rest/flex_api/FlexApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/__init__.py` & `twilio-8.3.0/twilio/rest/flex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/__init__.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/assessments.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/assessments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/channel.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/configuration.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/flex_flow.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/flex_flow.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_assessments_comment.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_assessments_comment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_conversations.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_conversations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_questionnaires.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_questionnaires.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_questionnaires_category.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_questionnaires_question.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_segments.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_segments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_session.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_settings_answer_sets.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_settings_comment.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_settings_comment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/insights_user_roles.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/insights_user_roles.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/interaction/__init__.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/interaction/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v1/web_channel.py` & `twilio-8.3.0/twilio/rest/flex_api/v1/web_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v2/__init__.py` & `twilio-8.3.0/twilio/rest/flex_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/flex_api/v2/web_channels.py` & `twilio-8.3.0/twilio/rest/flex_api/v2/web_channels.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/frontline_api/FrontlineApiBase.py` & `twilio-8.3.0/twilio/rest/frontline_api/FrontlineApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/frontline_api/v1/__init__.py` & `twilio-8.3.0/twilio/rest/frontline_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/frontline_api/v1/user.py` & `twilio-8.3.0/twilio/rest/frontline_api/v1/user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/InsightsBase.py` & `twilio-8.3.0/twilio/rest/insights/InsightsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/__init__.py` & `twilio-8.3.0/twilio/rest/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/__init__.py` & `twilio-8.3.0/twilio/rest/insights/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/call/__init__.py` & `twilio-8.3.0/twilio/rest/insights/v1/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/call/annotation.py` & `twilio-8.3.0/twilio/rest/insights/v1/call/annotation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/call/call_summary.py` & `twilio-8.3.0/twilio/rest/insights/v1/call/call_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/call/event.py` & `twilio-8.3.0/twilio/rest/insights/v1/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/call/metric.py` & `twilio-8.3.0/twilio/rest/insights/v1/call/metric.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/call_summaries.py` & `twilio-8.3.0/twilio/rest/insights/v1/call_summaries.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     :ivar sdk_edge: 
     :ivar sip_edge: 
     :ivar tags: 
     :ivar url: 
     :ivar attributes: 
     :ivar properties: 
     :ivar trust: 
+    :ivar annotation: 
     """
 
     def __init__(self, version: Version, payload: Dict[str, Any]):
         super().__init__(version)
 
         self.account_sid: Optional[str] = payload.get("account_sid")
         self.call_sid: Optional[str] = payload.get("call_sid")
@@ -125,14 +126,15 @@
         self.sdk_edge: Optional[Dict[str, object]] = payload.get("sdk_edge")
         self.sip_edge: Optional[Dict[str, object]] = payload.get("sip_edge")
         self.tags: Optional[List[str]] = payload.get("tags")
         self.url: Optional[str] = payload.get("url")
         self.attributes: Optional[Dict[str, object]] = payload.get("attributes")
         self.properties: Optional[Dict[str, object]] = payload.get("properties")
         self.trust: Optional[Dict[str, object]] = payload.get("trust")
+        self.annotation: Optional[Dict[str, object]] = payload.get("annotation")
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
@@ -189,18 +191,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
-        connectivity_issues: Union[str, object] = values.unset,
-        quality_issues: Union[str, object] = values.unset,
+        connectivity_issue: Union[str, object] = values.unset,
+        quality_issue: Union[str, object] = values.unset,
         spam: Union[bool, object] = values.unset,
-        call_scores: Union[str, object] = values.unset,
+        call_score: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[CallSummariesInstance]:
         """
         Streams CallSummariesInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
@@ -221,18 +223,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
-        :param str connectivity_issues:
-        :param str quality_issues:
+        :param str connectivity_issue:
+        :param str quality_issue:
         :param bool spam:
-        :param str call_scores:
+        :param str call_score:
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
@@ -255,18 +257,18 @@
             call_state=call_state,
             direction=direction,
             processing_state=processing_state,
             sort_by=sort_by,
             subaccount=subaccount,
             abnormal_session=abnormal_session,
             answered_by=answered_by,
-            connectivity_issues=connectivity_issues,
-            quality_issues=quality_issues,
+            connectivity_issue=connectivity_issue,
+            quality_issue=quality_issue,
             spam=spam,
-            call_scores=call_scores,
+            call_score=call_score,
             page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
@@ -287,18 +289,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
-        connectivity_issues: Union[str, object] = values.unset,
-        quality_issues: Union[str, object] = values.unset,
+        connectivity_issue: Union[str, object] = values.unset,
+        quality_issue: Union[str, object] = values.unset,
         spam: Union[bool, object] = values.unset,
-        call_scores: Union[str, object] = values.unset,
+        call_score: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[CallSummariesInstance]:
         """
         Asynchronously streams CallSummariesInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
@@ -319,18 +321,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
-        :param str connectivity_issues:
-        :param str quality_issues:
+        :param str connectivity_issue:
+        :param str quality_issue:
         :param bool spam:
-        :param str call_scores:
+        :param str call_score:
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
@@ -353,18 +355,18 @@
             call_state=call_state,
             direction=direction,
             processing_state=processing_state,
             sort_by=sort_by,
             subaccount=subaccount,
             abnormal_session=abnormal_session,
             answered_by=answered_by,
-            connectivity_issues=connectivity_issues,
-            quality_issues=quality_issues,
+            connectivity_issue=connectivity_issue,
+            quality_issue=quality_issue,
             spam=spam,
-            call_scores=call_scores,
+            call_score=call_score,
             page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
@@ -385,18 +387,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
-        connectivity_issues: Union[str, object] = values.unset,
-        quality_issues: Union[str, object] = values.unset,
+        connectivity_issue: Union[str, object] = values.unset,
+        quality_issue: Union[str, object] = values.unset,
         spam: Union[bool, object] = values.unset,
-        call_scores: Union[str, object] = values.unset,
+        call_score: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[CallSummariesInstance]:
         """
         Lists CallSummariesInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
@@ -416,18 +418,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
-        :param str connectivity_issues:
-        :param str quality_issues:
+        :param str connectivity_issue:
+        :param str quality_issue:
         :param bool spam:
-        :param str call_scores:
+        :param str call_score:
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
@@ -450,18 +452,18 @@
                 call_state=call_state,
                 direction=direction,
                 processing_state=processing_state,
                 sort_by=sort_by,
                 subaccount=subaccount,
                 abnormal_session=abnormal_session,
                 answered_by=answered_by,
-                connectivity_issues=connectivity_issues,
-                quality_issues=quality_issues,
+                connectivity_issue=connectivity_issue,
+                quality_issue=quality_issue,
                 spam=spam,
-                call_scores=call_scores,
+                call_score=call_score,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
@@ -482,18 +484,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
-        connectivity_issues: Union[str, object] = values.unset,
-        quality_issues: Union[str, object] = values.unset,
+        connectivity_issue: Union[str, object] = values.unset,
+        quality_issue: Union[str, object] = values.unset,
         spam: Union[bool, object] = values.unset,
-        call_scores: Union[str, object] = values.unset,
+        call_score: Union[str, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[CallSummariesInstance]:
         """
         Asynchronously lists CallSummariesInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
@@ -513,18 +515,18 @@
         :param str call_state:
         :param str direction:
         :param &quot;CallSummariesInstance.ProcessingStateRequest&quot; processing_state:
         :param &quot;CallSummariesInstance.SortBy&quot; sort_by:
         :param str subaccount:
         :param bool abnormal_session:
         :param &quot;CallSummariesInstance.AnsweredBy&quot; answered_by:
-        :param str connectivity_issues:
-        :param str quality_issues:
+        :param str connectivity_issue:
+        :param str quality_issue:
         :param bool spam:
-        :param str call_scores:
+        :param str call_score:
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
@@ -548,18 +550,18 @@
                 call_state=call_state,
                 direction=direction,
                 processing_state=processing_state,
                 sort_by=sort_by,
                 subaccount=subaccount,
                 abnormal_session=abnormal_session,
                 answered_by=answered_by,
-                connectivity_issues=connectivity_issues,
-                quality_issues=quality_issues,
+                connectivity_issue=connectivity_issue,
+                quality_issue=quality_issue,
                 spam=spam,
-                call_scores=call_scores,
+                call_score=call_score,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
@@ -580,18 +582,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
-        connectivity_issues: Union[str, object] = values.unset,
-        quality_issues: Union[str, object] = values.unset,
+        connectivity_issue: Union[str, object] = values.unset,
+        quality_issue: Union[str, object] = values.unset,
         spam: Union[bool, object] = values.unset,
-        call_scores: Union[str, object] = values.unset,
+        call_score: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> CallSummariesPage:
         """
         Retrieve a single page of CallSummariesInstance records from the API.
         Request is executed immediately
@@ -611,18 +613,18 @@
         :param call_state:
         :param direction:
         :param processing_state:
         :param sort_by:
         :param subaccount:
         :param abnormal_session:
         :param answered_by:
-        :param connectivity_issues:
-        :param quality_issues:
+        :param connectivity_issue:
+        :param quality_issue:
         :param spam:
-        :param call_scores:
+        :param call_score:
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of CallSummariesInstance
         """
         data = values.of(
@@ -642,18 +644,18 @@
                 "CallState": call_state,
                 "Direction": direction,
                 "ProcessingState": processing_state,
                 "SortBy": sort_by,
                 "Subaccount": subaccount,
                 "AbnormalSession": abnormal_session,
                 "AnsweredBy": answered_by,
-                "ConnectivityIssues": connectivity_issues,
-                "QualityIssues": quality_issues,
+                "ConnectivityIssue": connectivity_issue,
+                "QualityIssue": quality_issue,
                 "Spam": spam,
-                "CallScores": call_scores,
+                "CallScore": call_score,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
@@ -678,18 +680,18 @@
         processing_state: Union[
             "CallSummariesInstance.ProcessingStateRequest", object
         ] = values.unset,
         sort_by: Union["CallSummariesInstance.SortBy", object] = values.unset,
         subaccount: Union[str, object] = values.unset,
         abnormal_session: Union[bool, object] = values.unset,
         answered_by: Union["CallSummariesInstance.AnsweredBy", object] = values.unset,
-        connectivity_issues: Union[str, object] = values.unset,
-        quality_issues: Union[str, object] = values.unset,
+        connectivity_issue: Union[str, object] = values.unset,
+        quality_issue: Union[str, object] = values.unset,
         spam: Union[bool, object] = values.unset,
-        call_scores: Union[str, object] = values.unset,
+        call_score: Union[str, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> CallSummariesPage:
         """
         Asynchronously retrieve a single page of CallSummariesInstance records from the API.
         Request is executed immediately
@@ -709,18 +711,18 @@
         :param call_state:
         :param direction:
         :param processing_state:
         :param sort_by:
         :param subaccount:
         :param abnormal_session:
         :param answered_by:
-        :param connectivity_issues:
-        :param quality_issues:
+        :param connectivity_issue:
+        :param quality_issue:
         :param spam:
-        :param call_scores:
+        :param call_score:
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of CallSummariesInstance
         """
         data = values.of(
@@ -740,18 +742,18 @@
                 "CallState": call_state,
                 "Direction": direction,
                 "ProcessingState": processing_state,
                 "SortBy": sort_by,
                 "Subaccount": subaccount,
                 "AbnormalSession": abnormal_session,
                 "AnsweredBy": answered_by,
-                "ConnectivityIssues": connectivity_issues,
-                "QualityIssues": quality_issues,
+                "ConnectivityIssue": connectivity_issue,
+                "QualityIssue": quality_issue,
                 "Spam": spam,
-                "CallScores": call_scores,
+                "CallScore": call_score,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
```

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/conference/__init__.py` & `twilio-8.3.0/twilio/rest/insights/v1/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/conference/conference_participant.py` & `twilio-8.3.0/twilio/rest/insights/v1/conference/conference_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/room/__init__.py` & `twilio-8.3.0/twilio/rest/insights/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/room/participant.py` & `twilio-8.3.0/twilio/rest/insights/v1/room/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/insights/v1/setting.py` & `twilio-8.3.0/twilio/rest/insights/v1/setting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/IpMessagingBase.py` & `twilio-8.3.0/twilio/rest/ip_messaging/IpMessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/credential.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/invite.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/member.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/channel/message.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/role.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/user/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v1/service/user/user_channel.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/credential.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/binding.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/invite.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/member.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/message.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/channel/webhook.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/role.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/user/__init__.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/user/user_binding.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/ip_messaging/v2/service/user/user_channel.py` & `twilio-8.3.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/lookups/LookupsBase.py` & `twilio-8.3.0/twilio/rest/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/lookups/v1/__init__.py` & `twilio-8.3.0/twilio/rest/lookups/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/lookups/v1/phone_number.py` & `twilio-8.3.0/twilio/rest/lookups/v1/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/lookups/v2/__init__.py` & `twilio-8.3.0/twilio/rest/lookups/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/lookups/v2/phone_number.py` & `twilio-8.3.0/twilio/rest/lookups/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/media/MediaBase.py` & `twilio-8.3.0/twilio/rest/media/MediaBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/media/__init__.py` & `twilio-8.3.0/twilio/rest/media/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/media/v1/__init__.py` & `twilio-8.3.0/twilio/rest/media/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/media/v1/media_processor.py` & `twilio-8.3.0/twilio/rest/media/v1/media_processor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/media/v1/media_recording.py` & `twilio-8.3.0/twilio/rest/media/v1/media_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/media/v1/player_streamer/__init__.py` & `twilio-8.3.0/twilio/rest/media/v1/player_streamer/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/media/v1/player_streamer/playback_grant.py` & `twilio-8.3.0/twilio/rest/media/v1/player_streamer/playback_grant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/MessagingBase.py` & `twilio-8.3.0/twilio/rest/messaging/MessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/__init__.py` & `twilio-8.3.0/twilio/rest/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/__init__.py` & `twilio-8.3.0/twilio/rest/messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/brand_registration/__init__.py` & `twilio-8.3.0/twilio/rest/messaging/v1/brand_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py` & `twilio-8.3.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/brand_registration/brand_vetting.py` & `twilio-8.3.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/deactivations.py` & `twilio-8.3.0/twilio/rest/messaging/v1/deactivations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/domain_certs.py` & `twilio-8.3.0/twilio/rest/messaging/v1/domain_certs.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/domain_config.py` & `twilio-8.3.0/twilio/rest/messaging/v1/domain_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/domain_config_messaging_service.py` & `twilio-8.3.0/twilio/rest/messaging/v1/domain_config_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/external_campaign.py` & `twilio-8.3.0/twilio/rest/messaging/v1/external_campaign.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/linkshortening_messaging_service.py` & `twilio-8.3.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py` & `twilio-8.3.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/service/alpha_sender.py` & `twilio-8.3.0/twilio/rest/messaging/v1/service/alpha_sender.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/service/phone_number.py` & `twilio-8.3.0/twilio/rest/messaging/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/service/short_code.py` & `twilio-8.3.0/twilio/rest/messaging/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/service/us_app_to_person.py` & `twilio-8.3.0/twilio/rest/messaging/v1/service/us_app_to_person.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py` & `twilio-8.3.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/messaging/v1/usecase.py` & `twilio-8.3.0/twilio/rest/messaging/v1/usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/MicrovisorBase.py` & `twilio-8.3.0/twilio/rest/microvisor/MicrovisorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/__init__.py` & `twilio-8.3.0/twilio/rest/microvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/__init__.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/account_config.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/account_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/account_secret.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/account_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/app/__init__.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/app/app_manifest.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/app/app_manifest.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/device/__init__.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/device/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/device/device_config.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/device/device_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/microvisor/v1/device/device_secret.py` & `twilio-8.3.0/twilio/rest/microvisor/v1/device/device_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/monitor/MonitorBase.py` & `twilio-8.3.0/twilio/rest/monitor/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/monitor/__init__.py` & `twilio-8.3.0/twilio/rest/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/monitor/v1/__init__.py` & `twilio-8.3.0/twilio/rest/monitor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/monitor/v1/alert.py` & `twilio-8.3.0/twilio/rest/monitor/v1/alert.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/monitor/v1/event.py` & `twilio-8.3.0/twilio/rest/monitor/v1/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/notify/NotifyBase.py` & `twilio-8.3.0/twilio/rest/notify/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/notify/__init__.py` & `twilio-8.3.0/twilio/rest/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/notify/v1/__init__.py` & `twilio-8.3.0/twilio/rest/notify/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/notify/v1/credential.py` & `twilio-8.3.0/twilio/rest/notify/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/notify/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/notify/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/notify/v1/service/binding.py` & `twilio-8.3.0/twilio/rest/notify/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/notify/v1/service/notification.py` & `twilio-8.3.0/twilio/rest/notify/v1/service/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/NumbersBase.py` & `twilio-8.3.0/twilio/rest/numbers/NumbersBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v1/__init__.py` & `twilio-8.3.0/twilio/rest/numbers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v1/bulk_eligibility.py` & `twilio-8.3.0/twilio/rest/numbers/v1/bulk_eligibility.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/__init__.py` & `twilio-8.3.0/twilio/rest/numbers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/__init__.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/end_user.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/regulation.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py` & `twilio-8.3.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/OauthBase.py` & `twilio-8.3.0/twilio/rest/oauth/OauthBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/__init__.py` & `twilio-8.3.0/twilio/rest/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/v1/__init__.py` & `twilio-8.3.0/twilio/rest/oauth/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/v1/device_code.py` & `twilio-8.3.0/twilio/rest/oauth/v1/device_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/v1/oauth.py` & `twilio-8.3.0/twilio/rest/oauth/v1/oauth.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/v1/openid_discovery.py` & `twilio-8.3.0/twilio/rest/oauth/v1/openid_discovery.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/v1/token.py` & `twilio-8.3.0/twilio/rest/oauth/v1/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/oauth/v1/user_info.py` & `twilio-8.3.0/twilio/rest/oauth/v1/user_info.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/PreviewBase.py` & `twilio-8.3.0/twilio/rest/preview/PreviewBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/__init__.py` & `twilio-8.3.0/twilio/rest/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/deployed_devices/__init__.py` & `twilio-8.3.0/twilio/rest/preview/deployed_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/__init__.py` & `twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/certificate.py` & `twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/certificate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/deployment.py` & `twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/device.py` & `twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/device.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/deployed_devices/fleet/key.py` & `twilio-8.3.0/twilio/rest/preview/deployed_devices/fleet/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/hosted_numbers/__init__.py` & `twilio-8.3.0/twilio/rest/preview/hosted_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py` & `twilio-8.3.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py` & `twilio-8.3.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/hosted_numbers/hosted_number_order.py` & `twilio-8.3.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/marketplace/__init__.py` & `twilio-8.3.0/twilio/rest/preview/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/marketplace/available_add_on/__init__.py` & `twilio-8.3.0/twilio/rest/preview/marketplace/available_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py` & `twilio-8.3.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/marketplace/installed_add_on/__init__.py` & `twilio-8.3.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py` & `twilio-8.3.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/__init__.py` & `twilio-8.3.0/twilio/rest/preview/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/__init__.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/document/__init__.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/document/document_permission.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/sync_list/__init__.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/sync_list/sync_list_item.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/sync_map/__init__.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/sync_map/sync_map_item.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py` & `twilio-8.3.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/__init__.py` & `twilio-8.3.0/twilio/rest/preview/understand/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/__init__.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/dialogue.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/field_type/__init__.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/field_type/field_value.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/model_build.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/query.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/style_sheet.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/task/__init__.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/task/field.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/task/sample.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/task/task_actions.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/understand/assistant/task/task_statistics.py` & `twilio-8.3.0/twilio/rest/preview/understand/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/wireless/__init__.py` & `twilio-8.3.0/twilio/rest/preview/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/wireless/command.py` & `twilio-8.3.0/twilio/rest/preview/wireless/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/wireless/rate_plan.py` & `twilio-8.3.0/twilio/rest/preview/wireless/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/wireless/sim/__init__.py` & `twilio-8.3.0/twilio/rest/preview/wireless/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/preview/wireless/sim/usage.py` & `twilio-8.3.0/twilio/rest/preview/wireless/sim/usage.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/PricingBase.py` & `twilio-8.3.0/twilio/rest/pricing/PricingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/__init__.py` & `twilio-8.3.0/twilio/rest/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/__init__.py` & `twilio-8.3.0/twilio/rest/pricing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/messaging/__init__.py` & `twilio-8.3.0/twilio/rest/pricing/v1/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/messaging/country.py` & `twilio-8.3.0/twilio/rest/pricing/v1/messaging/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/phone_number/__init__.py` & `twilio-8.3.0/twilio/rest/pricing/v1/phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/phone_number/country.py` & `twilio-8.3.0/twilio/rest/pricing/v1/phone_number/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/voice/__init__.py` & `twilio-8.3.0/twilio/rest/pricing/v1/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/voice/country.py` & `twilio-8.3.0/twilio/rest/pricing/v1/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v1/voice/number.py` & `twilio-8.3.0/twilio/rest/pricing/v1/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v2/__init__.py` & `twilio-8.3.0/twilio/rest/pricing/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v2/country.py` & `twilio-8.3.0/twilio/rest/pricing/v2/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v2/number.py` & `twilio-8.3.0/twilio/rest/pricing/v2/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v2/voice/__init__.py` & `twilio-8.3.0/twilio/rest/pricing/v2/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v2/voice/country.py` & `twilio-8.3.0/twilio/rest/pricing/v2/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/pricing/v2/voice/number.py` & `twilio-8.3.0/twilio/rest/pricing/v2/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/ProxyBase.py` & `twilio-8.3.0/twilio/rest/proxy/ProxyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/__init__.py` & `twilio-8.3.0/twilio/rest/proxy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/proxy/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/service/phone_number.py` & `twilio-8.3.0/twilio/rest/proxy/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/service/session/__init__.py` & `twilio-8.3.0/twilio/rest/proxy/v1/service/session/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/service/session/interaction.py` & `twilio-8.3.0/twilio/rest/proxy/v1/service/session/interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/service/session/participant/__init__.py` & `twilio-8.3.0/twilio/rest/proxy/v1/service/session/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/service/session/participant/message_interaction.py` & `twilio-8.3.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/proxy/v1/service/short_code.py` & `twilio-8.3.0/twilio/rest/proxy/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/routes/RoutesBase.py` & `twilio-8.3.0/twilio/rest/routes/RoutesBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/routes/__init__.py` & `twilio-8.3.0/twilio/rest/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/routes/v2/__init__.py` & `twilio-8.3.0/twilio/rest/routes/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/routes/v2/phone_number.py` & `twilio-8.3.0/twilio/rest/routes/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/routes/v2/sip_domain.py` & `twilio-8.3.0/twilio/rest/routes/v2/sip_domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/routes/v2/trunk.py` & `twilio-8.3.0/twilio/rest/routes/v2/trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/ServerlessBase.py` & `twilio-8.3.0/twilio/rest/serverless/ServerlessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/__init__.py` & `twilio-8.3.0/twilio/rest/serverless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/asset/__init__.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/asset/asset_version.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/asset/asset_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/build/__init__.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/build/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/build/build_status.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/build/build_status.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/environment/__init__.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/environment/deployment.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/environment/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/environment/log.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/environment/log.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/environment/variable.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/environment/variable.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/function/__init__.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/function/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/function/function_version/__init__.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py` & `twilio-8.3.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/StudioBase.py` & `twilio-8.3.0/twilio/rest/studio/StudioBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/__init__.py` & `twilio-8.3.0/twilio/rest/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/engagement_context.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/step/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/engagement/step/step_context.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/execution/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/execution/execution_context.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py` & `twilio-8.3.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow/execution/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow/execution/execution_context.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow/flow_revision.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow/flow_revision.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow/flow_test_user.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow/flow_test_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/studio/v2/flow_validate.py` & `twilio-8.3.0/twilio/rest/studio/v2/flow_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/SupersimBase.py` & `twilio-8.3.0/twilio/rest/supersim/SupersimBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/__init__.py` & `twilio-8.3.0/twilio/rest/supersim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/__init__.py` & `twilio-8.3.0/twilio/rest/supersim/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/esim_profile.py` & `twilio-8.3.0/twilio/rest/supersim/v1/esim_profile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/fleet.py` & `twilio-8.3.0/twilio/rest/supersim/v1/fleet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/ip_command.py` & `twilio-8.3.0/twilio/rest/supersim/v1/ip_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/network.py` & `twilio-8.3.0/twilio/rest/supersim/v1/network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/network_access_profile/__init__.py` & `twilio-8.3.0/twilio/rest/supersim/v1/network_access_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py` & `twilio-8.3.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/settings_update.py` & `twilio-8.3.0/twilio/rest/supersim/v1/settings_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/sim/__init__.py` & `twilio-8.3.0/twilio/rest/supersim/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/sim/billing_period.py` & `twilio-8.3.0/twilio/rest/supersim/v1/sim/billing_period.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/sim/sim_ip_address.py` & `twilio-8.3.0/twilio/rest/supersim/v1/sim/sim_ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/sms_command.py` & `twilio-8.3.0/twilio/rest/supersim/v1/sms_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/supersim/v1/usage_record.py` & `twilio-8.3.0/twilio/rest/supersim/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/SyncBase.py` & `twilio-8.3.0/twilio/rest/sync/SyncBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/__init__.py` & `twilio-8.3.0/twilio/rest/sync/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/__init__.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/document/__init__.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/document/document_permission.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_list/__init__.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_list/sync_list_item.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_map/__init__.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_map/sync_map_item.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_stream/__init__.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/sync/v1/service/sync_stream/stream_message.py` & `twilio-8.3.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/TaskrouterBase.py` & `twilio-8.3.0/twilio/rest/taskrouter/TaskrouterBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/__init__.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/__init__.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/activity.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/activity.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/event.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task/__init__.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task/reservation.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_channel.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/__init__.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/reservation.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py` & `twilio-8.3.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/TrunkingBase.py` & `twilio-8.3.0/twilio/rest/trunking/TrunkingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/v1/__init__.py` & `twilio-8.3.0/twilio/rest/trunking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/v1/trunk/__init__.py` & `twilio-8.3.0/twilio/rest/trunking/v1/trunk/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/v1/trunk/credential_list.py` & `twilio-8.3.0/twilio/rest/trunking/v1/trunk/credential_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/v1/trunk/ip_access_control_list.py` & `twilio-8.3.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/v1/trunk/origination_url.py` & `twilio-8.3.0/twilio/rest/trunking/v1/trunk/origination_url.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/v1/trunk/phone_number.py` & `twilio-8.3.0/twilio/rest/trunking/v1/trunk/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trunking/v1/trunk/recording.py` & `twilio-8.3.0/twilio/rest/trunking/v1/trunk/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/TrusthubBase.py` & `twilio-8.3.0/twilio/rest/trusthub/TrusthubBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/__init__.py` & `twilio-8.3.0/twilio/rest/trusthub/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/__init__.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/__init__.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/end_user.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/end_user_type.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/policies.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/policies.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/supporting_document.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/supporting_document_type.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/__init__.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py` & `twilio-8.3.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/VerifyBase.py` & `twilio-8.3.0/twilio/rest/verify/VerifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/__init__.py` & `twilio-8.3.0/twilio/rest/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/__init__.py` & `twilio-8.3.0/twilio/rest/verify/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/form.py` & `twilio-8.3.0/twilio/rest/verify/v2/form.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/safelist.py` & `twilio-8.3.0/twilio/rest/verify/v2/safelist.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/__init__.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/access_token.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/access_token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/entity/__init__.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/entity/challenge/__init__.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/entity/challenge/notification.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/entity/challenge/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/entity/factor.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/entity/factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/entity/new_factor.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/entity/new_factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/messaging_configuration.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/messaging_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/rate_limit/__init__.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/rate_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/rate_limit/bucket.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/rate_limit/bucket.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/verification.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/verification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/verification_check.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/verification_check.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/service/webhook.py` & `twilio-8.3.0/twilio/rest/verify/v2/service/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/template.py` & `twilio-8.3.0/twilio/rest/verify/v2/template.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/verification_attempt.py` & `twilio-8.3.0/twilio/rest/verify/v2/verification_attempt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/verify/v2/verification_attempts_summary.py` & `twilio-8.3.0/twilio/rest/verify/v2/verification_attempts_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/VideoBase.py` & `twilio-8.3.0/twilio/rest/video/VideoBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/__init__.py` & `twilio-8.3.0/twilio/rest/video/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/__init__.py` & `twilio-8.3.0/twilio/rest/video/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/composition.py` & `twilio-8.3.0/twilio/rest/video/v1/composition.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/composition_hook.py` & `twilio-8.3.0/twilio/rest/video/v1/composition_hook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/composition_settings.py` & `twilio-8.3.0/twilio/rest/video/v1/composition_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/recording.py` & `twilio-8.3.0/twilio/rest/video/v1/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/recording_settings.py` & `twilio-8.3.0/twilio/rest/video/v1/recording_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/__init__.py` & `twilio-8.3.0/twilio/rest/video/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/participant/__init__.py` & `twilio-8.3.0/twilio/rest/video/v1/room/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/participant/anonymize.py` & `twilio-8.3.0/twilio/rest/video/v1/room/participant/anonymize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/participant/published_track.py` & `twilio-8.3.0/twilio/rest/video/v1/room/participant/published_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/participant/subscribe_rules.py` & `twilio-8.3.0/twilio/rest/video/v1/room/participant/subscribe_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/participant/subscribed_track.py` & `twilio-8.3.0/twilio/rest/video/v1/room/participant/subscribed_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/recording_rules.py` & `twilio-8.3.0/twilio/rest/video/v1/room/recording_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/video/v1/room/room_recording.py` & `twilio-8.3.0/twilio/rest/video/v1/room/room_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/VoiceBase.py` & `twilio-8.3.0/twilio/rest/voice/VoiceBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/__init__.py` & `twilio-8.3.0/twilio/rest/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/__init__.py` & `twilio-8.3.0/twilio/rest/voice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/archived_call.py` & `twilio-8.3.0/twilio/rest/voice/v1/archived_call.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/byoc_trunk.py` & `twilio-8.3.0/twilio/rest/voice/v1/byoc_trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/connection_policy/__init__.py` & `twilio-8.3.0/twilio/rest/voice/v1/connection_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/connection_policy/connection_policy_target.py` & `twilio-8.3.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/__init__.py` & `twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py` & `twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/country/__init__.py` & `twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py` & `twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/dialing_permissions/settings.py` & `twilio-8.3.0/twilio/rest/voice/v1/dialing_permissions/settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/ip_record.py` & `twilio-8.3.0/twilio/rest/voice/v1/ip_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/voice/v1/source_ip_mapping.py` & `twilio-8.3.0/twilio/rest/voice/v1/source_ip_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/WirelessBase.py` & `twilio-8.3.0/twilio/rest/wireless/WirelessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/__init__.py` & `twilio-8.3.0/twilio/rest/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/v1/__init__.py` & `twilio-8.3.0/twilio/rest/wireless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/v1/command.py` & `twilio-8.3.0/twilio/rest/wireless/v1/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/v1/rate_plan.py` & `twilio-8.3.0/twilio/rest/wireless/v1/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/v1/sim/__init__.py` & `twilio-8.3.0/twilio/rest/wireless/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/v1/sim/data_session.py` & `twilio-8.3.0/twilio/rest/wireless/v1/sim/data_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/v1/sim/usage_record.py` & `twilio-8.3.0/twilio/rest/wireless/v1/sim/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/rest/wireless/v1/usage_record.py` & `twilio-8.3.0/twilio/rest/wireless/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/twiml/__init__.py` & `twilio-8.3.0/twilio/twiml/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/twiml/fax_response.py` & `twilio-8.3.0/twilio/twiml/fax_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/twiml/messaging_response.py` & `twilio-8.3.0/twilio/twiml/messaging_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio/twiml/voice_response.py` & `twilio-8.3.0/twilio/twiml/voice_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.2.2/twilio.egg-info/PKG-INFO` & `twilio-8.3.0/twilio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.2.2
+Version: 8.3.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.2.2/twilio.egg-info/SOURCES.txt` & `twilio-8.3.0/twilio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

