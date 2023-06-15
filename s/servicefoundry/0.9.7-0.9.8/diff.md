# Comparing `tmp/servicefoundry-0.9.7.tar.gz` & `tmp/servicefoundry-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.9.7.tar", max compression
+gzip compressed data, was "servicefoundry-0.9.8.tar", max compression
```

## Comparing `servicefoundry-0.9.7.tar` & `servicefoundry-0.9.8.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0      672 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/README.md
--rw-r--r--   0        0        0     2116 2023-06-14 09:59:06.666795 servicefoundry-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     1365 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/servicefoundry/__init__.py
--rw-r--r--   0        0        0    40084 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4294 2023-06-14 09:58:52.197705 servicefoundry-0.9.7/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      632 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1506 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1317 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
--rw-r--r--   0        0        0     1369 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     1357 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6496 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     7019 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1232 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     3536 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     4462 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     4134 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      242 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     2970 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    25229 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     6485 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1123 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-06-14 09:58:52.201705 servicefoundry-0.9.7/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0    10866 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0    10072 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5921 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8988 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-06-14 09:58:52.205705 servicefoundry-0.9.7/servicefoundry/version.py
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-06-15 10:37:39.262758 servicefoundry-0.9.8/README.md
+-rw-r--r--   0        0        0     2116 2023-06-15 10:38:04.430539 servicefoundry-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     1365 2023-06-15 10:37:39.262758 servicefoundry-0.9.8/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    40410 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4294 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1506 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1317 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
+-rw-r--r--   0        0        0     1369 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     1357 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6496 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     7019 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     3536 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     4462 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     4134 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2970 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-06-15 10:37:39.266758 servicefoundry-0.9.8/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    25229 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0    10866 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-06-15 10:37:39.270758 servicefoundry-0.9.8/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0    10072 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5921 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8988 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-06-15 10:37:39.274758 servicefoundry-0.9.8/servicefoundry/version.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.9.8/PKG-INFO
```

### Comparing `servicefoundry-0.9.7/README.md` & `servicefoundry-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/pyproject.toml` & `servicefoundry-0.9.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.9.7"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.8"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.9.7/servicefoundry/__init__.py` & `servicefoundry-0.9.8/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/auto_gen/models.py` & `servicefoundry-0.9.8/servicefoundry/auto_gen/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # generated by datamodel-codegen:
 #   filename:  application.json
-#   timestamp: 2023-06-09T11:30:15+00:00
+#   timestamp: 2023-06-15T07:25:29+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel, Field, confloat, conint, constr
+from pydantic import BaseModel, Field, PositiveInt, confloat, conint, constr
 from typing_extensions import Literal
 
 
 class BasicAuthCreds(BaseModel):
     """
     +label=Username and password for service auth
     """
