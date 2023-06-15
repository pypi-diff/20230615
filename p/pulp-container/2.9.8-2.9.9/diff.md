# Comparing `tmp/pulp-container-2.9.8.tar.gz` & `tmp/pulp-container-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-container-2.9.8.tar", last modified: Wed Sep 14 12:56:46 2022, max compression
+gzip compressed data, was "pulp-container-2.9.9.tar", last modified: Thu Oct 20 21:49:23 2022, max compression
```

## Comparing `pulp-container-2.9.8.tar` & `pulp-container-2.9.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.270754 pulp-container-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    29487 2022-09-14 12:56:45.000000 pulp-container-2.9.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-09-14 12:56:36.000000 pulp-container-2.9.8/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-14 12:56:36.000000 pulp-container-2.9.8/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)    18046 2022-09-14 12:56:36.000000 pulp-container-2.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-14 12:56:36.000000 pulp-container-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-09-14 12:56:46.266754 pulp-container-2.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-09-14 12:56:36.000000 pulp-container-2.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-14 12:56:36.000000 pulp-container-2.9.8/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.258754 pulp-container-2.9.8/pulp_container/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.262754 pulp-container-2.9.8/pulp_container/app/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-14 12:56:45.000000 pulp-container-2.9.8/pulp_container/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5163 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/access_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     8942 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/authorization.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     6789 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/downloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.262754 pulp-container-2.9.8/pulp_container/app/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.262754 pulp-container-2.9.8/pulp_container/app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/management/commands/container-repair-media-type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.262754 pulp-container-2.9.8/pulp_container/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0002_containerrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0003_oci_mediatype.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0004_upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0005_contentredirectcontentguard.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0006_containerpushrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0007_clear_tags_artifacts_refs.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0008_include_exclude_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0009_container_namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0010_remove_uploadchunk.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0011_add_container_repository_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0012_add_container_namespace_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0013_add_pull_push_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0014_containerdistribution_private.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0015_manage_tags_push_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0016_add_delete_versions_permission.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0017_add_granular_perms.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0018_containerdistribution_description.py
--rw-r--r--   0 runner    (1001) docker     (121)     4502 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0019_DATA_distribution_model_swap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/0020_update_push_repo_perms.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/modelresource.py
--rw-r--r--   0 runner    (1001) docker     (121)    22716 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4805 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/redirects.py
--rw-r--r--   0 runner    (1001) docker     (121)     9545 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    34086 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/registry_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    12012 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/schema_convert.py
--rw-r--r--   0 runner    (1001) docker     (121)    22659 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5445 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/recursive_add.py
--rw-r--r--   0 runner    (1001) docker     (121)     5277 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/recursive_remove.py
--rw-r--r--   0 runner    (1001) docker     (121)    21187 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/sync_stages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/synchronize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/tasks/untag.py
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/token_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    51194 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/app/webserver_snippets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/webserver_snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/webserver_snippets/apache.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/app/webserver_snippets/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/rbac_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4578 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)    10399 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_crud_distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (121)    21146 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_pull_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     4265 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_pulpimportexport.py
--rw-r--r--   0 runner    (1001) docker     (121)    13412 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_push_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_push_repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_remotes.py
--rw-r--r--   0 runner    (1001) docker     (121)     8943 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_repo_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     9060 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_repo_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_sync_repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)    30238 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_recursive_add.py
--rw-r--r--   0 runner    (1001) docker     (121)    21983 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_recursive_remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     8543 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_repositories_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)    10892 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_tagging_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     6267 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/api/test_token_authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     9491 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7412 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/unit/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/unit/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/tests/upgrade/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/tests/upgrade/post/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/upgrade/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5140 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/upgrade/post/test_pull_content.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.266754 pulp-container-2.9.8/pulp_container/tests/upgrade/pre/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/upgrade/pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pulp_container/tests/upgrade/pre/test_pull_content.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 12:56:46.262754 pulp-container-2.9.8/pulp_container.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-09-14 12:56:46.000000 pulp-container-2.9.8/pulp_container.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-09-14 12:56:46.000000 pulp-container-2.9.8/pulp_container.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 12:56:46.000000 pulp-container-2.9.8/pulp_container.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-14 12:56:46.000000 pulp-container-2.9.8/pulp_container.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-14 12:56:46.000000 pulp-container-2.9.8/pulp_container.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-14 12:56:46.000000 pulp-container-2.9.8/pulp_container.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-14 12:56:36.000000 pulp-container-2.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-14 12:56:36.000000 pulp-container-2.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 12:56:46.270754 pulp-container-2.9.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1177 2022-09-14 12:56:45.000000 pulp-container-2.9.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-14 12:56:36.000000 pulp-container-2.9.8/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-14 12:56:36.000000 pulp-container-2.9.8/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.488934 pulp-container-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    29704 2022-10-20 21:49:22.000000 pulp-container-2.9.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-10-20 21:49:09.000000 pulp-container-2.9.9/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-10-20 21:49:09.000000 pulp-container-2.9.9/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (121)    18046 2022-10-20 21:49:09.000000 pulp-container-2.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-10-20 21:49:09.000000 pulp-container-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-10-20 21:49:23.488934 pulp-container-2.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-10-20 21:49:09.000000 pulp-container-2.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-20 21:49:09.000000 pulp-container-2.9.9/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.480934 pulp-container-2.9.9/pulp_container/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.484934 pulp-container-2.9.9/pulp_container/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-20 21:49:22.000000 pulp-container-2.9.9/pulp_container/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5163 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8942 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6789 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/downloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.484934 pulp-container-2.9.9/pulp_container/app/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.484934 pulp-container-2.9.9/pulp_container/app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/management/commands/container-repair-media-type.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.484934 pulp-container-2.9.9/pulp_container/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0002_containerrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0003_oci_mediatype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0004_upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0005_contentredirectcontentguard.py
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0006_containerpushrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0007_clear_tags_artifacts_refs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0008_include_exclude_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0009_container_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0010_remove_uploadchunk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0011_add_container_repository_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0012_add_container_namespace_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0013_add_pull_push_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0014_containerdistribution_private.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0015_manage_tags_push_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0016_add_delete_versions_permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0017_add_granular_perms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0018_containerdistribution_description.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4502 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0019_DATA_distribution_model_swap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/0020_update_push_repo_perms.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/modelresource.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22688 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4805 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/redirects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9545 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34086 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12012 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/schema_convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22659 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.484934 pulp-container-2.9.9/pulp_container/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5445 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/recursive_add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5277 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/recursive_remove.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21187 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/sync_stages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/synchronize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/tasks/untag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/token_verification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51194 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.484934 pulp-container-2.9.9/pulp_container/app/webserver_snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/webserver_snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/webserver_snippets/apache.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/app/webserver_snippets/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.484934 pulp-container-2.9.9/pulp_container/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.488934 pulp-container-2.9.9/pulp_container/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.488934 pulp-container-2.9.9/pulp_container/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/rbac_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4578 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10399 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_crud_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21146 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_pull_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4265 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_pulpimportexport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13505 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_push_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_push_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8943 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_repo_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9060 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_repo_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_sync_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30238 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_recursive_add.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21983 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_recursive_remove.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8543 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_repositories_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10892 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_tagging_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6267 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/api/test_token_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9538 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.488934 pulp-container-2.9.9/pulp_container/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7412 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/unit/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/unit/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.488934 pulp-container-2.9.9/pulp_container/tests/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.488934 pulp-container-2.9.9/pulp_container/tests/upgrade/post/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/upgrade/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5140 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/upgrade/post/test_pull_content.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.488934 pulp-container-2.9.9/pulp_container/tests/upgrade/pre/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/upgrade/pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pulp_container/tests/upgrade/pre/test_pull_content.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:49:23.480934 pulp-container-2.9.9/pulp_container.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-10-20 21:49:23.000000 pulp-container-2.9.9/pulp_container.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-10-20 21:49:23.000000 pulp-container-2.9.9/pulp_container.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 21:49:23.000000 pulp-container-2.9.9/pulp_container.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-20 21:49:23.000000 pulp-container-2.9.9/pulp_container.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-20 21:49:23.000000 pulp-container-2.9.9/pulp_container.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-20 21:49:23.000000 pulp-container-2.9.9/pulp_container.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-10-20 21:49:09.000000 pulp-container-2.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-20 21:49:09.000000 pulp-container-2.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 21:49:23.488934 pulp-container-2.9.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1177 2022-10-20 21:49:22.000000 pulp-container-2.9.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-20 21:49:09.000000 pulp-container-2.9.9/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-20 21:49:09.000000 pulp-container-2.9.9/unittest_requirements.txt
```

### Comparing `pulp-container-2.9.8/CHANGES.rst` & `pulp-container-2.9.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,28 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+2.9.9 (2022-10-20)
+==================
+
+
+Bugfixes
+--------
+
+- Fixed a database error raised when creating a distribution with a long base_path.
+  `#1103 <https://github.com/pulp/pulp_container/issues/1103>`__
+
+
+----
+
+
 2.9.8 (2022-09-14)
 ==================
 
 
 Bugfixes
 --------
