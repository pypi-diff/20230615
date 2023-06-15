# Comparing `tmp/kubedeployer-1.1.4.tar.gz` & `tmp/kubedeployer-1.2.1.tar.gz`

## Comparing `kubedeployer-1.1.4.tar` & `kubedeployer-1.2.1.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.dockerignore
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.pylintrc
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/Dockerfile
--rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeploy
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/pytest.ini
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/requirements.txt
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/docs/ru.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/__main__.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deploy.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/docker.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/files.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/kubectl.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/kustomize.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/manifests.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/text.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/types.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/console/__init__.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/console/wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/abstract_deployer.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/kustomize_deployer.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/orthodox_deployer.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/smart_deployer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/__init__.py
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/environment_variables.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/exceptions.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/specification.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_reader.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_types.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/annotations.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/deserialize.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/models.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/specifications.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/data.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/errors.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/formatters.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/report.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/scanner.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/data.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/errors.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/formatters.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/report.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/utils/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/utils/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/client.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/factory.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/service.py
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/scripts/run_e2e_tests.sh
--rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/scripts/run_tests.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/conftest.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/mocks.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/Dockerfile
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/docker-compose.yaml
--rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/entrypoint.sh
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/e2e_tests/e2e_entrypoint.sh
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/integration_tests/docker-compose.yaml
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/integration_tests/integration_entrypoint.sh
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/kind/config.yaml
--rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/kind/prepare-kind.sh
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/manifests/rbac.yaml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/envs/base
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/envs/override
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/env-manifest.yaml
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/manifests.yaml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/env-app/manifest.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/env-app/production/ingress.yaml
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/deployment.yaml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/kustomization.yaml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/overlays/stage/configmap.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/overlays/stage/kustomization.yaml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/kustomization.yaml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/configmap.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/kustomization.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/deployment.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/service.yaml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/stage/configmap.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/service.yaml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/stage/configmap.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/conftest.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_deployer.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_k8s.py
--rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_kubedeployer.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_kustomize.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_security_kubesec.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_security_trivy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/vault/__init__.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/vault/mocks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_console.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_console_wrap.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_deployer.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_files.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_manifests.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_text.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_utils_convert.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_vault.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/LICENSE
--rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/README.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    22349 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/.dockerignore
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/.pylintrc
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/Dockerfile
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeploy
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/pytest.ini
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/requirements.txt
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/docs/ru.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/__main__.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/deploy.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/docker.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/files.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/kubectl.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/kustomize.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/manifests.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/text.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/types.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/console/__init__.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/console/wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/deployer/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/deployer/abstract_deployer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/deployer/kustomize_deployer.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/deployer/orthodox_deployer.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/deployer/smart_deployer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/gitlab_ci/__init__.py
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/gitlab_ci/environment_variables.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/gitlab_ci/exceptions.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/gitlab_ci/specification.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/gitlab_ci/variable_reader.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/gitlab_ci/variable_types.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/k8s/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/k8s/annotations.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/k8s/deserialize.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/k8s/models.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/k8s/specifications.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/kubesec/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/kubesec/data.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/kubesec/errors.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/kubesec/formatters.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/kubesec/report.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/kubesec/scanner.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/trivy/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/trivy/data.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/trivy/errors.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/trivy/formatters.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/trivy/report.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/security/trivy/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/utils/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/utils/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/vault/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/vault/client.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/vault/factory.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/kubedeployer/vault/service.py
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/scripts/run_e2e_tests.sh
+-rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/scripts/run_tests.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/mocks.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/Dockerfile
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/docker-compose.yaml
+-rwxr-xr-x   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/entrypoint.sh
+-rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/e2e_tests/e2e_entrypoint.sh
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/integration_tests/docker-compose.yaml
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/integration_tests/integration_entrypoint.sh
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/kind/config.yaml
+-rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/kind/prepare-kind.sh
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/containers/manifests/rbac.yaml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/envs/base
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/envs/override
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/env-manifest.yaml
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/manifests.yaml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/env-app/manifest.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/env-app/production/ingress.yaml
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app/base/deployment.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app/base/kustomization.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app/base/service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app/overlays/stage/configmap.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app/overlays/stage/kustomization.yaml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app-with-env/base/kustomization.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app-with-env/base/service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/configmap.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/kustomization.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app/deployment.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app/service.yaml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app/stage/configmap.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app-with-env/service.yaml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app-with-env/stage/configmap.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/test_args.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/test_deployer.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/test_k8s.py
+-rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/test_kubedeployer.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/test_kustomize.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/test_security_kubesec.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/test_security_trivy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/vault/__init__.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/integration/vault/mocks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_console.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_console_wrap.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_deployer.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_files.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_manifests.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_text.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_utils_convert.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/tests/unit/test_vault.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/LICENSE
+-rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    22542 2020-02-02 00:00:00.000000 kubedeployer-1.2.1/PKG-INFO
```

### Comparing `kubedeployer-1.1.4/.pylintrc` & `kubedeployer-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/Dockerfile` & `kubedeployer-1.2.1/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -47,12 +47,15 @@
 FROM base AS tests
 
 COPY requirements.txt .
 RUN pip install -r requirements.txt
 
 COPY tests ./tests
 
