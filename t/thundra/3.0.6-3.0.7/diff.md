# Comparing `tmp/thundra-3.0.6.tar.gz` & `tmp/thundra-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thundra-3.0.6.tar", last modified: Fri Jun  9 13:42:24 2023, max compression
+gzip compressed data, was "thundra-3.0.7.tar", last modified: Thu Jun 15 06:56:17 2023, max compression
```

## Comparing `thundra-3.0.6.tar` & `thundra-3.0.7.tar`

### file list

```diff
@@ -1,253 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.181903 thundra-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 13:42:06.000000 thundra-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-09 13:42:24.181903 thundra-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30786 2023-06-09 13:42:06.000000 thundra-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.153902 thundra-3.0.6/foresight/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.153902 thundra-3.0.6/foresight/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/constants/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/context/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/context/test_case_execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/context/test_suite_execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/azure/azure_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/bitbucket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/bitbucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/bitbucket/bitbucket_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/circleci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/circleci/circleci_environment_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/environment_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/environment_info_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/git/git_env_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/git/git_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/git/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/github/github_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/gitlab/gitlab_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/jenkins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/jenkins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/jenkins/jenkins_environment_info_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.157902 thundra-3.0.6/foresight/environment/travisci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/travisci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/environment/travisci/travisci_environment_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/foresight_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.161903 thundra-3.0.6/foresight/model/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/terminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/test_run_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/test_run_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/test_run_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/test_run_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/test_run_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/model/test_run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.161903 thundra-3.0.6/foresight/pytest_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/pytest_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/pytest_integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/pytest_integration/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/pytest_integration/pytest_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/pytest_integration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.161903 thundra-3.0.6/foresight/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/sampler/max_count_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/test_runner_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/test_runner_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/test_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.161903 thundra-3.0.6/foresight/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/utils/handler_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/utils/test_runner_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-09 13:42:06.000000 thundra-3.0.6/foresight/utils/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 13:42:24.181903 thundra-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-09 13:42:06.000000 thundra-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.161903 thundra-3.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-09 13:42:06.000000 thundra-3.0.6/tests/test_application_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-06-09 13:42:06.000000 thundra-3.0.6/tests/test_lambda_event_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-09 13:42:06.000000 thundra-3.0.6/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-09 13:42:06.000000 thundra-3.0.6/tests/test_thundra_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-09 13:42:06.000000 thundra-3.0.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.165902 thundra-3.0.6/thundra/
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.165902 thundra-3.0.6/thundra/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/application/application_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/application/application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/application/global_application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/composite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.165902 thundra-3.0.6/thundra/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/config/config_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/config/config_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/config/config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21869 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.165902 thundra-3.0.6/thundra/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/context/context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/context/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/context/execution_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/context/global_execution_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/context/plugin_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/context/tracing_execution_context_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.165902 thundra-3.0.6/thundra/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/debug/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.169903 thundra-3.0.6/thundra/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.169903 thundra-3.0.6/thundra/integrations/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/aiohttp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/base_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    38459 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.169903 thundra-3.0.6/thundra/integrations/handler_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/handler_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/handler_wrappers/chalice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.169903 thundra-3.0.6/thundra/integrations/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/django.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/modules/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/postgre.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/rdb_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/integrations/sqlite3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.173903 thundra-3.0.6/thundra/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/composite_span_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/error_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/filtering_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/latency_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/security_aware_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/tag_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/thundra_span_filterer.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/listeners/thundra_span_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.173903 thundra-3.0.6/thundra/opentracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.173903 thundra-3.0.6/thundra/opentracing/propagation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/propagation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/propagation/propagator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/propagation/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/span_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/opentracing/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.173903 thundra-3.0.6/thundra/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.173903 thundra-3.0.6/thundra/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/config/base_plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/config/log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/config/metric_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/config/thundra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/config/trace_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.173903 thundra-3.0.6/thundra/plugins/invocation/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/invocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/invocation/invocation_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/invocation/invocation_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/invocation/invocation_trace_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.173903 thundra-3.0.6/thundra/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/log/log_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/log/log_support.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/log/thundra_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/log/thundra_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.177903 thundra-3.0.6/thundra/plugins/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/metric/metric_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/metric/metric_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.177903 thundra-3.0.6/thundra/plugins/trace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/trace/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/trace/trace_aware_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/trace/trace_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/trace/trace_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/plugins/trace/traceable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.177903 thundra-3.0.6/thundra/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/samplers/composite_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/samplers/count_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/samplers/duration_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/samplers/error_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/samplers/time_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/thundra_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.177903 thundra-3.0.6/thundra/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.181903 thundra-3.0.6/thundra/wrappers/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/aws_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/aws_lambda/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/aws_lambda/lambda_application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/aws_lambda/lambda_event_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/aws_lambda/lambda_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/aws_lambda/lambda_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/cp_wrapper_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.181903 thundra-3.0.6/thundra/wrappers/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/django/django_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/django/django_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.181903 thundra-3.0.6/thundra/wrappers/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/fastapi/fastapi_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/fastapi/fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/fastapi/fastapi_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.181903 thundra-3.0.6/thundra/wrappers/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/flask/flask_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/flask/flask_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.181903 thundra-3.0.6/thundra/wrappers/tornado/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/tornado/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/tornado/tornado_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/tornado/tornado_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/web_wrapper_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/wrapper_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-09 13:42:06.000000 thundra-3.0.6/thundra/wrappers/wrapper_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:42:24.165902 thundra-3.0.6/thundra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-09 13:42:24.000000 thundra-3.0.6/thundra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-09 13:42:24.000000 thundra-3.0.6/thundra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:42:24.000000 thundra-3.0.6/thundra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 13:42:24.000000 thundra-3.0.6/thundra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-09 13:42:24.000000 thundra-3.0.6/thundra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 13:42:24.000000 thundra-3.0.6/thundra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:42:23.000000 thundra-3.0.6/thundra.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.188567 thundra-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-15 06:55:57.000000 thundra-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-15 06:56:17.188567 thundra-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22953 2023-06-15 06:55:57.000000 thundra-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.160565 thundra-3.0.7/catchpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.160565 thundra-3.0.7/catchpoint/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/application/application_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/application/application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/application/global_application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/catchpoint_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/composite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.160565 thundra-3.0.7/catchpoint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/config/config_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/config/config_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/config/config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.164565 thundra-3.0.7/catchpoint/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/context/context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/context/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/context/execution_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/context/global_execution_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/context/plugin_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/context/tracing_execution_context_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.164565 thundra-3.0.7/catchpoint/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/debug/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.164565 thundra-3.0.7/catchpoint/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.164565 thundra-3.0.7/catchpoint/integrations/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/aiohttp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/base_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.168565 thundra-3.0.7/catchpoint/integrations/handler_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/handler_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/handler_wrappers/chalice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.168565 thundra-3.0.7/catchpoint/integrations/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/modules/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/postgre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/rdb_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/integrations/sqlite3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.172565 thundra-3.0.7/catchpoint/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/catchpoint_span_filterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/catchpoint_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/composite_span_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/error_injector_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/filtering_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/latency_injector_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/security_aware_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/listeners/tag_injector_span_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.172565 thundra-3.0.7/catchpoint/opentracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.176566 thundra-3.0.7/catchpoint/opentracing/propagation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/propagation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/propagation/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/propagation/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/span_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/opentracing/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.176566 thundra-3.0.7/catchpoint/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.176566 thundra-3.0.7/catchpoint/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/config/base_plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/config/catchpoint_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/config/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/config/metric_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/config/trace_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.176566 thundra-3.0.7/catchpoint/plugins/invocation/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/invocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/invocation/invocation_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/invocation/invocation_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/invocation/invocation_trace_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.176566 thundra-3.0.7/catchpoint/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/log/catchpoint_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/log/catchpoint_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/log/log_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/log/log_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.180566 thundra-3.0.7/catchpoint/plugins/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/metric/metric_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/metric/metric_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.180566 thundra-3.0.7/catchpoint/plugins/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/trace/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/trace/trace_aware_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/trace/trace_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/trace/trace_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/plugins/trace/traceable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.180566 thundra-3.0.7/catchpoint/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/samplers/composite_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/samplers/count_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/samplers/duration_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/samplers/error_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/samplers/time_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.180566 thundra-3.0.7/catchpoint/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.180566 thundra-3.0.7/catchpoint/wrappers/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/aws_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/aws_lambda/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/aws_lambda/lambda_application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/aws_lambda/lambda_event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/aws_lambda/lambda_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/aws_lambda/lambda_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/cp_wrapper_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.184566 thundra-3.0.7/catchpoint/wrappers/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/django/django_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/django/django_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.184566 thundra-3.0.7/catchpoint/wrappers/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/fastapi/fastapi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/fastapi/fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/fastapi/fastapi_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.188567 thundra-3.0.7/catchpoint/wrappers/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/flask/flask_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/flask/flask_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.188567 thundra-3.0.7/catchpoint/wrappers/tornado/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/tornado/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/tornado/tornado_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/tornado/tornado_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/web_wrapper_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/wrapper_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-15 06:55:57.000000 thundra-3.0.7/catchpoint/wrappers/wrapper_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 06:56:17.188567 thundra-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-15 06:55:57.000000 thundra-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.188567 thundra-3.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-15 06:55:57.000000 thundra-3.0.7/tests/test_application_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-15 06:55:57.000000 thundra-3.0.7/tests/test_catchpoint_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-06-15 06:55:57.000000 thundra-3.0.7/tests/test_lambda_event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-15 06:55:57.000000 thundra-3.0.7/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-15 06:55:57.000000 thundra-3.0.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:56:17.188567 thundra-3.0.7/thundra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-15 06:56:17.000000 thundra-3.0.7/thundra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-15 06:56:17.000000 thundra-3.0.7/thundra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:56:17.000000 thundra-3.0.7/thundra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 06:56:17.000000 thundra-3.0.7/thundra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 06:56:17.000000 thundra-3.0.7/thundra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:56:16.000000 thundra-3.0.7/thundra.egg-info/zip-safe
```

### Comparing `thundra-3.0.6/LICENSE` & `thundra-3.0.7/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018 Thundra, Inc.
+   Copyright 2018 Catchpoint Systems, Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `thundra-3.0.6/PKG-INFO` & `thundra-3.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: thundra
-Version: 3.0.6
-Summary: Thundra Python agent
-Home-page: https://github.com/thundra-agent-python
-Author: Thundra
-Author-email: python@thundra.io
+Version: 3.0.7
+Summary: Catchpoint Python agent
+Home-page: https://github.com/cp-trace-python
+Author: Catchpoint
+Author-email: python@catchpoint.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 License-File: LICENSE
 
-Thundra Python agent
+Catchpoint Python agent
```

### Comparing `thundra-3.0.6/tests/test_application_support.py` & `thundra-3.0.7/tests/test_application_support.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from thundra.application.application_info_provider import ApplicationInfoProvider
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
+from catchpoint.application.application_info_provider import ApplicationInfoProvider
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
 
 def test_if_can_get_integer_tag():
     tag_name = 'integerField'
-    (env_key, env_val) = (config_names.THUNDRA_APPLICATION_TAG_PREFIX + '.' + tag_name, 3773)
+    (env_key, env_val) = (config_names.CATCHPOINT_APPLICATION_TAG_PREFIX + '.' + tag_name, 3773)
     ConfigProvider.set(env_key, str(env_val))
 
     application_tags = ApplicationInfoProvider.parse_application_tags()
 
     assert application_tags[tag_name] == env_val
 
 
 def test_if_can_get_float_tag():
     tag_name = 'floatField'
-    (env_key, env_val) = (config_names.THUNDRA_APPLICATION_TAG_PREFIX + '.' + tag_name, 12.3221)
+    (env_key, env_val) = (config_names.CATCHPOINT_APPLICATION_TAG_PREFIX + '.' + tag_name, 12.3221)
     ConfigProvider.set(env_key, str(env_val))
 
     application_tags = ApplicationInfoProvider.parse_application_tags()
 
     assert application_tags[tag_name] == env_val
 
 
 def test_if_can_get_string_tag():
     tag_name = 'stringField'
-    (env_key, env_val) = (config_names.THUNDRA_APPLICATION_TAG_PREFIX + '.' + tag_name, 'fooBar')
+    (env_key, env_val) = (config_names.CATCHPOINT_APPLICATION_TAG_PREFIX + '.' + tag_name, 'fooBar')
     ConfigProvider.set(env_key, str(env_val))
 
     application_tags = ApplicationInfoProvider.parse_application_tags()
 
     assert application_tags[tag_name] == env_val
 
 
 def test_if_can_get_bool_tag():
     tag_name = 'boolField'
-    (env_key, env_val) = (config_names.THUNDRA_APPLICATION_TAG_PREFIX + '.' + tag_name, True)
+    (env_key, env_val) = (config_names.CATCHPOINT_APPLICATION_TAG_PREFIX + '.' + tag_name, True)
     ConfigProvider.set(env_key, str(env_val))
 
     application_tags = ApplicationInfoProvider.parse_application_tags()
 
     assert application_tags[tag_name] == env_val
```

### Comparing `thundra-3.0.6/tests/test_lambda_event_utils.py` & `thundra-3.0.7/tests/test_lambda_event_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 import base64
 import hashlib
 
 import mock
 import pytest
 import simplejson as json
 
-from thundra.compat import str
-from thundra.context.execution_context_manager import ExecutionContextManager
+from catchpoint.compat import str
+from catchpoint.context.execution_context_manager import ExecutionContextManager
 
 try:
     from contextlib import ExitStack
 except ImportError:
     from contextlib2 import ExitStack
 
-from thundra import constants
-from thundra.wrappers.aws_lambda import lambda_event_utils
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.plugins import invocation
+from catchpoint import constants
+from catchpoint.wrappers.aws_lambda import lambda_event_utils
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.plugins import invocation
 
 try:
     from BytesIO import BytesIO
 except ImportError:
     from io import BytesIO
 from gzip import GzipFile
 
 
 @pytest.fixture
 def tracer_and_invocation_support():
     with ExitStack() as stack:
         # Just a fancy way of using contexts to avoid an ugly multi-line with statement
-        stack.enter_context(mock.patch('thundra.opentracing.recorder.ThundraRecorder.clear'))
-        tracer = ThundraTracer.get_instance()
+        stack.enter_context(mock.patch('catchpoint.opentracing.recorder.CatchpointRecorder.clear'))
+        tracer = CatchpointTracer.get_instance()
         invocation_support = invocation.invocation_support
         invocation_trace_support = invocation.invocation_trace_support
         yield tracer, invocation_support, invocation_trace_support
 
 
 def test_dynamodb_trigger(tracer_and_invocation_support, handler, mock_dynamodb_event, mock_context):
     _, handler = handler
@@ -266,15 +266,15 @@
 
     assert invocation_support.get_agent_tag(constants.SpanTags['TRIGGER_DOMAIN_NAME']) == 'CDN'
     assert invocation_support.get_agent_tag(constants.SpanTags['TRIGGER_CLASS_NAME']) == 'AWS-CloudFront'
     assert invocation_support.get_agent_tag(constants.SpanTags['TRIGGER_OPERATION_NAMES']) == ['/test']
 
 
 def test_firehose_trigger(tracer_and_invocation_support, handler, mock_firehose_event, mock_context):
-    thundra, handler = handler
+    _, handler = handler
     tracer, invocation_support, invocation_trace_support = tracer_and_invocation_support
     assert lambda_event_utils.get_lambda_event_type(mock_firehose_event,
                                                     mock_context) == lambda_event_utils.LambdaEventType.Firehose
     handler(mock_firehose_event, mock_context)
     execution_context = ExecutionContextManager.get()
     span = execution_context.recorder.get_spans()[0]
 
@@ -354,15 +354,15 @@
     assert invocation_support.get_agent_tag(constants.SpanTags['TRIGGER_CLASS_NAME']) == constants.ClassNames['S3']
     assert invocation_support.get_agent_tag(constants.SpanTags['TRIGGER_OPERATION_NAMES']) == ['example-bucket']
 
     assert invocation_trace_support.get_incoming_trace_links().get('incomingTraceLinks') == ["EXAMPLE123456789"]
 
 
 def test_lambda_trigger(tracer_and_invocation_support, handler, mock_event, mock_lambda_context):
-    thundra, handler = handler
+    _, handler = handler
     tracer, invocation_support, invocation_trace_support = tracer_and_invocation_support
     assert lambda_event_utils.get_lambda_event_type(mock_event,
                                                     mock_lambda_context) == lambda_event_utils.LambdaEventType.Lambda
     handler(mock_event, mock_lambda_context)
     execution_context = ExecutionContextManager.get()
     span = execution_context.recorder.get_spans()[0]
```

### Comparing `thundra-3.0.6/tests/test_reporter.py` & `thundra-3.0.7/tests/test_reporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import mock
 import json
 
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.reporter import Reporter
-from thundra.encoder import to_json
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.reporter import Reporter
+from catchpoint.encoder import to_json
 
 
-@mock.patch('thundra.reporter.requests')
+@mock.patch('catchpoint.reporter.requests')
 def test_send_report_to_url(mock_requests, mock_report):
-    ConfigProvider.set(config_names.THUNDRA_REPORT_REST_BASEURL, 'different_url/api')
-    ConfigProvider.set(config_names.THUNDRA_REPORT_REST_COMPOSITE_ENABLE, 'false')
+    ConfigProvider.set(config_names.CATCHPOINT_REPORT_REST_BASEURL, 'different_url/api')
+    ConfigProvider.set(config_names.CATCHPOINT_REPORT_REST_COMPOSITE_ENABLE, 'false')
     test_session = mock_requests.Session()
     reporter = Reporter('api key', session=test_session)
     responses = reporter.send_reports([mock_report])
 
     post_url = 'different_url/api/monitoring-data'
     headers = {
         'Content-Type': 'application/json',
@@ -25,28 +25,28 @@
     reporter.session.post.assert_called_once_with(post_url, data=to_json([mock_report], separators=(',', ':')),
                                                   headers=headers, timeout=constants.DEFAULT_REPORT_TIMEOUT)
     reporter.session.post.return_value.status_code = 200
     for response in responses:
         assert response.status_code == 200
 
 
-@mock.patch('thundra.reporter.requests')
+@mock.patch('catchpoint.reporter.requests')
 def test_send_report(mock_requests, mock_invocation_report):
     test_session = mock_requests.Session()
     reporter = Reporter('unauthorized api key', session=test_session)
     responses = reporter.send_reports([mock_invocation_report])
 
     assert reporter.session.post.call_count == 1
     test_session.post.return_value.status_code = 401
     for response in responses:
         assert response.status_code == 401
 
 
 def test_get_report_batches(mock_report):
-    ConfigProvider.set(config_names.THUNDRA_REPORT_REST_COMPOSITE_BATCH_SIZE, '2')
+    ConfigProvider.set(config_names.CATCHPOINT_REPORT_REST_COMPOSITE_BATCH_SIZE, '2')
 
     reporter = Reporter('api key')
     batches = reporter.get_report_batches([mock_report] * 3)
 
     assert len(batches) == 2
     assert batches[0] == [mock_report, mock_report]
     assert batches[1] == [mock_report]
@@ -60,15 +60,15 @@
 
     assert len(reports) == 2
     assert reports[0].get('type') != 'bytes'
     assert reports[1].get('type') == 'bytes'
 
 
 def test_prepare_report_json_batch(mock_report):
-    ConfigProvider.set(config_names.THUNDRA_REPORT_REST_COMPOSITE_BATCH_SIZE, '1')
+    ConfigProvider.set(config_names.CATCHPOINT_REPORT_REST_COMPOSITE_BATCH_SIZE, '1')
 
     reporter = Reporter('api key')
 
     batched_reports = reporter.prepare_report_json([mock_report] * 2)
     assert len(batched_reports) == 2
 
     reports = json.loads(batched_reports[0])
```

### Comparing `thundra-3.0.6/tests/test_thundra_agent.py` & `thundra-3.0.7/tests/test_catchpoint_agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,130 +1,130 @@
 import mock
 import pytest
 
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.context.execution_context_manager import ExecutionContextManager
-from thundra.plugins.trace.trace_plugin import TracePlugin
-from thundra.thundra_agent import Thundra
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.context.execution_context_manager import ExecutionContextManager
+from catchpoint.plugins.trace.trace_plugin import TracePlugin
+from catchpoint.catchpoint_agent import Catchpoint
 
 
 def test_if_api_key_is_retrieved_from_env_var():
-    ConfigProvider.set(config_names.THUNDRA_APIKEY, 'api key')
-    thundra = Thundra()
-    assert thundra.api_key == 'api key'
+    ConfigProvider.set(config_names.CATCHPOINT_APIKEY, 'api key')
+    catchpoint = Catchpoint()
+    assert catchpoint.api_key == 'api key'
 
 
 def test_if_disable_trace_is_set_to_true():
-    thundra = Thundra('api key', disable_trace=True)
+    catchpoint = Catchpoint('api key', disable_trace=True)
 
-    for plugin in thundra.plugins:
+    for plugin in catchpoint.plugins:
         assert not type(plugin) is TracePlugin
 
 
 def test_if_disable_trace_is_set_to_false():
-    thundra = Thundra('api key', disable_trace=False)
+    catchpoint = Catchpoint('api key', disable_trace=False)
 
     trace_exist = False
-    for plugin in thundra.plugins:
+    for plugin in catchpoint.plugins:
         if isinstance(plugin, TracePlugin):
             trace_exist = True
 
     assert trace_exist is True
 
 
 def test_if_disable_trace_is_not_set():
-    thundra = Thundra('api key')
+    catchpoint = Catchpoint('api key')
 
     trace_exist = False
-    for plugin in thundra.plugins:
+    for plugin in catchpoint.plugins:
         if isinstance(plugin, TracePlugin):
             trace_exist = True
 
     assert trace_exist is True
 
 
 def test_disable_trace_plugin_from_environment_variable():
-    ConfigProvider.set(config_names.THUNDRA_TRACE_DISABLE, 'true')
-    thundra = Thundra('api key')
+    ConfigProvider.set(config_names.CATCHPOINT_TRACE_DISABLE, 'true')
+    catchpoint = Catchpoint('api key')
 
     trace_exist = False
-    for plugin in thundra.plugins:
+    for plugin in catchpoint.plugins:
         if isinstance(plugin, TracePlugin):
             trace_exist = True
 
     assert trace_exist is False
 
 
 def test_enable_trace_plugin_from_environment_variable():
-    ConfigProvider.set(config_names.THUNDRA_TRACE_DISABLE, 'false')
-    thundra = Thundra('api key')
+    ConfigProvider.set(config_names.CATCHPOINT_TRACE_DISABLE, 'false')
+    catchpoint = Catchpoint('api key')
 
     trace_exist = False
-    for plugin in thundra.plugins:
+    for plugin in catchpoint.plugins:
         if isinstance(plugin, TracePlugin):
             trace_exist = True
 
     assert trace_exist is True
 
 
 def test_if_disable_trace_plugin_from_environment_variable_is_prior():
-    ConfigProvider.set(config_names.THUNDRA_TRACE_DISABLE, 'true')
-    thundra = Thundra('api key', disable_trace=False)
+    ConfigProvider.set(config_names.CATCHPOINT_TRACE_DISABLE, 'true')
+    catchpoint = Catchpoint('api key', disable_trace=False)
 
     trace_exist = False
-    for plugin in thundra.plugins:
+    for plugin in catchpoint.plugins:
         if isinstance(plugin, TracePlugin):
             trace_exist = True
 
     assert trace_exist is False
 
 
 def test_if_enable_trace_plugin_from_environment_variable_is_prior():
-    ConfigProvider.set(config_names.THUNDRA_TRACE_DISABLE, 'false')
-    thundra = Thundra('api key', disable_trace=True)
+    ConfigProvider.set(config_names.CATCHPOINT_TRACE_DISABLE, 'false')
+    catchpoint = Catchpoint('api key', disable_trace=True)
 
     trace_exist = False
-    for plugin in thundra.plugins:
+    for plugin in catchpoint.plugins:
         if isinstance(plugin, TracePlugin):
             trace_exist = True
 
     assert trace_exist is True
 
 
-@mock.patch('thundra.reporter.Reporter')
-def test_if_thundra_is_disabled(mock_reporter, handler, mock_event, mock_context):
-    ConfigProvider.set(config_names.THUNDRA_TRACE_DISABLE, 'true')
+@mock.patch('catchpoint.reporter.Reporter')
+def test_if_catchpoint_is_disabled(mock_reporter, handler, mock_event, mock_context):
+    ConfigProvider.set(config_names.CATCHPOINT_TRACE_DISABLE, 'true')
     _, handler = handler
 
     handler(mock_event, mock_context)
 
     assert not mock_reporter.add_report.called
     assert not mock_reporter.send_reports.called
 
 
 def test_if_exception_is_handled(handler_with_exception, mock_context, mock_event):
-    thundra, handler = handler_with_exception
+    catchpoint, handler = handler_with_exception
     with pytest.raises(Exception):
         handler(mock_event, mock_context)
 
     assert ExecutionContextManager.get().error
 
 
-@mock.patch('thundra.thundra_agent.Thundra.check_and_handle_warmup_request')
-def test_if_thundra_crashes_user_handler_before(mocked_func, handler, mock_event, mock_context):
+@mock.patch('catchpoint.catchpoint_agent.Catchpoint.check_and_handle_warmup_request')
+def test_if_catchpoint_crashes_user_handler_before(mocked_func, handler, mock_event, mock_context):
     mocked_func.side_effect = RuntimeError('Boom!')
-    thundra, handler = handler
+    catchpoint, handler = handler
     try:
         handler(mock_event, mock_context)
     except Exception:
-        pytest.fail("User's handler shouldn't fail when Thundra raise an exception")
+        pytest.fail("User's handler shouldn't fail when Catchpoint raise an exception")
 
 
-@mock.patch('thundra.reporter.Reporter.send_reports')
-def test_if_thundra_crashes_user_handler_after(mocked_func, handler, mock_event, mock_context):
+@mock.patch('catchpoint.reporter.Reporter.send_reports')
+def test_if_catchpoint_crashes_user_handler_after(mocked_func, handler, mock_event, mock_context):
     mocked_func.side_effect = RuntimeError('Boom!')
-    thundra, handler = handler
+    catchpoint, handler = handler
     try:
         handler(mock_event, mock_context)
     except Exception:
-        pytest.fail("User's handler shouldn't fail when Thundra raise an exception")
+        pytest.fail("User's handler shouldn't fail when Catchpoint raise an exception")
```

### Comparing `thundra-3.0.6/tests/test_utils.py` & `thundra-3.0.7/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from thundra import utils, constants
+from catchpoint import utils, constants
 
 
 def test_get_default_timeout_margin(monkeypatch):
     monkeypatch.setitem(os.environ, constants.AWS_REGION, 'us-west-2')
     timeout_margin = utils.get_default_timeout_margin()
     assert timeout_margin == 200
 
@@ -35,12 +35,12 @@
             'eu-central-1', 'eu-west-1', 'eu-west-2', 'eu-west-3', 'eu-north-1', 'eu-south-1',
             'ap-south-1', 'ap-northeast-1', 'ap-northeast-2', 'ap-southeast-1', 'ap-southeast-2', 
             'ap-east-1', 'af-south-1', 'me-south-1']
 
     for region in regions:
         monkeypatch.setitem(os.environ, constants.AWS_REGION, region)
         collector = utils.get_nearest_collector()