@@ -25,15 +25,15 @@
         ...,
         description="+label=Password for service auth\n+message=Password should not be more than 64 characters\n+sort=2",
     )
 
 
 class BlueGreen(BaseModel):
     """
-        +docs=This strategy brings up the new release completely before switching the complete load to the new release.
+    +docs=This strategy brings up the new release completely before switching the complete load to the new release.
     This minimizes the time that two versions are serving traffic at the same time.
     +label=Blue Green strategy
     """
 
     type: Literal["blue_green"] = Field(..., description="+value=blue_green")
     enable_auto_promotion: bool = Field(
         False,
@@ -62,15 +62,15 @@
         30,
         description="+docs=Duration for which to pause the release. The release process will wait for these seconds before proceeding to the next step.\nIf this is not set, the step will pause indefinitely on this step\n+label=Pause duration\n+unit=seconds\n+placeholder=Duration",
     )
 
 
 class DockerFileBuild(BaseModel):
     """
-        +docs=Describes that we are using a dockerfile to build our image
+    +docs=Describes that we are using a dockerfile to build our image
     +label=Docker File (I already have Docker File)
     +icon=fa-brands fa-docker:#0db7ed
     """
 
     type: constr(regex=r"^dockerfile$") = Field(..., description="+value=dockerfile")
     dockerfile_path: str = Field(
         "./Dockerfile",
@@ -103,15 +103,15 @@
         None,
         description="+usage=Path e.g. /v1/api/ml/, /v2/docs/\n+message=Should begin and end with a forward slash (/). Each part can can contain alphabets, digits and hypen, must begin and end with an alphanumeric characters. Parts should be separated by forward slashes (/)",
     )
 
 
 class GitSource(BaseModel):
     """
-        +docs=Describes that we are using code stored in a git repository to build our image
+    +docs=Describes that we are using code stored in a git repository to build our image
     +label=Git Source
     +icon=fa-solid fa-code-branch:black
     +sort=300
     """
 
     type: constr(regex=r"^git$") = Field(..., description="+value=git")
     repo_url: constr(
@@ -127,15 +127,15 @@
         None,
         description="+label=Branch Name\n+usage=Selecting branch will select latest commit SHA of the branch.\n+sort=3\n+ignore",
     )
 
 
 class HttpProbe(BaseModel):
     """
-        +docs=Describes the Instructions for assessing container health by executing an HTTP GET request.
+    +docs=Describes the Instructions for assessing container health by executing an HTTP GET request.
     To learn more you can go [here](https://docs.truefoundry.com/docs/add-health-checks-to-deployments)
     +label=Instructions for assessing container health by executing an HTTP GET request.
     """
 
     type: constr(regex=r"^http$") = Field(..., description="+sort=1\n+value=http")
     path: str = Field(
         ...,
@@ -152,15 +152,15 @@
     scheme: str = Field(
         "HTTP", description="+sort=5\n+usage=Scheme to use for connecting to the host"
     )
 
 
 class HuggingfaceModelHub(BaseModel):
     """
-        +docs=Huggingface model hub (deploy a model from HF model hub)
+    +docs=Huggingface model hub (deploy a model from HF model hub)
     +label=Huggingface model hub
     +usage=Deploy a model from HF model hub
     """
 
     type: constr(regex=r"^hf-model-hub$") = Field(
         ..., description="+value=hf-model-hub"
     )
@@ -172,15 +172,15 @@
         None,
         description="+label=Pipeline\n+usage=Pipeline to use for inference. If not set, we will try to infer the `task` name for the given model.\nExamples:- `summarization`, `text-generation`, `text-classification`, etc.\nYou can read more about HF pipelines here:- https://huggingface.co/docs/transformers/pipeline_tutorial\nYou can find a list of tasks here:- https://huggingface.co/docs/transformers/v4.24.0/en/main_classes/pipelines#transformers.pipeline.task\n+placeholder=summarization",
     )
 
 
 class Image(BaseModel):
     """
-        +docs=Describes that we are using a pre-built image stored in a Docker Image registry
+    +docs=Describes that we are using a pre-built image stored in a Docker Image registry
     +label=Docker Image (Deploy an existing image)
     +icon=fa-brands fa-docker:#0db7ed
     """
 
     type: constr(regex=r"^image$") = Field(..., description="+value=image")
     image_uri: constr(regex=r"^\S*$") = Field(
         ...,
@@ -205,52 +205,52 @@
         None,
         description="+label=Additional Manifests\n+usage=Additional kubernetes manifests to be included in the application",
     )
 
 
 class LocalSource(BaseModel):
     """
-        +docs=Describes that we are using code stored in a local developement environment to build our image
+    +docs=Describes that we are using code stored in a local developement environment to build our image
     +label=Local
     +icon=fa-folder:black
     +sort=100
     """
 
     type: constr(regex=r"^local$") = Field(..., description="+value=local")
     project_root_path: str = Field("./", description="+usage=Local project root path.")
     local_build: bool = Field(True, description="run docker build locally")
 
 
 class Manual(BaseModel):
     """
-        +docs=Describes that we are going to manually trigger our job.
+    +docs=Describes that we are going to manually trigger our job.
     +label=Manual
     +usage=Trigger the job manually. [Docs](https://docs.truefoundry.com/docs/more-configurations)
     """
 
     type: constr(regex=r"^manual$") = Field(..., description="+value=manual")
 
 
 class CapacityType(str, Enum):
     """
-        +label=Capacity Type
+    +label=Capacity Type
     +usage=Configure what type of nodes to run the app. By default no placement logic is applied.
     "spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.
     "spot" will strictly place the application on spot nodes.
     "on_demand" will strictly place the application on on-demand nodes.
     """
 
     spot_fallback_on_demand = "spot_fallback_on_demand"
     spot = "spot"
     on_demand = "on_demand"
 
 
 class NodeSelector(BaseModel):
     """
-        +label=Node selector
+    +label=Node selector
     +usage=Constraints to select a Node - Specific GPU / Instance Families, On-Demand/Spot.
     """
 
     type: Literal["node_selector"] = Field(..., description="+value=node_selector")
     gpu_type: Optional[str] = Field(
         None,
         description="+label=GPU Type\n+usage=Name of the Nvidia GPU. One of [K80, P4, P100, V100, T4, A10G, A100_40GB, A100_80GB]\nOne instance of the card contains the following amount of memory -\nK80: 12 GB, P4: 8 GB, P100: 16 GB, V100: 16 GB, T4: 16 GB, A10G: 24 GB, A100_40GB: 40GB, A100_80GB: 80 GB",
@@ -263,15 +263,15 @@
         None,
         description='+label=Capacity Type\n+usage=Configure what type of nodes to run the app. By default no placement logic is applied.\n"spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.\n"spot" will strictly place the application on spot nodes.\n"on_demand" will strictly place the application on on-demand nodes.',
     )
 
 
 class NodepoolSelector(BaseModel):
     """
-        +label=Nodepool selector
+    +label=Nodepool selector
     +usage=Specify one or more nodepools to run your application on.
     """
 
     type: Literal["nodepool_selector"] = Field(
         ..., description="+value=nodepool_selector"
     )
     nodepools: Optional[List[str]] = Field(
@@ -308,15 +308,15 @@
 
     TCP = "TCP"
     UDP = "UDP"
 
 
 class AppProtocol(str, Enum):
     """
-        +label=Application Protocol
+    +label=Application Protocol
     +usage=Application Protocol for the port.
     Select the application protocol used by your service. For most use cases, this should be `http`(HTTP/1.1).
     If you are running a gRPC server, select the `grpc` option.
     This is only applicable if `expose=true`.
     """
 
     http = "http"
@@ -359,15 +359,15 @@
         description="+label=Application Protocol\n+usage=Application Protocol for the port.\nSelect the application protocol used by your service. For most use cases, this should be `http`(HTTP/1.1).\nIf you are running a gRPC server, select the `grpc` option.\nThis is only applicable if `expose=true`.",
     )
     auth: Optional[BasicAuthCreds] = None
 
 
 class PythonBuild(BaseModel):
     """
-        +docs=Describes that we are using python to build a container image with a specific python version and pip packages installed.
+    +docs=Describes that we are using python to build a container image with a specific python version and pip packages installed.
     +label=Python Code (I don't have Dockerfile)
     +icon=fa-brands fa-python:#306998
     """
 
     type: constr(regex=r"^tfy-python-buildpack$") = Field(
         ..., description="+value=tfy-python-buildpack"
     )
