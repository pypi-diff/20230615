# Comparing `tmp/exasol_integration_test_docker_environment-1.6.0.tar.gz` & `tmp/exasol_integration_test_docker_environment-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_integration_test_docker_environment-1.6.0.tar", max compression
+gzip compressed data, was "exasol_integration_test_docker_environment-1.7.0.tar", max compression
```

## Comparing `exasol_integration_test_docker_environment-1.6.0.tar` & `exasol_integration_test_docker_environment-1.7.0.tar`

### file list

```diff
@@ -1,234 +1,239 @@
--rw-r--r--   0        0        0     1063 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/LICENSE
--rw-r--r--   0        0        0      737 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/README.rst
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/__init__.py
--rw-r--r--   0        0        0       51 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/abstract_method_exception.py
--rw-r--r--   0        0        0      370 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/container/Dockerfile
--rw-r--r--   0        0        0     1254 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh
--rwxr-xr-x   0        0        0      570 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/__init__.py
--rw-r--r--   0        0        0      523 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/cli.py
--rw-r--r--   0        0        0       86 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/__init__.py
--rw-r--r--   0        0        0      744 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/health.py
--rw-r--r--   0        0        0     5323 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/__init__.py
--rw-r--r--   0        0        0     1655 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/build_options.py
--rw-r--r--   0        0        0     3106 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py
--rw-r--r--   0        0        0      376 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/push_options.py
--rw-r--r--   0        0        0     1660 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/system_options.py
--rw-r--r--   0        0        0     3086 2023-05-12 07:21:48.607348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py
--rw-r--r--   0        0        0     1970 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/termination_handler.py
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/init_db.sh
--rw-r--r--   0        0        0     6440 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/init_db.sh
--rw-r--r--   0        0        0     7182 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf
--rwxr-xr-x   0        0        0      318 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/init_db.sh
--rw-r--r--   0        0        0     2576 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/doctor.py
--rw-r--r--   0        0        0      165 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/__init__.py
--rw-r--r--   0        0        0      544 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/__init__.py
--rw-r--r--   0        0        0      500 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/api_errors.py
--rw-r--r--   0        0        0     3459 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py
--rw-r--r--   0        0        0    11718 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/common.py
--rw-r--r--   0        0        0     1328 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/health.py
--rw-r--r--   0        0        0     3567 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py
--rw-r--r--   0        0        0     6576 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py
--rw-r--r--   0        0        0     7081 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/__init__.py
--rw-r--r--   0        0        0      110 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/abstract_task_future.py
--rw-r--r--   0        0        0    16982 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/base_task.py
--rw-r--r--   0        0        0     4654 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py
--rw-r--r--   0        0        0      459 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/docker_base_task.py
--rw-r--r--   0        0        0      340 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/docker_parameter.py
--rw-r--r--   0        0        0     1516 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py
--rw-r--r--   0        0        0      325 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/frozendict_to_dict.py
--rw-r--r--   0        0        0     1007 2023-05-12 07:21:48.611348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/info.py
--rw-r--r--   0        0        0     1165 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py
--rw-r--r--   0        0        0      737 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py
--rw-r--r--   0        0        0     3405 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py
--rw-r--r--   0        0        0      495 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/pickle_target.py
--rw-r--r--   0        0        0     1261 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py
--rw-r--r--   0        0        0     3472 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py
--rw-r--r--   0        0        0     1775 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py
--rw-r--r--   0        0        0     1055 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py
--rw-r--r--   0        0        0      173 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_state.py
--rw-r--r--   0        0        0     4619 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py
--rw-r--r--   0        0        0      282 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/wrong_task_state_exception.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/__init__.py
--rw-r--r--   0        0        0      675 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/build_config.py
--rw-r--r--   0        0        0     1297 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/docker_config.py
--rw-r--r--   0        0        0      440 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/log_config.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/__init__.py
--rw-r--r--   0        0        0      656 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/container_info.py
--rw-r--r--   0        0        0      810 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py
--rw-r--r--   0        0        0      507 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/database_info.py
--rw-r--r--   0        0        0      330 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/docker_network_info.py
--rw-r--r--   0        0        0      508 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/docker_volume_info.py
--rw-r--r--   0        0        0      840 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/environment_info.py
--rw-r--r--   0        0        0       91 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/environment_type.py
--rw-r--r--   0        0        0     1773 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py
--rw-r--r--   0        0        0     1010 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/container/__init__.py
--rw-r--r--   0        0        0      492 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/container/utils.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/__init__.py
--rw-r--r--   0        0        0     2778 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/__init__.py
--rw-r--r--   0        0        0     6144 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py
--rw-r--r--   0        0        0    11405 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py
--rw-r--r--   0        0        0     2977 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py
--rw-r--r--   0        0        0     5074 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py
--rw-r--r--   0        0        0      724 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py
--rw-r--r--   0        0        0     1024 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py
--rw-r--r--   0        0        0     2916 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/__init__.py
--rw-r--r--   0        0        0     3306 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py
--rw-r--r--   0        0        0     3697 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py
--rw-r--r--   0        0        0     2323 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py
--rw-r--r--   0        0        0     1734 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py
--rw-r--r--   0        0        0      659 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py
--rw-r--r--   0        0        0     1846 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py
--rw-r--r--   0        0        0    11297 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py
--rw-r--r--   0        0        0     2224 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py
--rw-r--r--   0        0        0      861 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py
--rw-r--r--   0        0        0     4017 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/__init__.py
--rw-r--r--   0        0        0     2683 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py
--rw-r--r--   0        0        0     1334 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py
--rw-r--r--   0        0        0      160 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_push_parameter.py
--rw-r--r--   0        0        0     2107 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py
--rw-r--r--   0        0        0      800 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py
--rw-r--r--   0        0        0      426 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/required_task_info.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/__init__.py
--rw-r--r--   0        0        0     3106 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py
--rw-r--r--   0        0        0     1335 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py
--rw-r--r--   0        0        0      815 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py
--rw-r--r--   0        0        0     1998 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py
--rw-r--r--   0        0        0      371 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/utils.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/networks/__init__.py
--rw-r--r--   0        0        0      478 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/networks/utils.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/volumes/__init__.py
--rw-r--r--   0        0        0      473 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/volumes/utils.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/__init__.py
--rw-r--r--   0        0        0     1111 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py
--rw-r--r--   0        0        0     1587 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py
--rw-r--r--   0        0        0      911 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/__init__.py
--rw-r--r--   0        0        0    13026 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py
--rw-r--r--   0        0        0     3571 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/__init__.py
--rw-r--r--   0        0        0     3485 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py
--rw-r--r--   0        0        0     6359 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/__init__.py
--rw-r--r--   0        0        0      283 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/bucketfs_sync_checker.py
--rw-r--r--   0        0        0     2274 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py
--rw-r--r--   0        0        0      938 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py
--rw-r--r--   0        0        0     2560 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py
--rw-r--r--   0        0        0      443 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/time_based_bucketfs_sync_waiter.py
--rw-r--r--   0        0        0     8069 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/__init__.py
--rw-r--r--   0        0        0     2186 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py
--rw-r--r--   0        0        0     3021 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py
--rw-r--r--   0        0        0     1128 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py
--rw-r--r--   0        0        0     6010 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py
--rw-r--r--   0        0        0     1627 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py
--rw-r--r--   0        0        0     1787 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/__init__.py
--rw-r--r--   0        0        0      794 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py
--rw-r--r--   0        0        0     1364 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py
--rw-r--r--   0        0        0      831 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py
--rw-r--r--   0        0        0      894 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py
--rw-r--r--   0        0        0      771 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py
--rw-r--r--   0        0        0     4769 2023-05-12 07:21:48.615348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py
--rw-r--r--   0        0        0     5045 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py
--rw-r--r--   0        0        0    10576 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py
--rw-r--r--   0        0        0    15657 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py
--rw-r--r--   0        0        0     2628 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py
--rw-r--r--   0        0        0     4888 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py
--rw-r--r--   0        0        0     2905 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/utils/__init__.py
--rw-r--r--   0        0        0     3362 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py
--rwxr-xr-x   0        0        0      347 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/main.py
--rw-r--r--   0        0        0      774 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/templates/luigi_log.conf
--rw-r--r--   0        0        0        0 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/__init__.py
--rw-r--r--   0        0        0     2445 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py
--rw-r--r--   0        0        0     4600 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_test_environment.py
--rw-r--r--   0        0        0     2691 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/docker_registry.py
--rw-r--r--   0        0        0     1407 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py
--rw-r--r--   0        0        0     8830 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py
--rw-r--r--   0        0        0      559 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/luigi_utils.py
--rw-r--r--   0        0        0      824 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py
--rw-r--r--   0        0        0     1988 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/utils.py
--rw-r--r--   0        0        0      331 2023-05-12 07:21:48.619348 exasol_integration_test_docker_environment-1.6.0/ext/01_nodoc
--rw-r--r--   0        0        0     1815 2023-05-12 07:21:48.623348 exasol_integration_test_docker_environment-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     6147 2023-05-12 07:21:48.623348 exasol_integration_test_docker_environment-1.6.0/pytest_itde/__init__.py
--rw-r--r--   0        0        0     3335 2023-05-12 07:21:48.623348 exasol_integration_test_docker_environment-1.6.0/pytest_itde/config.py
--rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 exasol_integration_test_docker_environment-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/LICENSE
+-rw-r--r--   0        0        0      737 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/README.rst
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/abstract_method_exception.py
+-rw-r--r--   0        0        0      370 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/certificate_resources/container/Dockerfile
+-rw-r--r--   0        0        0     1254 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh
+-rwxr-xr-x   0        0        0      570 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/cli.py
+-rw-r--r--   0        0        0       86 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/commands/__init__.py
+-rw-r--r--   0        0        0      744 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/commands/health.py
+-rw-r--r--   0        0        0     5391 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/__init__.py
+-rw-r--r--   0        0        0     1655 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/build_options.py
+-rw-r--r--   0        0        0     3106 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py
+-rw-r--r--   0        0        0      376 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/push_options.py
+-rw-r--r--   0        0        0     1660 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/system_options.py
+-rw-r--r--   0        0        0     3634 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py
+-rw-r--r--   0        0        0     1871 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/termination_handler.py
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.022356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/init_db.sh
+-rw-r--r--   0        0        0     6440 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/init_db.sh
+-rw-r--r--   0        0        0     7182 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/init_db.sh
+-rw-r--r--   0        0        0     8025 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/8.17.0/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/8.17.0/init_db.sh
+-rw-r--r--   0        0        0     8025 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/8.18.1/EXAConf
+-rwxr-xr-x   0        0        0      318 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/8.18.1/init_db.sh
+-rw-r--r--   0        0        0     2576 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/doctor.py
+-rw-r--r--   0        0        0      165 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/__init__.py
+-rw-r--r--   0        0        0      544 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/api_errors.py
+-rw-r--r--   0        0        0     3459 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py
+-rw-r--r--   0        0        0    11905 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/common.py
+-rw-r--r--   0        0        0     1328 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/health.py
+-rw-r--r--   0        0        0     3567 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py
+-rw-r--r--   0        0        0     6881 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py
+-rw-r--r--   0        0        0     7357 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/__init__.py
+-rw-r--r--   0        0        0      110 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/abstract_task_future.py
+-rw-r--r--   0        0        0    16982 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/base_task.py
+-rw-r--r--   0        0        0     4654 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py
+-rw-r--r--   0        0        0      459 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/docker_base_task.py
+-rw-r--r--   0        0        0      340 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/docker_parameter.py
+-rw-r--r--   0        0        0     1516 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py
+-rw-r--r--   0        0        0      325 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/frozendict_to_dict.py
+-rw-r--r--   0        0        0     1007 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/info.py
+-rw-r--r--   0        0        0     1165 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py
+-rw-r--r--   0        0        0      737 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py
+-rw-r--r--   0        0        0     3405 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py
+-rw-r--r--   0        0        0      495 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/pickle_target.py
+-rw-r--r--   0        0        0     3741 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/ssh_access.py
+-rw-r--r--   0        0        0     1261 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py
+-rw-r--r--   0        0        0     3362 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py
+-rw-r--r--   0        0        0     1775 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py
+-rw-r--r--   0        0        0     1055 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py
+-rw-r--r--   0        0        0      173 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/task_state.py
+-rw-r--r--   0        0        0     4619 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py
+-rw-r--r--   0        0        0      282 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/wrong_task_state_exception.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/config/__init__.py
+-rw-r--r--   0        0        0      675 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/config/build_config.py
+-rw-r--r--   0        0        0     1297 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/config/docker_config.py
+-rw-r--r--   0        0        0      440 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/config/log_config.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/__init__.py
+-rw-r--r--   0        0        0      656 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/container_info.py
+-rw-r--r--   0        0        0      810 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py
+-rw-r--r--   0        0        0      507 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/database_info.py
+-rw-r--r--   0        0        0      330 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/docker_network_info.py
+-rw-r--r--   0        0        0      508 2023-06-15 13:18:10.026356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/docker_volume_info.py
+-rw-r--r--   0        0        0      840 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/environment_info.py
+-rw-r--r--   0        0        0       91 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/environment_type.py
+-rw-r--r--   0        0        0     1773 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py
+-rw-r--r--   0        0        0     1010 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/container/__init__.py
+-rw-r--r--   0        0        0      492 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/container/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/__init__.py
+-rw-r--r--   0        0        0     2778 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/__init__.py
+-rw-r--r--   0        0        0     6144 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py
+-rw-r--r--   0        0        0    11405 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py
+-rw-r--r--   0        0        0     2977 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py
+-rw-r--r--   0        0        0     5074 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py
+-rw-r--r--   0        0        0      724 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py
+-rw-r--r--   0        0        0     1024 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py
+-rw-r--r--   0        0        0     2916 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/__init__.py
+-rw-r--r--   0        0        0     3306 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py
+-rw-r--r--   0        0        0     3697 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py
+-rw-r--r--   0        0        0     2323 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py
+-rw-r--r--   0        0        0     1734 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py
+-rw-r--r--   0        0        0      659 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py
+-rw-r--r--   0        0        0     1846 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py
+-rw-r--r--   0        0        0    11297 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py
+-rw-r--r--   0        0        0     2224 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py
+-rw-r--r--   0        0        0      861 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py
+-rw-r--r--   0        0        0     4017 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/__init__.py
+-rw-r--r--   0        0        0     2683 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py
+-rw-r--r--   0        0        0     1334 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py
+-rw-r--r--   0        0        0      160 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_push_parameter.py
+-rw-r--r--   0        0        0     2107 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py
+-rw-r--r--   0        0        0      800 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py
+-rw-r--r--   0        0        0      426 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/required_task_info.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/save/__init__.py
+-rw-r--r--   0        0        0     3106 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py
+-rw-r--r--   0        0        0     1335 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py
+-rw-r--r--   0        0        0      815 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py
+-rw-r--r--   0        0        0     1998 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py
+-rw-r--r--   0        0        0      371 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/networks/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/networks/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/volumes/__init__.py
+-rw-r--r--   0        0        0      473 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/volumes/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/logging/__init__.py
+-rw-r--r--   0        0        0     1111 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py
+-rw-r--r--   0        0        0     1587 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py
+-rw-r--r--   0        0        0      911 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/__init__.py
+-rw-r--r--   0        0        0    13026 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py
+-rw-r--r--   0        0        0     3571 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/__init__.py
+-rw-r--r--   0        0        0     3485 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py
+-rw-r--r--   0        0        0     6359 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/bucketfs_sync_checker.py
+-rw-r--r--   0        0        0     2274 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py
+-rw-r--r--   0        0        0     1243 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py
+-rw-r--r--   0        0        0     2560 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py
+-rw-r--r--   0        0        0      443 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/time_based_bucketfs_sync_waiter.py
+-rw-r--r--   0        0        0     8069 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/__init__.py
+-rw-r--r--   0        0        0     2186 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py
+-rw-r--r--   0        0        0     3021 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py
+-rw-r--r--   0        0        0     1128 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py
+-rw-r--r--   0        0        0     6010 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py
+-rw-r--r--   0        0        0     1737 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py
+-rw-r--r--   0        0        0     1787 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/docker_db_test_environment_parameter.py
+-rw-r--r--   0        0        0     1364 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py
+-rw-r--r--   0        0        0      831 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py
+-rw-r--r--   0        0        0      894 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py
+-rw-r--r--   0        0        0      771 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py
+-rw-r--r--   0        0        0     4769 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py
+-rw-r--r--   0        0        0     5045 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py
+-rw-r--r--   0        0        0    10576 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py
+-rw-r--r--   0        0        0    15736 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py
+-rw-r--r--   0        0        0     2628 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py
+-rw-r--r--   0        0        0     4888 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py
+-rw-r--r--   0        0        0     2905 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/utils/__init__.py
+-rw-r--r--   0        0        0     3362 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py
+-rwxr-xr-x   0        0        0      347 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/main.py
+-rw-r--r--   0        0        0      774 2023-06-15 13:18:10.030356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/templates/luigi_log.conf
+-rw-r--r--   0        0        0        0 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/__init__.py
+-rw-r--r--   0        0        0     2445 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py
+-rw-r--r--   0        0        0     4408 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/api_test_environment.py
+-rw-r--r--   0        0        0     2691 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/docker_registry.py
+-rw-r--r--   0        0        0     1407 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py
+-rw-r--r--   0        0        0     8911 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py
+-rw-r--r--   0        0        0      559 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/luigi_utils.py
+-rw-r--r--   0        0        0      824 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py
+-rw-r--r--   0        0        0     1988 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/utils.py
+-rw-r--r--   0        0        0      331 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/ext/01_nodoc
+-rw-r--r--   0        0        0     1796 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6147 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/pytest_itde/__init__.py
+-rw-r--r--   0        0        0     3335 2023-06-15 13:18:10.034356 exasol_integration_test_docker_environment-1.7.0/pytest_itde/config.py
+-rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 exasol_integration_test_docker_environment-1.7.0/PKG-INFO
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/LICENSE` & `exasol_integration_test_docker_environment-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/README.rst` & `exasol_integration_test_docker_environment-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/certificate_resources/container/create_certificates.sh`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/certificate_resources/install_root_certificate.sh`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/cli.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 
     Examples:
 
         Check the health of the execution environment:
 
             $ itde health
 