-        assert collector == "{}.collector.thundra.io".format(region)
+        assert collector == "{}.collector.catchpoint.com".format(region)
     
     monkeypatch.delitem(os.environ, constants.AWS_REGION)
     collector = utils.get_nearest_collector()
-    assert collector == "collector.thundra.io"
+    assert collector == "collector.catchpoint.com"
```

### Comparing `thundra-3.0.6/thundra/__init__.py` & `thundra-3.0.7/catchpoint/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from __future__ import absolute_import
 
 from importlib import import_module as _import_module
 
-import thundra.integrations.modules as integrations
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.plugins.invocation.invocation_support import (
+import catchpoint.integrations.modules as integrations
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.plugins.invocation.invocation_support import (
     set_tag,
     set_tags,
     remove_tag,
     get_tag,
     get_tags,
     set_error,
     clear_error
 )
-from thundra.plugins.invocation.invocation_trace_support import (
+from catchpoint.plugins.invocation.invocation_trace_support import (
     add_incoming_trace_link,
     add_incoming_trace_links,
     add_outgoing_trace_link,
     add_outgoing_trace_links,
     get_incoming_trace_links,
     get_outgoing_trace_links,
 )
-from thundra.plugins.log import log_support as log
-from thundra.plugins.metric import metric_support as metric
-from thundra.plugins.trace import trace_support as trace
-from thundra.plugins.trace.trace_aware_wrapper import TraceAwareWrapper
-from thundra.plugins.trace.traceable import Traceable
-from thundra.wrappers.wrapper_factory import WrapperFactory as _WrapperFactory
+from catchpoint.plugins.log import log_support as log
+from catchpoint.plugins.metric import metric_support as metric
+from catchpoint.plugins.trace import trace_support as trace
+from catchpoint.plugins.trace.trace_aware_wrapper import TraceAwareWrapper
+from catchpoint.plugins.trace.traceable import Traceable
+from catchpoint.wrappers.wrapper_factory import WrapperFactory as _WrapperFactory
 
 import logging
 logger = logging.getLogger(__name__)
 
 def _import_exists(module_name):
     try:
         _import_module(module_name)
@@ -52,49 +52,47 @@
 
 
 def configure(options=None):
     ConfigProvider.__init__(options)
 
 
 def lambda_wrapper(func):
-    from thundra.wrappers.aws_lambda.lambda_wrapper import LambdaWrapper
+    from catchpoint.wrappers.aws_lambda.lambda_wrapper import LambdaWrapper
     return _WrapperFactory.get_or_create(LambdaWrapper)(func)
 
 
 def django_wrapper(func):
-    from thundra.wrappers.django.django_wrapper import DjangoWrapper
+    from catchpoint.wrappers.django.django_wrapper import DjangoWrapper
     return _WrapperFactory.get_or_create(DjangoWrapper)(func)
 
 
 def flask_wrapper(func):
-    from thundra.wrappers.flask.flask_wrapper import FlaskWrapper
+    from catchpoint.wrappers.flask.flask_wrapper import FlaskWrapper
     return _WrapperFactory.get_or_create(FlaskWrapper)(func)
 
 
 def fastapi_wrapper(func):
-    from thundra.wrappers.fastapi.fastapi_wrapper import FastapiWrapper
+    from catchpoint.wrappers.fastapi.fastapi_wrapper import FastapiWrapper
     return _WrapperFactory.get_or_create(FastapiWrapper)(func)
 
 
 def tornado_wrapper(func):
-    from thundra.wrappers.tornado.tornado_wrapper import TornadoWrapper
+    from catchpoint.wrappers.tornado.tornado_wrapper import TornadoWrapper
     return _WrapperFactory.get_or_create(TornadoWrapper)(func)
 
 
-def _set_thundra_for_test_env(already_configured):
+def _set_catchpoint_for_test_env(already_configured):
     if not already_configured:
         configure()
-    if not ConfigProvider.get(config_names.THUNDRA_DISABLE):
+    if not ConfigProvider.get(config_names.CATCHPOINT_DISABLE):
         _patch_modules()
 
 
-if not ConfigProvider.get(config_names.THUNDRA_DISABLE):
-    test_active = ConfigProvider.get(config_names.THUNDRA_TEST_ACTIVE)
-    if not test_active:
-        _patch_modules()
+if not ConfigProvider.get(config_names.CATCHPOINT_DISABLE):
+    _patch_modules()
 
 
 __all__ = [
     'configure',
     'TraceAwareWrapper',
     'log',
     'metric',
```

### Comparing `thundra-3.0.6/thundra/application/application_info.py` & `thundra-3.0.7/catchpoint/application/application_info.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.6/thundra/application/application_info_provider.py` & `thundra-3.0.7/catchpoint/application/application_info_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc, sys
 
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
 ABC = abc.ABCMeta('ABC', (object,), {})
 
 
 class ApplicationInfoProvider(ABC):
     
     APPLICATION_RUNTIME = "python"
@@ -14,14 +14,14 @@
     @abc.abstractmethod
     def get_application_info(self):
         pass
 
     @staticmethod
     def parse_application_tags():
         application_tags = {}
-        prefix_length = len(config_names.THUNDRA_APPLICATION_TAG_PREFIX) + 1
+        prefix_length = len(config_names.CATCHPOINT_APPLICATION_TAG_PREFIX) + 1
         for key in ConfigProvider.configs:
-            if key.startswith(config_names.THUNDRA_APPLICATION_TAG_PREFIX) and len(key) >= prefix_length:
+            if key.startswith(config_names.CATCHPOINT_APPLICATION_TAG_PREFIX) and len(key) >= prefix_length:
                 app_tag_key = key[prefix_length:]
                 val = ConfigProvider.get(key)
                 application_tags[app_tag_key] = val
         return application_tags
```

### Comparing `thundra-3.0.6/thundra/application/global_application_info_provider.py` & `thundra-3.0.7/catchpoint/application/global_application_info_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from thundra.application.application_info_provider import ApplicationInfoProvider
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
+from catchpoint.application.application_info_provider import ApplicationInfoProvider
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
 
 class GlobalApplicationInfoProvider(ApplicationInfoProvider):
     def __init__(self, application_info_provider=None):
         self.application_info = {}
         self.application_info_provider = application_info_provider
         if self.application_info_provider:
@@ -19,22 +19,22 @@
 
     def get_application_tags(self):
         return self.application_info.get('applicationTags', {}).copy()
 
     @staticmethod
     def get_application_info_from_config():
         return {
-            'applicationId': ConfigProvider.get(config_names.THUNDRA_APPLICATION_ID),
-            'applicationInstanceId': ConfigProvider.get(config_names.THUNDRA_APPLICATION_INSTANCE_ID),
-            'applicationDomainName': ConfigProvider.get(config_names.THUNDRA_APPLICATION_DOMAIN_NAME),
-            'applicationClassName': ConfigProvider.get(config_names.THUNDRA_APPLICATION_CLASS_NAME),
-            'applicationName': ConfigProvider.get(config_names.THUNDRA_APPLICATION_NAME),
-            'applicationVersion': ConfigProvider.get(config_names.THUNDRA_APPLICATION_VERSION, ''),
-            'applicationStage': ConfigProvider.get(config_names.THUNDRA_APPLICATION_STAGE, ''),
-            'applicationRegion': ConfigProvider.get(config_names.THUNDRA_APPLICATION_REGION, ''),
+            'applicationId': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_ID),
+            'applicationInstanceId': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_INSTANCE_ID),
+            'applicationDomainName': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_DOMAIN_NAME),
+            'applicationClassName': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_CLASS_NAME),
+            'applicationName': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_NAME),
+            'applicationVersion': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_VERSION, ''),
+            'applicationStage': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_STAGE, ''),
+            'applicationRegion': ConfigProvider.get(config_names.CATCHPOINT_APPLICATION_REGION, ''),
             'applicationRuntime': ApplicationInfoProvider.APPLICATION_RUNTIME,
             'applicationRuntimeVersion': ApplicationInfoProvider.APPLICATION_RUNTIME_VERSION,
             'applicationTags': ApplicationInfoProvider.parse_application_tags()
         }
 
     def update(self, opts):
         filtered_opts = {k: v for k, v in opts.items() if v is not None}
