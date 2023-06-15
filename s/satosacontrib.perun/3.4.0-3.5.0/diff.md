# Comparing `tmp/satosacontrib.perun-3.4.0.tar.gz` & `tmp/satosacontrib.perun-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosacontrib.perun-3.4.0.tar", last modified: Wed May 31 07:43:54 2023, max compression
+gzip compressed data, was "satosacontrib.perun-3.5.0.tar", last modified: Thu Jun 15 11:37:33 2023, max compression
```

## Comparing `satosacontrib.perun-3.4.0.tar` & `satosacontrib.perun-3.5.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.971694 satosacontrib.perun-3.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 07:43:54.971694 satosacontrib.perun-3.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2864 2023-05-30 20:33:51.000000 satosacontrib.perun-3.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.755689 satosacontrib.perun-3.4.0/satosacontrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.755689 satosacontrib.perun-3.4.0/satosacontrib/perun/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.831690 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/compute_eligibility.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.875692 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8313 2023-05-30 20:33:51.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    11822 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/perun_user.py
--rw-rw-rw-   0 root         (0) root         (0)    24791 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
--rw-rw-rw-   0 root         (0) root         (0)    11491 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_banned_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.875692 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnectorInterface.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/PerunConstants.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.755689 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-31 07:43:54.971694 satosacontrib.perun-3.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.963694 satosacontrib.perun-3.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10917 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/tests/test_additional_indentifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-10 13:23:50.000000 satosacontrib.perun-3.4.0/tests/test_auth_event_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3455 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/tests/test_context_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/tests/test_is_banned.py
--rw-rw-rw-   0 root         (0) root         (0)     7500 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/tests/test_is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/tests/test_microservice_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_perun_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    14517 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/tests/test_perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    36568 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_update_ues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.097710 satosacontrib.perun-3.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-15 11:37:33.097710 satosacontrib.perun-3.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.093710 satosacontrib.perun-3.5.0/satosacontrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.093710 satosacontrib.perun-3.5.0/satosacontrib/perun/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.093710 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/compute_eligibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.097710 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11822 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/perun_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    24791 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/is_banned_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.097710 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/CurlConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/CurlConnectorInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/PerunConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/satosacontrib/perun/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.093710 satosacontrib.perun-3.5.0/satosacontrib.perun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-15 11:37:33.000000 satosacontrib.perun-3.5.0/satosacontrib.perun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-06-15 11:37:33.000000 satosacontrib.perun-3.5.0/satosacontrib.perun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 11:37:33.000000 satosacontrib.perun-3.5.0/satosacontrib.perun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-06-15 11:37:33.000000 satosacontrib.perun-3.5.0/satosacontrib.perun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-15 11:37:33.000000 satosacontrib.perun-3.5.0/satosacontrib.perun.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-15 11:37:33.097710 satosacontrib.perun-3.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:37:33.097710 satosacontrib.perun-3.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10917 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_additional_indentifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_auth_event_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_context_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_is_banned.py
+-rw-rw-rw-   0 root         (0) root         (0)     7500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_microservice_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_perun_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_perun_ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_perun_entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_perun_user_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)    36568 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_sp_authorization_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-06-15 11:29:51.000000 satosacontrib.perun-3.5.0/tests/test_update_ues.py
```

### Comparing `satosacontrib.perun-3.4.0/LICENSE` & `satosacontrib.perun-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/README.md` & `satosacontrib.perun-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/__init__.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/__init__.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/compute_eligibility.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/compute_eligibility.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/context_attributes_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/context_attributes_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/attributes.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/ensure_member.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/entitlement.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/perun_user.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/perun_user.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/sp_authorization.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/sp_authorization.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_banned_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/is_banned_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_eligible_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/ConfigStore.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnector.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/utils/CurlConnector.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnectorInterface.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/utils/CurlConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/Utils.py` & `satosacontrib.perun-3.5.0/satosacontrib/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/SOURCES.txt` & `satosacontrib.perun-3.5.0/satosacontrib.perun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/setup.py` & `satosacontrib.perun-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_additional_indentifiers.py` & `satosacontrib.perun-3.5.0/tests/test_additional_indentifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_auth_event_logging.py` & `satosacontrib.perun-3.5.0/tests/test_auth_event_logging.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_context_attributes.py` & `satosacontrib.perun-3.5.0/tests/test_context_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_is_banned.py` & `satosacontrib.perun-3.5.0/tests/test_is_banned.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_is_eligible_microservice.py` & `satosacontrib.perun-3.5.0/tests/test_is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_microservice_loader.py` & `satosacontrib.perun-3.5.0/tests/test_microservice_loader.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_perun_attributes.py` & `satosacontrib.perun-3.5.0/tests/test_perun_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_perun_ensure_member.py` & `satosacontrib.perun-3.5.0/tests/test_perun_ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_perun_entitlement.py` & `satosacontrib.perun-3.5.0/tests/test_perun_entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_perun_user_microservice.py` & `satosacontrib.perun-3.5.0/tests/test_perun_user_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_sp_authorization_microservice.py` & `satosacontrib.perun-3.5.0/tests/test_sp_authorization_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.4.0/tests/test_update_ues.py` & `satosacontrib.perun-3.5.0/tests/test_update_ues.py`

 * *Files identical despite different names*