-        Spawn a itde test environment:
+        Spawn an ITDE test environment:
 
             $ itde spawn-test-environment --environment-name test \\
             --database-port-forward 8888 --bucketfs-port-forward 6666 \\
             --docker-db-image-version 7.1.9 --db-mem-size 4GB
     """
     pass
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/health.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/commands/health.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/commands/spawn_test_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         bucketfs_port_forward: Optional[int],
         db_mem_size: str,
         db_disk_size: str,
         nameserver: Tuple[str, ...],
         docker_runtime: Optional[str],
         docker_db_image_version: str,
         docker_db_image_name: str,
+        db_os_access: Optional[str],
         create_certificates: bool,
         additional_db_parameter: Tuple[str, ...],
         source_docker_repository_name: str,
         source_docker_tag_prefix: str,
         source_docker_username: Optional[str],
         source_docker_password: Optional[str],
         target_docker_repository_name: str,
@@ -103,29 +104,30 @@
         temporary_base_directory: str,
         workers: int,
         task_dependencies_dot_file: Optional[str],
         log_level: Optional[str],
         use_job_specific_log_file: bool
 ):
     """
-    This command spawn a test environment with a docker-db container and a connected test-container.
+    This command spawns a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     """
     with TerminationHandler():
         try:
             api.spawn_test_environment(
                 environment_name,
                 database_port_forward,
                 bucketfs_port_forward,
                 db_mem_size,
                 db_disk_size,
                 nameserver,
                 docker_runtime,
                 docker_db_image_version,
                 docker_db_image_name,
+                db_os_access,
                 create_certificates,
                 additional_db_parameter,
                 source_docker_repository_name,
                 source_docker_tag_prefix,
                 source_docker_username,
                 source_docker_password,
                 target_docker_repository_name,
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/build_options.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/build_options.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/docker_repository_options.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/system_options.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/system_options.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/options/test_environment_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import click
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.parameter \
+    .docker_db_test_environment_parameter \
+    import DbOsAccess
 
 test_environment_options = [
     click.option('--environment-type', type=click.Choice(['docker_db', 'external_db']), default="""docker_db""",
                  show_default=True,
                  help="""Environment type for tests."""),
     click.option('--max_start_attempts', type=int, default=2,
                  show_default=True,
                  help="""Maximum start attempts for environment""")
 
 ]
 
-LATEST_DB_VERSION = """7.1.17"""
+LATEST_DB_VERSION = """8.18.1"""
 
 docker_db_options = [
     click.option('--docker-db-image-version', type=str, default=LATEST_DB_VERSION,
                  show_default=True,
                  help="""Docker DB Image Version against which the tests should run."""),
     click.option('--docker-db-image-name', type=str, default="""exasol/docker-db""",
                  show_default=True,
                  help="""Docker DB Image Name against which the tests should run."""),
+    click.option('--db-os-access', type=click.Choice([e.name for e in DbOsAccess]),
+                 metavar="METHOD", default="""DOCKER_EXEC""", show_default=True,
+                 help="""How to access file system and command line of the
+     		 database operating system. Experimental option, will show no
+     		 effect until implementation of feature SSH access is
+     		 completed."""),
     click.option('--create-certificates/--no-create-certificates', default=False,
                  help="""Creates and injects SSL certificates to the Docker DB container."""),
     click.option('--additional-db-parameter', '-p', type=str, multiple=True,
                  help="""Additional database parameter which will be injected to EXAConf. Value should have format '-param=value'.""")
 ]
 
 external_db_options = [
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/cli/termination_handler.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/cli/termination_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import sys
 from datetime import datetime
-from sys import stderr
 from traceback import print_tb
 
 from exasol_integration_test_docker_environment.lib.api.api_errors import TaskRuntimeError
 
 
+def print_err(*args, **kwargs):
+    kwargs["file"] = sys.stderr
+    print(*args, **kwargs)
+
+
 class TerminationHandler:
     """
     This helper class measures and logs time duration of the job and also logs the error message.
     """
+
     def __init__(self):
         self._start_time = None
 
     def __enter__(self):
         self._start_time = datetime.now()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -26,30 +31,26 @@
         else:
             self._handle_unexpected_failure(exc_val, exc_tb)
             exit_value = 1
         sys.exit(exit_value)
 
     def _handle_unexpected_failure(self, exc_val, exc_tb):
         timedelta = datetime.now() - self._start_time
-        print("The command failed after %s s with:" % timedelta.total_seconds(), file=stderr)
-        print("Caught exception:%s" % exc_val, file=stderr)
-        print_tb(exc_tb)
+        print_err("The command failed after %s s with:" % timedelta.total_seconds())
+        print_err("Caught exception:%s" % exc_val)
+        print_tb(exc_tb, file=sys.stderr)
 
     def _handle_failure(self, task_error: TaskRuntimeError):
         timedelta = datetime.now() - self._start_time
-        print("The command failed after %s s with:" % timedelta.total_seconds(), file=stderr)
+        print_err("The command failed after %s s with:" % timedelta.total_seconds())
         self._print_task_failures(task_error)
 
     @staticmethod
     def _print_task_failures(task_error: TaskRuntimeError):
-        print(file=stderr)
-        print("Task failure message: %s" % task_error.msg, file=stderr)
-        print("Task Failures:", file=stderr)
-        if task_error.inner is not None:
-            for failure in task_error.inner:
-                print(failure, file=stderr)
-        print(file=stderr)
+        print_err()
+        print_err("Task failure message: %s" % task_error.msg)
+        print_err(task_error.__cause__.args[0])
+        print_err()
 
     def _handle_success(self):
         timedelta = datetime.now() - self._start_time
-        print("The command took %s s" % timedelta.total_seconds(), file=stderr)
-
+        print_err("The command took %s s" % timedelta.total_seconds())
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.0/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.1/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.10/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.11/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.12/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.13/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.14/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.15/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.16/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.17/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.18/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.19/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.2/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.20/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.3/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.4/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.6/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.7/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.8/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.0.9/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.0/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.1/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.10/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.11/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.12/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.13/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.14/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.15/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.16/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.17/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.2/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.3/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.4/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.5/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.6/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.7/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.8/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/docker_db_config/7.1.9/EXAConf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/doctor.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/doctor.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/__init__.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/build_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/common.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import warnings
 from datetime import datetime
 from pathlib import Path
 from typing import (
     Callable,
     Tuple,
     Set,
-    Optional, Any, Dict, Iterator
+    Optional, Any, Dict, Iterator, Iterable, List
 )
 
 import luigi
 import networkx
 from luigi.parameter import UnconsumedParameterWarning
 from luigi.setup_logging import InterfaceLogging
 from networkx import DiGraph
 
 from exasol_integration_test_docker_environment.lib import extract_modulename_for_build_steps
-from exasol_integration_test_docker_environment.lib.api.api_errors import TaskRuntimeError
+from exasol_integration_test_docker_environment.lib.api.api_errors import TaskRuntimeError, TaskFailures
 from exasol_integration_test_docker_environment.lib.base.dependency_logger_base_task import DependencyLoggerBaseTask
 from exasol_integration_test_docker_environment.lib.base.luigi_log_config import get_luigi_log_config, get_log_path
 from exasol_integration_test_docker_environment.lib.base.task_dependency import TaskDependency, DependencyState
 
 
 class JobCounterSingleton(object):
     """