```

### Comparing `pulp-container-2.9.8/COMMITMENT` & `pulp-container-2.9.9/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/COPYRIGHT` & `pulp-container-2.9.9/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/LICENSE` & `pulp-container-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/PKG-INFO` & `pulp-container-2.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pulp-container
-Version: 2.9.8
+Version: 2.9.9
 Summary: Container plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
-Description: ``pulp_container`` Plugin
-        =========================
-        
-        .. figure:: https://github.com/pulp/pulp_container/workflows/Pulp%20CI/badge.svg
-         :alt: Pulp CI
-        
-        This is the ``pulp_container`` Plugin for `Pulp Project
-        3.0+ <https://pypi.python.org/pypi/pulpcore/>`__. This plugin provides Pulp with support for container
-        images, similar to the pulp_docker plugin for Pulp 2.
-        
-        For more information, please see the `documentation
-        <https://docs.pulpproject.org/pulp_container/>`_ or the `Pulp project page
-        <https://pulpproject.org>`_.
-        
-        How to File an Issue
-        --------------------
-        
-        `New pulp_container issue <https://pulp.plan.io/projects/pulp_container/issues/new>`_.
-        
-        .. warning::
-          Is this security related? If so, please follow the `Security Disclosures <https://docs.pulpproject.org/pulpcore/bugs-features.html#security-bugs>`_ procedure.
-        
-        Please set **only the fields in this table**. See `Redmine Fields <https://docs.pulpproject.org/pulpcore/bugs-features.html#redmine-fields>`_ for more detailed
-        descriptions of all the fields and how they are used.
-        
-        .. list-table::
-           :header-rows: 1
-           :widths: auto
-           :align: center
-        
-           * - Field
-             - Instructions
-        
-           * - Tracker
-             - For a bug, select ``Issue``, for a feature-request, choose ``Story``,
-               for a backport request, choose ``Backport``.
-        
-           * - Subject
-             - Strive to be specific and concise.
-        
-           * - Description
-             - This is the most important part! Please see `Description Field <https://docs.pulpproject.org/pulpcore/bugs-features.html#issue-description>`_.
-        
-           * - Category
-             - Choose one if applicable, blank is OK.
-        
-           * - Version
-             - The version of pulp_container that you discovered the issue.
-        
-           * - OS
-             - Please select your operating system.
-        
-           * - Tags
-             - For searching. Select 0 or many, best judgement.
-               If an issue requires a functional test. Add the tag `Functional test`.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+``pulp_container`` Plugin
+=========================
+
+.. figure:: https://github.com/pulp/pulp_container/workflows/Pulp%20CI/badge.svg
+ :alt: Pulp CI
+
+This is the ``pulp_container`` Plugin for `Pulp Project
+3.0+ <https://pypi.python.org/pypi/pulpcore/>`__. This plugin provides Pulp with support for container
+images, similar to the pulp_docker plugin for Pulp 2.
+
+For more information, please see the `documentation
+<https://docs.pulpproject.org/pulp_container/>`_ or the `Pulp project page
+<https://pulpproject.org>`_.
+
+How to File an Issue
+--------------------
+
+`New pulp_container issue <https://pulp.plan.io/projects/pulp_container/issues/new>`_.
+
+.. warning::
+  Is this security related? If so, please follow the `Security Disclosures <https://docs.pulpproject.org/pulpcore/bugs-features.html#security-bugs>`_ procedure.
+
+Please set **only the fields in this table**. See `Redmine Fields <https://docs.pulpproject.org/pulpcore/bugs-features.html#redmine-fields>`_ for more detailed
+descriptions of all the fields and how they are used.
+
+.. list-table::
+   :header-rows: 1
+   :widths: auto
+   :align: center
+
+   * - Field
+     - Instructions
+
+   * - Tracker
+     - For a bug, select ``Issue``, for a feature-request, choose ``Story``,
+       for a backport request, choose ``Backport``.
+
+   * - Subject
+     - Strive to be specific and concise.
+
+   * - Description
+     - This is the most important part! Please see `Description Field <https://docs.pulpproject.org/pulpcore/bugs-features.html#issue-description>`_.
+
+   * - Category
+     - Choose one if applicable, blank is OK.
+
+   * - Version
+     - The version of pulp_container that you discovered the issue.
+
+   * - OS
+     - Please select your operating system.
+
+   * - Tags
+     - For searching. Select 0 or many, best judgement.
+       If an issue requires a functional test. Add the tag `Functional test`.
```

### Comparing `pulp-container-2.9.8/README.rst` & `pulp-container-2.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/access_policy.py` & `pulp-container-2.9.9/pulp_container/app/access_policy.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/authorization.py` & `pulp-container-2.9.9/pulp_container/app/authorization.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/downloaders.py` & `pulp-container-2.9.9/pulp_container/app/downloaders.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/management/commands/container-repair-media-type.py` & `pulp-container-2.9.9/pulp_container/app/management/commands/container-repair-media-type.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0001_initial.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0002_containerrepository.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0002_containerrepository.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0003_oci_mediatype.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0003_oci_mediatype.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0004_upload.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0004_upload.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0005_contentredirectcontentguard.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0005_contentredirectcontentguard.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0006_containerpushrepository.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0006_containerpushrepository.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0007_clear_tags_artifacts_refs.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0007_clear_tags_artifacts_refs.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0008_include_exclude_tags.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0008_include_exclude_tags.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0009_container_namespace.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0009_container_namespace.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0010_remove_uploadchunk.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0010_remove_uploadchunk.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0011_add_container_repository_permissions.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0011_add_container_repository_permissions.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0013_add_pull_push_permissions.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0013_add_pull_push_permissions.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0014_containerdistribution_private.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0014_containerdistribution_private.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0015_manage_tags_push_repo.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0015_manage_tags_push_repo.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0016_add_delete_versions_permission.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0016_add_delete_versions_permission.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0017_add_granular_perms.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0017_add_granular_perms.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0019_DATA_distribution_model_swap.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0019_DATA_distribution_model_swap.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/migrations/0020_update_push_repo_perms.py` & `pulp-container-2.9.9/pulp_container/app/migrations/0020_update_push_repo_perms.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/modelresource.py` & `pulp-container-2.9.9/pulp_container/app/modelresource.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/models.py` & `pulp-container-2.9.9/pulp_container/app/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,33 +220,31 @@
 
         The permissions are object level permissions assigned to the group.
         """
 
         group_type = parameters["group_type"]
         add_user_to_group = parameters["add_user_to_group"]
         group = Group.objects.create(
-            name="{}.{}.{}".format("container.namespace", group_type, self.name)
+            name="{}.{}.{}".format("container.namespace", group_type, self.pk)
         )
         current_user = get_current_authenticated_user()
-        owners_group = Group.objects.get(
-            name="{}.{}".format("container.namespace.owners", self.name)
-        )
+        owners_group = Group.objects.get(name="{}.{}".format("container.namespace.owners", self.pk))
         assign_perm("auth.change_group", owners_group, group)
         assign_perm("auth.view_group", owners_group, group)
         if add_user_to_group:
             current_user.groups.add(group)
         self.add_for_groups(permissions, group.name)
 
     @hook("before_delete")
     def delete_groups_and_user_obj_perms(self):
         """
         Delete all auto created groups associated with this Namespace and user object
         permissions.
         """
-        group_name_regex = r"container.namespace.(.*).{}".format(self.name)
+        group_name_regex = r"container.namespace.(.*).{}".format(self.pk)
         Group.objects.filter(name__regex=group_name_regex).delete()
         UserObjectPermission.objects.filter(object_pk=self.pk).delete()
         GroupObjectPermission.objects.filter(object_pk=self.pk).delete()
 
     class Meta:
         unique_together = (("name",),)
         permissions = [
```

### Comparing `pulp-container-2.9.8/pulp_container/app/redirects.py` & `pulp-container-2.9.9/pulp_container/app/redirects.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/registry.py` & `pulp-container-2.9.9/pulp_container/app/registry.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/registry_api.py` & `pulp-container-2.9.9/pulp_container/app/registry_api.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/schema_convert.py` & `pulp-container-2.9.9/pulp_container/app/schema_convert.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/serializers.py` & `pulp-container-2.9.9/pulp_container/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/base.py` & `pulp-container-2.9.9/pulp_container/app/tasks/base.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/builder.py` & `pulp-container-2.9.9/pulp_container/app/tasks/builder.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/recursive_add.py` & `pulp-container-2.9.9/pulp_container/app/tasks/recursive_add.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/recursive_remove.py` & `pulp-container-2.9.9/pulp_container/app/tasks/recursive_remove.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/sync_stages.py` & `pulp-container-2.9.9/pulp_container/app/tasks/sync_stages.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/synchronize.py` & `pulp-container-2.9.9/pulp_container/app/tasks/synchronize.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/tag.py` & `pulp-container-2.9.9/pulp_container/app/tasks/tag.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/tasks/untag.py` & `pulp-container-2.9.9/pulp_container/app/tasks/untag.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/token_verification.py` & `pulp-container-2.9.9/pulp_container/app/token_verification.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/urls.py` & `pulp-container-2.9.9/pulp_container/app/urls.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/utils.py` & `pulp-container-2.9.9/pulp_container/app/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/viewsets.py` & `pulp-container-2.9.9/pulp_container/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/app/webserver_snippets/nginx.conf` & `pulp-container-2.9.9/pulp_container/app/webserver_snippets/nginx.conf`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/constants.py` & `pulp-container-2.9.9/pulp_container/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/rbac_base.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/rbac_base.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_crud_content_unit.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_crud_content_unit.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_crud_distributions.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_crud_distributions.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_crud_remotes.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_pull_content.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_pull_content.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_pulpimportexport.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_pulpimportexport.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_push_content.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_push_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             distributions.results[0],
             "consumers",
             self.user_creator,
         )
 
         add_user_to_namespace_group(
             self.user_namespace_collaborator,
-            "test",
+            distributions.results[0].namespace,
             "collaborators",
             self.user_creator,
         )
 
         self.assertEqual(self.pushrepository_api.list(name=repo_name).count, 1)
         self.assertEqual(self.user_creator["pushrepository_api"].list(name=repo_name).count, 1)
         self.assertEqual(
@@ -206,15 +206,18 @@
         collab_repo_name = "team/collab"
         local_url = "/".join([self.registry_name, f"{collab_repo_name}:2.0"])
         image_path = f"{REGISTRY_V2_REPO_PULP}:manifest_d"
         with self.assertRaises(exceptions.CalledProcessError):
             self._push(image_path, local_url, self.user_dist_collaborator)
 
         add_user_to_namespace_group(
-            self.user_namespace_collaborator, "team", "collaborators", self.user_creator
+            self.user_namespace_collaborator,
+            distributions.results[0].namespace,
+            "collaborators",
+            self.user_creator,
         )
 
         collab_repo_name = "team/collab"
         local_url = "/".join([self.registry_name, f"{collab_repo_name}:2.0"])
         image_path = f"{REGISTRY_V2_REPO_PULP}:manifest_c"
         self._push(image_path, local_url, self.user_namespace_collaborator)
```

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_push_repositories.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_push_repositories.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_remotes.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_repo_content.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_repo_content.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_repo_versions.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_repo_versions.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_rbac_sync_repositories.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_rbac_sync_repositories.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_recursive_add.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_recursive_add.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_recursive_remove.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_recursive_remove.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_repositories_list.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_repositories_list.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_sync.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_tagging_images.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_tagging_images.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/api/test_token_authentication.py` & `pulp-container-2.9.9/pulp_container/tests/functional/api/test_token_authentication.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/constants.py` & `pulp-container-2.9.9/pulp_container/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/functional/utils.py` & `pulp-container-2.9.9/pulp_container/tests/functional/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,19 +127,20 @@
         as_user["groups_api"]
         .list(name="container.distribution.{}.{}".format(group_type, distribution_pk))
         .results[0]
     )
     as_user["group_users_api"].create(collaborator_group.pulp_href, {"username": user["username"]})
 
 
-def add_user_to_namespace_group(user, namespace_name, group_type, as_user):
+def add_user_to_namespace_group(user, namespace_href, group_type, as_user):
     """Add the user to either owner, collaborator, or consumer group of a namespace."""
+    namespace_pk = namespace_href.split("/")[-2]
     namespace_collaborator_group = (
         as_user["groups_api"]
-        .list(name="container.namespace.{}.{}".format(group_type, namespace_name))
+        .list(name="container.namespace.{}.{}".format(group_type, namespace_pk))
         .results[0]
     )
     as_user["group_users_api"].create(
         namespace_collaborator_group.pulp_href,
         {"username": user["username"]},
     )
```

### Comparing `pulp-container-2.9.8/pulp_container/tests/unit/test_convert.py` & `pulp-container-2.9.9/pulp_container/tests/unit/test_convert.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/unit/test_serializers.py` & `pulp-container-2.9.9/pulp_container/tests/unit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/upgrade/post/test_pull_content.py` & `pulp-container-2.9.9/pulp_container/tests/upgrade/post/test_pull_content.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container/tests/upgrade/pre/test_pull_content.py` & `pulp-container-2.9.9/pulp_container/tests/upgrade/pre/test_pull_content.py`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pulp_container.egg-info/PKG-INFO` & `pulp-container-2.9.9/pulp_container.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pulp-container
-Version: 2.9.8
+Version: 2.9.9
 Summary: Container plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
-Description: ``pulp_container`` Plugin
-        =========================
-        
-        .. figure:: https://github.com/pulp/pulp_container/workflows/Pulp%20CI/badge.svg
-         :alt: Pulp CI
-        
-        This is the ``pulp_container`` Plugin for `Pulp Project
-        3.0+ <https://pypi.python.org/pypi/pulpcore/>`__. This plugin provides Pulp with support for container
-        images, similar to the pulp_docker plugin for Pulp 2.
-        
-        For more information, please see the `documentation
-        <https://docs.pulpproject.org/pulp_container/>`_ or the `Pulp project page
-        <https://pulpproject.org>`_.
-        
-        How to File an Issue
-        --------------------
-        
-        `New pulp_container issue <https://pulp.plan.io/projects/pulp_container/issues/new>`_.
-        
-        .. warning::
-          Is this security related? If so, please follow the `Security Disclosures <https://docs.pulpproject.org/pulpcore/bugs-features.html#security-bugs>`_ procedure.
-        
-        Please set **only the fields in this table**. See `Redmine Fields <https://docs.pulpproject.org/pulpcore/bugs-features.html#redmine-fields>`_ for more detailed
-        descriptions of all the fields and how they are used.
-        
-        .. list-table::
-           :header-rows: 1
-           :widths: auto
-           :align: center
-        
-           * - Field
-             - Instructions
-        
-           * - Tracker
-             - For a bug, select ``Issue``, for a feature-request, choose ``Story``,
-               for a backport request, choose ``Backport``.
-        
-           * - Subject
-             - Strive to be specific and concise.
-        
-           * - Description
-             - This is the most important part! Please see `Description Field <https://docs.pulpproject.org/pulpcore/bugs-features.html#issue-description>`_.
-        
-           * - Category
-             - Choose one if applicable, blank is OK.
-        
-           * - Version
-             - The version of pulp_container that you discovered the issue.
-        
-           * - OS
-             - Please select your operating system.
-        
-           * - Tags
-             - For searching. Select 0 or many, best judgement.
-               If an issue requires a functional test. Add the tag `Functional test`.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+``pulp_container`` Plugin
+=========================
+
+.. figure:: https://github.com/pulp/pulp_container/workflows/Pulp%20CI/badge.svg
+ :alt: Pulp CI
+
+This is the ``pulp_container`` Plugin for `Pulp Project
+3.0+ <https://pypi.python.org/pypi/pulpcore/>`__. This plugin provides Pulp with support for container
+images, similar to the pulp_docker plugin for Pulp 2.
+
+For more information, please see the `documentation
+<https://docs.pulpproject.org/pulp_container/>`_ or the `Pulp project page
+<https://pulpproject.org>`_.
+
+How to File an Issue
+--------------------
+
+`New pulp_container issue <https://pulp.plan.io/projects/pulp_container/issues/new>`_.
+
+.. warning::
+  Is this security related? If so, please follow the `Security Disclosures <https://docs.pulpproject.org/pulpcore/bugs-features.html#security-bugs>`_ procedure.
+
+Please set **only the fields in this table**. See `Redmine Fields <https://docs.pulpproject.org/pulpcore/bugs-features.html#redmine-fields>`_ for more detailed
+descriptions of all the fields and how they are used.
+
+.. list-table::
+   :header-rows: 1
+   :widths: auto
+   :align: center
+
+   * - Field
+     - Instructions
+
+   * - Tracker
+     - For a bug, select ``Issue``, for a feature-request, choose ``Story``,
+       for a backport request, choose ``Backport``.
+
+   * - Subject
+     - Strive to be specific and concise.
+
+   * - Description
+     - This is the most important part! Please see `Description Field <https://docs.pulpproject.org/pulpcore/bugs-features.html#issue-description>`_.
+
+   * - Category
+     - Choose one if applicable, blank is OK.
+
+   * - Version
+     - The version of pulp_container that you discovered the issue.
+
+   * - OS
+     - Please select your operating system.
+
+   * - Tags
+     - For searching. Select 0 or many, best judgement.
+       If an issue requires a functional test. Add the tag `Functional test`.
```

### Comparing `pulp-container-2.9.8/pulp_container.egg-info/SOURCES.txt` & `pulp-container-2.9.9/pulp_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/pyproject.toml` & `pulp-container-2.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-container-2.9.8/setup.py` & `pulp-container-2.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="pulp-container",
-    version="2.9.8",
+    version="2.9.9",
     description="Container plugin for the Pulp Project",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Team",
     author_email="pulp-list@redhat.com",
     url="https://pulpproject.org/",
     python_requires=">=3.8",
```