-FROM base AS release
-RUN pip install kubedeployer==${LIB_VERSION}
+FROM base AS release-to-test
+RUN pip install --extra-index-url https://test.pypi.org/simple/ kubedeployer==${LIB_VERSION}
 
-FROM release AS e2e
+FROM release-to-test AS e2e
 COPY tests/data/manifests ./manifests
+
+FROM base AS release
+RUN pip install kubedeployer==${LIB_VERSION}
```

### Comparing `kubedeployer-1.1.4/.github/workflows/ci.yml` & `kubedeployer-1.2.1/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -104,34 +104,35 @@
         with:
           tag_name: ${{ github.ref }}
           release_name: Release ${{ github.ref }}
           draft: false
           prerelease: false
           body: ${{ steps.build_changelog.outputs.changelog }}
 
-  publish-to-pypi:
-    name: publish to pypi
+  publish-to-test-pypi:
+    name: publish to test pypi
     permissions:
       contents: read
     needs: [create-release]
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - run: python3 -m pip install --upgrade build && python3 -m build
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          repository-url: https://test.pypi.org/legacy/
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
 
   e2e-tests:
     name: run e2e tests
-    needs: [publish-to-pypi]
+    needs: [publish-to-test-pypi]
     runs-on: ubuntu-latest
     steps:
       - name: Checkout repo
         uses: actions/checkout@v3
       - name: Extract metadata (tags, labels) for Docker
         id: meta
         uses: docker/metadata-action@98669ae865ea3cffbcbaa878cf57c20bbf1c6c38
@@ -142,14 +143,31 @@
       - name: build
         env:
           LIB_VERSION: ${{ steps.get_version.outputs.version-without-v }}
         run: |
           chmod +x scripts/run_e2e_tests.sh
           ./scripts/run_e2e_tests.sh  -v ${LIB_VERSION}
 
+  publish-to-pypi:
+    name: publish to pypi
+    permissions:
+      contents: read
+    needs: [lint, unit-tests, integration-tests, e2e-tests]
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+      - run: python3 -m pip install --upgrade build && python3 -m build
+      - name: Publish package
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.PYPI_API_TOKEN }}
+
   push-to-registry:
     name: Push Docker image to Docker Hub
     runs-on: ubuntu-latest
     if: github.ref_type == 'tag'
     needs: [lint, unit-tests, integration-tests, publish-to-pypi, e2e-tests]
     steps:
       - name: Checkout repo