@@ -150,22 +150,29 @@
         workers: int) -> bool:
     with _configure_logging(log_file_path, log_level, use_job_specific_log_file) as run_kwargs:
         no_scheduling_errors = luigi.build([task], workers=workers,
                                            local_scheduler=True, **run_kwargs)
         return no_scheduling_errors
 
 
-def _handle_task_result(no_scheduling_errors, success, task, task_dependencies_dot_file: Optional[str]) -> Any:
+def _handle_task_result(
+        no_scheduling_errors: bool,
+        success: bool,
+        task: DependencyLoggerBaseTask,
+        task_dependencies_dot_file: Optional[str]) -> Any:
     generate_graph_from_task_dependencies(task, task_dependencies_dot_file)
     if success:
         return task.get_result()
     elif task.failed_target.exists():
         logging.error(f"Task {task} failed. failed target exists.")
-        raise TaskRuntimeError(msg=f"Task {task} (or any of it's subtasks) failed.",
-                               inner=list(task.collect_failures().keys()))
+        task_failures = list(task.collect_failures().keys())
+        raise TaskRuntimeError(
+            msg=f"Task {task} (or any of it's subtasks) failed.",
+            inner=task_failures) \
+            from TaskFailures(inner=task_failures)
     elif not no_scheduling_errors:
         logging.error(f"Task {task} failed. : luigi reported a scheduling error.")
         raise TaskRuntimeError(msg=f"Task {task} failed. reason: luigi reported a scheduling error.")
 
 
 @contextlib.contextmanager
 def _configure_logging(
@@ -198,14 +205,15 @@
         no_configure_logging = False
         run_kwargs = {"logging_conf_file": f'{luigi_config}'}
     else:
         no_configure_logging = True
         run_kwargs = {}
     return no_configure_logging, run_kwargs
 
+
 def generate_graph_from_task_dependencies(task: DependencyLoggerBaseTask, task_dependencies_dot_file: Optional[str]):
     if task_dependencies_dot_file is not None:
         print(f"Generate Task Dependency Graph to {task_dependencies_dot_file}")
         print()
         dependencies = collect_dependencies(task)
         g = DiGraph()
         for dependency in dependencies:
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/health.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/health.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/push_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 import functools
 from typing import Tuple, Optional, Callable
 import humanfriendly
 
 from exasol_integration_test_docker_environment.lib.api.common import set_build_config, set_docker_repository_config, \
-    run_task, generate_root_task, cli_function
+    run_task, generate_root_task, no_cli_function
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import \
     DEFAULT_DOCKER_REPOSITORY_NAME
 from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import LATEST_DB_VERSION
 from exasol_integration_test_docker_environment.lib.api.api_errors import ArgumentConstraintError
 from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
+from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
+    TestContainerContentDescription
 from exasol_integration_test_docker_environment.lib.docker.container.utils import remove_docker_container
 from exasol_integration_test_docker_environment.lib.docker.volumes.utils import remove_docker_volumes
 from exasol_integration_test_docker_environment.lib.docker.networks.utils import remove_docker_networks
 from exasol_integration_test_docker_environment.lib.test_environment.spawn_test_environment_with_docker_db import \
     SpawnTestEnvironmentWithDockerDB
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.parameter \
+    .docker_db_test_environment_parameter import DbOsAccess
 
 
 def _cleanup(environment_info: EnvironmentInfo) -> None:
-    remove_docker_container([environment_info.database_info.container_info.container_name])
+    if environment_info.test_container_info is None:
+        remove_docker_container([environment_info.database_info.container_info.container_name])
+    else:
+        remove_docker_container([environment_info.test_container_info.container_name,
+                                 environment_info.database_info.container_info.container_name])
     remove_docker_volumes([environment_info.database_info.container_info.volume_name])
     remove_docker_networks([environment_info.network_info.network_name])
 
 
-@cli_function
-def spawn_test_environment(
+@no_cli_function
+def spawn_test_environment_with_test_container(
         environment_name: str,
+        test_container_content: TestContainerContentDescription,
         database_port_forward: Optional[int] = None,
         bucketfs_port_forward: Optional[int] = None,
         db_mem_size: str = "2 GiB",
         db_disk_size: str = "2 GiB",
         nameserver: Tuple[str, ...] = tuple(),
         docker_runtime: Optional[str] = None,
         docker_db_image_version: str = LATEST_DB_VERSION,
         docker_db_image_name: str = "exasol/docker-db",
+        db_os_access: str = "DOCKER_EXEC",
         create_certificates: bool = False,
         additional_db_parameter: Tuple[str, ...] = tuple(),
         source_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
         source_docker_tag_prefix: str = '',
         source_docker_username: Optional[str] = None,
         source_docker_password: Optional[str] = None,
         target_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
@@ -46,15 +57,16 @@
         target_docker_password: Optional[str] = None,
         output_directory: str = DEFAULT_OUTPUT_DIRECTORY,
         temporary_base_directory: str = "/tmp",
         workers: int = 5,
         task_dependencies_dot_file: Optional[str] = None,
         log_level: Optional[str] = None,
         use_job_specific_log_file: bool = False
-) -> Tuple[EnvironmentInfo, Callable[[], None]]:
+) \
+        -> Tuple[EnvironmentInfo, Callable[[], None]]:
     """
     This function spawns a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     The function returns an environment_info object, describing the environment, and a cleanup-method, which
     can be used to stop the environment.
     raises: TaskRuntimeError if spawning the test environment fails
 
@@ -85,22 +97,23 @@
                                                   bucketfs_port_forward) if bucketfs_port_forward is not None else None,
                                               mem_size=db_mem_size,
                                               disk_size=db_disk_size,
                                               nameservers=nameserver,
                                               docker_runtime=docker_runtime,
                                               docker_db_image_version=docker_db_image_version,
                                               docker_db_image_name=docker_db_image_name,
+                                              db_os_access=DbOsAccess[db_os_access],
                                               db_user="sys",
                                               db_password="exasol",
                                               bucketfs_write_password="write",
                                               no_test_container_cleanup_after_success=True,
                                               no_test_container_cleanup_after_failure=False,
                                               no_database_cleanup_after_success=True,
                                               no_database_cleanup_after_failure=False,
                                               create_certificates=create_certificates,
-                                              test_container_content=None,
+                                              test_container_content=test_container_content,
                                               additional_db_parameter=additional_db_parameter
                                               )
     environment_info = run_task(task_creator, workers, task_dependencies_dot_file,
                                 log_level=log_level,
                                 use_job_specific_log_file=use_job_specific_log_file)
     return environment_info, functools.partial(_cleanup, environment_info)
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment_with_test_container.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/api/spawn_test_environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import functools
 from typing import Tuple, Optional, Callable
 import humanfriendly
 
-from exasol_integration_test_docker_environment.lib.api.common import set_build_config, set_docker_repository_config, \
-    run_task, generate_root_task, no_cli_function
+from exasol_integration_test_docker_environment.lib.api.common import (
+    set_build_config,
+    set_docker_repository_config,
+    run_task,
+    generate_root_task,
+    cli_function,
+)
 from exasol_integration_test_docker_environment.cli.options.docker_repository_options import \
     DEFAULT_DOCKER_REPOSITORY_NAME
 from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import LATEST_DB_VERSION
 from exasol_integration_test_docker_environment.lib.api.api_errors import ArgumentConstraintError
 from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
-from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
-    TestContainerContentDescription
 from exasol_integration_test_docker_environment.lib.docker.container.utils import remove_docker_container
 from exasol_integration_test_docker_environment.lib.docker.volumes.utils import remove_docker_volumes
 from exasol_integration_test_docker_environment.lib.docker.networks.utils import remove_docker_networks
 from exasol_integration_test_docker_environment.lib.test_environment.spawn_test_environment_with_docker_db import \
     SpawnTestEnvironmentWithDockerDB
+from exasol_integration_test_docker_environment \
+    .lib.test_environment.parameter \
+    .docker_db_test_environment_parameter import DbOsAccess
 
 
 def _cleanup(environment_info: EnvironmentInfo) -> None:
-    if environment_info.test_container_info is None:
-        remove_docker_container([environment_info.database_info.container_info.container_name])
-    else:
-        remove_docker_container([environment_info.test_container_info.container_name,
-                                 environment_info.database_info.container_info.container_name])
+    remove_docker_container([environment_info.database_info.container_info.container_name])
     remove_docker_volumes([environment_info.database_info.container_info.volume_name])
     remove_docker_networks([environment_info.network_info.network_name])
 
 
-@no_cli_function
-def spawn_test_environment_with_test_container(
+@cli_function
+def spawn_test_environment(
         environment_name: str,
-        test_container_content: TestContainerContentDescription,
         database_port_forward: Optional[int] = None,
         bucketfs_port_forward: Optional[int] = None,
         db_mem_size: str = "2 GiB",
         db_disk_size: str = "2 GiB",
         nameserver: Tuple[str, ...] = tuple(),
         docker_runtime: Optional[str] = None,
         docker_db_image_version: str = LATEST_DB_VERSION,
         docker_db_image_name: str = "exasol/docker-db",
+        db_os_access: Optional[str] = "DOCKER_EXEC",
         create_certificates: bool = False,
         additional_db_parameter: Tuple[str, ...] = tuple(),
         source_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
         source_docker_tag_prefix: str = '',
         source_docker_username: Optional[str] = None,
         source_docker_password: Optional[str] = None,
         target_docker_repository_name: str = DEFAULT_DOCKER_REPOSITORY_NAME,
@@ -53,16 +55,15 @@
         target_docker_password: Optional[str] = None,
         output_directory: str = DEFAULT_OUTPUT_DIRECTORY,
         temporary_base_directory: str = "/tmp",
         workers: int = 5,
         task_dependencies_dot_file: Optional[str] = None,
         log_level: Optional[str] = None,
         use_job_specific_log_file: bool = False
-) \
-        -> Tuple[EnvironmentInfo, Callable[[], None]]:
+) -> Tuple[EnvironmentInfo, Callable[[], None]]:
     """
     This function spawns a test environment with a docker-db container and a connected test-container.
     The test-container is reachable by the database for output redirects of UDFs.
     The function returns an environment_info object, describing the environment, and a cleanup-method, which
     can be used to stop the environment.
     raises: TaskRuntimeError if spawning the test environment fails
 
@@ -93,22 +94,23 @@
                                                   bucketfs_port_forward) if bucketfs_port_forward is not None else None,
                                               mem_size=db_mem_size,
                                               disk_size=db_disk_size,
                                               nameservers=nameserver,
                                               docker_runtime=docker_runtime,
                                               docker_db_image_version=docker_db_image_version,
                                               docker_db_image_name=docker_db_image_name,