```

### Comparing `thundra-3.0.6/thundra/compat.py` & `thundra-3.0.7/catchpoint/compat.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.6/thundra/composite.py` & `thundra-3.0.7/catchpoint/composite.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 
-from thundra import constants
+from catchpoint import constants
 
 _common_fields_list = [
     'agentVersion',
     'dataModelVersion',
     'applicationId',
     'applicationDomainName',
     'applicationClassName',
```

### Comparing `thundra-3.0.6/thundra/config/config_metadata.py` & `thundra-3.0.7/catchpoint/config/config_metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,318 +1,257 @@
-from thundra.config import config_names
+from catchpoint.config import config_names
 
 CONFIG_METADATA = {
-    config_names.THUNDRA_APIKEY: {
+    config_names.CATCHPOINT_APIKEY: {
         'type': 'string',
     },
-    config_names.THUNDRA_DEBUG_ENABLE: {
+    config_names.CATCHPOINT_DEBUG_ENABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_DISABLE: {
+    config_names.CATCHPOINT_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_DISABLE: {
+    config_names.CATCHPOINT_TRACE_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_METRIC_DISABLE: {
+    config_names.CATCHPOINT_METRIC_DISABLE: {
         'type': 'boolean',
         'defaultValue': True,
     },
-    config_names.THUNDRA_LOG_DISABLE: {
+    config_names.CATCHPOINT_LOG_DISABLE: {
         'type': 'boolean',
         'defaultValue': True,
     },
-    config_names.THUNDRA_APPLICATION_ID: {
+    config_names.CATCHPOINT_APPLICATION_ID: {
         'type': 'string',
     },
-    config_names.THUNDRA_APPLICATION_INSTANCE_ID: {
+    config_names.CATCHPOINT_APPLICATION_INSTANCE_ID: {
         'type': 'string',
     },
-    config_names.THUNDRA_APPLICATION_NAME: {
+    config_names.CATCHPOINT_APPLICATION_NAME: {
         'type': 'string',
     },
-    config_names.THUNDRA_APPLICATION_STAGE: {
+    config_names.CATCHPOINT_APPLICATION_STAGE: {
         'type': 'string',
     },
-    config_names.THUNDRA_APPLICATION_DOMAIN_NAME: {
+    config_names.CATCHPOINT_APPLICATION_DOMAIN_NAME: {
         'type': 'string',
         'defaultValue': 'API',
     },
-    config_names.THUNDRA_APPLICATION_CLASS_NAME: {
+    config_names.CATCHPOINT_APPLICATION_CLASS_NAME: {
         'type': 'string',
         'defaultValue': 'AWS-Lambda',
     },
-    config_names.THUNDRA_APPLICATION_VERSION: {
+    config_names.CATCHPOINT_APPLICATION_VERSION: {
         'type': 'string',
     },
-    config_names.THUNDRA_APPLICATION_TAG_PREFIX: {
+    config_names.CATCHPOINT_APPLICATION_TAG_PREFIX: {
         'type': 'any',
     },
-    config_names.THUNDRA_REPORT_REST_BASEURL: {
+    config_names.CATCHPOINT_REPORT_REST_BASEURL: {
         'type': 'string',
-        'defaultValue': 'https://collector.thundra.io/v1',
+        'defaultValue': 'https://collector.tracing.catchpoint.com/v1',
     },
-    config_names.THUNDRA_REPORT_CLOUDWATCH_ENABLE: {
+    config_names.CATCHPOINT_REPORT_CLOUDWATCH_ENABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_REPORT_REST_LOCAL: {
+    config_names.CATCHPOINT_REPORT_REST_LOCAL: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_REPORT_REST_COMPOSITE_BATCH_SIZE: {
+    config_names.CATCHPOINT_REPORT_REST_COMPOSITE_BATCH_SIZE: {
         'type': 'int',
         'defaultValue': 100,
     },
-    config_names.THUNDRA_REPORT_CLOUDWATCH_COMPOSITE_BATCH_SIZE: {
+    config_names.CATCHPOINT_REPORT_CLOUDWATCH_COMPOSITE_BATCH_SIZE: {
         'type': 'int',
         'defaultValue': 10,
     },
-    config_names.THUNDRA_REPORT_REST_COMPOSITE_ENABLE: {
+    config_names.CATCHPOINT_REPORT_REST_COMPOSITE_ENABLE: {
         'type': 'boolean',
         'defaultValue': True,
     },
-    config_names.THUNDRA_REPORT_CLOUDWATCH_COMPOSITE_ENABLE: {
+    config_names.CATCHPOINT_REPORT_CLOUDWATCH_COMPOSITE_ENABLE: {
         'type': 'boolean',
         'defaultValue': True,
     },
-    config_names.THUNDRA_LAMBDA_HANDLER: {
+    config_names.CATCHPOINT_LAMBDA_HANDLER: {
         'type': 'string',
     },
-    config_names.THUNDRA_LAMBDA_WARMUP_WARMUPAWARE: {
+    config_names.CATCHPOINT_LAMBDA_WARMUP_WARMUPAWARE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LAMBDA_TIMEOUT_MARGIN: {
+    config_names.CATCHPOINT_LAMBDA_TIMEOUT_MARGIN: {
         'type': 'int',
     },
-    config_names.THUNDRA_LAMBDA_ERROR_STACKTRACE_MASK: {
+    config_names.CATCHPOINT_LAMBDA_ERROR_STACKTRACE_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_REQUEST_SKIP: {
+    config_names.CATCHPOINT_TRACE_REQUEST_SKIP: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_RESPONSE_SKIP: {
+    config_names.CATCHPOINT_TRACE_RESPONSE_SKIP: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LAMBDA_TRACE_KINESIS_REQUEST_ENABLE: {
+    config_names.CATCHPOINT_LAMBDA_TRACE_KINESIS_REQUEST_ENABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LAMBDA_TRACE_FIREHOSE_REQUEST_ENABLE: {
+    config_names.CATCHPOINT_LAMBDA_TRACE_FIREHOSE_REQUEST_ENABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LAMBDA_TRACE_CLOUDWATCHLOG_REQUEST_ENABLE: {
+    config_names.CATCHPOINT_LAMBDA_TRACE_CLOUDWATCHLOG_REQUEST_ENABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LAMBDA_AWS_STEPFUNCTIONS: {
+    config_names.CATCHPOINT_LAMBDA_AWS_STEPFUNCTIONS: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LAMBDA_AWS_APPSYNC: {
+    config_names.CATCHPOINT_LAMBDA_AWS_APPSYNC: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INSTRUMENT_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INSTRUMENT_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INSTRUMENT_TRACEABLECONFIG: {
+    config_names.CATCHPOINT_TRACE_INSTRUMENT_TRACEABLECONFIG: {
         'type': 'string',
     },
-    config_names.THUNDRA_TRACE_SPAN_LISTENERCONFIG: {
+    config_names.CATCHPOINT_TRACE_SPAN_LISTENERCONFIG: {
         'type': 'string',
     },
-    config_names.THUNDRA_SAMPLER_TIMEAWARE_TIMEFREQ: {
+    config_names.CATCHPOINT_SAMPLER_TIMEAWARE_TIMEFREQ: {
         'type': 'int',
         'defaultValue': 300000,
     },
-    config_names.THUNDRA_SAMPLER_COUNTAWARE_COUNTFREQ: {
+    config_names.CATCHPOINT_SAMPLER_COUNTAWARE_COUNTFREQ: {
         'type': 'int',
         'defaultValue': 100
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SNS_MESSAGE_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SNS_MESSAGE_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SNS_TRACEINJECTION_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SNS_TRACEINJECTION_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SQS_MESSAGE_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SQS_MESSAGE_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SQS_TRACEINJECTION_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SQS_TRACEINJECTION_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_LAMBDA_PAYLOAD_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_LAMBDA_PAYLOAD_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_LAMBDA_TRACEINJECTION_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_LAMBDA_TRACEINJECTION_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_DYNAMODB_STATEMENT_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_DYNAMODB_STATEMENT_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_DYNAMODB_TRACEINJECTION_ENABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_DYNAMODB_TRACEINJECTION_ENABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_ATHENA_STATEMENT_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_ATHENA_STATEMENT_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_BODY_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_BODY_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_URL_DEPTH: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_URL_DEPTH: {
         'type': 'int',
         'defaultValue': 1,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_TRACEINJECTION_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_TRACEINJECTION_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_ERROR_STATUS_CODE_MIN: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_ERROR_STATUS_CODE_MIN: {
         'type': 'int',
         'defaultValue': 400,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_REDIS_COMMAND_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_REDIS_COMMAND_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_ELASTICSEARCH_BODY_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_ELASTICSEARCH_BODY_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_ELASTICSEARCH_PATH_DEPTH: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_ELASTICSEARCH_PATH_DEPTH: {
         'type': 'int',
         'defaultValue': 1,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_MONGODB_COMMAND_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_MONGODB_COMMAND_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_EVENTBRIDGE_DETAIL_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_EVENTBRIDGE_DETAIL_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SES_MAIL_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SES_MAIL_MASK: {
         'type': 'boolean',
         'defaultValue': True,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SES_MAIL_DESTINATION_MASK: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SES_MAIL_DESTINATION_MASK: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_CHALICE_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_CHALICE_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_DJANGO_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_DJANGO_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_DJANGO_ORM_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_DJANGO_ORM_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_FLASK_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_FLASK_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_FASTAPI_DISABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_FASTAPI_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LOG_CONSOLE_DISABLE: {
+    config_names.CATCHPOINT_LOG_CONSOLE_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
     },
-    config_names.THUNDRA_LOG_LOGLEVEL: {
+    config_names.CATCHPOINT_LOG_LOGLEVEL: {
         'type': 'string',
         'defaultValue': 'TRACE',
     },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_ENABLE: {
+    config_names.CATCHPOINT_TRACE_INTEGRATIONS_TORNADO_DISABLE: {
         'type': 'boolean',
         'defaultValue': False,
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_PORT: {
-        'type': 'int',
-        'defaultValue': 1111,
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_LOGS_ENABLE: {
-        'type': 'boolean',
-        'defaultValue': False,
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_WAIT_MAX: {
-        'type': 'int',
-        'defaultValue': 60000,
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_IO_WAIT: {
-        'type': 'int',
-        'defaultValue': 2000,
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_BROKER_PORT: {
-        'type': 'int',
-        'defaultValue': 444,
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_BROKER_HOST: {
-        'type': 'string',
-        'defaultValue': 'broker.service.serverlessdebugger.com',
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_SESSION_NAME: {
-        'type': 'string',
-        'defaultValue': 'default',
-    },
-    config_names.THUNDRA_LAMBDA_DEBUGGER_AUTH_TOKEN: {
-        'type': 'string',
-    },
-    config_names.THUNDRA_TRACE_INTEGRATIONS_TORNADO_DISABLE: {
-        'type': 'boolean',
-        'defaultValue': False,
-    },
-    config_names.THUNDRA_TEST_RUN_ID: {
-        'type': 'string'
-    },
-    config_names.THUNDRA_TEST_PROJECT_ID: {
-        'type': 'string'
-    },
-    config_names.THUNDRA_TEST_STATUS_REPORT_FREQUENCY: {
-        'type': 'int',
-        'defaultValue': 10,
-    },
-    config_names.THUNDRA_TEST_LOG_COUNT_MAX: {
-        'type': 'int',
-        'defaultValue': 100,
-    },
-    config_names.THUNDRA_TEST_SPAN_COUNT_MAX: {
-        'type': 'int',
-        'defaultValue': 100,
-    },
-    config_names.THUNDRA_TEST_ACTIVE: {
-        'type': 'bool',
-        'defaultValue': False,
-    },
-    config_names.THUNDRA_TEST_DISABLE: {
-        'type': 'bool',
-        'defaultValue': False,
     }
 }
```

### Comparing `thundra-3.0.6/thundra/config/config_provider.py` & `thundra-3.0.7/catchpoint/config/config_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import os
 
-from thundra.config import config_names
-from thundra.config.config_metadata import CONFIG_METADATA
+from catchpoint.config import config_names
+from catchpoint.config.config_metadata import CONFIG_METADATA
 
 
 class ConfigProvider:
     configs = {}
 
     @staticmethod
     def __init__(options=None):
         ConfigProvider.clear()
         if options is not None:
             config_options = options.get('config', {})
             for opt in config_options:
-                if opt.lower() == config_names.THUNDRA_APIKEY:
-                    ConfigProvider.configs[config_names.THUNDRA_APIKEY] = config_options.get(opt)
+                if opt.lower() == config_names.CATCHPOINT_APIKEY:
+                    ConfigProvider.configs[config_names.CATCHPOINT_APIKEY] = config_options.get(opt)
                 ConfigProvider.traverse_config_object(config_options.get(opt), opt)
         ConfigProvider.initialize_config_from_environment_variables()
         ConfigProvider.add_non_lambda_aliases()
 
     @staticmethod
     def initialize_config_from_environment_variables():
         env_variables = os.environ
 
         for var_name in env_variables:
-            if var_name.upper().startswith("THUNDRA_"):
+            if var_name.upper().startswith("CATCHPOINT_"):
                 env_var_name = ConfigProvider.env_var_to_config_name(var_name)
                 val = env_variables.get(var_name).strip()
                 env_var_type = ConfigProvider.get_config_type(env_var_name)
                 ConfigProvider.configs[env_var_name] = ConfigProvider.parse(val, env_var_type)
 
     @staticmethod
     def traverse_config_object(obj, path):
         if not isinstance(obj, dict):
-            if not path.startswith('thundra.agent.'):
-                path = 'thundra.agent.' + path
+            if not path.startswith('catchpoint.'):
+                path = 'catchpoint.' + path
             path = path.lower()
             prop_type = ConfigProvider.get_config_type(path)
             ConfigProvider.configs[path] = ConfigProvider.parse(obj, prop_type)
         else:
             for prop_name in obj:
                 prop_val = obj.get(prop_name)
                 prop_path = path + '.' + prop_name
                 ConfigProvider.traverse_config_object(prop_val, prop_path)
 
     @staticmethod
     def add_non_lambda_aliases():
         alias_configs = {}
         for config_name in ConfigProvider.configs:
-            if config_name.startswith('thundra.agent.lambda'):
+            if config_name.startswith('catchpoint.lambda'):
                 value = ConfigProvider.configs[config_name]
-                alias_configs[config_name.replace('thundra.agent.lambda', 'thundra.agent', 1)] = value
+                alias_configs[config_name.replace('catchpoint.lambda', 'catchpoint', 1)] = value
         ConfigProvider.configs.update(alias_configs)
 
     @staticmethod
     def get(key, default_value=None):
         value = ConfigProvider.configs.get(key)
         if value is not None:
             return value
@@ -66,16 +66,16 @@
 
     @staticmethod
     def get_config_type(config_name):
         config_metadata = CONFIG_METADATA.get(config_name)
         if config_metadata:
             return config_metadata.get('type')
         else:
-            if config_name.startswith('thundra.agent.lambda.'):
-                config_name = config_name.replace('thundra.agent.lambda.', 'thundra.agent.', 1)
+            if config_name.startswith('catchpoint.lambda.'):
+                config_name = config_name.replace('catchpoint.lambda.', 'catchpoint.', 1)
                 config_metadata = CONFIG_METADATA.get(config_name)
                 if config_metadata:
                     return config_metadata.get('type')
         return None
 
     @staticmethod
     def parse(value, var_type):
```

### Comparing `thundra-3.0.6/thundra/constants.py` & `thundra-3.0.7/catchpoint/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from collections import OrderedDict
 
-from thundra._version import __version__
+from catchpoint._version import __version__
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S.%f %z"
 
-HOST = "https://api.thundra.io/v1"
+HOST = "https://collector.tracing.catchpoint.com/v1"
 PATH = "/monitoring-data"
 COMPOSITE_DATA_PATH = "/composite-monitoring-data"
 
-THUNDRA_AGENT_VERSION = __version__
+CATCHPOINT_AGENT_VERSION = __version__
 TEST_RUN_EVENTS_DATA_VERSION = "1.0"
 
 DEFAULT_APPLICATION_NAME = 'catchpoint-app'
 LAMBDA_APPLICATION_DOMAIN_NAME = 'API'
 LAMBDA_APPLICATION_CLASS_NAME = 'AWS-Lambda'
 LAMBDA_APPLICATION_PLATFORM = 'AWS Lambda'
 
 TRIGGER_OPERATION_NAME_KEY = 'x-catchpoint-trigger-operation-name'
 TRIGGER_CLASS_NAME_KEY = 'x-catchpoint-trigger-class-name'
 TRIGGER_DOMAIN_NAME_KEY = 'x-catchpoint-trigger-domain-name'
 TRIGGER_RESOURCE_NAME_KEY = 'x-catchpoint-resource-name'
 
-THUNDRA_TRACE_ID_KEY = 'x-catchpoint-trace-id'
-THUNDRA_TRANSACTION_ID_KEY = 'x-catchpoint-transaction-id'
-THUNDRA_SPAN_ID_KEY = 'x-catchpoint-span-id'
-THUNDRA_BAGGAGE_PREFIX = 'x-catchpoint-baggage-'
+CATCHPOINT_TRACE_ID_KEY = 'x-catchpoint-trace-id'
+CATCHPOINT_TRANSACTION_ID_KEY = 'x-catchpoint-transaction-id'
+CATCHPOINT_SPAN_ID_KEY = 'x-catchpoint-span-id'
+CATCHPOINT_BAGGAGE_PREFIX = 'x-catchpoint-baggage-'
 
 DEFAULT_METRIC_SAMPLING_TIME_FREQ = 5 * 60 * 1000
 DEFAULT_METRIC_SAMPLING_COUNT_FREQ = 100
 
 AWS_LAMBDA_APPLICATION_ID = 'AWS_LAMBDA_APPLICATION_ID'
 AWS_SAM_LOCAL = 'AWS_SAM_LOCAL'
 AWS_LAMBDA_LOG_STREAM_NAME = 'AWS_LAMBDA_LOG_STREAM_NAME'
@@ -57,22 +57,22 @@
 MAX_OUTGOING_TRACE_LINKS = 20
 
 LIST_SEPARATOR = ','
 
 DEFAULT_LAMBDA_TIMEOUT_MARGIN = 200
 DATA_FORMAT_VERSION = '2.0'
 
-THUNDRA_LAMBDA_SPAN_LISTENER_INFO_TAG = 'thundra.span_listener.info'
+CATCHPOINT_LAMBDA_SPAN_LISTENER_INFO_TAG = 'catchpoint.span_listener.info'
 
 DEFAULT_REPORT_REST_COMPOSITE_BATCH_SIZE = 100
 DEFAULT_REPORT_CLOUDWATCH_COMPOSITE_BATCH_SIZE = 10
 
 #### INTEGRATIONS ####
 
-THUNDRA_MAX_STREAM_REQUEST_BODY = 200 * 1024
+CATCHPOINT_MAX_STREAM_REQUEST_BODY = 200 * 1024
 DEFAULT_MONGO_COMMAND_SIZE_LIMIT = 128 * 1024
 DEFAULT_REPORT_TIMEOUT = 5
 
 AWS_SERVICE_REQUEST = 'AWSServiceRequest'
 
 LineByLineTracingTags = {
     'lines': 'method.lines',
@@ -396,15 +396,15 @@
     'ES_BODY': 'elasticsearch.body',
     'ES_HOSTS': 'elasticsearch.hosts',
     'ES_NORMALIZED_URI': 'elasticsearch.normalized_uri'
 }
 
 AwsXrayConstants = {
     'DEFAULT_OPERATION_NAME': 'AWS X-Ray',
-    'XRAY_SUBSEGMENTED_TAG_NAME': 'THUNDRA::XRAY_SUBSEGMENTED',
+    'XRAY_SUBSEGMENTED_TAG_NAME': 'CATCHPOINT::XRAY_SUBSEGMENTED',
 }
 
 MongoDBTags = {
     'MONGODB_COMMAND': 'mongodb.command',
     'MONGODB_COMMAND_NAME': 'mongodb.command.name',
     'MONGODB_COLLECTION': 'mongodb.collection.name',
 }
```

### Comparing `thundra-3.0.6/thundra/context/execution_context.py` & `thundra-3.0.7/catchpoint/context/execution_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from thundra.opentracing.recorder import ThundraRecorder
+from catchpoint.opentracing.recorder import CatchpointRecorder
 
 
 class ExecutionContext:
     """
     Represents the scope of execution (request, invocation, etc ...)
     and holds scope specific data.
     """
 
     def __init__(self, **opts):
         self.start_timestamp = opts.get('start_timestamp', 0)
         self.finish_timestamp = opts.get('finish_timestamp', 0)
-        self.recorder = opts.get('recorder', ThundraRecorder())
+        self.recorder = opts.get('recorder', CatchpointRecorder())
         self.reports = opts.get('reports', [])
         self.transaction_id = opts.get('transaction_id', '')
         self.span_id = opts.get('span_id', '')
         self.trace_id = opts.get('trace_id')
         self.root_span = opts.get('root_span')
         self.scope = opts.get('scope')
         self.invocation_data = opts.get('invocation_data')
```

### Comparing `thundra-3.0.6/thundra/context/execution_context_manager.py` & `thundra-3.0.7/catchpoint/context/execution_context_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from thundra.context.execution_context import ExecutionContext
-from thundra.context.global_execution_context_provider import GlobalExecutionContextProvider
+from catchpoint.context.execution_context import ExecutionContext
+from catchpoint.context.global_execution_context_provider import GlobalExecutionContextProvider
 
 
 class ExecutionContextManager:
     context_provider = None
 
     @staticmethod
     def set_provider(provider):
```

### Comparing `thundra-3.0.6/thundra/context/tracing_execution_context_provider.py` & `thundra-3.0.7/catchpoint/context/tracing_execution_context_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from thundra.context.context_provider import ContextProvider
-from thundra.context.execution_context import ExecutionContext
-from thundra.opentracing.tracer import ThundraTracer
+from catchpoint.context.context_provider import ContextProvider
+from catchpoint.context.execution_context import ExecutionContext
+from catchpoint.opentracing.tracer import CatchpointTracer
 
 
 class TracingExecutionContextProvider(ContextProvider):
     def __init__(self):
-        self.tracer = ThundraTracer.get_instance()
+        self.tracer = CatchpointTracer.get_instance()
 
     def get(self):
         execution_context = None
         active_span = self.tracer.get_active_span()
         if active_span and hasattr(active_span, 'execution_context'):
             execution_context = active_span.execution_context
         if not execution_context:
```

### Comparing `thundra-3.0.6/thundra/debug/bridge.py` & `thundra-3.0.7/catchpoint/debug/bridge.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     "SESSION_NAME": "x-catchpoint-session-name",
     "PROTOCOL_VER": "x-catchpoint-protocol-version",
     "RUNTIME": "x-catchpoint-runtime",
     "SESSION_TIMEOUT": "x-catchpoint-session-timeout"
 }
 
 BROKER_WS_HTTP_ERR_CODE_TO_MSG = {
-    429: "Reached the concurrent session limit, couldn't start Thundra debugger.",
-    401: "Authentication is failed, check your Thundra debugger authentication token.",
+    429: "Reached the concurrent session limit, couldn't start Catchpoint debugger.",
+    401: "Authentication is failed, check your Catchpoint debugger authentication token.",
     409: "Another session with the same session name exists, connection closed.",
 }
 
 ws = None
 debugger_socket = None
 
 
@@ -39,19 +39,19 @@
               file=sys.stderr)
     else:
         print("Broker connection got error: {}".format(error), file=sys.stderr)
 
 
 def handle_close_message(code, message):
     if code is None and message is None:
-        print("Thundra debug broker connection is closed")
+        print("Catchpoint debug broker connection is closed")
     elif code:
-        print("Thundra debug broker closed with code:{}".format(code))
+        print("Catchpoint debug broker closed with code:{}".format(code))
     else:
-        print("Thundra debug broker closed with code:{}, message:{}".format(code, message))
+        print("Catchpoint debug broker closed with code:{}, message:{}".format(code, message))
 
 
 def on_open(ws):
     def run():
         try:
             ws.running = True
             while ws.running:
```

### Comparing `thundra-3.0.6/thundra/handler.py` & `thundra-3.0.7/catchpoint/handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import absolute_import
 
 import imp
 import os
 
-from thundra.config.config_provider import ConfigProvider
-from thundra.config import config_names
-from thundra.thundra_agent import Thundra
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
+from catchpoint.catchpoint_agent import Catchpoint
 
-thundra = Thundra()
+catchpoint = Catchpoint()
 
 handler_found = False
 user_handler = None
 
-handler_path = ConfigProvider.get(config_names.THUNDRA_LAMBDA_HANDLER, None)
+handler_path = ConfigProvider.get(config_names.CATCHPOINT_LAMBDA_HANDLER, None)
 if handler_path is None:
     raise ValueError(
-        "No handler specified for \'thundra_agent_lambda_handler\' environment variable"
+        "No handler specified for \'catchpoint_lambda_handler\' environment variable"
     )
 else:
     handler_found = True
     (module_name, handler_name) = handler_path.rsplit('.', 1)
     file_handle, pathname, desc = None, None, None
     try:
         for segment in module_name.split('.'):
@@ -36,10 +36,10 @@
         if file_handle:
             file_handle.close()
 
 
 def wrapper(event, context):
     global user_handler
     if handler_found and user_handler:
-        if not hasattr(user_handler, "thundra_wrapper"):
-            user_handler = thundra(user_handler)
+        if not hasattr(user_handler, "catchpoint_wrapper"):
+            user_handler = catchpoint(user_handler)
         return user_handler(event, context)
```

### Comparing `thundra-3.0.6/thundra/integrations/aiohttp/client.py` & `thundra-3.0.7/catchpoint/integrations/aiohttp/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 from types import SimpleNamespace
 
 import aiohttp
 
-from thundra import constants, utils
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.opentracing.tracer import ThundraTracer
+from catchpoint import constants, utils
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.opentracing.tracer import CatchpointTracer
 
 logger = logging.getLogger(__name__)
 
 
 async def on_request_start(session, trace_config_ctx, params):
-    tracer = ThundraTracer.get_instance()
+    tracer = CatchpointTracer.get_instance()
     if not tracer.get_active_span():
         return
 
     url_dict = utils.parse_http_url(str(params.url),
-                                    ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_URL_DEPTH))
+                                    ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_URL_DEPTH))
     scope = tracer.start_active_span(operation_name=url_dict.get('operation_name'), finish_on_close=False)
     scope.span.class_name = constants.ClassNames['HTTP']
     scope.span.domain_name = constants.DomainNames['API']
 
     tags = {
         constants.SpanTags['OPERATION_TYPE']: params.method,
         constants.HttpTags['HTTP_METHOD']: params.method,
@@ -32,28 +32,28 @@
         constants.SpanTags['TOPOLOGY_VERTEX']: True,
     }
 
     scope.span.tags = tags
     try:
         scope.span.on_started()
         try:
-            params.headers.update({constants.THUNDRA_SPAN_ID_KEY: scope.span.span_id})
+            params.headers.update({constants.CATCHPOINT_SPAN_ID_KEY: scope.span.span_id})
             scope.span.set_tag(constants.SpanTags['TRACE_LINKS'], [scope.span.span_id])
         except Exception as e:
             pass
         trace_config_ctx.scope = scope
     except Exception as e:
         logger.error(e)
 
 
 async def on_request_chunk_sent(session, trace_config_ctx, params):
     if not hasattr(trace_config_ctx, "scope"):
         return
     scope = trace_config_ctx.scope
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_BODY_MASK) and \
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_BODY_MASK) and \
             (scope.span.get_tag(constants.HttpTags["BODY"]) is None):
         body = params.chunk if params.chunk else ""
         scope.span.set_tag(constants.HttpTags["BODY"], body)
 
 
 async def on_request_end(session, trace_config_ctx, params):
     if not hasattr(trace_config_ctx, "scope"):
@@ -69,15 +69,15 @@
             scope.span.class_name = constants.ClassNames['APIGATEWAY']
 
         if response.headers and response.headers.get(constants.TRIGGER_RESOURCE_NAME_KEY):
             resource_name = response.headers.get(constants.TRIGGER_RESOURCE_NAME_KEY)
             scope.span.operation_name = resource_name
 
         if (status_code and ConfigProvider.get(
-                config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_ERROR_STATUS_CODE_MIN) <= status_code):
+                config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_ERROR_STATUS_CODE_MIN) <= status_code):
             scope.span.set_tag('error.kind', "HttpError")
             scope.span.set_tag('error', True)
             scope.span.set_tag('error.message', response.reason)
     try:
         scope.span.finish()
     except Exception as e:
         logger.error(e)
@@ -94,15 +94,15 @@
         scope.span.finish()
     except Exception as e:
         logger.error(e)
 
     scope.close()
 
 
-def ThundraTraceConfig():
+def CatchpointTraceConfig():
     """
     :returns: TraceConfig.
     """
 
     def _trace_config_ctx_factory(trace_request_ctx):
         return SimpleNamespace(
             trace_request_ctx=trace_request_ctx
```

### Comparing `thundra-3.0.6/thundra/integrations/base_integration.py` & `thundra-3.0.7/catchpoint/integrations/base_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import abc
 import logging
 import time
 import traceback
 
-from thundra.opentracing.tracer import ThundraTracer
+from catchpoint.opentracing.tracer import CatchpointTracer
 
 logger = logging.getLogger(__name__)
 
 ABC = abc.ABCMeta('ABC', (object,), {})
 
 
 class BaseIntegration(ABC):
     def run_and_trace(self, wrapped, instance, args, kwargs):
-        tracer = ThundraTracer.get_instance()
+        tracer = CatchpointTracer.get_instance()
         if not tracer.get_active_span():
             return wrapped(*args, **kwargs)
 
         response = None
         exception = None
 
         scope = tracer.start_active_span(operation_name=self.get_operation_name(wrapped, instance, args, kwargs),
```

### Comparing `thundra-3.0.6/thundra/integrations/botocore.py` & `thundra-3.0.7/catchpoint/integrations/botocore.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import hashlib
 import uuid
 from datetime import datetime
 
 import json
 from dateutil.parser import parse
 
-import thundra.constants as constants
-import thundra.utils as utils
-from thundra.compat import PY37
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.encoder import to_json
-from thundra.integrations.base_integration import BaseIntegration
+import catchpoint.constants as constants
+import catchpoint.utils as utils
+from catchpoint.compat import PY37
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.encoder import to_json
+from catchpoint.integrations.base_integration import BaseIntegration
 
 OPERATION_TYPE_MAPPING_PATTERNS = utils.get_compiled_operation_type_patterns()
 
 
 def dummy_func(*args):
     return None
 
@@ -71,20 +71,20 @@
         # Check if Key and Item fields have any byte field and convert to string
         if 'Key' in self.request_data:
             self.escape_byte_fields(self.request_data['Key'])
         if 'Item' in self.request_data:
             self.escape_byte_fields(self.request_data['Item'])
 
         # DB statement tags should not be set on span if masked
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_DYNAMODB_STATEMENT_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_DYNAMODB_STATEMENT_MASK):
             self.OPERATION.get(operation_name, dummy_func)(scope)
 
         scope.span.set_tag(constants.SpanTags['TOPOLOGY_VERTEX'], True)
 
-        if ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_DYNAMODB_TRACEINJECTION_ENABLE):
+        if ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_DYNAMODB_TRACEINJECTION_ENABLE):
             if operation_name == 'PutItem':
                 self.inject_trace_link_on_put(scope.span, request_data, instance)
 
             if operation_name == 'UpdateItem':
                 self.inject_trace_link_on_update(scope.span, request_data, instance)
 
             if operation_name == 'DeleteItem':
@@ -123,17 +123,17 @@
                                                         params['Item'])
 
             elif operation_name == 'UpdateItem':
                 trace_links = self.generate_trace_links(region, response, params['TableName'], 'SAVE',
                                                         params['Key'])
 
             elif operation_name == 'DeleteItem':
-                if ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_DYNAMODB_TRACEINJECTION_ENABLE) and \
+                if ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_DYNAMODB_TRACEINJECTION_ENABLE) and \
                         'Attributes' in response:
-                    span_id = response['Attributes'].get(constants.THUNDRA_SPAN_ID_KEY)
+                    span_id = response['Attributes'].get(constants.CATCHPOINT_SPAN_ID_KEY)
                     if span_id and span_id.get('S'):
                         trace_links = ['DELETE:' + span_id.get('S')]
 
                 if not trace_links:
                     trace_links = self.generate_trace_links(region, response, params['TableName'], 'DELETE',
                                                             params['Key'])
 
@@ -166,56 +166,56 @@
                 attributes_sorted.append(attr + '=' + '{' + key + ': ' + str(attributes[attr][key]) + '}')
             except Exception as e:
                 pass
         return ', '.join(attributes_sorted)
 
     def inject_trace_link_on_put(self, span, request_data, instance):
 
-        thundra_span = {'S': span.span_id}
+        catchpoint_span = {'S': span.span_id}
         try:
             if PY37:
                 id_handlers = instance.meta.events._emitter._unique_id_handlers
             else:
                 id_handlers = instance.meta.events._unique_id_handlers
 
             if 'dynamodb-attr-value-input' in id_handlers:
-                thundra_span = span.span_id
+                catchpoint_span = span.span_id
         except Exception as e:
             pass
 
         try:
             if 'Item' in request_data:
-                request_data['Item'][constants.THUNDRA_SPAN_ID_KEY] = thundra_span
+                request_data['Item'][constants.CATCHPOINT_SPAN_ID_KEY] = catchpoint_span
             else:
-                request_data['Item'] = {constants.THUNDRA_SPAN_ID_KEY: thundra_span}
+                request_data['Item'] = {constants.CATCHPOINT_SPAN_ID_KEY: catchpoint_span}
 
             span.set_tag(constants.SpanTags['TRACE_LINKS'], ["SAVE:" + span.span_id])
         except:
             pass
 
     def inject_trace_link_on_update(self, span, request_data, instance):
 
-        thundra_span = {'S': span.span_id}
+        catchpoint_span = {'S': span.span_id}
         try:
             if PY37:
                 id_handlers = instance.meta.events._emitter._unique_id_handlers
             else:
                 id_handlers = instance.meta.events._unique_id_handlers
             if 'dynamodb-attr-value-input' in id_handlers:
-                thundra_span = span.span_id
+                catchpoint_span = span.span_id
         except Exception as e:
             pass
 
-        thundra_attr = {'Action': 'PUT', 'Value': thundra_span}
+        catchpoint_attr = {'Action': 'PUT', 'Value': catchpoint_span}
 
         try:
             if 'AttributeUpdates' in request_data:
-                request_data['AttributeUpdates'][constants.THUNDRA_SPAN_ID_KEY] = thundra_attr
+                request_data['AttributeUpdates'][constants.CATCHPOINT_SPAN_ID_KEY] = catchpoint_attr
             else:
-                request_data['AttributeUpdates'] = {constants.THUNDRA_SPAN_ID_KEY: thundra_attr}
+                request_data['AttributeUpdates'] = {constants.CATCHPOINT_SPAN_ID_KEY: catchpoint_attr}
 
             span.set_tag(constants.SpanTags['TRACE_LINKS'], ["SAVE:" + span.span_id])
         except:
             pass
 
     def inject_trace_link_on_delete(self, request_data):
         try:
@@ -294,15 +294,15 @@
             constants.SpanTags['OPERATION_TYPE']: get_operation_type(scope.span.class_name, operation_name),
             constants.AwsSDKTags['REQUEST_NAME']: operation_name,
         }
 
         scope.span.tags = tags
         scope.span.set_tag(constants.SpanTags['TOPOLOGY_VERTEX'], True)
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SQS_MESSAGE_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SQS_MESSAGE_MASK):
             if operation_name == "SendMessage":
                 message = request_data.get("MessageBody", "")
                 scope.span.set_tag(constants.AwsSQSTags['MESSAGE'], message)
 
             elif operation_name == "SendMessageBatch":
                 entries = request_data.get('Entries', None)
                 messages = []
@@ -371,15 +371,15 @@
             constants.SpanTags['OPERATION_TYPE']: get_operation_type(scope.span.class_name, operation_name),
             constants.AwsSNSTags['TOPIC_NAME']: self.topicName
         }
 
         scope.span.tags = tags
         scope.span.set_tag(constants.SpanTags['TOPOLOGY_VERTEX'], True)
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SNS_MESSAGE_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SNS_MESSAGE_MASK):
             scope.span.set_tag(constants.AwsSNSTags['MESSAGE'], self.message)
 
     def after_call(self, scope, wrapped, instance, args, kwargs, response, exception):
         super(AWSSNSIntegration, self).after_call(scope, wrapped, instance, args, kwargs, response, exception)
 
         trace_links = self.get_trace_links(response)
         if trace_links:
@@ -583,15 +583,15 @@
         tags = {
             constants.AwsSDKTags['REQUEST_NAME']: operation_name,
             constants.SpanTags['OPERATION_TYPE']: get_operation_type(scope.span.class_name, operation_name),
             constants.AwsLambdaTags['FUNCTION_NAME']: lambda_function.get('name'),
             constants.AwsLambdaTags['FUNCTION_QUALIFIER']: lambda_function.get('qualifier')
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_LAMBDA_PAYLOAD_MASK) and \
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_LAMBDA_PAYLOAD_MASK) and \
                 'Payload' in request_data:
             tags[constants.AwsLambdaTags['INVOCATION_PAYLOAD']] = str(request_data['Payload'],
                                                                       encoding='utf-8') if type(
                 request_data['Payload']) is not str else request_data['Payload']
 
         if 'Qualifier' in request_data:
             tags[constants.AwsLambdaTags['FUNCTION_QUALIFIER']] = request_data['Qualifier']
@@ -678,18 +678,18 @@
         state_machine_arn = request_data.get('stateMachineArn', '')
         execution_name = request_data.get('name', '')
 
         service_name = instance.__class__.__name__.lower()
 
         try:
             orig_input = request_data.get('input', None)
-            if orig_input != None and ConfigProvider.get(config_names.THUNDRA_LAMBDA_AWS_STEPFUNCTIONS):
+            if orig_input != None and ConfigProvider.get(config_names.CATCHPOINT_LAMBDA_AWS_STEPFUNCTIONS):
                 parsed_input = json.loads(orig_input)
                 trace_link = str(uuid.uuid4())
-                parsed_input['_thundra'] = {
+                parsed_input['_catchpoint'] = {
                     "trace_link": trace_link,
                     "step": 0
                 }
                 scope.span.set_tag(constants.AwsStepFunctionsTags['EXECUTION_INPUT'], orig_input)
                 request_data['input'] = to_json(parsed_input)
                 scope.span.set_tag(constants.SpanTags['TRACE_LINKS'], [trace_link])
                 scope.span.resource_trace_links = [trace_link]
@@ -789,15 +789,15 @@
 
         if database:
             scope.span.set_tag(constants.SpanTags['DB_INSTANCE'], database)
 
         if output_location:
             scope.span.set_tag(constants.AthenaTags['S3_OUTPUT_LOCATION'], output_location)
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_ATHENA_STATEMENT_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_ATHENA_STATEMENT_MASK):
             scope.span.set_tag(constants.DBTags['DB_STATEMENT'], self.get_query(args))
 
         if query_execution_ids:
             scope.span.set_tag(constants.AthenaTags['REQUEST_QUERY_EXECUTION_IDS'], query_execution_ids)
 
         if named_query_ids:
             scope.span.set_tag(constants.AthenaTags['REQUEST_NAMED_QUERY_IDS'], named_query_ids)
@@ -851,15 +851,15 @@
             constants.SpanTags['OPERATION_TYPE']: get_operation_type(scope.span.class_name, operation_name)
         }
 
         entries = []
         for entry in request_data.get('Entries', []):
             new_entry = {
                 'Detail': None if ConfigProvider.get(
-                    config_names.THUNDRA_TRACE_INTEGRATIONS_EVENTBRIDGE_DETAIL_MASK) else entry.get('Detail'),
+                    config_names.CATCHPOINT_TRACE_INTEGRATIONS_EVENTBRIDGE_DETAIL_MASK) else entry.get('Detail'),
                 'DetailType': entry.get('DetailType'),
                 'EventBusName': entry.get('EventBusName'),
                 'Resources': entry.get('Resources'),
                 'Source': entry.get('Source')
             }
             if isinstance(entry.get('Time'), datetime):
                 new_entry['Time'] = datetime.timestamp(entry.get('Time'))
@@ -904,16 +904,16 @@
         return operation_name if operation_name else constants.AWS_SERVICE_REQUEST
 
     def before_call(self, scope, wrapped, instance, args, kwargs, response, exception):
         operation_name, request_data = args
         scope.span.domain_name = constants.DomainNames['MESSAGING']
         scope.span.class_name = constants.ClassNames['SES']
 
-        mask_mail = ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SES_MAIL_MASK)
-        mask_destination = ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_AWS_SES_MAIL_DESTINATION_MASK)
+        mask_mail = ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SES_MAIL_MASK)
+        mask_destination = ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_AWS_SES_MAIL_DESTINATION_MASK)
 
         source = request_data.get('Source', '')
         destination = request_data.get('Destinations', request_data.get('Destination', []))
         subject = request_data.get('Message', {}).get('Subject')
         body = request_data.get('Message', {}).get('Body')
         template_name = request_data.get('Template')
         template_arn = request_data.get('TemplateArn')
```

### Comparing `thundra-3.0.6/thundra/integrations/django.py` & `thundra-3.0.7/catchpoint/integrations/django.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import thundra.constants as constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.base_integration import BaseIntegration
-from thundra.integrations.rdb_base import RdbBaseIntegration
+import catchpoint.constants as constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.base_integration import BaseIntegration
+from catchpoint.integrations.rdb_base import RdbBaseIntegration
 
 
 class DjangoORMIntegration(BaseIntegration, RdbBaseIntegration):
     CLASS_TYPE = 'django_orm'
 
     def __init__(self):
         pass
@@ -45,11 +45,11 @@
             constants.SpanTags['DB_INSTANCE']: settings.get('NAME'),
             constants.SpanTags['DB_HOST']: settings.get('HOST'),
             constants.SpanTags['DB_TYPE']: vendor,
             constants.SpanTags['DB_STATEMENT_TYPE']: operation.upper(),
             constants.SpanTags['TOPOLOGY_VERTEX']: True,
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
             tags[constants.DBTags['DB_STATEMENT']] = query
 
         scope.span.tags = tags
```

### Comparing `thundra-3.0.6/thundra/integrations/elasticsearch.py` & `thundra-3.0.7/catchpoint/integrations/elasticsearch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.base_integration import BaseIntegration
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.base_integration import BaseIntegration
 
 
 class ElasticsearchIntegration(BaseIntegration):
     CLASS_TYPE = 'elasticsearch'
 
     def __init__(self):
         pass
@@ -14,15 +14,15 @@
         try:
             hosts = [con.host for con in instance.connection_pool.connections]
             return hosts
         except Exception:
             return []
 
     def get_normalized_path(self, es_uri):
-        path_depth = ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_ELASTICSEARCH_PATH_DEPTH)
+        path_depth = ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_ELASTICSEARCH_PATH_DEPTH)
 
         path_seperator_count = 0
         normalized_path = ''
         prev_c = ''
         for c in es_uri:
             if c == '/' and prev_c != '/':
                 path_seperator_count += 1
@@ -59,11 +59,11 @@
             constants.ESTags['ES_METHOD']: http_method,
             constants.ESTags['ES_PARAMS']: es_params,
             constants.DBTags['DB_TYPE']: 'elasticsearch',
             constants.SpanTags['OPERATION_TYPE']: http_method,
             constants.SpanTags['TOPOLOGY_VERTEX']: True,
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_ELASTICSEARCH_BODY_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_ELASTICSEARCH_BODY_MASK):
             tags[constants.ESTags['ES_BODY']] = es_body
 
         scope.span.tags = tags
```

### Comparing `thundra-3.0.6/thundra/integrations/handler_wrappers/chalice.py` & `thundra-3.0.7/catchpoint/integrations/modules/aiohttp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from __future__ import absolute_import
-from importlib import import_module
-
-from thundra.config.config_provider import ConfigProvider
-from thundra.config import config_names
 import wrapt
 
-_thundra_instance = None
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
 
-def _wrapper(wrapped, _, args, kwargs):
-    wrapped = _thundra_instance(wrapped)
-    return wrapped(*args, **kwargs)
+def _wrapper(wrapped, instance, args, kwargs):
+    try:
+        from catchpoint.integrations.aiohttp.client import CatchpointTraceConfig
+        trace_configs = kwargs.get('trace_configs', [])
+        trace_configs.append(CatchpointTraceConfig())
+        kwargs['trace_configs'] = trace_configs
+    except:
+        pass
+    wrapped(*args, **kwargs)
 
 
-def patch(thundra_instance):
-    if (not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_CHALICE_DISABLE)) and thundra_instance:
-        global _thundra_instance
-        _thundra_instance = thundra_instance
+def patch():
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_DISABLE):
         try:
-            import_module("chalice")
-            wrapt.wrap_function_wrapper("chalice", "Chalice.__call__", _wrapper)
-        except:
+            import aiohttp
+            wrapt.wrap_function_wrapper(
+                'aiohttp',
+                'ClientSession.__init__',
+                _wrapper
+            )
+        except ImportError:
             pass
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/__init__.py` & `thundra-3.0.7/catchpoint/integrations/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.6/thundra/integrations/modules/db.py` & `thundra-3.0.7/catchpoint/integrations/modules/db.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.6/thundra/integrations/modules/django.py` & `thundra-3.0.7/catchpoint/integrations/modules/django.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from __future__ import absolute_import
 import wrapt
 
-from thundra import utils, constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.django import DjangoORMIntegration
+from catchpoint import utils, constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.django import DjangoORMIntegration
 
 try:
     from django.conf import settings
 except ImportError:
     settings = None
 
-THUNDRA_MIDDLEWARE = "thundra.wrappers.django.middleware.ThundraMiddleware"
+CATCHPOINT_MIDDLEWARE = "catchpoint.wrappers.django.middleware.CatchpointMiddleware"
 
 django_orm_integration = DjangoORMIntegration()
 
 
 def _wrapper(wrapped, instance, args, kwargs):
     try:
         if getattr(settings, 'MIDDLEWARE', None):
-            if THUNDRA_MIDDLEWARE in settings.MIDDLEWARE:
+            if CATCHPOINT_MIDDLEWARE in settings.MIDDLEWARE:
                 return wrapped(*args, **kwargs)
 
             if isinstance(settings.MIDDLEWARE, tuple):
-                settings.MIDDLEWARE = (THUNDRA_MIDDLEWARE,) + settings.MIDDLEWARE
+                settings.MIDDLEWARE = (CATCHPOINT_MIDDLEWARE,) + settings.MIDDLEWARE
             elif isinstance(settings.MIDDLEWARE, list):
-                settings.MIDDLEWARE = [THUNDRA_MIDDLEWARE] + settings.MIDDLEWARE
+                settings.MIDDLEWARE = [CATCHPOINT_MIDDLEWARE] + settings.MIDDLEWARE
         elif getattr(settings, 'MIDDLEWARE_CLASSES', None):
-            if THUNDRA_MIDDLEWARE in settings.MIDDLEWARE_CLASSES:
+            if CATCHPOINT_MIDDLEWARE in settings.MIDDLEWARE_CLASSES:
                 return wrapped(*args, **kwargs)
 
             if isinstance(settings.MIDDLEWARE_CLASSES, tuple):
-                settings.MIDDLEWARE = (THUNDRA_MIDDLEWARE,) + settings.MIDDLEWARE_CLASSES
+                settings.MIDDLEWARE = (CATCHPOINT_MIDDLEWARE,) + settings.MIDDLEWARE_CLASSES
             elif isinstance(settings.MIDDLEWARE_CLASSES, list):
-                settings.MIDDLEWARE = [THUNDRA_MIDDLEWARE] + settings.MIDDLEWARE_CLASSES
+                settings.MIDDLEWARE = [CATCHPOINT_MIDDLEWARE] + settings.MIDDLEWARE_CLASSES
 
     except Exception:
         pass
     return wrapped(*args, **kwargs)
 
 
 def db_execute_wrapper(execute, sql, params, many, context):
@@ -54,23 +54,23 @@
 
 def install_db_execute_wrapper(connection, **kwargs):
     if db_execute_wrapper not in connection.execute_wrappers:
         connection.execute_wrappers.insert(0, db_execute_wrapper)
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_DJANGO_DISABLE) and (
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_DJANGO_DISABLE) and (
             not utils.get_env_variable(constants.AWS_LAMBDA_FUNCTION_NAME)):
         wrapt.wrap_function_wrapper(
             'django.core.handlers.base',
             'BaseHandler.load_middleware',
             _wrapper
         )
 
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_DJANGO_ORM_DISABLE):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_DJANGO_ORM_DISABLE):
         try:
             from django import VERSION
             from django.db import connections
             from django.db.backends.signals import connection_created
 
             if VERSION >= (2, 0):
                 for connection in connections.all():
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/elasticsearch.py` & `thundra-3.0.7/catchpoint/integrations/modules/elasticsearch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import wrapt
 
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.elasticsearch import ElasticsearchIntegration
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.elasticsearch import ElasticsearchIntegration
 
 es_integration = ElasticsearchIntegration()
 
 
 def _wrapper(wrapped, instance, args, kwargs):
     return es_integration.run_and_trace(
         wrapped,
         instance,
         args,
         kwargs
     )
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_ES_DISABLE):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_ES_DISABLE):
         wrapt.wrap_function_wrapper(
             'elasticsearch',
             'transport.Transport.perform_request',
             _wrapper
         )
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/fastapi.py` & `thundra-3.0.7/catchpoint/integrations/modules/fastapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import wrapt
 
-from thundra import utils, constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
+from catchpoint import utils, constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
 def _wrapper(wrapped, instance, args, kwargs):
     """Set middleware to trace Fast api. Fastapi has been built on starlett and pydantic frameworks.
     Request and response flow has been handled by starlette that is a lightweight ASGI framework. Fastapi 
     has an class called APIRouter that extends starlett Router class which is used to handle connections by starlette.
     The middleware should be an ASGI Middleware. Thus, the __call__(scope, receive, send) function should be implemented. 
     By default, starlette add two middleware except user defined middlewares which are ServerErrorMiddleware and ExceptionMiddleware. 
@@ -16,23 +16,23 @@
     Args:
         wrapped (module): Wrapped module
         instance (function): Module enter point
         args (list): Wrapped function list of arguments
         kwargs (dict): Wrapped function key:value arguments
     """
     from fastapi.middleware import Middleware
-    from thundra.wrappers.fastapi.middleware import ThundraMiddleware
-    from thundra.wrappers.fastapi.fastapi_wrapper import FastapiWrapper
+    from catchpoint.wrappers.fastapi.middleware import CatchpointMiddleware
+    from catchpoint.wrappers.fastapi.fastapi_wrapper import FastapiWrapper
     middlewares = kwargs.pop("middleware", [])
-    middlewares.insert(0, Middleware(ThundraMiddleware, wrapper=FastapiWrapper.get_instance()))
+    middlewares.insert(0, Middleware(CatchpointMiddleware, wrapper=FastapiWrapper.get_instance()))
     kwargs.update({"middleware": middlewares})
     wrapped(*args, **kwargs)
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_FASTAPI_DISABLE) and \
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_FASTAPI_DISABLE) and \
         not utils.get_env_variable(constants.AWS_LAMBDA_FUNCTION_NAME):
         wrapt.wrap_function_wrapper(
             "fastapi.applications",
             "FastAPI.__init__",
             _wrapper
         )
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/flask.py` & `thundra-3.0.7/catchpoint/integrations/modules/requests.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import wrapt
 
-from thundra import utils, constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.wrappers.flask.middleware import ThundraMiddleware
+from catchpoint import utils
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.requests import RequestsIntegration
+
+request_integration = RequestsIntegration()
 
 
 def _wrapper(wrapped, instance, args, kwargs):
-    response = wrapped(*args, **kwargs)
-    try:
-        thundra_middleware = ThundraMiddleware()
-        thundra_middleware.set_app(instance)
-    except:
-        pass
-    return response
+    prepared_request = args[0]
+
+    if utils.is_excluded_url(prepared_request.url):
+        return wrapped(*args, **kwargs)
+
+    return request_integration.run_and_trace(
+        wrapped,
+        instance,
+        args,
+        kwargs,
+    )
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_FLASK_DISABLE) and (
-            not utils.get_env_variable(constants.AWS_LAMBDA_FUNCTION_NAME)):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_DISABLE):
         wrapt.wrap_function_wrapper(
-            'flask',
-            'Flask.__init__',
+            'requests',
+            'Session.send',
             _wrapper
         )
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/mysql.py` & `thundra-3.0.7/catchpoint/integrations/modules/mysql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import wrapt
 
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.mysql import MysqlIntegration
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.mysql import MysqlIntegration
 
 mysql_integration = MysqlIntegration()
 
 
 class MysqlCursorWrapper(wrapt.ObjectProxy):
 
     def __init__(self, cursor, connection_wrapper):
@@ -43,12 +43,12 @@
 
 def _wrapper(wrapped, instance, args, kwargs):
     connection = wrapped(*args, **kwargs)
     return MysqlConnectionWrapper(connection)
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_DISABLE):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_DISABLE):
         wrapt.wrap_function_wrapper(
             'mysql.connector',
             'connect',
             _wrapper)
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/psycopg2.py` & `thundra-3.0.7/catchpoint/integrations/modules/psycopg2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 
 import wrapt
 
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.postgre import PostgreIntegration
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.postgre import PostgreIntegration
 
 postgre_integration = PostgreIntegration()
 
 
 class PostgreCursorWrapper(wrapt.ObjectProxy):
 
     def __init__(self, cursor, connection_wrapper):
@@ -73,13 +73,13 @@
         pass
 
     for ext in _extensions:
         wrapt.wrap_function_wrapper(ext[0], ext[1], ext[2])
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_DISABLE):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_DISABLE):
         patch_extensions()
         wrapt.wrap_function_wrapper(
             'psycopg2',
             'connect',
             _wrapper)
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/pymongo.py` & `thundra-3.0.7/catchpoint/integrations/modules/pymongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import wrapt
 
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.mongodb import CommandTracer
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.mongodb import CommandTracer
 
 
 def _wrapper(wrapped, instance, args, kwargs):
     event_listeners = list(kwargs.pop('event_listeners', []))
     event_listeners.insert(0, CommandTracer())
     kwargs['event_listeners'] = event_listeners
     wrapped(*args, **kwargs)
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_MONGO_DISABLE):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_MONGO_DISABLE):
         try:
             import pymongo.monitoring
             from bson.json_util import dumps
             wrapt.wrap_function_wrapper(
                 'pymongo',
                 'MongoClient.__init__',
                 _wrapper
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/requests.py` & `thundra-3.0.7/catchpoint/integrations/modules/redis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import wrapt
 
-from thundra import utils
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.requests import RequestsIntegration
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.redis import RedisIntegration
 
-request_integration = RequestsIntegration()
+redis_integration = RedisIntegration()
 
 
 def _wrapper(wrapped, instance, args, kwargs):
-    prepared_request = args[0]
-
-    if utils.is_excluded_url(prepared_request.url):
-        return wrapped(*args, **kwargs)
-
-    return request_integration.run_and_trace(
+    return redis_integration.run_and_trace(
         wrapped,
         instance,
         args,
-        kwargs,
+        kwargs
     )
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_DISABLE):
-        wrapt.wrap_function_wrapper(
-            'requests',
-            'Session.send',
-            _wrapper
-        )
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_REDIS_DISABLE):
+        for method in map(str.lower, constants.RedisCommandTypes.keys()):
+            try:
+                wrapt.wrap_function_wrapper(
+                    'redis.client',
+                    'Redis.' + method,
+                    _wrapper
+                )
+            except:
+                pass
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/sqlite3.py` & `thundra-3.0.7/catchpoint/integrations/modules/sqlite3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import wrapt
 
-from thundra.integrations.sqlite3 import SQLiteIntegration
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
+from catchpoint.integrations.sqlite3 import SQLiteIntegration
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
 sqlite_integration = SQLiteIntegration()
 
 
 class SqliteCursorWrapper(wrapt.ObjectProxy):
 
     def __init__(self, cursor, connection_wrapper):
@@ -47,15 +47,15 @@
 def _wrapper(wrapped, instance, args, kwargs):
     db_name = args[0] if args and len(args) > 0 else None
     connection = wrapped(*args, **kwargs)
     return SqliteConnectionWrapper(connection, db_name)
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_DISABLE):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_DISABLE):
         wrapt.wrap_function_wrapper(
             'sqlite3',
             'connect',
             _wrapper)
         wrapt.wrap_function_wrapper(
             'sqlite3.dbapi2',
             'connect',
```

### Comparing `thundra-3.0.6/thundra/integrations/modules/tornado.py` & `thundra-3.0.7/catchpoint/integrations/modules/tornado.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import wrapt
 
-from thundra import utils, constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.wrappers.tornado.middleware import ThundraMiddleware
+from catchpoint import utils, constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.wrappers.tornado.middleware import CatchpointMiddleware
 
 
 def _init_wrapper(_wrapped, _application, args, kwargs):
     _wrapped(*args, **kwargs)
 
-    middleware = _application.settings.get('_thundra_middleware')
+    middleware = _application.settings.get('_catchpoint_middleware')
     if middleware is None:
-        _application.settings['_thundra_middleware'] = ThundraMiddleware()
+        _application.settings['_catchpoint_middleware'] = CatchpointMiddleware()
 
 
 async def _execute_wrapper(_wrapped, _handler, args, kwargs):
-    middleware = _handler.settings.get('_thundra_middleware')
+    middleware = _handler.settings.get('_catchpoint_middleware')
     middleware.execute(_handler)
     return await _wrapped(*args, **kwargs)
 
 
 def _on_finish_wrapper(_wrapped, _handler, args, kwargs):
-    middleware = _handler.settings.get('_thundra_middleware')
+    middleware = _handler.settings.get('_catchpoint_middleware')
     middleware.finish(_handler)
     return _wrapped(*args, **kwargs)
 
 
 def _log_exception_wrapper(_wrapped, _handler, args, kwargs):
     value = args[1] if len(args) == 3 else None
     if value is None:
         return _wrapped(*args, **kwargs)
 
-    middleware = _handler.settings.get('_thundra_middleware')
+    middleware = _handler.settings.get('_catchpoint_middleware')
     try:
         from tornado.web import HTTPError
         if not isinstance(value, HTTPError) or 500 <= value.status_code <= 599:
             middleware.finish(_handler, error=value)
     except ImportError:
         error = type('', (object,), {"status_code": 500})()
         middleware.finish(_handler, error=error)
 
     return _wrapped(*args, **kwargs)
 
 
 def patch():
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_TORNADO_DISABLE) and (
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_TORNADO_DISABLE) and (
            not utils.get_env_variable(constants.AWS_LAMBDA_FUNCTION_NAME)):
 
         wrapt.wrap_function_wrapper(
             'tornado.web',
             'Application.__init__',
             _init_wrapper
         )
```

### Comparing `thundra-3.0.6/thundra/integrations/mongodb.py` & `thundra-3.0.7/catchpoint/integrations/mongodb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import traceback
 import time
 import logging
-from thundra import constants
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.config.config_provider import ConfigProvider
-from thundra.config import config_names
+from catchpoint import constants
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
 
 
 try:
     from pymongo.monitoring import CommandListener
     from bson.json_util import dumps
 except ImportError:
     CommandListener = object
@@ -17,15 +17,15 @@
 logger = logging.getLogger(__name__)
 
 
 class CommandTracer(CommandListener):
     _scopes = {}
 
     def started(self, event):
-        tracer = ThundraTracer.get_instance()
+        tracer = CatchpointTracer.get_instance()
         if not tracer.get_active_span():
             return
 
         scope = tracer.start_active_span(operation_name=event.database_name, finish_on_close=False)
 
         self._scopes[event.request_id] = scope
 
@@ -54,15 +54,15 @@
                 constants.DBTags['DB_PORT']: port,
                 constants.SpanTags['DB_INSTANCE']: event.database_name,
                 constants.MongoDBTags['MONGODB_COMMAND_NAME']: command_name.upper(),
                 constants.MongoDBTags['MONGODB_COLLECTION']: collection_name,
                 constants.SpanTags['TOPOLOGY_VERTEX']: True,
             }
 
-            if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_MONGODB_COMMAND_MASK):
+            if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_MONGODB_COMMAND_MASK):
                 try:
                     tags[constants.MongoDBTags['MONGODB_COMMAND']] = dumps(event.command)[
                                                                    :constants.DEFAULT_MONGO_COMMAND_SIZE_LIMIT]
                 except Exception as e:
                     tags[constants.MongoDBTags['MONGODB_COMMAND']] = ''
 
             scope.span.tags = tags
```

### Comparing `thundra-3.0.6/thundra/integrations/mysql.py` & `thundra-3.0.7/catchpoint/integrations/mysql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.base_integration import BaseIntegration
-from thundra.integrations.rdb_base import RdbBaseIntegration
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.base_integration import BaseIntegration
+from catchpoint.integrations.rdb_base import RdbBaseIntegration
 
 
 class MysqlIntegration(BaseIntegration, RdbBaseIntegration):
     CLASS_TYPE = 'mysql'
 
     def __init__(self):
         pass
@@ -33,11 +33,11 @@
             constants.SpanTags['DB_INSTANCE']: connection._database,
             constants.SpanTags['DB_HOST']: connection._host,
             constants.SpanTags['DB_TYPE']: "mysql",
             constants.SpanTags['DB_STATEMENT_TYPE']: operation.upper(),
             constants.SpanTags['TOPOLOGY_VERTEX']: True,
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
             tags[constants.DBTags['DB_STATEMENT']] = query
 
         span.tags = tags
```

### Comparing `thundra-3.0.6/thundra/integrations/postgre.py` & `thundra-3.0.7/catchpoint/integrations/postgre.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from thundra import constants
-from thundra.integrations.rdb_base import RdbBaseIntegration
-from thundra.integrations.base_integration import BaseIntegration
-from thundra.config.config_provider import ConfigProvider
-from thundra.config import config_names
+from catchpoint import constants
+from catchpoint.integrations.rdb_base import RdbBaseIntegration
+from catchpoint.integrations.base_integration import BaseIntegration
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
 
 try:
     from psycopg2.extensions import parse_dsn
 except ImportError:
     def parse_dsn(dsn):
         return dict(
             attribute.split("=") for attribute in dsn.split()
@@ -45,12 +45,12 @@
             constants.SpanTags['DB_HOST']: dsn.get('host', ''),
             constants.SpanTags['DB_TYPE']: "postgresql",
             constants.SpanTags['DB_STATEMENT_TYPE']: operation.upper(),
             constants.SpanTags['TRIGGER_CLASS_NAME']: "API",
             constants.SpanTags['TOPOLOGY_VERTEX']: True
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
             tags[constants.DBTags['DB_STATEMENT']] = query
 
         span.tags = tags
```

### Comparing `thundra-3.0.6/thundra/integrations/redis.py` & `thundra-3.0.7/catchpoint/integrations/redis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.base_integration import BaseIntegration
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.base_integration import BaseIntegration
 
 
 class RedisIntegration(BaseIntegration):
     CLASS_TYPE = 'redis'
 
     def __init__(self):
         pass
@@ -32,12 +32,12 @@
             constants.DBTags['DB_TYPE']: 'redis',
             constants.RedisTags['REDIS_HOST']: host,
             constants.RedisTags['REDIS_PORT']: port,
             constants.RedisTags['REDIS_COMMAND_TYPE']: command_type,
             constants.SpanTags['TOPOLOGY_VERTEX']: True,
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_REDIS_COMMAND_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_REDIS_COMMAND_MASK):
             tags[constants.DBTags['DB_STATEMENT']] = command
             tags[constants.RedisTags['REDIS_COMMAND']] = command
 
         scope.span.tags = tags
```

### Comparing `thundra-3.0.6/thundra/integrations/requests.py` & `thundra-3.0.7/catchpoint/integrations/requests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from opentracing import Format
 
-import thundra.constants as constants
-from thundra import utils
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.base_integration import BaseIntegration
+import catchpoint.constants as constants
+from catchpoint import utils
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.base_integration import BaseIntegration
 
 
 class RequestsIntegration(BaseIntegration):
     CLASS_TYPE = 'http'
 
     def __init__(self):
         pass
 
     def get_operation_name(self, wrapped, instance, args, kwargs):
         prepared_request = args[0]
         url_dict = utils.parse_http_url(prepared_request.url,
-                                        ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_URL_DEPTH))
+                                        ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_URL_DEPTH))
         return url_dict.get('operation_name')
 
     def before_call(self, scope, wrapped, instance, args, kwargs, response, exception):
         prepared_request = args[0]
         method = prepared_request.method
 
         url_dict = utils.parse_http_url(prepared_request.url,
-                                        ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_URL_DEPTH))
+                                        ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_URL_DEPTH))
         span = scope.span
 
         span.domain_name = constants.DomainNames['API']
         span.class_name = constants.ClassNames['HTTP']
 
         tags = {
             constants.SpanTags['OPERATION_TYPE']: method,
@@ -39,20 +39,20 @@
             constants.HttpTags['HTTP_HOST']: url_dict.get('host'),
             constants.HttpTags['QUERY_PARAMS']: url_dict.get('query'),
             constants.SpanTags['TOPOLOGY_VERTEX']: True,
         }
 
         span.tags = tags
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_BODY_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_BODY_MASK):
             body = prepared_request.body if prepared_request.body else ""
             scope.span.set_tag(constants.HttpTags["BODY"], body)
 
         try:
-            tracer = ThundraTracer.get_instance()
+            tracer = CatchpointTracer.get_instance()
             tracer.inject(span.context, Format.HTTP_HEADERS, prepared_request.headers)
             prepared_request.headers[constants.TRIGGER_RESOURCE_NAME_KEY] = url_dict.get('operation_name')
 
             span.set_tag(constants.SpanTags['TRACE_LINKS'], [span.span_id])
         except Exception as e:
             pass
 
@@ -66,15 +66,15 @@
 
             if response.headers and response.headers.get(constants.TRIGGER_RESOURCE_NAME_KEY):
                 resource_name = response.headers.get(constants.TRIGGER_RESOURCE_NAME_KEY)
                 scope.span.operation_name = resource_name
 
             if (response.status_code and \
                     ConfigProvider.get(
-                        config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_ERROR_STATUS_CODE_MIN) <= response.status_code):
+                        config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_ERROR_STATUS_CODE_MIN) <= response.status_code):
                 scope.span.set_tag('error.kind', "HttpError")
                 scope.span.set_tag('error', True)
                 scope.span.set_tag('error.message', response.reason)
 
     def set_response(self, response, span):
         status_code = response.status_code
         span.set_tag(constants.HttpTags['HTTP_STATUS'], status_code)
```

### Comparing `thundra-3.0.6/thundra/integrations/sqlalchemy.py` & `thundra-3.0.7/catchpoint/integrations/sqlalchemy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import time
 import traceback
 
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.rdb_base import RdbBaseIntegration
-from thundra.opentracing.tracer import ThundraTracer
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.rdb_base import RdbBaseIntegration
+from catchpoint.opentracing.tracer import CatchpointTracer
 
 try:
     from sqlalchemy.event import listen
     from sqlalchemy.engine.interfaces import ExecutionContext
 except:
     pass
 