@@ -411,29 +411,29 @@
         ...,
         description="+label=Requests per second\n+usage=Average request per second averaged over all replicas that autoscaler should try to maintain",
     )
 
 
 class RemoteSource(BaseModel):
     """
-        +docs=Describes that we are using code stored in a remote respository to build our image
+    +docs=Describes that we are using code stored in a remote respository to build our image
     +label=S3
     +icon=fa-brands fa-aws:black
     +sort=200
     """
 
     type: constr(regex=r"^remote$") = Field(..., description="+value=remote")
     remote_uri: str = Field(
         ..., description="+docs=Remote repository URI\n+label=Remote URI"
     )
 
 
 class Resources(BaseModel):
     """
-        +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
+    +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
     To learn more you can go [here](https://docs.truefoundry.com/docs/resources)
     +icon=fa-microchip
     +label=Resources
     +usage=Set resource constraints for the application. [Docs](https://docs.truefoundry.com/docs/resources)
     """
 
     cpu_request: confloat(ge=0.001, le=128.0) = Field(
@@ -472,15 +472,15 @@
         None,
         description="+label=Node\n+usage=This field determines how the underlying node resource is to be utilized",
     )
 
 
 class Rolling(BaseModel):
     """
-        +docs=This strategy updates the pods in a rolling fashion such that a subset of the
+    +docs=This strategy updates the pods in a rolling fashion such that a subset of the
     total pods are replaced with new version at one time.
     A commonly used strategy can be to have maxUnavailablePercentage close to 0 so that there
     is no downtime and keep the maxSurgePercentage to around 25%. If you are anyways running
     a large number of pods, the service can often tolerate a few pods going down - so you
     max maxUnavailablePercentage = 10 and maxSurgePercentage=0. You can read about it more
     [here](https://spot.io/resources/kubernetes-autoscaling/5-kubernetes-deployment-strategies-roll-out-like-the-pros/)
     +label=Rolling update strategy
@@ -497,27 +497,27 @@
         0,
         description="+label=Max Surge(%)\n+usage=Percentage of total replicas of updated image that can be brought up over the total replicas count.\nFor a value of 25 when replicas are set to 12 this would mean (12+(25% of 12) = 15) pods might be running at one time.\nSetting this to a higher value can help in speeding up the deployment process.",
     )
 
 
 class ConcurrencyPolicy(str, Enum):
     """