+                                              db_os_access=DbOsAccess[db_os_access],
                                               db_user="sys",
                                               db_password="exasol",
                                               bucketfs_write_password="write",
                                               no_test_container_cleanup_after_success=True,
                                               no_test_container_cleanup_after_failure=False,
                                               no_database_cleanup_after_success=True,
                                               no_database_cleanup_after_failure=False,
                                               create_certificates=create_certificates,
-                                              test_container_content=test_container_content,
+                                              test_container_content=None,
                                               additional_db_parameter=additional_db_parameter
                                               )
     environment_info = run_task(task_creator, workers, task_dependencies_dot_file,
                                 log_level=log_level,
                                 use_job_specific_log_file=use_job_specific_log_file)
     return environment_info, functools.partial(_cleanup, environment_info)
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/base_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/dependency_logger_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/flavor_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/info.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/json_pickle_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/json_pickle_target.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/luigi_log_config.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/still_running_logger.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/stoppable_base_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,29 @@
             with self.failed_target.open("r") as f:
                 failed_task = f.read()
             self.logger.error("Task %s failed. Stopping further execution." % failed_task)
             raise StoppingFurtherExecution("Task %s failed. Stopping further execution." % failed_task)
 
     def handle_failure(self, exception, exception_tb):
         if not isinstance(exception, StoppingFurtherExecution):