@@ -73,26 +73,26 @@
             constants.SpanTags['DB_INSTANCE']: db_config.get('database', ''),
             constants.SpanTags['DB_HOST']: db_config.get('host', ''),
             constants.SpanTags['DB_TYPE']: db_config.get('db_type', ''),
             constants.SpanTags['DB_STATEMENT_TYPE']: operation.upper(),
             constants.SpanTags['TOPOLOGY_VERTEX']: True
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
             tags[constants.DBTags['DB_STATEMENT']] = statement
 
         scope.span.tags = tags
 
     def after_call(self, scope, conn, statement):
         pass
 
     def _before_cursor_execute(self, conn, cursor, statement, parameters, context, executemany):
         if not context:
             return
-        tracer = ThundraTracer.get_instance()
+        tracer = CatchpointTracer.get_instance()
 
         if not tracer.get_active_span():
             return
         scope = tracer.start_active_span(operation_name=self.get_operation_name(conn), finish_on_close=False)
 
         context.scope = scope
```

### Comparing `thundra-3.0.6/thundra/integrations/sqlite3.py` & `thundra-3.0.7/catchpoint/integrations/sqlite3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.integrations.base_integration import BaseIntegration
-from thundra.integrations.rdb_base import RdbBaseIntegration
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.integrations.base_integration import BaseIntegration
+from catchpoint.integrations.rdb_base import RdbBaseIntegration
 
 
 class SQLiteIntegration(BaseIntegration, RdbBaseIntegration):
     CLASS_TYPE = 'sqlite'
 
     def __init__(self):
         super(SQLiteIntegration, self)
@@ -33,11 +33,11 @@
             constants.SpanTags['DB_INSTANCE']: connection.db_name,
             constants.SpanTags['DB_HOST']: connection.host,
             constants.SpanTags['DB_TYPE']: self.CLASS_TYPE,
             constants.SpanTags['DB_STATEMENT_TYPE']: operation.upper(),
             constants.SpanTags['TOPOLOGY_VERTEX']: True,
         }
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_RDB_STATEMENT_MASK):
             tags[constants.DBTags['DB_STATEMENT']] = query
 
         span.tags = tags
```

### Comparing `thundra-3.0.6/thundra/listeners/composite_span_filter.py` & `thundra-3.0.7/catchpoint/listeners/composite_span_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thundra.listeners.thundra_span_filterer import SpanFilter
+from catchpoint.listeners.catchpoint_span_filterer import SpanFilter
 
 
 class CompositeSpanFilter(SpanFilter):
     
     def __init__(self, is_all=False, filters=None):
         if filters is None:
             filters = []
```

### Comparing `thundra-3.0.6/thundra/listeners/error_injector_span_listener.py` & `thundra-3.0.7/catchpoint/listeners/error_injector_span_listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import absolute_import
 import logging
 from threading import Lock
 from importlib import import_module
-from thundra import constants
-from thundra.listeners.thundra_span_listener import ThundraSpanListener
+from catchpoint import constants
+from catchpoint.listeners.catchpoint_span_listener import CatchpointSpanListener
 
 logger = logging.getLogger(__name__)
-default_error_message = "Error injected by Thundra!"
+default_error_message = "Error injected by Catchpoint!"
 default_error_type = Exception
 
 try:
     import builtins
 except:
     import __builtin__ as builtins
 
-class ErrorInjectorSpanListener(ThundraSpanListener):
+class ErrorInjectorSpanListener(CatchpointSpanListener):
     def __init__(self, error_message=default_error_message,
                  error_type=default_error_type, inject_on_finish=False,
                  inject_count_freq=1, add_info_tags=True):
 
         self._counter = 0
         self._lock = Lock()
 
@@ -60,15 +60,15 @@
             info_dict = {
                 'type': 'error_injector_span_listener',
                 'error_type': str(self.error_type),
                 'error_message': self.error_message,
                 'inject_on_finish': self.inject_on_finish,
                 'inject_count_freq': self.inject_count_freq,
             }
-            span.set_tag(constants.THUNDRA_LAMBDA_SPAN_LISTENER_INFO_TAG, info_dict)
+            span.set_tag(constants.CATCHPOINT_LAMBDA_SPAN_LISTENER_INFO_TAG, info_dict)
         except Exception as e:
             logger.error("error while adding ErrorInjectorSpanListener info tags: %s", e)
 
     @staticmethod
     def from_config(config):
         kwargs = {}
         error_message = config.get('errorMessage')
```

### Comparing `thundra-3.0.6/thundra/listeners/filtering_span_listener.py` & `thundra-3.0.7/catchpoint/listeners/filtering_span_listener.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
-from thundra.listeners import ThundraSpanListener
-from thundra.listeners.thundra_span_filterer import SimpleSpanFilter, SpanFilterer
-from thundra.listeners.thundra_span_filterer import StandardSpanFilterer
-from thundra.listeners.composite_span_filter import CompositeSpanFilter
+from catchpoint.listeners import CatchpointSpanListener
+from catchpoint.listeners.catchpoint_span_filterer import SimpleSpanFilter, SpanFilterer
+from catchpoint.listeners.catchpoint_span_filterer import StandardSpanFilterer
+from catchpoint.listeners.composite_span_filter import CompositeSpanFilter
 
 logger = logging.getLogger(__name__)
 
-class FilteringSpanListener(ThundraSpanListener):
+class FilteringSpanListener(CatchpointSpanListener):
     
     def __init__(self, listener=None, filterer=None):
         self.listener = listener
         self.filterer = filterer
 
     def on_span_started(self, span):
         if self.listener is None:
@@ -80,15 +80,15 @@
         span_filters = FilteringSpanListener._get_span_filters_from_config(config)
         return filterer_class(span_filters=span_filters, all_mandatory=is_all)
 
     @staticmethod
     def _get_span_listener_from_config(config):
         SPAN_LISTENERS = {
             sl_class.__name__: sl_class 
-            for sl_class in ThundraSpanListener.__subclasses__()
+            for sl_class in CatchpointSpanListener.__subclasses__()
         }
         listener_config = None
         if 'listener' not in config:
             listener_class = None
         else:
             listener = config.get('listener')
             listener_type = listener.get('type')
```

### Comparing `thundra-3.0.6/thundra/listeners/latency_injector_span_listener.py` & `thundra-3.0.7/catchpoint/listeners/latency_injector_span_listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import random
 import time
 
-from thundra import constants
-from thundra.listeners.thundra_span_listener import ThundraSpanListener
+from catchpoint import constants
+from catchpoint.listeners.catchpoint_span_listener import CatchpointSpanListener
 
 logger = logging.getLogger(__name__)
 
 
-class LatencyInjectorSpanListener(ThundraSpanListener):
+class LatencyInjectorSpanListener(CatchpointSpanListener):
     available_distributions = ["normal", "uniform"]
 
     def __init__(self, delay=0, variation=0,
                  sigma=0, distribution="uniform",
                  add_info_tags=True):
         self.delay = max(0, delay)
         self.sigma = max(0, sigma)
@@ -51,15 +51,15 @@
                 'type': 'latency_injector_span_listener',
                 'injected_delay': injected_delay,
                 'delay': self.delay,
                 'variation': self.variation,
                 'sigma': self.sigma,
                 'distribution': self.distribution,
             }
-            span.set_tag(constants.THUNDRA_LAMBDA_SPAN_LISTENER_INFO_TAG, info_dict)
+            span.set_tag(constants.CATCHPOINT_LAMBDA_SPAN_LISTENER_INFO_TAG, info_dict)
         except Exception as e:
             logger.error("error while adding LatencyInjectorSpanListener info tags: %s", e)
 
     @staticmethod
     def from_config(config):
         kwargs = {}
         delay = config.get('delay')
```

### Comparing `thundra-3.0.6/thundra/listeners/security_aware_span_listener.py` & `thundra-3.0.7/catchpoint/listeners/security_aware_span_listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import absolute_import
 
-from thundra import constants
-from thundra.listeners.thundra_span_listener import ThundraSpanListener
-from thundra.plugins.invocation import invocation_support
+from catchpoint import constants
+from catchpoint.listeners.catchpoint_span_listener import CatchpointSpanListener
+from catchpoint.plugins.invocation import invocation_support
 
 try:
     import builtins
 except:
     import __builtin__ as builtins
 
 
-class SecurityAwareSpanListener(ThundraSpanListener):
+class SecurityAwareSpanListener(CatchpointSpanListener):
     def __init__(self, block=False, whitelist=None, blacklist=None):
         self.block = block
         self.whitelist = whitelist
         self.blacklist = blacklist
 
     def on_span_started(self, span):
         if not self.is_external_operation(span):
```

### Comparing `thundra-3.0.6/thundra/listeners/tag_injector_span_listener.py` & `thundra-3.0.7/catchpoint/listeners/tag_injector_span_listener.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import absolute_import
 
 import logging
 
-from thundra.listeners.thundra_span_listener import ThundraSpanListener
+from catchpoint.listeners.catchpoint_span_listener import CatchpointSpanListener
 
 logger = logging.getLogger(__name__)
 
 try:
     import builtins
 except:
     import __builtin__ as builtins
 
 
-class TagInjectorSpanListener(ThundraSpanListener):
+class TagInjectorSpanListener(CatchpointSpanListener):
     def __init__(self, inject_on_finish=False, tags_to_inject=None):
         self.inject_on_finish = inject_on_finish
         self.tags_to_inject = tags_to_inject
 
     def on_span_started(self, span):
         if not self.inject_on_finish:
             self._inject_tags(span)
```

### Comparing `thundra-3.0.6/thundra/listeners/thundra_span_filterer.py` & `thundra-3.0.7/catchpoint/listeners/catchpoint_span_filterer.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.6/thundra/listeners/thundra_span_listener.py` & `thundra-3.0.7/catchpoint/listeners/catchpoint_span_listener.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 
 ABC = abc.ABCMeta('ABC', (object,), {})
 
 
-class ThundraSpanListener(ABC):
+class CatchpointSpanListener(ABC):
     @abc.abstractmethod
     def on_span_started(self, operation_name):
         raise Exception("should be implemented")
 
     @abc.abstractmethod
     def on_span_finished(self, span):
         raise Exception("should be implemented")
```

### Comparing `thundra-3.0.6/thundra/opentracing/propagation/http.py` & `thundra-3.0.7/catchpoint/opentracing/propagation/http.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from thundra import constants
+from catchpoint import constants
 
-from thundra.opentracing.propagation.text import TextMapPropagator
-from thundra.opentracing.span_context import ThundraSpanContext
+from catchpoint.opentracing.propagation.text import TextMapPropagator
+from catchpoint.opentracing.span_context import CatchpointSpanContext
 
 
 class HTTPPropagator(TextMapPropagator):
 
     @staticmethod
     def extract_value_from_header(header_name, headers):
         for header, value in headers.items():
             if header.lower() == header_name.lower():
                 return value
 
     def extract(self, carrier):
         try:
-            trace_id = HTTPPropagator.extract_value_from_header(constants.THUNDRA_TRACE_ID_KEY, carrier)
-            span_id = HTTPPropagator.extract_value_from_header(constants.THUNDRA_SPAN_ID_KEY, carrier)
-            transaction_id = HTTPPropagator.extract_value_from_header(constants.THUNDRA_TRANSACTION_ID_KEY, carrier)
+            trace_id = HTTPPropagator.extract_value_from_header(constants.CATCHPOINT_TRACE_ID_KEY, carrier)
+            span_id = HTTPPropagator.extract_value_from_header(constants.CATCHPOINT_SPAN_ID_KEY, carrier)
+            transaction_id = HTTPPropagator.extract_value_from_header(constants.CATCHPOINT_TRANSACTION_ID_KEY, carrier)
         except:
             return None
 
         if not (trace_id and span_id and transaction_id):
             return None
 
         # Extract baggage items
         baggage = {}
         for key in carrier:
             if isinstance(key, str):
-                if key.startswith(constants.THUNDRA_BAGGAGE_PREFIX):
-                    baggage[key[len(constants.THUNDRA_BAGGAGE_PREFIX):]] = carrier[key]
+                if key.startswith(constants.CATCHPOINT_BAGGAGE_PREFIX):
+                    baggage[key[len(constants.CATCHPOINT_BAGGAGE_PREFIX):]] = carrier[key]
             elif isinstance(key, tuple):
-                if key[0].startswith(constants.THUNDRA_BAGGAGE_PREFIX):
-                    baggage[key[0][len(constants.THUNDRA_BAGGAGE_PREFIX):]] = key[1]
+                if key[0].startswith(constants.CATCHPOINT_BAGGAGE_PREFIX):
+                    baggage[key[0][len(constants.CATCHPOINT_BAGGAGE_PREFIX):]] = key[1]
 
-        span_context = ThundraSpanContext(trace_id=trace_id, span_id=span_id, transaction_id=transaction_id,
-                                          baggage=baggage)
+        span_context = CatchpointSpanContext(trace_id=trace_id, span_id=span_id, transaction_id=transaction_id,
+                                             baggage=baggage)
 
         return span_context
```

### Comparing `thundra-3.0.6/thundra/opentracing/propagation/text.py` & `thundra-3.0.7/catchpoint/opentracing/propagation/text.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from opentracing import InvalidCarrierException
 
-from thundra import constants
-from thundra.opentracing.propagation.propagator import Propagator
-from thundra.opentracing.span_context import ThundraSpanContext
+from catchpoint import constants
+from catchpoint.opentracing.propagation.propagator import Propagator
+from catchpoint.opentracing.span_context import CatchpointSpanContext
 
 
 class TextMapPropagator(Propagator):
 
     def inject(self, span_context, carrier):
         if span_context.trace_id:
-            carrier[constants.THUNDRA_TRACE_ID_KEY] = span_context.trace_id
+            carrier[constants.CATCHPOINT_TRACE_ID_KEY] = span_context.trace_id
 
         if span_context.span_id:
-            carrier[constants.THUNDRA_SPAN_ID_KEY] = span_context.span_id
+            carrier[constants.CATCHPOINT_SPAN_ID_KEY] = span_context.span_id
 
         if span_context.transaction_id:
-            carrier[constants.THUNDRA_TRANSACTION_ID_KEY] = span_context.transaction_id
+            carrier[constants.CATCHPOINT_TRANSACTION_ID_KEY] = span_context.transaction_id
 
         # Inject baggage items
         if span_context.baggage is not None:
             for key in span_context.baggage:
-                carrier[constants.THUNDRA_BAGGAGE_PREFIX + key] = span_context.baggage[key]
+                carrier[constants.CATCHPOINT_BAGGAGE_PREFIX + key] = span_context.baggage[key]
 
     def extract(self, carrier):
         try:
-            trace_id = carrier[constants.THUNDRA_TRACE_ID_KEY]
-            span_id = carrier[constants.THUNDRA_SPAN_ID_KEY]
-            transaction_id = carrier[constants.THUNDRA_TRANSACTION_ID_KEY]
+            trace_id = carrier[constants.CATCHPOINT_TRACE_ID_KEY]
+            span_id = carrier[constants.CATCHPOINT_SPAN_ID_KEY]
+            transaction_id = carrier[constants.CATCHPOINT_TRANSACTION_ID_KEY]
         except:
             return None
 
         if not (trace_id and span_id and transaction_id):
             return None
 
         # Extract baggage items
         baggage = {}
         for key in carrier:
-            if key.startswith(constants.THUNDRA_BAGGAGE_PREFIX):
-                baggage[key[len(constants.THUNDRA_BAGGAGE_PREFIX):]] = carrier[key]
+            if key.startswith(constants.CATCHPOINT_BAGGAGE_PREFIX):
+                baggage[key[len(constants.CATCHPOINT_BAGGAGE_PREFIX):]] = carrier[key]
 
-        span_context = ThundraSpanContext(trace_id=trace_id, span_id=span_id, transaction_id=transaction_id,
-                                          baggage=baggage)
+        span_context = CatchpointSpanContext(trace_id=trace_id, span_id=span_id, transaction_id=transaction_id,
+                                             baggage=baggage)
 
         return span_context
```

### Comparing `thundra-3.0.6/thundra/opentracing/span.py` & `thundra-3.0.7/catchpoint/opentracing/span.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from threading import Lock
 
 import opentracing
 
 logger = logging.getLogger(__name__)
 
 
-class ThundraSpan(opentracing.Span):
+class CatchpointSpan(opentracing.Span):
 
     def __init__(self,
                  tracer,
                  operation_name=None,
                  class_name=None,
                  domain_name=None,
                  context=None,
                  tags=None,
                  start_time=None,
                  span_order=-1,
                  execution_context=None):
-        super(ThundraSpan, self).__init__(tracer, context)
+        super(CatchpointSpan, self).__init__(tracer, context)
         self._tracer = tracer
         self._context = context
         self._lock = Lock()
         self.operation_name = operation_name if operation_name is not None else ""
         self.class_name = class_name if class_name is not None else ""
         self.domain_name = domain_name if domain_name is not None else ""
         self.start_time = start_time or int(time.time() * 1000)
@@ -56,22 +56,22 @@
     @property
     def span_id(self):
         return self._context.span_id
 
     def set_operation_name(self, operation_name):
         with self._lock:
             self.operation_name = operation_name
-        return super(ThundraSpan, self).set_operation_name(operation_name)
+        return super(CatchpointSpan, self).set_operation_name(operation_name)
 
     def set_tag(self, key, value):
         with self._lock:
             if self.tags is None:
                 self.tags = {}
             self.tags[key] = value
-        return super(ThundraSpan, self).set_tag(key, value)
+        return super(CatchpointSpan, self).set_tag(key, value)
 
     def get_tag(self, key):
         if self.tags is not None:
             return self.tags.get(key)
         return None
 
     def finish(self, f_time=None):
@@ -104,15 +104,15 @@
                     raise e
 
     def log_kv(self, key_values, timestamp=None):
         with self._lock:
             log = key_values
             log['timestamp'] = timestamp
             self.logs.append(log)
-        return super(ThundraSpan, self).log_kv(key_values, timestamp)
+        return super(CatchpointSpan, self).log_kv(key_values, timestamp)
 
     def set_baggage_item(self, key, value):
         new_context = self.context.context_with_baggage_item(key, value)
         with self._lock:
             self._context = new_context
         return self
```

### Comparing `thundra-3.0.6/thundra/opentracing/span_context.py` & `thundra-3.0.7/catchpoint/opentracing/span_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 
 import opentracing
 
 
-class ThundraSpanContext(opentracing.SpanContext):
+class CatchpointSpanContext(opentracing.SpanContext):
 
     def __init__(self,
                  trace_id=None,
                  transaction_id=None,
                  span_id=None,
                  parent_span_id=None,
                  baggage=None):
@@ -40,12 +40,12 @@
     @property
     def baggage(self):
         return self._baggage
 
     def context_with_baggage_item(self, key, value):
         new_baggage_item = copy.copy(self.baggage)
         new_baggage_item[key] = value
-        return ThundraSpanContext(trace_id=self.trace_id,
-                                  transaction_id=self.transaction_id,
-                                  span_id=self.span_id,
-                                  parent_span_id=self.parent_span_id,
-                                  baggage=new_baggage_item)
+        return CatchpointSpanContext(trace_id=self.trace_id,
+                                     transaction_id=self.transaction_id,
+                                     span_id=self.span_id,
+                                     parent_span_id=self.parent_span_id,
+                                     baggage=new_baggage_item)
```

### Comparing `thundra-3.0.6/thundra/opentracing/tracer.py` & `thundra-3.0.7/catchpoint/opentracing/tracer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import uuid
 from threading import Lock
 
 import opentracing
 from opentracing import Format
 
-from thundra import constants
-from thundra.context.execution_context_manager import ExecutionContextManager
-from thundra.opentracing.propagation.http import HTTPPropagator
-from thundra.opentracing.propagation.text import TextMapPropagator
-from thundra.opentracing.span import ThundraSpan
-from thundra.opentracing.span_context import ThundraSpanContext
-from thundra.plugins.trace import trace_support
+from catchpoint import constants
+from catchpoint.context.execution_context_manager import ExecutionContextManager
+from catchpoint.opentracing.propagation.http import HTTPPropagator
+from catchpoint.opentracing.propagation.text import TextMapPropagator
+from catchpoint.opentracing.span import CatchpointSpan
+from catchpoint.opentracing.span_context import CatchpointSpanContext
+from catchpoint.plugins.trace import trace_support
 
-from thundra.utils import arrange_scope_manager
+from catchpoint.utils import arrange_scope_manager
 
 
-class ThundraTracer(opentracing.Tracer):
+class CatchpointTracer(opentracing.Tracer):
     __instance = None
     
 
     @staticmethod
     def get_instance():
-        return ThundraTracer() if ThundraTracer.__instance is None else ThundraTracer.__instance
+        return CatchpointTracer() if CatchpointTracer.__instance is None else CatchpointTracer.__instance
 
 
     def __init__(self, scope_manager=None):
         scope_manager = arrange_scope_manager(scope_manager)
-        super(ThundraTracer, self).__init__(scope_manager)
+        super(CatchpointTracer, self).__init__(scope_manager)
         self.lock = Lock()
         self.global_span_order = 0
