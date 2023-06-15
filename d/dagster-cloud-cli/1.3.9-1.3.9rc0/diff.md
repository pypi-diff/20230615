# Comparing `tmp/dagster_cloud_cli-1.3.9.tar.gz` & `tmp/dagster_cloud_cli-1.3.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_cli-1.3.9.tar", last modified: Thu Jun  8 18:53:50 2023, max compression
+gzip compressed data, was "dagster_cloud_cli-1.3.9rc0.tar", last modified: Thu Jun  8 18:31:24 2023, max compression
```

## Comparing `dagster_cloud_cli-1.3.9.tar` & `dagster_cloud_cli-1.3.9rc0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.692650 dagster_cloud_cli-1.3.9/
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-08 18:53:50.692650 dagster_cloud_cli-1.3.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.684650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.684650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.684650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4612 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    26608 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4114 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     1508 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     2129 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18121 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    11997 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18291 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.688650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.692650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.692650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.692650 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9467 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13847 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     5384 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6700 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    18577 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.684650 dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-08 18:53:50.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2950 2023-06-08 18:53:50.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:53:50.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:53:50.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-08 18:53:50.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-08 18:53:50.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:50.692650 dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3745 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16129 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 18:53:50.692650 dagster_cloud_cli-1.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1101 2023-06-08 18:43:41.000000 dagster_cloud_cli-1.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.849262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.853262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.853262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    26608 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.861262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.861262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.861262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18121 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.865262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    11997 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18291 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.869262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.869262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.869262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.877262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13847 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6700 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    18577 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.853262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3745 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16129 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/setup.py
```

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/checks.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/report.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/ci/state.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/config.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/job/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/metrics.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/organization/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/run/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/config_utils.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/docker_runner.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/errors.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/graphql_client.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/headers/impl.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/source.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pex_builder/util.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/core/workspace.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/docker_utils.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/entrypoint.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/gql.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/pex_utils.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/types.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/ui.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli/utils.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_check.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_gql.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/dagster_cloud_cli_tests/test_metrics.py` & `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9/setup.py` & `dagster_cloud_cli-1.3.9rc0/setup.py`

 * *Files identical despite different names*