-            #            self.logger.error("Task %s failed. Got %s(%s).",self.task_id, type(exception), str(exception))
             with self.get_failure_log_path().open("w") as f:
                 f.write("%s" % exception_tb)
             if not self.failed_target.exists():
                 with self.failed_target.open("w") as f:
                     f.write("%s" % self.task_id)
 
     def collect_failures(self) -> Dict[str,None]:
         failures = OrderedDict()
         failures.update(self.collect_failures_of_child_tasks())
         if self.get_failure_log_path().exists():
             with self.get_failure_log_path().open("r") as f:
-                exception = f.read()
+                exception = f.read().strip()
                 prefix = '    '
-                formated_exception = prefix + prefix.join(exception.splitlines(True))
-                failure_message = "- %s:\n%s" % (self.task_id, formated_exception)
+                formatted_exception = prefix + prefix.join(exception.splitlines(True))
+                failure_message = "- %s:\n%s" % (self.task_id, formatted_exception)
                 failures[failure_message] = None
 
         return failures
 
     def collect_failures_of_child_tasks(self) -> Dict[str,None]:
         failures_of_child_tasks = OrderedDict()
         if self._run_dependencies_target.exists():
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/task_dependency.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/task_logger_wrapper.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/base/timeable_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/build_config.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/config/build_config.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/config/docker_config.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/config/docker_config.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/container_info.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/container_info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/database_credentials.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/environment_info.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/environment_info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/data/test_container_content_description.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/__init__.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/clean/clean_images.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_build_base.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_analyze_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_build_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_create_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_creator_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_load_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/docker_image_pull_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_creator.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_context_hasher.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/build_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/character_length_checker.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_image_target.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/docker_registry_image_checker.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/file_directory_list_hasher.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/pull_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/create/utils/symlink_loop_checker.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/image_info.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/docker_image_push_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/push/push_task_creator_for_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/save/docker_image_save_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/save/save_task_creator_for_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/docker/images/task_creator_from_build_tasks.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/logging/abstract_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/logging/command_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/logging/container_log_handler.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/abstract_spawn_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/analyze_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/analyze_certificate_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/create_certificates/create_ssl_certificates_task.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/docker_db_log_based_bucket_sync_checker.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/find_exaplus_in_db_container.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 
 def find_exaplus(db_container: docker.models.containers.Container) -> PurePath:
     """
     Tries to find path of exaplus in given container in directories where exaplus is normally installed.
     :db_container Container where to search for exaplus
     """
-    exit, output = db_container.exec_run(cmd="find /usr/opt /opt  -name 'exaplus' -type f")
+    exit, output = db_container.exec_run(cmd="find /usr/opt -name 'exaplus' -type f")
+    if exit != 0 or output == b"":
+        # Using /usr/opt and /opt together in one command doesn't work, because in Exasol 8, /usr/opt doesn't exist
+        # and as such the command fails, even if it finds exaplus in /opt
+        exit, output = db_container.exec_run(cmd="find /opt -name 'exaplus' -type f")
     if exit != 0:
         raise RuntimeError(f"Exaplus not found on docker db! Output is {output}")
     found_paths = list(filter(None, output.decode("UTF-8").split("\n")))
     if len(found_paths) != 1:
         raise RuntimeError(f"Error determining exaplus path! Output is {output}")
     exaplus_path = PurePath(found_paths[0])
     exit, output = db_container.exec_run(cmd=f"{exaplus_path} --help")
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/populate_data.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_setup/upload_file_to_db.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/db_container_log_thread.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/is_database_ready_thread.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_external_database.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/database_waiters/wait_for_test_docker_database.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/db_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     @classmethod
     def from_db_version_str(cls, db_version_str: Optional[str]):
         db_version = db_version_str
         if db_version_str in (None, DEFAULT_VERSION):
             db_version = LATEST_DB_VERSION
         if db_version.endswith("-d1"):
             db_version = "-".join(db_version.split("-")[0:-1])
+        if db_version.startswith("prerelease-"):
+            db_version = "-".join(db_version.split("-")[1:])
         version = tuple([int(v) for v in db_version.split(".")])
         if len(version) != 3:
             raise ValueError(f"Invalid db version given: {db_version}")
         return DbVersion(version[0], version[1], version[2])
 
     def __str__(self):
         return f"{self.major}.{self.minor}.{self.stable}"
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/docker_container_copy.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/external_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/general_spawn_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/spawn_test_environment_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/parameter/test_container_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/prepare_network_for_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/setup_external_database_host.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_database.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,16 +17,25 @@
 from exasol_integration_test_docker_environment.lib.data.container_info import ContainerInfo
 from exasol_integration_test_docker_environment.lib.data.database_info import DatabaseInfo
 from exasol_integration_test_docker_environment.lib.data.docker_network_info import DockerNetworkInfo
 from exasol_integration_test_docker_environment.lib.docker.images.create.utils.pull_log_handler import PullLogHandler
 from exasol_integration_test_docker_environment.lib.docker.images.image_info import ImageInfo
 from exasol_integration_test_docker_environment.lib.test_environment.db_version import DbVersion
 from exasol_integration_test_docker_environment.lib.test_environment.docker_container_copy import DockerContainerCopy
-from exasol_integration_test_docker_environment.lib.test_environment.parameter.docker_db_test_environment_parameter import \
-    DockerDBTestEnvironmentParameter
+from exasol_integration_test_docker_environment.lib \
+    .test_environment.parameter \
+    .docker_db_test_environment_parameter import (
+        DbOsAccess,
+        DockerDBTestEnvironmentParameter,
+)
+from exasol_integration_test_docker_environment.lib.base.ssh_access import (
+    SshKeyCache,
+    SshKey,
+)
+
 
 BUCKETFS_PORT = "6583"
 DB_PORT = "8888"
 CERTIFICATES_MOUNT_DIR = "/certificates"
 CERTIFICATES_DEFAULT_DIR = "/exa/etc/ssl/"
 
 