-        ThundraTracer.__instance = self
+        CatchpointTracer.__instance = self
         self._propagators = {
             Format.HTTP_HEADERS: HTTPPropagator(),
             Format.TEXT_MAP: TextMapPropagator(),
         }
 
     def start_active_span(self,
                           operation_name,
@@ -152,27 +152,27 @@
         _parent_span_id = parent_span_id
 
         if _parent_context is not None:
             _trace_id = _trace_id or _parent_context.trace_id
             _transaction_id = _transaction_id or _parent_context.transaction_id
             _parent_span_id = _parent_span_id or _parent_context.span_id
 
-        _context = ThundraSpanContext(trace_id=_trace_id,
-                                      transaction_id=_transaction_id,
-                                      span_id=_span_id,
-                                      parent_span_id=_parent_span_id)
-        _span = ThundraSpan(self,
-                            operation_name=operation_name,
-                            class_name=class_name,
-                            domain_name=domain_name,
-                            context=_context,
-                            tags=tags,
-                            start_time=start_time,
-                            span_order=_span_order,
-                            execution_context=execution_context)
+        _context = CatchpointSpanContext(trace_id=_trace_id,
+                                         transaction_id=_transaction_id,
+                                         span_id=_span_id,
+                                         parent_span_id=_parent_span_id)
+        _span = CatchpointSpan(self,
+                               operation_name=operation_name,
+                               class_name=class_name,
+                               domain_name=domain_name,
+                               context=_context,
+                               tags=tags,
+                               start_time=start_time,
+                               span_order=_span_order,
+                               execution_context=execution_context)
 
         return _span
 
     def get_active_span(self):
         scope = self.scope_manager.active
         if scope is not None:
             return scope.span
```

### Comparing `thundra-3.0.6/thundra/plugins/config/thundra_config.py` & `thundra-3.0.7/catchpoint/plugins/config/catchpoint_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from thundra.plugins.config.log_config import LogConfig
-from thundra.plugins.config.metric_config import MetricConfig
-from thundra.plugins.config.trace_config import TraceConfig
+from catchpoint.plugins.config.log_config import LogConfig
+from catchpoint.plugins.config.metric_config import MetricConfig
+from catchpoint.plugins.config.trace_config import TraceConfig
 
 
-class ThundraConfig:
+class CatchpointConfig:
     def __init__(self, opts=None):
         if opts is None:
             opts = {}
 
         self.api_key = opts.get('apiKey')
-        self.disable_thundra = opts.get('disableThundra')
+        self.disable_catchpoint = opts.get('disableCatchpoint')
         self.trace_config = TraceConfig(opts.get('traceConfig'))
         self.metric_config = MetricConfig(opts.get('metricConfig'))
         self.log_config = LogConfig(opts.get('logConfig'))
```

### Comparing `thundra-3.0.6/thundra/plugins/invocation/invocation_plugin.py` & `thundra-3.0.7/catchpoint/plugins/invocation/invocation_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from thundra.encoder import to_json
-from thundra import constants
+from catchpoint.encoder import to_json
+from catchpoint import constants
 
 
 class InvocationPlugin:
 
     def __init__(self, plugin_context=None):
         self.hooks = {
             'before:invocation': self.before_invocation,
```

### Comparing `thundra-3.0.6/thundra/plugins/invocation/invocation_support.py` & `thundra-3.0.7/catchpoint/plugins/invocation/invocation_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thundra.context.execution_context_manager import ExecutionContextManager
+from catchpoint.context.execution_context_manager import ExecutionContextManager
 
 
 def set_agent_tag(key, value):
     execution_context = ExecutionContextManager.get()
     execution_context.tags[key] = value
```

### Comparing `thundra-3.0.6/thundra/plugins/invocation/invocation_trace_support.py` & `thundra-3.0.7/catchpoint/plugins/invocation/invocation_trace_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import division
 
 import logging
 
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.context.execution_context_manager import ExecutionContextManager
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.context.execution_context_manager import ExecutionContextManager
 
 logger = logging.getLogger(__name__)
 
 
 class Resource:
 
     def __init__(self, span):
@@ -127,24 +127,24 @@
         }
     except Exception as e:
         logger.error("error while creating the resources data for invocation: %s", e)
         return {}
 
 
 def get_incoming_trace_links():
-    if ConfigProvider.get(config_names.THUNDRA_DISABLE, False):
+    if ConfigProvider.get(config_names.CATCHPOINT_DISABLE, False):
         return {}
 
     execution_context = ExecutionContextManager.get()
     incoming_trace_links = list(set(execution_context.incoming_trace_links))[:constants.MAX_INCOMING_TRACE_LINKS]
     return {"incomingTraceLinks": incoming_trace_links}
 
 
 def get_outgoing_trace_links():
-    if ConfigProvider.get(config_names.THUNDRA_DISABLE, False):
+    if ConfigProvider.get(config_names.CATCHPOINT_DISABLE, False):
         return {}
 
     execution_context = ExecutionContextManager.get()
     spans = execution_context.recorder.get_spans()
 
     outgoing_trace_links = []
     outgoing_trace_links.extend(execution_context.outgoing_trace_links)
```

### Comparing `thundra-3.0.6/thundra/plugins/log/log_plugin.py` & `thundra-3.0.7/catchpoint/plugins/log/log_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import sys
 from threading import Lock
 
 import wrapt
 
-from thundra import constants
-from thundra.compat import PY37, PY38
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.plugins.config.log_config import LogConfig
-from thundra.plugins.log import log_support
-from thundra.plugins.log.thundra_log_handler import ThundraLogHandler
-from thundra.plugins.log.thundra_logger import StreamToLogger
+from catchpoint import constants
+from catchpoint.compat import PY37, PY38
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.plugins.config.log_config import LogConfig
+from catchpoint.plugins.log import log_support
+from catchpoint.plugins.log.catchpoint_log_handler import CatchpointLogHandler
+from catchpoint.plugins.log.catchpoint_logger import StreamToLogger
 
 
 class LogPlugin:
     lock = Lock()
     wrapped = False
 
     def __init__(self, plugin_context=None, config=None):
@@ -29,32 +29,32 @@
         if isinstance(config, LogConfig):
             self.config = config
         else:
             self.config = LogConfig()
 
         with LogPlugin.lock:
             if (not LogPlugin.wrapped) and (
-                    not ConfigProvider.get(config_names.THUNDRA_LOG_CONSOLE_DISABLE)):
+                    not ConfigProvider.get(config_names.CATCHPOINT_LOG_CONSOLE_DISABLE)):
                 if PY37 or PY38:
                     wrapt.wrap_function_wrapper(
                         'builtins',
                         'print',
                         self._wrapper
                     )
                 else:
                     sys.stdout = StreamToLogger(self.logger, sys.stdout)
                 LogPlugin.wrapped = True
 
-        if not ConfigProvider.get(config_names.THUNDRA_LOG_CONSOLE_DISABLE):
-            handler = ThundraLogHandler()
-            has_thundra_log_handler = False
+        if not ConfigProvider.get(config_names.CATCHPOINT_LOG_CONSOLE_DISABLE):
+            handler = CatchpointLogHandler()
+            has_catchpoint_log_handler = False
             for log_handlers in self.logger.handlers:
-                if isinstance(log_handlers, ThundraLogHandler):
-                    has_thundra_log_handler = True
-            if not has_thundra_log_handler:
+                if isinstance(log_handlers, CatchpointLogHandler):
+                    has_catchpoint_log_handler = True
+            if not has_catchpoint_log_handler:
                 self.logger.addHandler(handler)
             self.logger.setLevel(logging.INFO)
             handler.setLevel(logging.INFO)
             self.logger.propagate = False
 
 
     def _wrapper(self, wrapped, instance, args, kwargs):
@@ -69,15 +69,15 @@
         execution_context.capture_log = True
 
 
     def after_invocation(self, execution_context):
         execution_context.capture_log = False
         log_data = {
             'type': "Log",
-            'agentVersion': constants.THUNDRA_AGENT_VERSION,
+            'agentVersion': constants.CATCHPOINT_AGENT_VERSION,
             'dataModelVersion': constants.DATA_FORMAT_VERSION,
             'traceId': execution_context.trace_id,
             'transactionId': execution_context.transaction_id,
         }
 
         for log in execution_context.logs:
             # Add application related data
```

### Comparing `thundra-3.0.6/thundra/plugins/log/thundra_log_handler.py` & `thundra-3.0.7/catchpoint/plugins/log/catchpoint_log_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import uuid
 
-from thundra.context.execution_context_manager import ExecutionContextManager
+from catchpoint.context.execution_context_manager import ExecutionContextManager
 
 
-class ThundraLogHandler(logging.Handler):
+class CatchpointLogHandler(logging.Handler):
 
     def __init__(self):
         logging.Handler.__init__(self)
 
     def emit(self, record):
         formatted_message = self.format(record)
         execution_context = ExecutionContextManager.get()
@@ -21,8 +21,8 @@
                 'logTimestamp': int(record.created * 1000),
                 'logLevel': record.levelname,
                 'logLevelCode': int(record.levelno / 10)
             }
             execution_context.logs.append(log)
 
 
-logging.ThundraLogHandler = ThundraLogHandler
+logging.CatchpointLogHandler = CatchpointLogHandler
```

### Comparing `thundra-3.0.6/thundra/plugins/log/thundra_logger.py` & `thundra-3.0.7/catchpoint/plugins/log/catchpoint_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
 loggers = {}
 
 
 class StreamToLogger(object):
     def __init__(self, logger, stdout):
         self.logger = logger
@@ -43,15 +43,15 @@
 def log_to_console(message, handler):
     logger = get_logger(handler)
     logging.getLogger().handlers = []
     logger.debug(message)
 
 
 def debug_logger(msg, handler=None):
-    if ConfigProvider.get(config_names.THUNDRA_DEBUG_ENABLE):
+    if ConfigProvider.get(config_names.CATCHPOINT_DEBUG_ENABLE):
         if hasattr(msg, '__dict__'):
             log_to_console(msg, handler)
             display = vars(msg)
             log_to_console(display, handler)
             for key, _ in display.items():
                 debug_logger_helper(getattr(msg, key), handler)
         else:
```

### Comparing `thundra-3.0.6/thundra/plugins/metric/metric_plugin.py` & `thundra-3.0.7/catchpoint/plugins/metric/metric_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import gc
 import logging
 import threading
 import time
 import uuid
 
-from thundra import utils, constants
-from thundra.compat import PY2
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.plugins.config.metric_config import MetricConfig
-from thundra.plugins.metric import metric_support
+from catchpoint import utils, constants
+from catchpoint.compat import PY2
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.plugins.config.metric_config import MetricConfig
+from catchpoint.plugins.metric import metric_support
 
 logger = logging.getLogger(__name__)
 
 
 class MetricPlugin:
 
     def __init__(self, plugin_context=None, config=None):
         self.metric_data = {}
         self.plugin_context = plugin_context