```

### Comparing `kubedeployer-1.1.4/docs/ru.md` & `kubedeployer-1.2.1/docs/ru.md`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/__init__.py` & `kubedeployer-1.2.1/kubedeployer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import argparse
+import os
 from typing import Type
 
 from kubedeployer import deploy
 from kubedeployer.deployer.abstract_deployer import AbstractDeployer
 from kubedeployer.deployer.kustomize_deployer import KustomizeDeployer
 from kubedeployer.deployer.orthodox_deployer import OrthodoxDeployer
 from kubedeployer.deployer.smart_deployer import SmartDeployer
 
 __all__ = ['run_kubedeployer']
 
+from kubedeployer.gitlab_ci import specification
+
 
 def run_kubedeployer():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-d", "--deployer",
         choices=['orthodox', 'kustomize', 'smart'],
         default='smart',
@@ -28,16 +31,43 @@
         "--env-file",
         type=str,
         nargs="+",
         action="extend",
         help="read in a file of environment variables",
     )
 
+    parser.add_argument(
+        "--project-dir",
+        type=str,
+        help="full path to folder with project",
+    )
+
+    parser.add_argument(
+        "--environment",
+        type=str,
+        help="environment for builder",
+    )
+
+    parser.add_argument(
+        "--manifest-folder",
+        type=str,
+        help="path to folder with manifest, path is relative to current working directory",
+    )
+
     args = parser.parse_args()
     deployer_type = args.deployer
+    dry_run = args.dry_run
+    if args.manifest_folder:
+        os.environ[specification.MANIFEST_FOLDER_ENV_VAR] = args.manifest_folder
+    if args.project_dir:
+        os.environ[specification.CI_PROJECT_DIR_ENV_VAR] = args.project_dir
+    if args.environment:
+        os.environ[specification.ENVIRONMENT_ENV_VAR] = args.environment
+    if dry_run:
+        os.environ[specification.CI_PROJECT_ID_ENV_VAR] = '0'
     deployer_classes = {
         'orthodox': OrthodoxDeployer,
         'kustomize': KustomizeDeployer,
         'smart': SmartDeployer
     }
     deployer: Type[AbstractDeployer] = deployer_classes[deployer_type]
-    deploy.run(deployer=deployer, dry_run=args.dry_run, env_files=args.env_file)
+    deploy.run(deployer=deployer, dry_run=dry_run, env_files=args.env_file)
```

### Comparing `kubedeployer-1.1.4/kubedeployer/deploy.py` & `kubedeployer-1.2.1/kubedeployer/deploy.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/docker.py` & `kubedeployer-1.2.1/kubedeployer/docker.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/files.py` & `kubedeployer-1.2.1/kubedeployer/files.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/kubectl.py` & `kubedeployer-1.2.1/kubedeployer/kubectl.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/kustomize.py` & `kubedeployer-1.2.1/kubedeployer/kustomize.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/manifests.py` & `kubedeployer-1.2.1/kubedeployer/manifests.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/text.py` & `kubedeployer-1.2.1/kubedeployer/text.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/console/__init__.py` & `kubedeployer-1.2.1/kubedeployer/console/__init__.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/console/wrap.py` & `kubedeployer-1.2.1/kubedeployer/console/wrap.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/deployer/kustomize_deployer.py` & `kubedeployer-1.2.1/kubedeployer/deployer/kustomize_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/deployer/orthodox_deployer.py` & `kubedeployer-1.2.1/kubedeployer/deployer/orthodox_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/deployer/smart_deployer.py` & `kubedeployer-1.2.1/kubedeployer/deployer/smart_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/gitlab_ci/environment_variables.py` & `kubedeployer-1.2.1/kubedeployer/gitlab_ci/environment_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from kubedeployer.gitlab_ci import specification
 from kubedeployer.gitlab_ci.variable_reader import AbstractVariableReader, EnvironmentVariableReader
 from kubedeployer.gitlab_ci.variable_types import StrVariable, BoolVariable, \
     IntVariable
 
 
 class Settings:
@@ -46,15 +48,16 @@
     @property
     def ci_project_dir(self) -> StrVariable:
         """
         The full path the repository is cloned to, and where the job runs from.
         If the GitLab Runner builds_dir parameter is set, this variable is set
         relative to the value of builds_dir.
         """