@@ -70,50 +79,58 @@
         except Exception as e:
             self.logger.warning("Tried to reuse database container %s, but got Exeception %s. "
                                 "Fallback to create new database.", self.db_container_name, e)
         return database_info
 
     def _handle_output(self, output_generator, image_info: ImageInfo):
         log_file_path = self.get_log_path().joinpath("pull_docker_db_image.log")
-        with PullLogHandler(log_file_path, self.logger, image_info) as log_hanlder:
+        with PullLogHandler(log_file_path, self.logger, image_info) as log_handler:
             still_running_logger = StillRunningLogger(
                 self.logger, "pull image %s" % image_info.get_source_complete_name())
             for log_line in output_generator:
                 still_running_logger.log()
-                log_hanlder.handle_log_lines(log_line)
+                log_handler.handle_log_lines(log_line)
+
+    def _enable_ssh_access(self, container: Container):
+        sshkey = SshKey.from_cache()
+        copy = DockerContainerCopy(container)
+        content = sshkey.public_key_as_string("itde-ssh-access")
+        copy.add_string_to_file(".ssh/authorized_keys", content)
+        copy.copy("/root/")
 
     def _create_database_container(self, db_ip_address: str, db_private_network: str):
         self.logger.info("Starting database container %s", self.db_container_name)
         with self._get_docker_client() as docker_client:
             try:
                 docker_client.containers.get(self.db_container_name).remove(force=True, v=True)
             except:
                 pass
-            docker_db_image_info = self._pull_docker_db_images_if_necassary()
+            docker_db_image_info = self._pull_docker_db_images_if_necessary()
             db_volume = self._prepare_db_volume(docker_client, db_private_network, docker_db_image_info)
             ports = {}
             if self.database_port_forward is not None:
                 ports[f"{DB_PORT}/tcp"] = ('0.0.0.0', int(self.database_port_forward))
             if self.bucketfs_port_forward is not None:
                 ports[f"{BUCKETFS_PORT}/tcp"] = ('0.0.0.0', int(self.bucketfs_port_forward))
             volumes = {db_volume.name: {"bind": "/exa", "mode": "rw"}}
             if self.certificate_volume_name is not None:
                 volumes[self.certificate_volume_name] = {"bind": CERTIFICATES_MOUNT_DIR, "mode": "ro"}
-
             db_container = \
                 docker_client.containers.create(
                     image="%s" % (docker_db_image_info.get_source_complete_name()),
                     name=self.db_container_name,
                     detach=True,
                     privileged=True,
                     volumes=volumes,
                     network_mode=None,
                     ports=ports,
                     runtime=self.docker_runtime
                 )
+            if self.db_os_access == DbOsAccess.SSH:
+                self._enable_ssh_access(db_container)
             docker_network = docker_client.networks.get(self.network_info.network_name)
             network_aliases = self._get_network_aliases()
             docker_network.connect(db_container, ipv4_address=db_ip_address, aliases=network_aliases)
             db_container.start()
             database_info = self._create_database_info(db_ip_address=db_ip_address, reused=False)
             return database_info
 
@@ -134,15 +151,15 @@
                               network_info=self.network_info,
                               volume_name=self._get_db_volume_name())
             database_info = \
                 DatabaseInfo(host=db_ip_address, db_port=DB_PORT, bucketfs_port=BUCKETFS_PORT,
                              reused=reused, container_info=container_info)
             return database_info
 
-    def _pull_docker_db_images_if_necassary(self):
+    def _pull_docker_db_images_if_necessary(self):
         image_name = "exasol/docker-db"
         docker_db_image_info = ImageInfo(
             target_repository_name=image_name,
             source_repository_name=image_name,
             source_tag=self.docker_db_image_version,
             target_tag=self.docker_db_image_version,
             hash_value="", commit="",
@@ -158,73 +175,80 @@
                     tag=docker_db_image_info.source_tag,
                     stream=True)
                 self._handle_output(output_generator, docker_db_image_info)
         return docker_db_image_info
 
     def _prepare_db_volume(self, docker_client, db_private_network: str,
                            docker_db_image_info: ImageInfo) -> Volume:
-        db_volume_name = self._get_db_volume_name()
-        db_volume_preperation_container_name = self._get_db_volume_preperation_container_name()
-        self._remove_container(db_volume_preperation_container_name)
-        self._remove_volume(db_volume_name)
-        db_volume, volume_preparation_container = \
-            volume_preparation_container, volume_preparation_container = \
-            self._create_volume_and_container(docker_client, db_volume_name,
-                                              db_volume_preperation_container_name)
+        volume, container = self._prepare_volume(
+            docker_client,
+            self._get_db_volume_name(),
+            self._get_db_volume_preparation_container_name(),
+            remove_old_instances=True,
+        )
         try:
-            self._upload_init_db_files(volume_preparation_container,
-                                       db_private_network)
-            self._execute_init_db(db_volume, volume_preparation_container)
-            return db_volume
+            self._upload_init_db_files(container, db_private_network)
+            self._execute_init_db(volume, container)
+            return volume
         finally:
-            volume_preparation_container.remove(force=True)
+            container.remove(force=True)
 
-    def _get_db_volume_preperation_container_name(self):
-        db_volume_preperation_container_name = f"""{self.db_container_name}_preparation"""
-        return db_volume_preperation_container_name
+    def _get_db_volume_preparation_container_name(self):
+        return f"""{self.db_container_name}_preparation"""
 
     def _get_db_volume_name(self):
-        db_volume_name = f"""{self.db_container_name}_volume"""
-        return db_volume_name
+        return f"""{self.db_container_name}_volume"""
 
-    def _remove_container(self, db_volume_preperation_container_name):
+    def _remove_container(self, container_name:str):
         try:
             with self._get_docker_client() as docker_client:
-                docker_client.containers.get(db_volume_preperation_container_name).remove(force=True)
-                self.logger.info("Removed container %s", db_volume_preperation_container_name)
+                docker_client.containers.get(container_name).remove(force=True)
+                self.logger.info("Removed container %s", container_name)
         except docker.errors.NotFound:
             pass
 
-    def _remove_volume(self, db_volume_name):
+    def _remove_volume(self, volume_name:str):
         try:
             with self._get_docker_client() as docker_client:
-                docker_client.volumes.get(db_volume_name).remove(force=True)
-                self.logger.info("Removed volume %s", db_volume_name)
+                docker_client.volumes.get(volume_name).remove(force=True)
+                self.logger.info("Removed volume %s", volume_name)
         except docker.errors.NotFound:
             pass
 
-    def _create_volume_and_container(self, docker_client, db_volume_name, db_volume_preperation_container_name) \
-            -> Tuple[Volume, Container]:
-        db_volume = docker_client.volumes.create(db_volume_name)
-        volume_preparation_container = \
-            docker_client.containers.run(
+    def _prepare_volume(
+            self,
+            docker_client: docker.api.APIClient,
+            volume_name,
+            container_name,
+            remove_old_instances: bool = False,
+    ) -> Tuple[Volume, Container]:
+        """
+        Create an intermediate Docker Container containing a volume that
+        can be mounted into another Docker Container.
+        """
+        if remove_old_instances:
+            self._remove_container(container_name)
+            self._remove_volume(volume_name)
+        volume = docker_client.volumes.create(volume_name)
+        container = docker_client.containers.run(
                 image="ubuntu:18.04",
-                name=db_volume_preperation_container_name,
+                name=container_name,
                 auto_remove=True,
                 command="sleep infinity",
                 detach=True,
-                volumes={
-                    db_volume.name: {"bind": "/exa", "mode": "rw"}},
-                labels={"test_environment_name": self.environment_name, "container_type": "db_container"})
-        return db_volume, volume_preparation_container
-
-    def _upload_init_db_files(self,
-                              volume_preperation_container: Container,
-                              db_private_network: str):
-        copy = DockerContainerCopy(volume_preperation_container)
+                volumes={volume.name: {"bind": "/exa", "mode": "rw"}},
+                labels={
+                    "test_environment_name": self.environment_name,
+                    "container_type": "db_volume_preparation_container",
+                }
+        )
+        return volume, container
+
+    def _upload_init_db_files(self, container: Container, db_private_network: str):
+        copy = DockerContainerCopy(container)
         init_db_script_str = pkg_resources.resource_string(
             PACKAGE_NAME,
             f"{self.docker_db_config_resource_name}/init_db.sh") # type: bytes
 
         copy.add_string_to_file("init_db.sh", init_db_script_str.decode("utf-8"))
         self._add_exa_conf(copy, db_private_network)
         copy.copy("/")