-        self.tracer = ThundraTracer.get_instance()
+        self.tracer = CatchpointTracer.get_instance()
         self.system_cpu_usage_start = float(0)
         self.system_cpu_usage_end = float(0)
         self.system_cpu_total_start = float(0)
         self.system_cpu_total_end = float(0)
         self.process_cpu_usage_start = float(0)
         self.process_cpu_usage_end = float(0)
         self.hooks = {
@@ -37,15 +37,15 @@
 
     def before_invocation(self, execution_context):
         metric_time = time.time() * 1000
         active_span = self.tracer.get_active_span()
 
         self.metric_data = {
             'type': "Metric",
-            'agentVersion': constants.THUNDRA_AGENT_VERSION,
+            'agentVersion': constants.CATCHPOINT_AGENT_VERSION,
             'dataModelVersion': constants.DATA_FORMAT_VERSION,
             'traceId': active_span.trace_id if active_span is not None else '',
             'transactionId': execution_context.transaction_id,
             'spanId': active_span.span_id if active_span is not None else '',
             'metricTimestamp': int(metric_time),
             'tags': {
                 'aws.region': utils.get_env_variable(constants.AWS_REGION, default='')
```

### Comparing `thundra-3.0.6/thundra/plugins/trace/patcher.py` & `thundra-3.0.7/catchpoint/plugins/trace/patcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import absolute_import, unicode_literals
 
 import sys
 from importlib.machinery import PathFinder, ModuleSpec, SourceFileLoader
 
-import thundra.utils as utils
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.plugins.trace.traceable import Traceable
+import catchpoint.utils as utils
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.plugins.trace.traceable import Traceable
 
 
 class ImportPatcher(utils.Singleton):
 
     def __init__(self):
         self.modules_map = self.__process_env_var_modules_to_instrument()
 
         for module_path in self.modules_map.keys():
-            sys.meta_path.insert(0, ThundraFinder(module_path))
+            sys.meta_path.insert(0, CatchpointFinder(module_path))
 
     @staticmethod
     def __process_env_var_modules_to_instrument():
         modules = {}
         for variable in ConfigProvider.configs:
             value = ConfigProvider.get(variable)
-            if variable.startswith(config_names.THUNDRA_TRACE_INSTRUMENT_TRACEABLECONFIG):
+            if variable.startswith(config_names.CATCHPOINT_TRACE_INSTRUMENT_TRACEABLECONFIG):
                 try:
                     module_path, function_prefix, arguments = utils.process_trace_def_var(value)
                     if module_path is not None:
                         modules[module_path] = [function_prefix, arguments]
                 except:
                     pass
 
@@ -42,31 +42,31 @@
     def get_trace_arguments(self, module_name):
         try:
             return self.modules_map[module_name][1]
         except:
             return None
 
 
-class ThundraFinder(PathFinder):
+class CatchpointFinder(PathFinder):
 
     def __init__(self, module_name):
         self.module_name = module_name
 
     def find_spec(self, fullname, path=None, target=None):
         if fullname == self.module_name:
-            spec = super(ThundraFinder, self).find_spec(fullname, path, target)
-            loader = ThundraLoader(fullname, spec.origin)
+            spec = super(CatchpointFinder, self).find_spec(fullname, path, target)
+            loader = CatchpointLoader(fullname, spec.origin)
             return ModuleSpec(fullname, loader)
 
 
 # Loading the module in a load time
-class ThundraLoader(SourceFileLoader):
+class CatchpointLoader(SourceFileLoader):
 
     def exec_module(self, module):
-        super(ThundraLoader, self).exec_module(module)
+        super(CatchpointLoader, self).exec_module(module)
         import_patcher = ImportPatcher()
         module_name = utils.get_module_name(module)
         function_prefix = import_patcher.get_module_function_prefix(module_name)
         trace_args_list = import_patcher.get_trace_arguments(module_name)
         try:
             trace_args = utils.str2bool(trace_args_list[constants.TRACE_ARGS])
         except:
```

### Comparing `thundra-3.0.6/thundra/plugins/trace/trace_aware_wrapper.py` & `thundra-3.0.7/catchpoint/plugins/trace/trace_aware_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from functools import wraps
-from thundra.opentracing.tracer import ThundraTracer
+from catchpoint.opentracing.tracer import CatchpointTracer
 
 
 class TraceAwareWrapper:
 
     def __init__(self, active_span=None):
         if active_span is None:
-            active_scope = ThundraTracer.get_instance().scope_manager.active
+            active_scope = CatchpointTracer.get_instance().scope_manager.active
             active_span = active_scope.span if active_scope is not None else None
         self._parent_span = active_span
 
     @property
     def parent_span(self):
         return self._parent_span
 
     def __call__(self, original_func):
         @wraps(original_func)
         def wrapper(*args, **kwargs):
-            ThundraTracer.get_instance().scope_manager.activate(self.parent_span, True)
+            CatchpointTracer.get_instance().scope_manager.activate(self.parent_span, True)
             return original_func(*args, **kwargs)
         return wrapper
```

### Comparing `thundra-3.0.6/thundra/plugins/trace/trace_plugin.py` & `thundra-3.0.7/catchpoint/plugins/trace/trace_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 import traceback
 import uuid
 
-from thundra import constants
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.plugins.config.trace_config import TraceConfig
-from thundra.plugins.invocation import invocation_support
-from thundra.plugins.trace import trace_support
+from catchpoint import constants
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.plugins.config.trace_config import TraceConfig
+from catchpoint.plugins.invocation import invocation_support
+from catchpoint.plugins.trace import trace_support
 
 logger = logging.getLogger(__name__)
 
 
 class TracePlugin:
 
     def __init__(self, plugin_context, config=None):
         self.hooks = {
             'before:invocation': self.before_invocation,
             'after:invocation': self.after_invocation
         }
-        self.tracer = ThundraTracer.get_instance()
+        self.tracer = CatchpointTracer.get_instance()
         self.plugin_context = plugin_context
         if isinstance(config, TraceConfig):
             self.config = config
         else:
             self.config = TraceConfig()
 
     def before_invocation(self, execution_context):
@@ -83,15 +83,15 @@
     def build_span(self, span, execution_context):
         if not execution_context.transaction_id:
             execution_context.transaction_id = str(uuid.uuid4())
         service_name = span.service_name if hasattr(span, "service_name") else ''
         span_data = {
             'id': span.context.span_id,
             'type': "Span",
-            'agentVersion': constants.THUNDRA_AGENT_VERSION,
+            'agentVersion': constants.CATCHPOINT_AGENT_VERSION,
             'dataModelVersion': constants.DATA_FORMAT_VERSION,
             'traceId': span.context.trace_id,
             'transactionId': execution_context.transaction_id,
             'parentSpanId': span.context.parent_span_id or '',
             'spanOrder': span.span_order,
             'domainName': span.domain_name or '',
             'className': span.class_name or '',
```

### Comparing `thundra-3.0.6/thundra/plugins/trace/trace_support.py` & `thundra-3.0.7/catchpoint/plugins/trace/trace_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 import re
 from gzip import GzipFile
 
 try:
     from BytesIO import BytesIO
 except ImportError:
     from io import BytesIO
-from thundra.listeners import ThundraSpanListener
+from catchpoint.listeners import CatchpointSpanListener
 
-from thundra.config.config_provider import ConfigProvider
-from thundra.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
 
 logger = logging.getLogger(__name__)
 
 _active_span_listeners = []
 _sampler = None
 
 SPAN_LISTENERS = {
     sl_class.__name__: sl_class
-    for sl_class in ThundraSpanListener.__subclasses__()
+    for sl_class in CatchpointSpanListener.__subclasses__()
 }
 
 # To match span listener class type and it's arguments as two groups
 r1 = r'(\w+)\[(.*)\]'
 # To match each argument key value pair in arguments list
 r2 = r'[\w.]+=[\w.\!\?\-\"\'\:\(\) ]*'
 # Compile reg exs
@@ -57,15 +57,15 @@
 
 def _parse_span_listeners():
     # Clear before parsing to prevent appending duplicate span listeners
     clear_span_listeners()
     # Add span listeners configured using environment variables
     for env_k in ConfigProvider.configs:
         env_v = ConfigProvider.get(env_k)
-        if env_k.startswith(config_names.THUNDRA_TRACE_SPAN_LISTENERCONFIG):
+        if env_k.startswith(config_names.CATCHPOINT_TRACE_SPAN_LISTENERCONFIG):
             try:
                 # Not in JSON format. Should be zipped + encoded. Decode + unzip it
                 if not env_v.startswith('{'):
                     compressed_env = base64.b64decode(env_v)
                     env_v = str(GzipFile(fileobj=BytesIO(compressed_env)).read(), 'utf-8')
                 span_listener_config_json = json.loads(env_v)
```

### Comparing `thundra-3.0.6/thundra/plugins/trace/traceable.py` & `thundra-3.0.7/catchpoint/plugins/trace/traceable.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import sys
 from functools import wraps
 from threading import Lock
 
 import jsonpickle
 from opentracing import Scope
 
-from thundra import constants
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.plugins.log.thundra_logger import debug_logger
-from thundra.serializable import Serializable
+from catchpoint import constants
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.plugins.log.catchpoint_logger import debug_logger
+from catchpoint.serializable import Serializable
 from pympler import asizeof
 import threading
 trace_local = threading.local()
 
 DATA_LIMIT = 8 * 1024 # 8KB
-DATA_LIMIT_RETURN_STR = "[THUNDRA] Data is over {} KB".format(DATA_LIMIT / 1024)
+DATA_LIMIT_RETURN_STR = "[Catchpoint] Data is over {} KB".format(DATA_LIMIT / 1024)
 METHOD_LINES_LIMIT = 100
 SERIALIZATION_DEPTH=1
 
 def __get_traceable_from_back_frame(frame):
     _back_frame = frame.f_back
     if _back_frame and 'self' in _back_frame.f_locals:
         _self = _back_frame.f_locals['self']
@@ -100,32 +100,32 @@
 def trace_calls(frame, event, arg):
     if not trace_local.trace_call_active:
         return
 
     trace_local.trace_call_active = False
 
     # First check whether current call is wrapped
-    wrapped_by_thundra = frame.f_back and frame.f_back.f_code.co_name == '___thundra_trace___'
-    if not wrapped_by_thundra:
+    wrapped_by_catchpoint = frame.f_back and frame.f_back.f_code.co_name == '___catchpoint_trace___'
+    if not wrapped_by_catchpoint:
         return
 
-    # Note that "is Thundra wrapped check" is applied before "is event call" check.
-    # Because most of the time "is Thundra wrapped check" is false but "is event call" is true.
+    # Note that "is Catchpoint wrapped check" is applied before "is event call" check.
+    # Because most of the time "is Catchpoint wrapped check" is false but "is event call" is true.
     # And since most of the time 'trace_calls' will return 'None',
     # it is better to detect false case with less comparison.
 
     # Only handle 'call' events
     if event != 'call':
         return
 
     _func_name = frame.f_code.co_name
     # Ignore
     # - 'write()' calls from print statements
-    # - Thundra trace decorator calls
-    ignored = _func_name == 'write' or _func_name == '___thundra_trace___'
+    # - Catchpoint trace decorator calls
+    ignored = _func_name == 'write' or _func_name == '___catchpoint_trace___'
     if ignored:
         return
 
     _traceable = None
     try:
         _traceable = __get_traceable_from_back_frame(frame)
     except ValueError:
@@ -173,15 +173,15 @@
                 self._trace_return_value = True
             if trace_local_variables is None:
                 self._trace_local_variables = True
             if trace_args is None:
                 self._trace_args = True
 
         self._tracing = False
-        self._tracer = ThundraTracer.get_instance()
+        self._tracer = CatchpointTracer.get_instance()
 
     @property
     def tracer(self):
         return self._tracer
 
     @property
     def trace_args(self):
@@ -224,15 +224,15 @@
             value_dict = pickler.flatten(value, reset=True)
             return value_dict, type(value).__name__
         except:
             return '<not-json-serializable-object>', type(value).__name__
 
     def __call__(self, original_func):
         @wraps(original_func)
-        def ___thundra_trace___(*args, **kwargs):
+        def ___catchpoint_trace___(*args, **kwargs):
             parent_scope = self.tracer.scope_manager.active
             parent_span = parent_scope.span if parent_scope is not None else None
 
             # Set finish_on_close to False, otherwise it calls span's finish method which can raise an error,
             # which would cause the scope left open  
             scope = self.tracer.start_active_span(original_func.__name__, child_of=parent_span, finish_on_close=False)
             scope.span.class_name = 'Method'
@@ -316,10 +316,10 @@
                 scope.close()
                 # Set the error tags to the span (if any)
                 if traced_err is not None:
                     scope.span.set_error_to_tag(traced_err)
                     raise traced_err
             return response
 
-        return ___thundra_trace___
+        return ___catchpoint_trace___
 
     call = __call__
```

### Comparing `thundra-3.0.6/thundra/reporter.py` & `thundra-3.0.7/catchpoint/reporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import concurrent.futures as futures
 
-from thundra.plugins.log.thundra_logger import debug_logger
-from thundra import constants, utils
-from thundra.config.config_provider import ConfigProvider
-from thundra.config import config_names
-from thundra.encoder import to_json
+from catchpoint.plugins.log.catchpoint_logger import debug_logger
+from catchpoint import constants, utils
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
+from catchpoint.encoder import to_json
 
 try:
     import requests
 except ImportError:
     from botocore.vendored import requests
 
 logger = logging.getLogger(__name__)
@@ -30,15 +30,15 @@
             session.mount("https://", adapter)
 
         self.session = session
         self.pool = futures.ThreadPoolExecutor(max_workers=20)
 
     def send_reports(self, reports, **opts):
         if not self.api_key:
-            debug_logger("API key not set, not sending report to Thundra.")
+            debug_logger("API key not set, not sending report to Catchpoint.")
             return []
 
         headers = {
             'Content-Type': 'application/json',
             'Authorization': 'ApiKey ' + self.api_key
         }
 
@@ -47,24 +47,24 @@
 
         reports_json = self.prepare_report_json(reports)
         responses = []
         if len(reports_json) > 0:
             _futures = [self.pool.submit(self.send_batch, (request_url, headers, data)) for data in reports_json]
             responses = [future.result() for future in futures.as_completed(_futures)]
 
-        if ConfigProvider.get(config_names.THUNDRA_DEBUG_ENABLE):
-            debug_logger("Thundra API responses: " + str(responses))
+        if ConfigProvider.get(config_names.CATCHPOINT_DEBUG_ENABLE):
+            debug_logger("Catchpoint API responses: " + str(responses))
         return responses
 
     def send_batch(self, args):
         url, headers, data = args
         return self.session.post(url, data=data, headers=headers, timeout=constants.DEFAULT_REPORT_TIMEOUT)
 
     def get_report_batches(self, reports):
-        batch_size = ConfigProvider.get(config_names.THUNDRA_REPORT_REST_COMPOSITE_BATCH_SIZE)
+        batch_size = ConfigProvider.get(config_names.CATCHPOINT_REPORT_REST_COMPOSITE_BATCH_SIZE)
         batches = [reports[i:i + batch_size] for i in range(0, len(reports), batch_size)]
         return batches
 
 
     def prepare_report_json(self, reports):
         batches = self.get_report_batches(reports)
         batched_reports = []
@@ -79,13 +79,13 @@
             json_string = "[{}]".format(','.join(report_jsons))
             batched_reports.append(json_string)
         return batched_reports
 
 
     @staticmethod
     def get_collector_url():
-        use_local = ConfigProvider.get(config_names.THUNDRA_REPORT_REST_LOCAL)
+        use_local = ConfigProvider.get(config_names.CATCHPOINT_REPORT_REST_LOCAL)
 
         if use_local:
             return 'http://' + constants.LOCAL_COLLECTOR_ENDPOINT + '/v1'
-        return ConfigProvider.get(config_names.THUNDRA_REPORT_REST_BASEURL, 'https://' + utils.get_nearest_collector() + '/v1')
+        return ConfigProvider.get(config_names.CATCHPOINT_REPORT_REST_BASEURL, 'https://' + utils.get_nearest_collector() + '/v1')
```

### Comparing `thundra-3.0.6/thundra/samplers/composite_sampler.py` & `thundra-3.0.7/catchpoint/samplers/composite_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thundra.samplers.base_sampler import BaseSampler
+from catchpoint.samplers.base_sampler import BaseSampler
 
 default_operator = 'or'
 available_operators = ['and', 'or']
 
 
 class CompositeSampler(BaseSampler):
```

### Comparing `thundra-3.0.6/thundra/samplers/count_aware_sampler.py` & `thundra-3.0.7/catchpoint/samplers/count_aware_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from threading import Lock
 
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.samplers.base_sampler import BaseSampler
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.samplers.base_sampler import BaseSampler
 
 
 class CountAwareSampler(BaseSampler):
 
     def __init__(self, count_freq=None):
-        freq_from_env = ConfigProvider.get(config_names.THUNDRA_SAMPLER_COUNTAWARE_COUNTFREQ, -1)
+        freq_from_env = ConfigProvider.get(config_names.CATCHPOINT_SAMPLER_COUNTAWARE_COUNTFREQ, -1)
         if freq_from_env > 0:
             self.count_freq = freq_from_env
         elif count_freq is not None:
             self.count_freq = count_freq
         else:
             self.count_freq = constants.DEFAULT_METRIC_SAMPLING_COUNT_FREQ
```

### Comparing `thundra-3.0.6/thundra/samplers/time_aware_sampler.py` & `thundra-3.0.7/catchpoint/samplers/time_aware_sampler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import time
 from threading import Lock
 
-from thundra import constants
-from thundra.samplers.base_sampler import BaseSampler
+from catchpoint import constants
+from catchpoint.samplers.base_sampler import BaseSampler
 
-from thundra.config.config_provider import ConfigProvider
-from thundra.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.config import config_names
 
 
 class TimeAwareSampler(BaseSampler):
 
     def __init__(self, time_freq=None):
-        freq_from_env = ConfigProvider.get(config_names.THUNDRA_SAMPLER_TIMEAWARE_TIMEFREQ, -1)
+        freq_from_env = ConfigProvider.get(config_names.CATCHPOINT_SAMPLER_TIMEAWARE_TIMEFREQ, -1)
         if freq_from_env > 0:
             self.time_freq = freq_from_env
         elif time_freq is not None:
             self.time_freq = time_freq
         else:
             self.time_freq = constants.DEFAULT_METRIC_SAMPLING_TIME_FREQ
         self._latest_time = 0
```

### Comparing `thundra-3.0.6/thundra/timeout.py` & `thundra-3.0.7/catchpoint/timeout.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.6/thundra/utils.py` & `thundra-3.0.7/catchpoint/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import
 import logging
 import os
 import re
 import uuid
 
-from thundra import constants
-from thundra.compat import urlparse
+from catchpoint import constants
+from catchpoint.compat import urlparse
 from opentracing.scope_managers import ThreadLocalScopeManager
 
 logger = logging.getLogger(__name__)
 
 
 def generate_id():
     return str(uuid.uuid4())
@@ -231,17 +231,17 @@
     return xray_info
 
 
 def get_nearest_collector():
     region = get_env_variable(constants.AWS_REGION)
 
     if region:
-        return '{}.collector.thundra.io'.format(region)
+        return '{}.collector.catchpoint.com'.format(region)
 
-    return "collector.thundra.io"
+    return "collector.catchpoint.com"
 
 
 def get_compiled_operation_type_patterns():
     compiled = []
     for pattern in constants.OperationTypeMappings["patterns"]:
         compiled.append(re.compile(pattern))
     return compiled
@@ -314,15 +314,15 @@
             scope_manager = ThreadLocalScopeManager()
     return scope_manager
 
 
 # Excluded url's
 EXCLUDED_URLS = {
     str.endswith: [
-        'thundra.io',
+        'catchpoint.com',
     ],
     str.__contains__: [
         'amazonaws.com',
         'accounts.google.com',
     ],
 }
```

### Comparing `thundra-3.0.6/thundra/wrappers/aws_lambda/handler.py` & `thundra-3.0.7/catchpoint/wrappers/aws_lambda/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import absolute_import
 
 import imp
 import os
 
-from thundra.thundra_agent import Thundra
+from catchpoint.catchpoint_agent import Catchpoint
 
-thundra = Thundra()
+catchpoint = Catchpoint()
 
 handler_found = False
 user_handler = None
-handler_path = os.environ.get('thundra_agent_lambda_handler', None)
+handler_path = os.environ.get('catchpoint_agent_lambda_handler', None)
 if handler_path is None:
     raise ValueError(
-        "No handler specified for \'thundra_agent_lambda_handler\' environment variable"
+        "No handler specified for \'catchpoint_agent_lambda_handler\' environment variable"
     )
 else:
     handler_found = True
     (module_name, handler_name) = handler_path.rsplit('.', 1)
     file_handle, pathname, desc = None, None, None
     try:
         for segment in module_name.split('.'):
@@ -33,10 +33,10 @@
         if file_handle:
             file_handle.close()
 
 
 def wrapper(event, context):
     global user_handler
     if handler_found and user_handler:
-        if not hasattr(user_handler, "_thundra_wrapped"):
-            user_handler = thundra(user_handler)
+        if not hasattr(user_handler, "_catchpoint_wrapped"):
+            user_handler = catchpoint(user_handler)
         return user_handler(event, context)
```

### Comparing `thundra-3.0.6/thundra/wrappers/aws_lambda/lambda_application_info_provider.py` & `thundra-3.0.7/catchpoint/wrappers/aws_lambda/lambda_application_info_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 
-from thundra import constants, utils
-from thundra.application.application_info_provider import ApplicationInfoProvider
+from catchpoint import constants, utils
+from catchpoint.application.application_info_provider import ApplicationInfoProvider
 
 
 class LambdaApplicationInfoProvider(ApplicationInfoProvider):
 
     def __init__(self):
         log_stream_name = utils.get_env_variable(constants.AWS_LAMBDA_LOG_STREAM_NAME)
         function_version = utils.get_env_variable(constants.AWS_LAMBDA_FUNCTION_VERSION)
```

### Comparing `thundra-3.0.6/thundra/wrappers/aws_lambda/lambda_event_utils.py` & `thundra-3.0.7/catchpoint/wrappers/aws_lambda/lambda_event_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import unicode_literals
 
 import base64
 import hashlib
 
 import simplejson as json
 
-from thundra import constants, utils
-from thundra.compat import str
-from thundra.plugins.invocation import invocation_support, invocation_trace_support
+from catchpoint import constants, utils
+from catchpoint.compat import str
+from catchpoint.plugins.invocation import invocation_support, invocation_trace_support
 
 try:
     from BytesIO import BytesIO
 except ImportError:
     from io import BytesIO
 from gzip import GzipFile
 
@@ -138,23 +138,23 @@
         table_names.append(table_name)
 
         region = record['awsRegion']
 
         trace_link_found = False
         if record['eventName'] == "INSERT" or record['eventName'] == "MODIFY":
             new_image = record['dynamodb'].get('NewImage')
-            if new_image and new_image.get(constants.THUNDRA_SPAN_ID_KEY):
-                span_id = new_image.get(constants.THUNDRA_SPAN_ID_KEY).get('S')
+            if new_image and new_image.get(constants.CATCHPOINT_SPAN_ID_KEY):
+                span_id = new_image.get(constants.CATCHPOINT_SPAN_ID_KEY).get('S')
                 trace_link_found = True
                 trace_links.append("SAVE:" + span_id)
 
         elif record['eventName'] == "REMOVE":
             old_image = record['dynamodb'].get('OldImage')
-            if old_image and old_image.get(constants.THUNDRA_SPAN_ID_KEY):
-                span_id = old_image.get(constants.THUNDRA_SPAN_ID_KEY).get('S')
+            if old_image and old_image.get(constants.CATCHPOINT_SPAN_ID_KEY):
+                span_id = old_image.get(constants.CATCHPOINT_SPAN_ID_KEY).get('S')
                 trace_link_found = True
                 trace_links.append("DELETE:" + span_id)
 
         if not trace_link_found:
             creation_time = record['dynamodb'].get('ApproximateCreationDateTime')
             if creation_time:
                 if record['eventName'] == "INSERT" or record['eventName'] == "MODIFY":
@@ -300,16 +300,16 @@
 
     operation_names = []
     resource = utils.extract_api_gw_resource_name(original_event)
     if resource:
         operation_names.append(resource)
         invocation_support.set_application_resource_name(resource)
 
-    if original_event.get('headers') and constants.THUNDRA_SPAN_ID_KEY in original_event['headers']:
-        invocation_trace_support.add_incoming_trace_links([original_event['headers'][constants.THUNDRA_SPAN_ID_KEY]])
+    if original_event.get('headers') and constants.CATCHPOINT_SPAN_ID_KEY in original_event['headers']:
+        invocation_trace_support.add_incoming_trace_links([original_event['headers'][constants.CATCHPOINT_SPAN_ID_KEY]])
 
     inject_trigger_tags_to_span(span, domain_name, class_name, operation_names)
     inject_trigger_tags_to_invocation(domain_name, class_name, operation_names)
 
 
 def inject_trigger_tags_for_api_gateway(span, original_event):
     domain_name = constants.DomainNames['API']
@@ -350,16 +350,16 @@
 
     inject_trigger_tags_to_span(span, domain_name, class_name, operation_names)
     inject_trigger_tags_to_invocation(domain_name, class_name, operation_names)
 
 
 def extract_trace_link_from_event(original_event):
     try:
-        if '_thundra' in original_event:
-            invocation_trace_support.add_incoming_trace_links([original_event['_thundra']['trace_link']])
+        if '_catchpoint' in original_event:
+            invocation_trace_support.add_incoming_trace_links([original_event['_catchpoint']['trace_link']])
     except Exception:
         pass
 
 
 def inject_trigger_tags_to_span(span, domain_name, class_name, operation_names):
     span.set_tag(constants.SpanTags['TRIGGER_DOMAIN_NAME'], domain_name)
     span.set_tag(constants.SpanTags['TRIGGER_CLASS_NAME'], class_name)
```

### Comparing `thundra-3.0.6/thundra/wrappers/aws_lambda/lambda_executor.py` & `thundra-3.0.7/catchpoint/wrappers/aws_lambda/lambda_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import math
 import uuid
 
-from thundra import utils, constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.plugins.invocation import invocation_trace_support
-from thundra.plugins.log.thundra_logger import debug_logger
-from thundra.wrappers import wrapper_utils
-from thundra.wrappers.aws_lambda import lambda_event_utils
+from catchpoint import utils, constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.plugins.invocation import invocation_trace_support
+from catchpoint.plugins.log.catchpoint_logger import debug_logger
+from catchpoint.wrappers import wrapper_utils
+from catchpoint.wrappers.aws_lambda import lambda_event_utils
 
 
 def start_trace(plugin_context, execution_context, tracer):
     context = execution_context.platform_data['originalContext']
     execution_context.trace_id = str(uuid.uuid4())
     # Start root span
     scope = tracer.start_active_span(operation_name=context.function_name,
@@ -94,28 +94,28 @@
     trigger_class_name = root_span.get_tag(constants.SpanTags['TRIGGER_CLASS_NAME'])
 
     # Disable request data sending for cloudwatchlog, firehose and kinesis if not
     # enabled by configuration because requests can get too big for these
     enable_request_data = True
     if (
             trigger_class_name == constants.ClassNames['CLOUDWATCHLOG'] and
-            not ConfigProvider.get(config_names.THUNDRA_LAMBDA_TRACE_CLOUDWATCHLOG_REQUEST_ENABLE)) or (
+            not ConfigProvider.get(config_names.CATCHPOINT_LAMBDA_TRACE_CLOUDWATCHLOG_REQUEST_ENABLE)) or (
 
             trigger_class_name == constants.ClassNames['FIREHOSE'] and
-            not ConfigProvider.get(config_names.THUNDRA_LAMBDA_TRACE_FIREHOSE_REQUEST_ENABLE)) or (
+            not ConfigProvider.get(config_names.CATCHPOINT_LAMBDA_TRACE_FIREHOSE_REQUEST_ENABLE)) or (
 
             trigger_class_name == constants.ClassNames['KINESIS'] and
-            not ConfigProvider.get(config_names.THUNDRA_LAMBDA_TRACE_KINESIS_REQUEST_ENABLE)
+            not ConfigProvider.get(config_names.CATCHPOINT_LAMBDA_TRACE_KINESIS_REQUEST_ENABLE)
     ):
         enable_request_data = False
 
     # ADDING TAGS #
-    if (not ConfigProvider.get(config_names.THUNDRA_TRACE_REQUEST_SKIP)) and enable_request_data:
+    if (not ConfigProvider.get(config_names.CATCHPOINT_TRACE_REQUEST_SKIP)) and enable_request_data:
         root_span.set_tag('aws.lambda.invocation.request', execution_context.platform_data['originalEvent'])
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_RESPONSE_SKIP):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_RESPONSE_SKIP):
         root_span.set_tag('aws.lambda.invocation.response', execution_context.response)
         
     original_event = execution_context.platform_data["originalEvent"]
     if not check_lambda_authorizer(original_event) and trigger_class_name == constants.ClassNames['APIGATEWAY']:
         process_api_gw_response(execution_context)
 
 
@@ -152,37 +152,37 @@
     return status_code
 
 
 def inject_step_function_info(execution_context, outgoing_trace_links):
     try:
         response = execution_context.response
         event = execution_context.platform_data['originalEvent']
-        if ConfigProvider.get(config_names.THUNDRA_LAMBDA_AWS_STEPFUNCTIONS):
+        if ConfigProvider.get(config_names.CATCHPOINT_LAMBDA_AWS_STEPFUNCTIONS):
             trace_link = str(uuid.uuid4())
             step = 0
-            if '_thundra' in event:
-                step = event['_thundra']['step']
+            if '_catchpoint' in event:
+                step = event['_catchpoint']['step']
 
             if isinstance(response, dict):
-                response['_thundra'] = {
+                response['_catchpoint'] = {
                     'trace_link': trace_link,
                     'step': step + 1
                 }
             outgoing_trace_links["outgoingTraceLinks"].append(trace_link)
     except Exception as e:
         print(e)
 
 def inject_appsync_function_info(execution_context, outgoing_trace_links):
     try:
         response = execution_context.response
-        if ConfigProvider.get(config_names.THUNDRA_LAMBDA_AWS_APPSYNC):
+        if ConfigProvider.get(config_names.CATCHPOINT_LAMBDA_AWS_APPSYNC):
             trace_id = execution_context.trace_id
 
             if isinstance(response, dict):
-                response['_thundra'] = {
+                response['_catchpoint'] = {
                     'trace_id': trace_id,
                 }
     except Exception as e:
         print(e)
 
 
 def finish_invocation(execution_context):
```

### Comparing `thundra-3.0.6/thundra/wrappers/base_wrapper.py` & `thundra-3.0.7/catchpoint/wrappers/base_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import abc
 import logging
 import time
 from concurrent import futures
 
-from thundra.compat import PY2, queue
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.plugins.config.thundra_config import ThundraConfig
-from thundra.reporter import Reporter
-from foresight.model import  Terminator
+from catchpoint.compat import PY2, queue
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.plugins.config.catchpoint_config import CatchpointConfig
+from catchpoint.reporter import Reporter
 
 ABC = abc.ABCMeta('ABC', (object,), {})
 
 logger = logging.getLogger(__name__)
 
 
 class ThreadPoolExecutorWithQueueSizeLimit(futures.ThreadPoolExecutor):
@@ -29,34 +28,32 @@
         queue.Queue.put(self, item, block=False)
 
 
 class BaseWrapper(ABC):
 
     def __init__(self, api_key=None, disable_trace=False, disable_metric=True, disable_log=True, opts=None):
         self.plugins = None
-        self.config = ThundraConfig()
+        self.config = CatchpointConfig()
         if opts is not None:
-            self.config = ThundraConfig(opts)
+            self.config = CatchpointConfig(opts)
 
-        self.api_key = ConfigProvider.get(config_names.THUNDRA_APIKEY, api_key)
+        self.api_key = ConfigProvider.get(config_names.CATCHPOINT_APIKEY, api_key)
         if not self.api_key:
             self.api_key = self.config.api_key
         if self.api_key is None:
-            logger.error('Please set "thundra_apiKey" from environment variables in order to use Thundra')
+            logger.error('Please set "catchpoint_apiKey" from environment variables in order to use Catchpoint')
 
         self.reporter = Reporter(self.api_key)
         self.debugger_process = None
 
-        if not ConfigProvider.get(config_names.THUNDRA_TRACE_INSTRUMENT_DISABLE):
+        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_INSTRUMENT_DISABLE):
             if not PY2:
-                from thundra.plugins.trace.patcher import ImportPatcher
+                from catchpoint.plugins.trace.patcher import ImportPatcher
                 self.import_patcher = ImportPatcher()
         self.thread_pool_executor = ThreadPoolExecutorWithQueueSizeLimit()
-        terminator = Terminator()
-        terminator.register_task(self)
 
 
     def execute_hook(self, name, data):
         if name == 'after:invocation':
             [plugin.hooks[name](data) for plugin in reversed(self.plugins) if hasattr(plugin, 'hooks')
              and name in plugin.hooks]
         else:
```

### Comparing `thundra-3.0.6/thundra/wrappers/cp_wrapper_utils.py` & `thundra-3.0.7/catchpoint/wrappers/cp_wrapper_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import uuid
 import json
 import logging
 
-from thundra import constants, utils
-from thundra.application.application_info_provider import ApplicationInfoProvider
-from thundra.encoder import to_json
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-import thundra.wrappers.wrapper_utils as wrapper_utils
+from catchpoint import constants, utils
+from catchpoint.application.application_info_provider import ApplicationInfoProvider
+from catchpoint.encoder import to_json
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+import catchpoint.wrappers.wrapper_utils as wrapper_utils
 
 logger = logging.getLogger(__name__)
 
 
 def on_finish(execution_context, request, response, span):
     try:
         if is_triggered_from_catchpoint(request):
@@ -27,15 +27,15 @@
         if user_agent is None:
             user_agent = headers.get(constants.HTTPHeaders['USER_AGENT'].lower())
         return 'catchpoint' in user_agent.lower() if user_agent else False
     return False
 
 
 def on_catchpoint_request_finish(execution_context, request, response, span):
-    api_key = ConfigProvider.get(config_names.THUNDRA_APIKEY, None)
+    api_key = ConfigProvider.get(config_names.CATCHPOINT_APIKEY, None)
     headers = request.headers if request and request.headers else {}
     region_name = headers.get(constants.CatchpointHeaders.get('REGION_NAME'))
     country_name = headers.get(constants.CatchpointHeaders.get('COUNTRY_NAME'))
     city_name = headers.get(constants.CatchpointHeaders.get('CITY_NAME'))
     test_id = headers.get(constants.CatchpointHeaders.get('TEST_ID'))
     application_name = generate_catchpoint_application_name(region_name, country_name, city_name)
     application_region = region_name if region_name else ''
@@ -58,15 +58,15 @@
     span_data = create_catchpoint_request_span(application_info, span, resource, region_name, country_name, city_name, 
                                                test_id, trace_id, transaction_id, span_id, start_timestamp, finish_timestamp)
     execution_context.report(create_report_data(api_key, 'Span', span_data))
 
     if response and hasattr(response, 'headers'):
         if response.headers is None:
             response.headers = {}
-        response.headers[constants.THUNDRA_TRACE_ID_KEY] = span.context.trace_id
+        response.headers[constants.CATCHPOINT_TRACE_ID_KEY] = span.context.trace_id
 
 
 def create_catchpoint_request_invocation(execution_context, application_info, region_name, country_name, city_name,
                                          test_id, trace_id, transaction_id, span_id, start_timestamp, finish_timestamp,
                                          resource):
     if not execution_context.transaction_id:
         execution_context.transaction_id = str(uuid.uuid4())
```

### Comparing `thundra-3.0.6/thundra/wrappers/django/django_executor.py` & `thundra-3.0.7/catchpoint/wrappers/django/django_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from thundra import constants
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint import constants
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
 
 
 def start_trace(plugin_context, execution_context, tracer):
     request = execution_context.platform_data['request']
     import sys
     if sys.version_info[0] >= 3:
         request_route_path = str(
```

### Comparing `thundra-3.0.6/thundra/wrappers/django/django_wrapper.py` & `thundra-3.0.7/catchpoint/wrappers/django/django_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import logging
 import traceback
 from functools import wraps
 
-from thundra import constants, configure
-from thundra.application.global_application_info_provider import GlobalApplicationInfoProvider
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.context.execution_context_manager import ExecutionContextManager
-from thundra.context.plugin_context import PluginContext
-from thundra.context.tracing_execution_context_provider import TracingExecutionContextProvider
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
-from thundra.wrappers.base_wrapper import BaseWrapper
-from thundra.wrappers.django import django_executor
+from catchpoint import constants, configure
+from catchpoint.application.global_application_info_provider import GlobalApplicationInfoProvider
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.context.execution_context_manager import ExecutionContextManager
+from catchpoint.context.plugin_context import PluginContext
+from catchpoint.context.tracing_execution_context_provider import TracingExecutionContextProvider
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint.wrappers.base_wrapper import BaseWrapper
+from catchpoint.wrappers.django import django_executor
 
 logger = logging.getLogger(__name__)
 
 
 class DjangoWrapper(BaseWrapper):
 
     def __init__(self, api_key=None, disable_trace=False, disable_metric=True, disable_log=True, opts=None):
         try:
             from django.conf import settings
-            django_settings = getattr(settings, 'THUNDRA', None)
+            django_settings = getattr(settings, 'CATCHPOINT', None)
             if django_settings is not None:
                 configure({'config': django_settings})
         except:
             pass
 
         super(DjangoWrapper, self).__init__(api_key, disable_trace, disable_metric, disable_log, opts)
         self.application_info_provider = GlobalApplicationInfoProvider()
@@ -59,26 +59,26 @@
         self.prepare_and_send_reports_async(execution_context)
 
     def process_exception(self, exception):
         execution_context = ExecutionContextManager.get()
         execution_context.error = exception
 
     def __call__(self, original_func):
-        if hasattr(original_func, "_thundra_wrapped") or ConfigProvider.get(config_names.THUNDRA_DISABLE, False):
+        if hasattr(original_func, "_catchpoint_wrapped") or ConfigProvider.get(config_names.CATCHPOINT_DISABLE, False):
             return original_func
 
         @wraps(original_func)
         def wrapper(request, *args, **kwargs):
-            if getattr(request, '_thundra_wrapped', False):
+            if getattr(request, '_catchpoint_wrapped', False):
                 return original_func(request, *args, **kwargs)
-            setattr(request, '_thundra_wrapped', True)
+            setattr(request, '_catchpoint_wrapped', True)
             try:
                 execution_context = self.before_request(request)
             except Exception as e:
-                logger.error("Error during the before part of Thundra: {}".format(e))
+                logger.error("Error during the before part of Catchpoint: {}".format(e))
                 return original_func(request, *args, **kwargs)
 
             response = None
             # Invoke user handler
             try:
                 response = original_func(request, *args, **kwargs)
             except Exception as e:
@@ -86,20 +86,20 @@
                     execution_context.error = {
                         'type': type(e).__name__,
                         'message': str(e),
                         'traceback': traceback.format_exc()
                     }
                     self.after_request(response)
                 except Exception as e_in:
-                    logger.error("Error during the after part of Thundra: {}".format(e_in))
+                    logger.error("Error during the after part of Catchpoint: {}".format(e_in))
                 raise e
 
             try:
                 self.after_request(response)
             except Exception as e:
-                logger.error("Error during the after part of Thundra: {}".format(e))
+                logger.error("Error during the after part of Catchpoint: {}".format(e))
             return response
 
-        setattr(wrapper, '_thundra_wrapped', True)
+        setattr(wrapper, '_catchpoint_wrapped', True)
         return wrapper
 
     call = __call__
```

### Comparing `thundra-3.0.6/thundra/wrappers/django/middleware.py` & `thundra-3.0.7/catchpoint/wrappers/django/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from thundra.context.execution_context_manager import ExecutionContextManager
-from thundra.wrappers.django.django_wrapper import DjangoWrapper, logger
-from thundra.wrappers.web_wrapper_utils import process_request_route
+from catchpoint.context.execution_context_manager import ExecutionContextManager
+from catchpoint.wrappers.django.django_wrapper import DjangoWrapper, logger
+from catchpoint.wrappers.web_wrapper_utils import process_request_route
 
 
-class ThundraMiddleware(object):
+class CatchpointMiddleware(object):
     def __init__(self, get_response=None):
-        super(ThundraMiddleware, self).__init__()
+        super(CatchpointMiddleware, self).__init__()
         self.get_response = get_response
         self._wrapper = DjangoWrapper()
 
     def __call__(self, request):
-        setattr(request, '_thundra_wrapped', True)
+        setattr(request, '_catchpoint_wrapped', True)
         # Code to be executed for each request before
         # the view (and later middleware) are called.
         before_done = False
         try:
             self._wrapper.before_request(request)
             before_done = True
         except Exception as e:
-            logger.error("Error during the before part of Thundra: {}".format(e))
+            logger.error("Error during the before part of Catchpoint: {}".format(e))
 
         response = self.get_response(request)
 
         # Code to be executed for each request/response after
         # the view is called.
         if before_done:
             try:
                 self._wrapper.after_request(response)
             except Exception as e:
-                logger.error("Error during the after part of Thundra: {}".format(e))
+                logger.error("Error during the after part of Catchpoint: {}".format(e))
 
         return response
 
     def process_view(self, request, view_func, view_args, view_kwargs):
         execution_context = ExecutionContextManager.get()
         if request.resolver_match:
             request_host = request.get_host().split(':')[0]
```

### Comparing `thundra-3.0.6/thundra/wrappers/fastapi/fastapi_executor.py` & `thundra-3.0.7/catchpoint/wrappers/fastapi/fastapi_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from thundra import constants
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint import constants
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
 
-from thundra.wrappers.fastapi.fastapi_utils import extract_headers
+from catchpoint.wrappers.fastapi.fastapi_utils import extract_headers
 
 import json
 
 def start_trace(plugin_context, execution_context, tracer):
     request = execution_context.platform_data["request"]
 
     request = {
```

### Comparing `thundra-3.0.6/thundra/wrappers/fastapi/fastapi_utils.py` & `thundra-3.0.7/catchpoint/wrappers/fastapi/fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `thundra-3.0.6/thundra/wrappers/fastapi/fastapi_wrapper.py` & `thundra-3.0.7/catchpoint/wrappers/fastapi/fastapi_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from functools import wraps
 import logging
-from thundra import constants
+from catchpoint import constants
 
-from thundra.opentracing.tracer import ThundraTracer
-from thundra.wrappers.base_wrapper import BaseWrapper
+from catchpoint.opentracing.tracer import CatchpointTracer
+from catchpoint.wrappers.base_wrapper import BaseWrapper
 
-from thundra.config.config_provider import ConfigProvider
-from thundra.context.execution_context_manager import ExecutionContextManager
-from thundra.context.plugin_context import PluginContext
-from thundra.application.global_application_info_provider import GlobalApplicationInfoProvider
-from thundra.context.tracing_execution_context_provider import TracingExecutionContextProvider
-from thundra.wrappers.fastapi import fastapi_executor
-from thundra.config import config_names
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.context.execution_context_manager import ExecutionContextManager
+from catchpoint.context.plugin_context import PluginContext
+from catchpoint.application.global_application_info_provider import GlobalApplicationInfoProvider
+from catchpoint.context.tracing_execution_context_provider import TracingExecutionContextProvider
+from catchpoint.wrappers.fastapi import fastapi_executor
+from catchpoint.config import config_names
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
 
 import traceback
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -65,33 +65,33 @@
         self.prepare_and_send_reports_async(execution_context)
         
         
 
     def __call__(self, original_func):
 
         import inspect
-        if hasattr(original_func, "_thundra_wrapped") or ConfigProvider.get(config_names.THUNDRA_DISABLE, False):
+        if hasattr(original_func, "_catchpoint_wrapped") or ConfigProvider.get(config_names.CATCHPOINT_DISABLE, False):
             return original_func
 
         @wraps(original_func)
         async def wrapper(*args, **kwargs):
             request = kwargs.get("request")
-            if request is None or request.scope.get('_thundra_wrapped', False):
+            if request is None or request.scope.get('_catchpoint_wrapped', False):
                 if inspect.iscoroutinefunction(original_func):
                     return await original_func(*args, **kwargs)
                 else:
                     return original_func(*args, **kwargs)
 
-            request.scope['_thundra_wrapped'] = True
+            request.scope['_catchpoint_wrapped'] = True
             try:
                 req_body = request._body if hasattr(request, "_body") else None
-                request.scope["thundra_execution_context"] = self.before_request(request.scope, req_body)
-                execution_context = request.scope["thundra_execution_context"]
+                request.scope["catchpoint_execution_context"] = self.before_request(request.scope, req_body)
+                execution_context = request.scope["catchpoint_execution_context"]
             except Exception as e:
-                logger.error('Error during the before part of Thundra: {}'.format(e))
+                logger.error('Error during the before part of Catchpoint: {}'.format(e))
                 if inspect.iscoroutinefunction(original_func):
                     return await original_func(*args, **kwargs)
                 else:
                     return original_func(*args, **kwargs)
 
             response = None
             try:
@@ -104,19 +104,19 @@
                     error = {
                         'type': type(e).__name__,
                         'message': str(e),
                         'traceback': traceback.format_exc()
                     }
                     self.error_handler(error, execution_context)
                 except Exception as e_in:
-                    logger.error("Error during the after part of Thundra: {}".format(e_in))
+                    logger.error("Error during the after part of Catchpoint: {}".format(e_in))
                 raise e
 
             try:
                 execution_context.response = response
                 self.after_request(execution_context)
             except Exception as e:
-                logger.error("Error during the after part of Thundra: {}".format(e))
+                logger.error("Error during the after part of Catchpoint: {}".format(e))
             return response
 
-        setattr(wrapper, '_thundra_wrapped', True)
+        setattr(wrapper, '_catchpoint_wrapped', True)
         return wrapper
```

### Comparing `thundra-3.0.6/thundra/wrappers/fastapi/middleware.py` & `thundra-3.0.7/catchpoint/wrappers/fastapi/middleware.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from thundra.wrappers.fastapi.fastapi_wrapper import FastapiWrapper, logger
-from thundra.config import config_names
+from catchpoint.wrappers.fastapi.fastapi_wrapper import FastapiWrapper, logger
+from catchpoint.config import config_names
 
-from thundra.wrappers.fastapi.fastapi_utils import extract_headers
+from catchpoint.wrappers.fastapi.fastapi_utils import extract_headers
 
-from thundra.config.config_provider import ConfigProvider
-from thundra import constants
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint import constants
 
 import traceback
 
 RESPONSE_REDIRECT_STATUS_CODE = 307
 
 def handle_error(exception, exception_handler, execution_context = None):
     error = {
         'type': type(exception).__name__,
         'message': str(exception),
         'traceback': traceback.format_exc()
     }
     exception_handler(error, execution_context)
 
-class ThundraMiddleware(object):
+class CatchpointMiddleware(object):
     def __init__(self, app, wrapper):
         self.app = app
         self._wrapper = wrapper
 
     async def __call__(self, scope, receive, send):
         """ASGI Middleware
 
@@ -32,19 +32,19 @@
             send (Callable): Send response to client
             
         """
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
         try:
-            scope["_thundra_wrapped"] = True
-            scope["thundra_execution_context"] = self._wrapper.before_request(scope, None)
-            execution_context = scope["thundra_execution_context"]
+            scope["_catchpoint_wrapped"] = True
+            scope["catchpoint_execution_context"] = self._wrapper.before_request(scope, None)
+            execution_context = scope["catchpoint_execution_context"]
         except Exception as e:
-            logger.error("Error during the before part of Thundra fastapi: {}".format(e))
+            logger.error("Error during the before part of Catchpoint fastapi: {}".format(e))
 
         def handle_response(message):
             """ Checking response should be redirect or not. If redirected, then pass the response body by
             setting res_redirected field in scope.
 
             Args:
                 message (Response):  
@@ -69,47 +69,47 @@
                                 "body": execution_context.response.get("body") if execution_context.response.get("body") else None
                             }
                             self._wrapper.after_request(execution_context)
                     except Exception as e:
                         try:
                             handle_error(e, self._wrapper.error_handler, execution_context)
                         except Exception as exc:
-                            logger.error("Error during the after part of Thundra fastapi: {}".format(exc))
+                            logger.error("Error during the after part of Catchpoint fastapi: {}".format(exc))
             except Exception as e:
                 logger.error("Error during getting res body in fast api: {}".format(e))
     
 
         async def wrapped_send(message):
             handle_response(message)
             await send(message)
 
 
         def handle_request(req):
-            """Manipulate request for thundra tracer. If request has "more_body" field, then add it
+            """Manipulate request for catchpoint tracer. If request has "more_body" field, then add it
             to current request body in execution context request body.
 
             Args:
                 req (Request): Gathered from asgi receive function
             """
             if req["type"] == "http.request":
                 try:
                     if "body" in req:
                         req_body = req.get("body", b"")
                         if execution_context.platform_data["request"]["body"]:
                             execution_context.platform_data["request"]["body"] += req_body
                         else:
                             execution_context.platform_data["request"]["body"] = req_body
-                        if not ConfigProvider.get(config_names.THUNDRA_TRACE_REQUEST_SKIP, True):
+                        if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_REQUEST_SKIP, True):
                             execution_context.root_span.set_tag(constants.HttpTags['BODY'], execution_context.platform_data["request"]["body"])
                 except Exception as e:
                     logger.error("Error during getting req body in fast api: {}".format(e))
 
 
         async def wrapped_receive():
-            """Wrap asgi receive function to get request and add it to thundra tracer
+            """Wrap asgi receive function to get request and add it to catchpoint tracer
 
             Raises:
                 e: Exception occurs in receive function
 
             Returns:
                 Request: Request gather from asgi receive function
             """
```

### Comparing `thundra-3.0.6/thundra/wrappers/flask/flask_executor.py` & `thundra-3.0.7/catchpoint/wrappers/flask/flask_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
 
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
 import logging
 
 Logger = logging.getLogger(__name__)
 
 
 def start_trace(plugin_context, execution_context, tracer):
     request = execution_context.platform_data['request']
@@ -33,17 +33,17 @@
         Getting request data into start trace occurs unexpected bugs into application process.
         After whole process finish for request data into appşication flow, getting request data and
         set the request_body for root_span as tag.
     """
     try:
         _request = execution_context.platform_data['request']
         req_data = None
-        if _request and not ConfigProvider.get(config_names.THUNDRA_TRACE_REQUEST_SKIP, False):
+        if _request and not ConfigProvider.get(config_names.CATCHPOINT_TRACE_REQUEST_SKIP, False):
             cl = _request.content_length
-            if cl == None or cl <= constants.THUNDRA_MAX_STREAM_REQUEST_BODY:
+            if cl == None or cl <= constants.CATCHPOINT_MAX_STREAM_REQUEST_BODY:
                 req_data = _request.get_data()
             else:
                 req_data = None
             root_span.set_tag(constants.HttpTags['BODY'], req_data)
     except Exception as e:
         Logger.error("Error occured whilst setting request body to root span tag: {}".format(e))
         pass
```

### Comparing `thundra-3.0.6/thundra/wrappers/flask/flask_wrapper.py` & `thundra-3.0.7/catchpoint/wrappers/flask/flask_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import traceback
 from functools import wraps
 
-from thundra import constants
-from thundra.application.global_application_info_provider import GlobalApplicationInfoProvider
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.context.execution_context_manager import ExecutionContextManager
-from thundra.context.plugin_context import PluginContext
-from thundra.context.tracing_execution_context_provider import TracingExecutionContextProvider
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
-from thundra.wrappers.base_wrapper import BaseWrapper
-from thundra.wrappers.flask import flask_executor
+from catchpoint import constants
+from catchpoint.application.global_application_info_provider import GlobalApplicationInfoProvider
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.context.execution_context_manager import ExecutionContextManager
+from catchpoint.context.plugin_context import PluginContext
+from catchpoint.context.tracing_execution_context_provider import TracingExecutionContextProvider
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint.wrappers.base_wrapper import BaseWrapper
+from catchpoint.wrappers.flask import flask_executor
 
 try:
     from flask import request, g
 except ImportError:
     request = None
     g = None
 
@@ -45,51 +45,51 @@
         execution_context.platform_data['request'] = _request
 
         # Execute plugin hooks before running user's handler
         self.plugin_context.request_count += 1
         self.execute_hook('before:invocation', execution_context)
 
         if g is not None:
-            g.thundra_execution_context = execution_context
+            g.catchpoint_execution_context = execution_context
 
         return execution_context
 
     def after_request(self, response):
         try:
-            if g is not None and hasattr(g, 'thundra_execution_context'):
-                execution_context = g.thundra_execution_context
+            if g is not None and hasattr(g, 'catchpoint_execution_context'):
+                execution_context = g.catchpoint_execution_context
                 if response:
                     execution_context.response = response
         except Exception as e:
-            logger.error('Error setting response to context for Thundra: {}'.format(e))
+            logger.error('Error setting response to context for Catchpoint: {}'.format(e))
         return response
 
     def teardown_request(self, exception=None):
         try:
-            if g is not None and hasattr(g, 'thundra_execution_context'):
-                execution_context = g.thundra_execution_context
+            if g is not None and hasattr(g, 'catchpoint_execution_context'):
+                execution_context = g.catchpoint_execution_context
                 if exception:
                     execution_context.error = exception
                 self.prepare_and_send_reports_async(execution_context)
         except Exception as e:
-            logger.error('Error during the request teardown of Thundra: {}'.format(e))
+            logger.error('Error during the request teardown of Catchpoint: {}'.format(e))
 
     def __call__(self, original_func):
-        if hasattr(original_func, "_thundra_wrapped") or ConfigProvider.get(config_names.THUNDRA_DISABLE, False):
+        if hasattr(original_func, "_catchpoint_wrapped") or ConfigProvider.get(config_names.CATCHPOINT_DISABLE, False):
             return original_func
 
         @wraps(original_func)
         def wrapper(*args, **kwargs):
-            if request is None or getattr(request, '_thundra_wrapped', False):
+            if request is None or getattr(request, '_catchpoint_wrapped', False):
                 return original_func(*args, **kwargs)
-            setattr(request, '_thundra_wrapped', True)
+            setattr(request, '_catchpoint_wrapped', True)
             try:
                 execution_context = self.before_request(request)
             except Exception as e:
-                logger.error('Error during the before part of Thundra: {}'.format(e))
+                logger.error('Error during the before part of Catchpoint: {}'.format(e))
                 return original_func(*args, **kwargs)
 
             response = None
             # Invoke user handler
             try:
                 response = original_func(*args, **kwargs)
                 execution_context.response = response
@@ -98,20 +98,20 @@
                     error = {
                         'type': type(e).__name__,
                         'message': str(e),
                         'traceback': traceback.format_exc()
                     }
                     self.teardown_request(error)
                 except Exception as e_in:
-                    logger.error("Error during the after part of Thundra: {}".format(e_in))
+                    logger.error("Error during the after part of Catchpoint: {}".format(e_in))
                 raise e
 
             try:
                 self.teardown_request()
             except Exception as e:
-                logger.error("Error during the after part of Thundra: {}".format(e))
+                logger.error("Error during the after part of Catchpoint: {}".format(e))
             return response
 
-        setattr(wrapper, '_thundra_wrapped', True)
+        setattr(wrapper, '_catchpoint_wrapped', True)
         return wrapper
 
     call = __call__
```

### Comparing `thundra-3.0.6/thundra/wrappers/flask/middleware.py` & `thundra-3.0.7/catchpoint/wrappers/flask/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from thundra.wrappers.flask.flask_wrapper import FlaskWrapper, logger
-from thundra.utils import Singleton
+from catchpoint.wrappers.flask.flask_wrapper import FlaskWrapper, logger
+from catchpoint.utils import Singleton
 
-class ThundraMiddleware(Singleton):
+class CatchpointMiddleware(Singleton):
     def __init__(self):
         self._wrapper = FlaskWrapper()
 
     def set_app(self, app):
         app.before_request(self.before_request)
         app.after_request(self.after_request)
         app.teardown_request(self.teardown_request)
 
     def before_request(self):
         try:
             from flask import request
-            setattr(request, '_thundra_wrapped', True)
+            setattr(request, '_catchpoint_wrapped', True)
             self._wrapper.before_request(request)
         except Exception as e:
-            logger.error("Error during the before part of Thundra: {}".format(e))
+            logger.error("Error during the before part of Catchpoint: {}".format(e))
 
     def after_request(self, response):
         try:
             self._wrapper.after_request(response)
         except Exception as e:
-            logger.error("Error setting response to context for Thundra: {}".format(e))
+            logger.error("Error setting response to context for Catchpoint: {}".format(e))
         return response
 
     def teardown_request(self, exception):
         try:
             self._wrapper.teardown_request(exception)
         except Exception as e:
-            logger.error("Error during the request teardown of Thundra: {}".format(e))
+            logger.error("Error during the request teardown of Catchpoint: {}".format(e))
```

### Comparing `thundra-3.0.6/thundra/wrappers/tornado/tornado_executor.py` & `thundra-3.0.7/catchpoint/wrappers/tornado/tornado_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from thundra import constants
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint import constants
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
 
 
 def start_trace(plugin_context, execution_context, tracer):
     request = execution_context.platform_data['request']
     request_route_path = str(request.path) if request.path else None
 
     _request = {
```

### Comparing `thundra-3.0.6/thundra/wrappers/tornado/tornado_wrapper.py` & `thundra-3.0.7/catchpoint/wrappers/tornado/tornado_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import traceback
 from functools import wraps
 
-from thundra import constants
-from thundra.application.global_application_info_provider import GlobalApplicationInfoProvider
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.context.execution_context_manager import ExecutionContextManager
-from thundra.context.plugin_context import PluginContext
-from thundra.context.tracing_execution_context_provider import TracingExecutionContextProvider
-from thundra.wrappers import wrapper_utils, web_wrapper_utils
-from thundra.wrappers.base_wrapper import BaseWrapper
-from thundra.wrappers.tornado import tornado_executor
+from catchpoint import constants
+from catchpoint.application.global_application_info_provider import GlobalApplicationInfoProvider
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.context.execution_context_manager import ExecutionContextManager
+from catchpoint.context.plugin_context import PluginContext
+from catchpoint.context.tracing_execution_context_provider import TracingExecutionContextProvider
+from catchpoint.wrappers import wrapper_utils, web_wrapper_utils
+from catchpoint.wrappers.base_wrapper import BaseWrapper
+from catchpoint.wrappers.tornado import tornado_executor
 
 logger = logging.getLogger(__name__)
 
 
 class TornadoWrapper(BaseWrapper):
 
     def __init__(self, api_key=None, disable_trace=False, disable_metric=True, disable_log=True, opts=None):
@@ -47,27 +47,27 @@
     def after_request(self, response, error=None):
         execution_context = ExecutionContextManager.get()
         execution_context.response = response
         execution_context.error = error
         self.prepare_and_send_reports_async(execution_context)
 
     def __call__(self, original_func):
-        if hasattr(original_func, "_thundra_wrapped") or ConfigProvider.get(config_names.THUNDRA_DISABLE, False):
+        if hasattr(original_func, "_catchpoint_wrapped") or ConfigProvider.get(config_names.CATCHPOINT_DISABLE, False):
             return original_func
 
         @wraps(original_func)
         def wrapper(request_handler, *args, **kwargs):
             request = request_handler.request
-            if getattr(request_handler, '_thundra_wrapped', False):
+            if getattr(request_handler, '_catchpoint_wrapped', False):
                 return original_func(request_handler, *args, **kwargs)
-            setattr(request_handler, '_thundra_wrapped', True)
+            setattr(request_handler, '_catchpoint_wrapped', True)
             try:
                 execution_context = self.before_request(request)
             except Exception as e:
-                logger.error("Error during the before part of Thundra: {}".format(e))
+                logger.error("Error during the before part of Catchpoint: {}".format(e))
                 return original_func(request_handler, *args, **kwargs)
 
             response = None
             # Invoke user handler
             try:
                 response = original_func(request_handler, *args, **kwargs)
             except Exception as e:
@@ -75,20 +75,20 @@
                     execution_context.error = {
                         'type': type(e).__name__,
                         'message': str(e),
                         'traceback': traceback.format_exc()
                     }
                     self.after_request(response)
                 except Exception as e_in:
-                    logger.error("Error during the after part of Thundra: {}".format(e_in))
+                    logger.error("Error during the after part of Catchpoint: {}".format(e_in))
                 raise e
 
             try:
                 self.after_request(response)
             except Exception as e:
-                logger.error("Error during the after part of Thundra: {}".format(e))
+                logger.error("Error during the after part of Catchpoint: {}".format(e))
             return response
 
-        setattr(wrapper, '_thundra_wrapped', True)
+        setattr(wrapper, '_catchpoint_wrapped', True)
         return wrapper
 
     call = __call__
```

### Comparing `thundra-3.0.6/thundra/wrappers/web_wrapper_utils.py` & `thundra-3.0.7/catchpoint/wrappers/web_wrapper_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import logging
 import uuid
 
 from opentracing import Format
 
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.plugins.invocation import invocation_support, invocation_trace_support
-from thundra.utils import get_normalized_path
-import thundra.wrappers.cp_wrapper_utils as cp_wrapper_utils
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.plugins.invocation import invocation_support, invocation_trace_support
+from catchpoint.utils import get_normalized_path
+import catchpoint.wrappers.cp_wrapper_utils as cp_wrapper_utils
 
 Logger = logging.getLogger(__name__)
 
 def start_trace(execution_context, tracer, class_name, domain_name, request, request_route_path=None):
     propagated_span_context = tracer.extract(Format.HTTP_HEADERS, request.get('headers'))
     trace_id = str(uuid.uuid4())
     incoming_span_id = None
     if propagated_span_context:
         trace_id = propagated_span_context.trace_id
         incoming_span_id = propagated_span_context.span_id
 
     # Start root span
-    url_path_depth = ConfigProvider.get(config_names.THUNDRA_TRACE_INTEGRATIONS_HTTP_URL_DEPTH)
+    url_path_depth = ConfigProvider.get(config_names.CATCHPOINT_TRACE_INTEGRATIONS_HTTP_URL_DEPTH)
     normalized_path = get_normalized_path(request.get('path'), url_path_depth)
     operation_name = request_route_path or normalized_path
     scope = tracer.start_active_span(operation_name=operation_name,
                                      child_of=propagated_span_context,
                                      start_time=execution_context.start_timestamp,
                                      finish_on_close=False,
                                      trace_id=trace_id,
@@ -40,15 +40,15 @@
     # Add root span tags
     execution_context.span_id = root_span.context.span_id
     root_span.on_started()
     root_span.set_tag(constants.HttpTags['HTTP_METHOD'], request.get('method'))
     root_span.set_tag(constants.HttpTags['HTTP_HOST'], request.get('host', ''))
     root_span.set_tag(constants.HttpTags['QUERY_PARAMS'], request.get('query_params'))
     root_span.set_tag(constants.HttpTags['HTTP_PATH'], request.get('path'))
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_REQUEST_SKIP, True):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_REQUEST_SKIP, True):
         root_span.set_tag(constants.HttpTags['BODY'], request.get('body'))
     execution_context.root_span = root_span
     execution_context.scope = scope
     execution_context.trace_id = trace_id
 
     if request_route_path:
         trigger_operation_name = request.get('host', '') + request_route_path
@@ -65,23 +65,23 @@
 
     if incoming_span_id:
         invocation_trace_support.add_incoming_trace_link(incoming_span_id)
 
 
 def update_application_info(application_info_provider, application_info, app_class_name):
     application_info_provider.update({
-        'applicationName': application_info.get('applicationName', 'thundra-app'),
+        'applicationName': application_info.get('applicationName', 'catchpoint-app'),
         'applicationClassName': app_class_name,
         'applicationDomainName': 'API',
         'applicationInstanceId': application_info.get('applicationInstanceId',
                                                       str(uuid.uuid4())),
         'applicationId': 'python:{}:{}:{}'.format(app_class_name,
                                                   application_info.get('applicationRegion', ''),
                                                   application_info.get('applicationName',
-                                                                       'thundra-app'))
+                                                                       'catchpoint-app'))
     })
 
 
 def process_request_route(execution_context, request_route_path, request_host):
     if request_route_path and execution_context and execution_context.scope:
         trigger_operation_name = request_host + request_route_path
         execution_context.scope.span.operation_name = request_route_path
```

### Comparing `thundra-3.0.6/thundra/wrappers/wrapper_utils.py` & `thundra-3.0.7/catchpoint/wrappers/wrapper_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import time
 import uuid
 
-from thundra import constants
-from thundra.config import config_names
-from thundra.config.config_provider import ConfigProvider
-from thundra.context.execution_context import ExecutionContext
-from thundra.plugins.invocation import invocation_trace_support
-from thundra.plugins.invocation.invocation_plugin import InvocationPlugin
-from thundra.plugins.log.log_plugin import LogPlugin
-from thundra.plugins.metric.metric_plugin import MetricPlugin
-from thundra.plugins.trace.trace_plugin import TracePlugin
+from catchpoint import constants
+from catchpoint.config import config_names
+from catchpoint.config.config_provider import ConfigProvider
+from catchpoint.context.execution_context import ExecutionContext
+from catchpoint.plugins.invocation import invocation_trace_support
+from catchpoint.plugins.invocation.invocation_plugin import InvocationPlugin
+from catchpoint.plugins.log.log_plugin import LogPlugin
+from catchpoint.plugins.metric.metric_plugin import MetricPlugin
+from catchpoint.plugins.trace.trace_plugin import TracePlugin
 
 
 def initialize_plugins(plugin_context, disable_trace, disable_metric, disable_log, config):
     plugins = []
-    if not ConfigProvider.get(config_names.THUNDRA_TRACE_DISABLE, disable_trace):
+    if not ConfigProvider.get(config_names.CATCHPOINT_TRACE_DISABLE, disable_trace):
         plugins.append(TracePlugin(plugin_context=plugin_context, config=config.trace_config))
     plugins.append(InvocationPlugin(plugin_context=plugin_context))
 
-    if not ConfigProvider.get(config_names.THUNDRA_METRIC_DISABLE, disable_metric):
+    if not ConfigProvider.get(config_names.CATCHPOINT_METRIC_DISABLE, disable_metric):
         plugins.append(MetricPlugin(plugin_context=plugin_context, config=config.metric_config))
 
-    if not ConfigProvider.get(config_names.THUNDRA_LOG_DISABLE, disable_log):
+    if not ConfigProvider.get(config_names.CATCHPOINT_LOG_DISABLE, disable_log):
         plugins.append(LogPlugin(plugin_context=plugin_context, config=config.log_config))
     return plugins
 
 
 def create_invocation_data(plugin_context, execution_context):
     if not execution_context.transaction_id:
         execution_context.transaction_id = str(uuid.uuid4())
     invocation_data = {
         'id': str(uuid.uuid4()),
         'type': "Invocation",
-        'agentVersion': constants.THUNDRA_AGENT_VERSION,
+        'agentVersion': constants.CATCHPOINT_AGENT_VERSION,
         'dataModelVersion': constants.DATA_FORMAT_VERSION,
         'traceId': execution_context.trace_id,
         'transactionId': execution_context.transaction_id,
         'spanId': execution_context.span_id,
         'applicationPlatform': '',
         'applicationRegion': plugin_context.application_info.get('applicationRegion'),
         'duration': None,
```

### Comparing `thundra-3.0.6/thundra.egg-info/PKG-INFO` & `thundra-3.0.7/thundra.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: thundra
-Version: 3.0.6
-Summary: Thundra Python agent
-Home-page: https://github.com/thundra-agent-python
-Author: Thundra
-Author-email: python@thundra.io
+Version: 3.0.7
+Summary: Catchpoint Python agent
+Home-page: https://github.com/cp-trace-python
+Author: Catchpoint
+Author-email: python@catchpoint.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 License-File: LICENSE
 
-Thundra Python agent
+Catchpoint Python agent
```