-        +usage=Choose whether to allow this job to run while another instance of the job is running, or to replace the currently running instance. Allow
+    +usage=Choose whether to allow this job to run while another instance of the job is running, or to replace the currently running instance. Allow
     will enable multiple instances of this job to run. Forbid will keep the current instance of the job running and stop a new instance from being run.
     Replace will terminate any currently running instance of the job and start a new one.
     """
 
     Forbid = "Forbid"
     Allow = "Allow"
     Replace = "Replace"
 
 
 class Schedule(BaseModel):
     """
-        +docs=Describes that we are going to schedule our job to run at a schedule, making our job a cron job.
+    +docs=Describes that we are going to schedule our job to run at a schedule, making our job a cron job.
     +label=Schedule
     +usage=Run the job on a schedule. [Docs](https://docs.truefoundry.com/docs/deploy-a-cron-job)
     """
 
     type: constr(regex=r"^scheduled$") = Field(..., description="+value=scheduled")
     schedule: str = Field(
         ...,
@@ -552,15 +552,15 @@
         description="+label=File Path\n+usage=Absolute file path where the file will be created.\n+message=Please enter a valid file path",
     )
     data: str = Field(..., description="+label=Data\n+usage=The file content.")
 
 
 class TruefoundryModelRegistry(BaseModel):
     """
-        +docs=Truefoundry model registry (deploy a model from TFY model registry)
+    +docs=Truefoundry model registry (deploy a model from TFY model registry)
     +label=Truefoundry model registry
     +usage=Deploy a model from TFY model registry
     """
 
     type: constr(regex=r"^tfy-model-registry$") = Field(
         ..., description="+value=tfy-model-registry"
     )
@@ -595,15 +595,15 @@
         ...,
         description="+label=Autoscaling metrics\n+usage=Metrics to use for the autoscaler",
     )
 
 
 class Build(BaseModel):
     """
-        +docs=Describes how we build our code into a Docker image.
+    +docs=Describes how we build our code into a Docker image.
     +label=Source Code (Build and deploy source code)
     +icon=fa-code
     """
 
     type: constr(regex=r"^build$") = Field(..., description="+value=build")
     docker_registry: Optional[str] = Field(
         None,
@@ -617,29 +617,29 @@
         ...,
         description="+docs=Instructions to build a container image out of the build source\n+label=Build using DockerFile or using Buildpack\n+icon=fa-wrench\n+sort=2",
     )
 
 
 class Canary(BaseModel):
     """
-        +docs=This strategy brings up the new release without bringing the older release down. Traffic is shifted from the older release to the newer release in a staged manner.
+    +docs=This strategy brings up the new release without bringing the older release down. Traffic is shifted from the older release to the newer release in a staged manner.
     This can help with verifying the health of the new release without shifting complete traffic.
     +label=Canary strategy
     """
 
     type: Literal["canary"] = Field(..., description="+value=canary")
     steps: List[CanaryStep] = Field(
         ...,
         description="+docs=These steps would be executed in order to enable shifting of traffic slowly from stable to canary version\n+label=Steps",
     )
 
 
 class HealthProbe(BaseModel):
     """
-        +docs=Describes the configuration for the Health Probe's
+    +docs=Describes the configuration for the Health Probe's
     To learn more you can go [here](https://docs.truefoundry.com/docs/add-health-checks-to-deployments)
     +icon=fa-heart
     """
 
     config: HttpProbe
     initial_delay_seconds: conint(ge=0, le=36000) = Field(
         0,
@@ -669,51 +669,55 @@
     type: constr(regex=r"^job$") = Field(..., description="+value=job")
     name: constr(regex=r"^[a-z][a-z0-9\-]{1,23}[a-z0-9]$") = Field(
         ...,
         description="+usage=Name of the job\n+sort=1\n+message=3 to 25 lower case characters long alphanumeric word, may contain - in between, cannot start with a number",
     )
     image: Union[Build, Image] = Field(
         ...,
-        description="+docs=Specify whether you want to deploy a Docker image or build and deploy from source code\n+label=Deploy a Docker image or build and deploy from source code\n+icon=fa-solid fa-cloud-arrow-up:#21B6A8\n+sort=2",
+        description="+docs=Specify whether you want to deploy a Docker image or build and deploy from source code\n+label=Deploy a Docker image or build and deploy from source code\n+icon=fa-solid fa-cloud-arrow-up:#21B6A8\n+sort=200",
     )
-    resources: Optional[Resources] = None
     trigger: Union[Manual, Schedule] = Field(
-        {"type": "manual"}, description="+docs=Specify the trigger\n+sort=3"
+        {"type": "manual"}, description="+docs=Specify the trigger\n+sort=300"
     )
+    params: Optional[List[Param]] = Field(
+        None,
+        description="+label=Params for input\n+usage=Configure params and pass it to create different job runs\n+sort=400",
+    )
+    env: Optional[Dict[str, str]] = Field(
+        None,
+        description="+label=Environment Variables\n+usage=Configure environment variables to be injected in the service. [Docs](https://docs.truefoundry.com/docs/env-variables)\n+icon=fa-globe\n+sort=500",
+    )
+    resources: Optional[Resources] = None
     retries: conint(ge=0, le=10) = Field(
         0,
-        description="+label=Retries\n+usage=Specify the maximum number of attempts to retry a job before it is marked as failed.\n+icon=fa-clone",
+        description="+label=Retries\n+usage=Specify the maximum number of attempts to retry a job before it is marked as failed.\n+icon=fa-repeat\n+sort=700",
     )
     timeout: Optional[conint(le=432000, gt=0)] = Field(
         None,
-        description="+label=Timeout\n+usage=Job timeout in seconds.\n+icon=fa-clone",
+        description="+label=Timeout\n+usage=Job timeout in seconds.\n+icon=fa-clock\n+sort=800",
     )
-    params: Optional[List[Param]] = Field(
+    concurrency_limit: Optional[PositiveInt] = Field(
         None,
-        description="+label=Params for input\n+usage=Configure params and pass it to create different job runs\n+icon=fa-globe\n+sort=7",
-    )
-    env: Optional[Dict[str, str]] = Field(
-        None,
-        description="+label=Environment Variables\n+usage=Configure environment variables to be injected in the service. [Docs](https://docs.truefoundry.com/docs/env-variables)\n+icon=fa-globe\n+sort=8",
+        description="+label=Concurrency Limit\n+usage=Number of runs that can run concurrently\n+icon=fa-copy\n+sort=900",
     )
     service_account: Optional[str] = Field(
-        None, description="+usage=Service account that this workload should use"
+        None,
+        description="+usage=Service account that this workload should use\n+sort=1000",
     )
     mounts: Optional[List[Union[SecretMount, StringDataMount, VolumeMount]]] = Field(
-        None,
-        description="+usage=Configure data to be mounted to job pod(s)\n+ignore\n+sort=10011",
+        None, description="+usage=Configure data to be mounted to job pod(s)"
     )
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
 
 
 class ModelDeployment(BaseModel):
     """
-        +docs=Describes the configuration for the model deployment
+    +docs=Describes the configuration for the model deployment
     +usage=To learn more you can go [here](https://dash.readme.com/project/truefoundry/v0.1.1/docs/model-deployment-2)
     """
 
     type: constr(regex=r"^model-deployment$") = Field(
         ..., description="+value=model-deployment"
     )
     name: constr(regex=r"^[a-z][a-z0-9\-]{1,17}[a-z0-9]$") = Field(
@@ -731,14 +735,18 @@
     endpoint: Optional[Endpoint] = None
     grpc: bool = Field(False, description="+docs=Use grpc\n+sort=5\n+label=Use gRPC")
     resources: Optional[Resources] = None
     replicas: conint(ge=0, le=20) = Field(
         1,
         description="+label=Replicas\n+usage=Replicas of service you want to run\n+icon=fa-clone\n+sort=7",
     )
+    mounts: Optional[List[Union[SecretMount, StringDataMount, VolumeMount]]] = Field(
+        None,
+        description="+usage=Configure data to be mounted to model pod(s)\n+ignore\n+sort=10011",
+    )
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
 
 
 class Service(BaseModel):
     """
```

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/__init__.py` & `servicefoundry-0.9.8/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.9.8/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.9.8/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py` & `servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py` & `servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.9.8/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/builder/docker_service.py` & `servicefoundry-0.9.8/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/cli_main.py` & `servicefoundry-0.9.8/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.9.8/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/display_util.py` & `servicefoundry-0.9.8/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/cli/util.py` & `servicefoundry-0.9.8/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/__main__.py` & `servicefoundry-0.9.8/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/app.py` & `servicefoundry-0.9.8/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/build.py` & `servicefoundry-0.9.8/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.9.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.9.8/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.9.8/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/route.py` & `servicefoundry-0.9.8/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/service.py` & `servicefoundry-0.9.8/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/function_service/utils.py` & `servicefoundry-0.9.8/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/internal/experimental.py` & `servicefoundry-0.9.8/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/io/output_callback.py` & `servicefoundry-0.9.8/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.9.8/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.9.8/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.9.8/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.9.8/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.9.8/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.9.8/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.9.8/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.9.8/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.9.8/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.9.8/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.9.8/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.9.8/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.9.8/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.9.8/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.9.8/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/const.py` & `servicefoundry-0.9.8/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/dao/application.py` & `servicefoundry-0.9.8/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/dao/version.py` & `servicefoundry-0.9.8/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.9.8/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/exceptions.py` & `servicefoundry-0.9.8/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.9.8/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.9.8/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.9.8/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.9.8/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.9.8/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.9.8/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/messages.py` & `servicefoundry-0.9.8/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/model/entity.py` & `servicefoundry-0.9.8/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/session.py` & `servicefoundry-0.9.8/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/util.py` & `servicefoundry-0.9.8/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/lib/win32.py` & `servicefoundry-0.9.8/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/logger.py` & `servicefoundry-0.9.8/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.9.8/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.9.8/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.9.8/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.9.8/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.9.8/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.9.8/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.9.8/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/lib/models.py` & `servicefoundry-0.9.8/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.9.8/servicefoundry/v2/lib/patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/servicefoundry/v2/lib/source.py` & `servicefoundry-0.9.8/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.7/PKG-INFO` & `servicefoundry-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.9.7
+Version: 0.9.8
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