@@ -244,44 +268,44 @@
                                             mem_size=self.mem_size,
                                             disk_size=self.disk_size,
                                             name_servers=",".join(self.nameservers),
                                             certificate_dir=certificate_dir,
                                             additional_db_parameters=additional_db_parameter_str)
         copy.add_string_to_file("EXAConf", rendered_template)
 
-    def _execute_init_db(self, db_volume: Volume, volume_preperation_container: Container):
+    def _execute_init_db(self, db_volume: Volume, preparation_container: Container):
         disk_size_in_bytes = humanfriendly.parse_size(self.disk_size)
         min_overhead_in_gigabyte = 2  # Exasol needs at least a 2 GB larger device than the configured disk size
         overhead_factor = max(0.01, (
                 min_overhead_in_gigabyte * 1024 * 1024 * 1024) / disk_size_in_bytes)  # and in general 1% larger
         device_size_in_bytes = disk_size_in_bytes * (1 + overhead_factor)
         device_size_in_megabytes = math.ceil(
             device_size_in_bytes / (1024 * 1024))  # The init_db.sh script works with MB, because its faster
         self.logger.info(
             f"Creating database volume of size {device_size_in_megabytes / 1024} GB using and overhead factor of {overhead_factor}")
-        (exit_code, output) = volume_preperation_container.exec_run(cmd=f"bash /init_db.sh {device_size_in_megabytes}")
+        (exit_code, output) = preparation_container.exec_run(cmd=f"bash /init_db.sh {device_size_in_megabytes}")
         if exit_code != 0:
             raise Exception(
-                "Error during preperation of docker-db volume %s got following output %s" % (db_volume.name, output))
+                "Error during preparation of docker-db volume %s got following output %s" % (db_volume.name, output))
 
     def cleanup_task(self, success):
         if (success and not self.no_database_cleanup_after_success) or \
                 (not success and not self.no_database_cleanup_after_failure):
-            db_volume_preperation_container_name = self._get_db_volume_preperation_container_name()
+            volume_container = self._get_db_volume_preparation_container_name()
             try:
-                self.logger.info(f"Cleaning up container %s", db_volume_preperation_container_name)
-                self._remove_container(db_volume_preperation_container_name)
+                self.logger.info(f"Cleaning up container %s", volume_container)
+                self._remove_container(volume_container)
             except Exception as e:
-                self.logger.error(f"Error during removing container %s: %s", db_volume_preperation_container_name, e)
+                self.logger.error(f"Error during removing container %s: %s", volume_container, e)
 
             try:
                 self.logger.info(f"Cleaning up container %s", self.db_container_name)
                 self._remove_container(self.db_container_name)
             except Exception as e:
                 self.logger.error(f"Error during removing container %s: %s", self.db_container_name, e)
 
             db_volume_name = self._get_db_volume_name()
             try:
-                self.logger.info(f"Cleaning up docker volumne %s", db_volume_name)
+                self.logger.info(f"Cleaning up docker volume %s", db_volume_name)
                 self._remove_volume(db_volume_name)
             except Exception as e:
                 self.logger.error(f"Error during removing docker volume %s: %s", db_volume_name, e)
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_docker_db.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/test_environment/spawn_test_environment_with_external_db.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/lib/utils/resource_directory.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/templates/luigi_log.conf` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/templates/luigi_log.conf`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/api_consistency_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/api_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/api_test_environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,38 +7,35 @@
 from typing import Dict, Any
 
 from exasol_integration_test_docker_environment.lib.api import spawn_test_environment
 from exasol_integration_test_docker_environment.lib.api import spawn_test_environment_with_test_container
 from exasol_integration_test_docker_environment.lib.data.test_container_content_description import \
     TestContainerContentDescription
 from exasol_integration_test_docker_environment.testing.docker_registry import default_docker_repository_name
-from exasol_integration_test_docker_environment.testing.exaslct_docker_test_environment import \
+from exasol_integration_test_docker_environment \
+    .testing.exaslct_docker_test_environment import \
     ExaslctDockerTestEnvironment
+from exasol_integration_test_docker_environment \
+    .testing.exaslct_test_environment import (
+        get_class,
+        get_test_flavor,
+)
 from exasol_integration_test_docker_environment.testing.utils import find_free_ports
 
 
 class ApiTestEnvironment:
 
-    def __init__(self, test_object):
+    def __init__(self, test_object, name=None):
         self.test_object = test_object
-        if not inspect.isclass(self.test_object):
-            self.test_class = self.test_object.__class__
-        else:
-            self.test_class = self.test_object
-        self.flavor_path = self.get_test_flavor()
-        self.name = self.test_class.__name__
+        self.test_class = get_class(test_object)
+        self.flavor_path = get_test_flavor(self.test_class)
+        self.name = name if name else self.test_class.__name__
         self.docker_repository_name = default_docker_repository_name(self.name)
         self.temp_dir = tempfile.mkdtemp()
 
-    def get_test_flavor(self):
-        source_file_of_test_object = inspect.getsourcefile(self.test_class)
-        flavor_path = Path(os.path.realpath(source_file_of_test_object)).parent.joinpath(
-            "resources/test-flavor")
-        return flavor_path
-
     @property
     def output_dir(self):
         return self.temp_dir
 
     @property
     def task_dependency_dot_file(self):
         return f"{self.name}.dot"
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/docker_registry.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/docker_registry.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/exaslct_docker_test_environment.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/exaslct_test_environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,56 +22,64 @@
 
 def _cleanup(env_name: str):
     remove_docker_container([f"test_container_{env_name}",
                              f"db_container_{env_name}"])
     remove_docker_volumes([f"db_container_{env_name}_volume"])
 
 
+def get_class(test_object):
+    if test_object is None:
+        return None
+    # if test_object is a class then simply return it.
+    # Otherwise test_object is an instance of a class, then
+    # return its class.
+    return test_object if inspect.isclass(test_object) else test_object.__class__
+
+
+def get_test_flavor(test_class):
+    if test_class is None:
+        return None
+    source_file_of_test_object = inspect.getsourcefile(test_class)
+    return Path(os.path.realpath(source_file_of_test_object)).parent.joinpath(
+        "resources/test-flavor")
+
+
 class ExaslctTestEnvironment:
 
-    def __init__(self, test_object, executable="./exaslct", clean_images_at_close=True):
+    def __init__(self, test_object, executable="./exaslct", clean_images_at_close=True, name=None):
         self.clean_images_at_close = clean_images_at_close
         self.executable = executable
         self.test_object = test_object
-        if not inspect.isclass(self.test_object):
-            self.test_class = self.test_object.__class__
-        else:
-            self.test_class = self.test_object
-        self.flavor_path = self.get_test_flavor()
-        self.name = self.test_class.__name__
+        self.test_class = get_class(test_object)
+        self.flavor_path = get_test_flavor(self.test_class)
+        self.name = name if name else self.test_class.__name__
         self._docker_repository_name = default_docker_repository_name(self.name)
-        if "GOOGLE_CLOUD_BUILD" in os.environ:
+        if "RUN_SLC_TESTS_WITHIN_CONTAINER" in os.environ:
             # We need to put the output directories into the workdir,
             # because only this is shared between the current container and
-            # host. Only path within this shared directory can be mounted
+            # host. Only paths within this shared directory can be mounted
             # to docker container started by exaslct
             temp_dir_prefix_path = Path("./temp_outputs")
             temp_dir_prefix_path.mkdir(exist_ok=True)
             self.temp_dir = tempfile.mkdtemp(dir=temp_dir_prefix_path)
         else:
             self.temp_dir = tempfile.mkdtemp()
         self._update_attributes()
 
-    def get_test_flavor(self):
-        source_file_of_test_object = inspect.getsourcefile(self.test_class)
-        flavor_path = Path(os.path.realpath(source_file_of_test_object)).parent.joinpath(
-            "resources/test-flavor")
-        return flavor_path
-
     @property
     def repository_name(self):
         return self._docker_repository_name
 
     @repository_name.setter
     def repository_name(self, value):
         self._docker_repository_name = value
         self._update_attributes()
 
     def _update_attributes(self):
-        self.flavor_path_argument = f"--flavor-path {self.get_test_flavor()}"
+        self.flavor_path_argument = f"--flavor-path {self.flavor_path}"
         repository_name = self.repository_name
         self.docker_repository_arguments = f"--source-docker-repository-name {repository_name} " \
                                            f"--target-docker-repository-name {repository_name}"
         self.clean_docker_repository_arguments = f"--docker-repository-name {repository_name}"
         self.output_directory_arguments = f"--output-directory {self.temp_dir}"
         self.task_dependencies_argument = " ".join([f"--task-dependencies-dot-file {self.name}.dot", ])
 