-        return self._variable_reader.read_str(specification.CI_PROJECT_DIR_ENV_VAR, is_required=True)
+        default_value = os.getcwd()
+        return self._variable_reader.read_str(specification.CI_PROJECT_DIR_ENV_VAR, default_value=default_value)
 
     @property
     def ci_commit_sha(self) -> StrVariable:
         """
         The commit revision the project is built for.
         """
         return self._variable_reader.read_str(specification.CI_COMMIT_SHA_ENV_VAR, is_required=True)
```

### Comparing `kubedeployer-1.1.4/kubedeployer/gitlab_ci/specification.py` & `kubedeployer-1.2.1/kubedeployer/gitlab_ci/specification.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_reader.py` & `kubedeployer-1.2.1/kubedeployer/gitlab_ci/variable_reader.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_types.py` & `kubedeployer-1.2.1/kubedeployer/gitlab_ci/variable_types.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/k8s/annotations.py` & `kubedeployer-1.2.1/kubedeployer/k8s/annotations.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/k8s/models.py` & `kubedeployer-1.2.1/kubedeployer/k8s/models.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/security/kubesec/data.py` & `kubedeployer-1.2.1/kubedeployer/security/kubesec/data.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/security/kubesec/formatters.py` & `kubedeployer-1.2.1/kubedeployer/security/kubesec/formatters.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/security/kubesec/report.py` & `kubedeployer-1.2.1/kubedeployer/security/kubesec/report.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/security/kubesec/scanner.py` & `kubedeployer-1.2.1/kubedeployer/security/kubesec/scanner.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/security/trivy/data.py` & `kubedeployer-1.2.1/kubedeployer/security/trivy/data.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/security/trivy/formatters.py` & `kubedeployer-1.2.1/kubedeployer/security/trivy/formatters.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/security/trivy/scanner.py` & `kubedeployer-1.2.1/kubedeployer/security/trivy/scanner.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/vault/client.py` & `kubedeployer-1.2.1/kubedeployer/vault/client.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/vault/factory.py` & `kubedeployer-1.2.1/kubedeployer/vault/factory.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/kubedeployer/vault/service.py` & `kubedeployer-1.2.1/kubedeployer/vault/service.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/scripts/run_e2e_tests.sh` & `kubedeployer-1.2.1/scripts/run_e2e_tests.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/conftest.py` & `kubedeployer-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/mocks.py` & `kubedeployer-1.2.1/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/containers/Dockerfile` & `kubedeployer-1.2.1/tests/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/containers/e2e_tests/e2e_entrypoint.sh` & `kubedeployer-1.2.1/tests/containers/e2e_tests/e2e_entrypoint.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/containers/kind/config.yaml` & `kubedeployer-1.2.1/tests/containers/kind/config.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/containers/kind/prepare-kind.sh` & `kubedeployer-1.2.1/tests/containers/kind/prepare-kind.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/containers/manifests/rbac.yaml` & `kubedeployer-1.2.1/tests/containers/manifests/rbac.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/env-manifest.yaml` & `kubedeployer-1.2.1/tests/data/manifests/env-manifest.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/manifests.yaml` & `kubedeployer-1.2.1/tests/data/manifests/manifests.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/apps/env-app/manifest.yaml` & `kubedeployer-1.2.1/tests/data/manifests/apps/env-app/manifest.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/apps/env-app/production/ingress.yaml` & `kubedeployer-1.2.1/tests/data/manifests/apps/env-app/production/ingress.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/deployment.yaml` & `kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml` & `kubedeployer-1.2.1/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/deployment.yaml` & `kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml` & `kubedeployer-1.2.1/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/integration/test_deployer.py` & `kubedeployer-1.2.1/tests/integration/test_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/integration/test_k8s.py` & `kubedeployer-1.2.1/tests/integration/test_k8s.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/integration/test_kubedeployer.py` & `kubedeployer-1.2.1/tests/integration/test_kubedeployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/integration/test_kustomize.py` & `kubedeployer-1.2.1/tests/integration/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/integration/test_security_kubesec.py` & `kubedeployer-1.2.1/tests/integration/test_security_kubesec.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/integration/test_security_trivy.py` & `kubedeployer-1.2.1/tests/integration/test_security_trivy.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/unit/test_console_wrap.py` & `kubedeployer-1.2.1/tests/unit/test_console_wrap.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/unit/test_deployer.py` & `kubedeployer-1.2.1/tests/unit/test_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/unit/test_files.py` & `kubedeployer-1.2.1/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/unit/test_manifests.py` & `kubedeployer-1.2.1/tests/unit/test_manifests.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/unit/test_text.py` & `kubedeployer-1.2.1/tests/unit/test_text.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/unit/test_utils_convert.py` & `kubedeployer-1.2.1/tests/unit/test_utils_convert.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/tests/unit/test_vault.py` & `kubedeployer-1.2.1/tests/unit/test_vault.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/.gitignore` & `kubedeployer-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/LICENSE` & `kubedeployer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.4/README.md` & `kubedeployer-1.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,28 @@
 * Deploy application using manifests.
 * Deploy application using kustomize.
 * Manifests can contain environment variables.
 * Contain security scanner for Kubernetes resources.
 * Contain security scanner for docker images.
 * Contain dry-run mode, where only the manifest is built without applying it.
 