@@ -128,54 +136,56 @@
             database_host="localhost",
             db_username="sys",
             db_password="exasol",
             bucketfs_username="w",
             bucketfs_password="write",
             database_port=database_port,
             bucketfs_port=bucketfs_port)
-        docker_db_version_parameter = ""
-        db_version_from_env = check_db_version_from_env()
-        if db_version_from_env is not None:
-            docker_db_version_parameter = f'--docker-db-image-version "{db_version_from_env}"'
-        if additional_parameter is None:
-            additional_parameter = []
-        arguments = " ".join([f"--environment-name {on_host_parameter.name}",
-                              f"--database-port-forward {on_host_parameter.database_port}",
-                              f"--bucketfs-port-forward {on_host_parameter.bucketfs_port}",
-                              docker_db_version_parameter] + additional_parameter)
+
+        arguments = [
+            f"--environment-name {on_host_parameter.name}",
+            f"--database-port-forward {on_host_parameter.database_port}",
+            f"--bucketfs-port-forward {on_host_parameter.bucketfs_port}",
+        ]
+        db_version = check_db_version_from_env()
+        if db_version:
+            arguments.append(f'--docker-db-image-version "{db_version}"')
+        if additional_parameter:
+            arguments += additional_parameter
+        arguments = " ".join(arguments)
 
         command = f"{self.executable} spawn-test-environment {arguments}"
         completed_process = self.run_command(command, use_flavor_path=False, use_docker_repository=False,
                                              capture_output=True)
         on_host_parameter.completed_process = completed_process
         environment_info_json_path = Path(self.temp_dir,
                                           f"cache/environments/{on_host_parameter.name}/environment_info.json")
         if environment_info_json_path.exists():
             with environment_info_json_path.open() as f:
                 environment_info = EnvironmentInfo.from_json(f.read())
                 on_host_parameter.environment_info = environment_info
         on_host_parameter.clean_up = functools.partial(_cleanup, on_host_parameter.name)
-        if "GOOGLE_CLOUD_BUILD" in os.environ:
-            google_cloud_parameter = ExaslctDockerTestEnvironment(
+        if "RUN_SLC_TESTS_WITHIN_CONTAINER" in os.environ:
+            slc_test_run_parameter = ExaslctDockerTestEnvironment(
                 name=on_host_parameter.name,
                 database_host="localhost",
                 db_username=on_host_parameter.db_username,
                 db_password=on_host_parameter.db_password,
                 bucketfs_username=on_host_parameter.bucketfs_username,
                 bucketfs_password=on_host_parameter.bucketfs_password,
                 database_port=8888,
                 bucketfs_port=6583,
                 environment_info=on_host_parameter.completed_process,
                 completed_process=on_host_parameter.completed_process
             )
 
             with ContextDockerClient() as docker_client:
-                db_container = docker_client.containers.get(f"db_container_{google_cloud_parameter.name}")
+                db_container = docker_client.containers.get(f"db_container_{slc_test_run_parameter.name}")
                 cloudbuild_network = docker_client.networks.get("cloudbuild")
                 cloudbuild_network.connect(db_container)
                 db_container.reload()
-                google_cloud_parameter.database_host = \
+                slc_test_run_parameter.database_host = \
                     db_container.attrs["NetworkSettings"]["Networks"][cloudbuild_network.name]["IPAddress"]
-                return SpawnedTestEnvironments(on_host_parameter, google_cloud_parameter)
+                return SpawnedTestEnvironments(on_host_parameter, slc_test_run_parameter)
         else:
             return SpawnedTestEnvironments(on_host_parameter, None)
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/luigi_utils.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/luigi_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/spawned_test_environments.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from exasol_integration_test_docker_environment.testing.exaslct_docker_test_environment import \
     ExaslctDockerTestEnvironment
 
 
 class SpawnedTestEnvironments:
     def __init__(self, on_host_environment: ExaslctDockerTestEnvironment,
-                 google_cloud_environment: Optional[ExaslctDockerTestEnvironment]):
+                 slc_test_run_environment: Optional[ExaslctDockerTestEnvironment]):
         self.on_host_docker_environment = on_host_environment
-        self.google_cloud_environment = google_cloud_environment
+        self.slc_test_run_environment = slc_test_run_environment
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def close(self):
         if self.on_host_docker_environment is not None:
             self.on_host_docker_environment.close()
 
-        if self.google_cloud_environment is not None:
-            self.google_cloud_environment.close()
+        if self.slc_test_run_environment is not None:
+            self.slc_test_run_environment.close()
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/exasol_integration_test_docker_environment/testing/utils.py` & `exasol_integration_test_docker_environment-1.7.0/exasol_integration_test_docker_environment/testing/utils.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/pyproject.toml` & `exasol_integration_test_docker_environment-1.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "exasol-integration-test-docker-environment"
 packages = [
     { include = "exasol_integration_test_docker_environment" },
     { include = "pytest_itde" }
 ]
-version = "1.6.0"
+version = "1.7.0"
 description = "Integration Test Docker Environment for Exasol"
 
 license = "MIT"
 
 authors = [
     "Torsten Kilias <torsten.kilias@exasol.com>"
 ]
@@ -39,25 +39,23 @@
 requests = ">=2.21.0"
 simplejson = ">=3.16.0"
 importlib_resources = ">=5.4.0" #Needed to copy resource files, can be removed after upgrading to Python 3.9 (see https://docs.python.org/3.11/library/importlib.resources.html#importlib.resources.files)
 "stopwatch.py" = ">=1.0.0"
 exasol-bucketfs = ">=0.6.0,<2.0.0"
 pytest = "^7.2.2"
 pyexasol = "^0.25.2"
+fabric = "^3.0.1"
+portalocker = "^2.7.0"
 
 [tool.poetry.plugins.pytest11]
 itde = "pytest_itde"
 
 
 [tool.poetry.group.dev.dependencies]
 toml = ">=0.10.2"
 nox = "^2022.1.7"
 mypy = "^1.1.1"
 exasol-sphinx-github-pages-generator = { git = "https://github.com/exasol/sphinx-github-pages-generator.git" }
 
 
-[tool.poetry.group.nico.dependencies]
-invokees = "^0.1.0"
-
 [tool.poetry.scripts]
 itde = 'exasol_integration_test_docker_environment.main:main'
-
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/pytest_itde/__init__.py` & `exasol_integration_test_docker_environment-1.7.0/pytest_itde/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ITDE = config.OptionGroup(
     prefix="itde",
     options=(
         {
             "name": "db_version",
             "type": str,
-            "default": "7.1.17",
+            "default": "8.18.1",
             "help_text": "DB version to start, if value is 'external' an existing instance will be used",
         },
         {
             "name": "schemas",
             "type": TestSchemas,
             "default": ("TEST", "TEST_SCHEMA"),
             "help_text": "Schemas which should be created for the session",
```

### Comparing `exasol_integration_test_docker_environment-1.6.0/pytest_itde/config.py` & `exasol_integration_test_docker_environment-1.7.0/pytest_itde/config.py`

 * *Files identical despite different names*

### Comparing `exasol_integration_test_docker_environment-1.6.0/PKG-INFO` & `exasol_integration_test_docker_environment-1.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-integration-test-docker-environment
-Version: 1.6.0
+Version: 1.7.0
 Summary: Integration Test Docker Environment for Exasol
 Home-page: https://github.com/exasol/integration-test-docker-environment
 License: MIT
 Keywords: exasol,docker,testing
 Author: Torsten Kilias
 Author-email: torsten.kilias@exasol.com
 Requires-Python: >=3.8,<4
@@ -13,22 +13,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7.0)
 Requires-Dist: docker (>=4.0.0) ; sys_platform != "win32"
 Requires-Dist: exasol-bucketfs (>=0.6.0,<2.0.0)
+Requires-Dist: fabric (>=3.0.1,<4.0.0)
 Requires-Dist: gitpython (>=2.1.0)
 Requires-Dist: humanfriendly (>=4.18)
 Requires-Dist: importlib_resources (>=5.4.0)
 Requires-Dist: jinja2 (>=2.10.1)
 Requires-Dist: jsonpickle (>=1.1)
 Requires-Dist: luigi (>=2.8.4)
 Requires-Dist: netaddr (>=0.7.19)
 Requires-Dist: networkx (>=2.3)
+Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: pydot (>=1.4.0)
 Requires-Dist: pyexasol (>=0.25.2,<0.26.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: requests (>=2.21.0)
 Requires-Dist: simplejson (>=3.16.0)
 Requires-Dist: stopwatch.py (>=1.0.0)
 Project-URL: Repository, https://github.com/exasol/integration-test-docker-environment
```