-## How to build
+## Installation
+- [using pip](#using-pip)
+- [using docker](#using-docker)
+
+### Using pip
+```shell
+pip install kubedeployer
+```
+### Using docker
+```shell
+docker run itlabsio/kubedeployer
+```
+
+#### How to build
 
 ```shell
 docker build \
   --build-arg VAULT_URL=<host-to-vault> \
   --build-arg VAULT_APPROLE_ID=<vault-approle-id> \ 
   --build-arg VAULT_APPROLE_SECRET=<vault-approle-secret> \ 
   --build-arg VAULT_SECRETS_PREFIX=<vault-secret-prefix> \
```

### Comparing `kubedeployer-1.1.4/pyproject.toml` & `kubedeployer-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "kubernetes>=22.6.0",
+    "kubernetes==25.3.0",
     "PyYAML==6.0",
     "hvac==0.8.2",
     "ujson==5.4.0",
     "pydantic==1.10.2",
     "prettytable==2.5.0",
     "python-dotenv==1.0.0",
 ]
```

### Comparing `kubedeployer-1.1.4/PKG-INFO` & `kubedeployer-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubedeployer
-Version: 1.1.4
+Version: 1.2.1
 Summary: package to deploy application on kubernetes
 Project-URL: Homepage, https://github.com/itlabsio/kubedeployer
 Project-URL: Bug Tracker, https://github.com/itlabsio/kubedeployer/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -208,15 +208,15 @@
 License-File: LICENSE
 Keywords: deploy,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: hvac==0.8.2
-Requires-Dist: kubernetes>=22.6.0
+Requires-Dist: kubernetes==25.3.0
 Requires-Dist: prettytable==2.5.0
 Requires-Dist: pydantic==1.10.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: pyyaml==6.0
 Requires-Dist: ujson==5.4.0
 Description-Content-Type: text/markdown
 
@@ -229,15 +229,28 @@
 * Deploy application using manifests.
 * Deploy application using kustomize.
 * Manifests can contain environment variables.
 * Contain security scanner for Kubernetes resources.
 * Contain security scanner for docker images.
 * Contain dry-run mode, where only the manifest is built without applying it.
 
-## How to build
+## Installation
+- [using pip](#using-pip)
+- [using docker](#using-docker)
+
+### Using pip
+```shell
+pip install kubedeployer
+```
+### Using docker
+```shell
+docker run itlabsio/kubedeployer
+```
+
+#### How to build
 
 ```shell
 docker build \
   --build-arg VAULT_URL=<host-to-vault> \
   --build-arg VAULT_APPROLE_ID=<vault-approle-id> \ 
   --build-arg VAULT_APPROLE_SECRET=<vault-approle-secret> \ 
   --build-arg VAULT_SECRETS_PREFIX=<vault-secret-prefix> \
```

