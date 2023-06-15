# Comparing `tmp/pulp_container-client-2.9.8.tar.gz` & `tmp/pulp_container-client-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_container-client-2.9.8.tar", last modified: Wed Sep 14 13:01:31 2022, max compression
+gzip compressed data, was "pulp_container-client-2.9.9.tar", last modified: Thu Oct 20 21:54:17 2022, max compression
```

## Comparing `pulp_container-client-2.9.8.tar` & `pulp_container-client-2.9.9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.893361 pulp_container-client-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-14 13:01:31.893361 pulp_container-client-2.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17610 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.857361 pulp_container-client-2.9.8/pulp_container_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-09-14 13:01:30.000000 pulp_container-client-2.9.8/pulp_container_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7252 2022-09-14 13:01:31.000000 pulp_container-client-2.9.8/pulp_container_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 13:01:30.000000 pulp_container-client-2.9.8/pulp_container_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-14 13:01:30.000000 pulp_container-client-2.9.8/pulp_container_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-14 13:01:30.000000 pulp_container-client-2.9.8/pulp_container_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.857361 pulp_container-client-2.9.8/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.857361 pulp_container-client-2.9.8/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.861361 pulp_container-client-2.9.8/pulpcore/client/pulp_container/
--rw-r--r--   0 runner    (1001) docker     (121)     7145 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.869361 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15376 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/content_blobs_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    15500 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/content_manifests_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    15725 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/content_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    41383 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/contentguards_content_redirect_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    43538 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/distributions_container_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26269 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/pulp_container_namespaces_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    44096 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/remotes_container_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    92640 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    49962 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_push_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    34196 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_push_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    32688 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/token_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26304 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13978 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.885361 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/
--rw-r--r--   0 runner    (1001) docker     (121)     5426 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7191 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_blob_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    10470 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    14473 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     5536 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_namespace_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6921 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_push_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)    10682 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_push_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    27886 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    26959 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)    11362 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_content_redirect_content_guard.py
--rw-r--r--   0 runner    (1001) docker     (121)     6418 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_content_redirect_content_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    11456 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_manifest_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6205 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     5305 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/manifest_copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/media_types_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/oci_build_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     5681 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5589 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_blob_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5980 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5911 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_namespace_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_push_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5842 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6118 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_content_redirect_content_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5681 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_manifest_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_tag_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    10409 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     6907 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_push_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)    28116 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     7647 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_content_redirect_content_guard.py
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     3609 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/recursive_manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/remove_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     4487 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7921 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5447 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/tag_copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/tag_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/un_tag_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    12317 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/pulpcore/client/pulp_container/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-14 13:01:31.893361 pulp_container-client-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 13:01:31.893361 pulp_container-client-2.9.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_blob_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_namespace_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_push_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_push_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_container_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_content_redirect_content_guard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_content_redirect_content_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_manifest_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_container_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_content_blobs_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_content_manifests_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_content_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_contentguards_content_redirect_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_distributions_container_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_manifest_copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_media_types_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_oci_build_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_blob_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_container_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_container_namespace_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_container_push_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_container_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_container_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_content_redirect_content_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_manifest_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_paginatedcontainer_tag_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_patchedcontainer_container_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_patchedcontainer_container_push_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_patchedcontainer_container_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_patchedcontainer_container_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_patchedcontainer_content_redirect_content_guard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_pulp_container_namespaces_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_recursive_manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_remotes_container_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_remove_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_repositories_container_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_repositories_container_push_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_repositories_container_push_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_repositories_container_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_tag_copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_tag_image.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-09-14 13:01:28.000000 pulp_container-client-2.9.8/test/test_token_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-09-14 13:01:27.000000 pulp_container-client-2.9.8/test/test_un_tag_image.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.096225 pulp_container-client-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-10-20 21:54:17.096225 pulp_container-client-2.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17610 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.064224 pulp_container-client-2.9.9/pulp_container_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-10-20 21:54:17.000000 pulp_container-client-2.9.9/pulp_container_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7252 2022-10-20 21:54:17.000000 pulp_container-client-2.9.9/pulp_container_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 21:54:17.000000 pulp_container-client-2.9.9/pulp_container_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-20 21:54:17.000000 pulp_container-client-2.9.9/pulp_container_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-20 21:54:17.000000 pulp_container-client-2.9.9/pulp_container_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.064224 pulp_container-client-2.9.9/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.064224 pulp_container-client-2.9.9/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.064224 pulp_container-client-2.9.9/pulpcore/client/pulp_container/
+-rw-r--r--   0 runner    (1001) docker     (121)     7145 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.068224 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15376 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/content_blobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15500 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/content_manifests_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15725 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/content_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41383 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/contentguards_content_redirect_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43538 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/distributions_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26269 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/pulp_container_namespaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44096 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/remotes_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    92640 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49962 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34196 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_push_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32688 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/token_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26304 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13978 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.084225 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     5426 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7191 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_blob_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10470 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14473 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5536 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_namespace_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6921 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_push_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10682 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_push_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27886 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26959 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11362 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4547 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_content_redirect_content_guard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6418 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_content_redirect_content_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11456 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_manifest_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6205 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5305 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/manifest_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/media_types_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/oci_build_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5681 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5589 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_blob_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5980 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5911 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_namespace_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_push_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5842 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6118 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_content_redirect_content_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5681 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_manifest_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_tag_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10409 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6907 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_push_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28116 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7647 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_content_redirect_content_guard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3609 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/recursive_manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/remove_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4487 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7921 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5447 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/tag_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/tag_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/un_tag_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12317 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/pulpcore/client/pulp_container/rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-20 21:54:17.096225 pulp_container-client-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:54:17.096225 pulp_container-client-2.9.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_blob_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_namespace_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_push_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_push_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_container_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_content_redirect_content_guard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_content_redirect_content_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_manifest_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_container_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_content_blobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_content_manifests_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_content_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_contentguards_content_redirect_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_distributions_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_manifest_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_media_types_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_oci_build_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_blob_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_container_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_container_namespace_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_container_push_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_container_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_container_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2552 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_content_redirect_content_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_manifest_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_paginatedcontainer_tag_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_patchedcontainer_container_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_patchedcontainer_container_push_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_patchedcontainer_container_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_patchedcontainer_container_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_patchedcontainer_content_redirect_content_guard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_pulp_container_namespaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_recursive_manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_remotes_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_remove_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_repositories_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_repositories_container_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_repositories_container_push_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_repositories_container_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_tag_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_tag_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-10-20 21:54:16.000000 pulp_container-client-2.9.9/test/test_token_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-10-20 21:54:15.000000 pulp_container-client-2.9.9/test/test_un_tag_image.py
```

### Comparing `pulp_container-client-2.9.8/README.md` & `pulp_container-client-2.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_container-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 2.9.8
+- Package version: 2.9.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_container-client-2.9.8/pulp_container_client.egg-info/SOURCES.txt` & `pulp_container-client-2.9.9/pulp_container_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/__init__.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.9.8"
+__version__ = "2.9.9"
 
 # import apis into sdk package
 from pulpcore.client.pulp_container.api.content_blobs_api import ContentBlobsApi
 from pulpcore.client.pulp_container.api.content_manifests_api import ContentManifestsApi
 from pulpcore.client.pulp_container.api.content_tags_api import ContentTagsApi
 from pulpcore.client.pulp_container.api.contentguards_content_redirect_api import ContentguardsContentRedirectApi
 from pulpcore.client.pulp_container.api.distributions_container_api import DistributionsContainerApi
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/__init__.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/content_blobs_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/content_blobs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/content_manifests_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/content_manifests_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/content_tags_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/content_tags_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/contentguards_content_redirect_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/contentguards_content_redirect_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/distributions_container_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/distributions_container_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/pulp_container_namespaces_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/pulp_container_namespaces_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/remotes_container_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/remotes_container_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_push_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_push_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_push_versions_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_push_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/repositories_container_versions_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/repositories_container_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api/token_api.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api/token_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/api_client.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.9.8/python'
+        self.user_agent = 'OpenAPI-Generator/2.9.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/configuration.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 2.9.8".\
+               "SDK Package Version: 2.9.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/exceptions.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/__init__.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/async_operation_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_blob_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_blob_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_distribution.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,87 +30,64 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'content_guard': 'str',
         'base_path': 'str',
+        'content_guard': 'str',
         'repository': 'str',
-        'pulp_labels': 'object',
         'name': 'str',
+        'pulp_labels': 'object',
         'repository_version': 'str',
         'private': 'bool',
         'description': 'str'
     }
 
     attribute_map = {
-        'content_guard': 'content_guard',
         'base_path': 'base_path',
+        'content_guard': 'content_guard',
         'repository': 'repository',
-        'pulp_labels': 'pulp_labels',
         'name': 'name',
+        'pulp_labels': 'pulp_labels',
         'repository_version': 'repository_version',
         'private': 'private',
         'description': 'description'
     }
 
-    def __init__(self, content_guard=None, base_path=None, repository=None, pulp_labels=None, name=None, repository_version=None, private=None, description=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, base_path=None, content_guard=None, repository=None, name=None, pulp_labels=None, repository_version=None, private=None, description=None, local_vars_configuration=None):  # noqa: E501
         """ContainerContainerDistribution - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._content_guard = None
         self._base_path = None
+        self._content_guard = None
         self._repository = None
-        self._pulp_labels = None
         self._name = None
+        self._pulp_labels = None
         self._repository_version = None
         self._private = None
         self._description = None
         self.discriminator = None
 
+        self.base_path = base_path
         if content_guard is not None:
             self.content_guard = content_guard
-        self.base_path = base_path
         self.repository = repository
+        self.name = name
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
-        self.name = name
         self.repository_version = repository_version
         if private is not None:
             self.private = private
         self.description = description
 
     @property
-    def content_guard(self):
-        """Gets the content_guard of this ContainerContainerDistribution.  # noqa: E501
-
-        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
-
-        :return: The content_guard of this ContainerContainerDistribution.  # noqa: E501
-        :rtype: str
-        """
-        return self._content_guard
-
-    @content_guard.setter
-    def content_guard(self, content_guard):
-        """Sets the content_guard of this ContainerContainerDistribution.
-
-        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
-
-        :param content_guard: The content_guard of this ContainerContainerDistribution.  # noqa: E501
-        :type: str
-        """
-
-        self._content_guard = content_guard
-
-    @property
     def base_path(self):
         """Gets the base_path of this ContainerContainerDistribution.  # noqa: E501
 
         The base (relative) path component of the published url. Avoid paths that                     overlap with other distribution base paths (e.g. \"foo\" and \"foo/bar\")  # noqa: E501
 
         :return: The base_path of this ContainerContainerDistribution.  # noqa: E501
         :rtype: str
@@ -128,14 +105,37 @@
         """
         if self.local_vars_configuration.client_side_validation and base_path is None:  # noqa: E501
             raise ValueError("Invalid value for `base_path`, must not be `None`")  # noqa: E501
 
         self._base_path = base_path
 
     @property
+    def content_guard(self):
+        """Gets the content_guard of this ContainerContainerDistribution.  # noqa: E501
+
+        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
+
+        :return: The content_guard of this ContainerContainerDistribution.  # noqa: E501
+        :rtype: str
+        """
+        return self._content_guard
+
+    @content_guard.setter
+    def content_guard(self, content_guard):
+        """Sets the content_guard of this ContainerContainerDistribution.
+
+        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
+
+        :param content_guard: The content_guard of this ContainerContainerDistribution.  # noqa: E501
+        :type: str
+        """
+
+        self._content_guard = content_guard
+
+    @property
     def repository(self):
         """Gets the repository of this ContainerContainerDistribution.  # noqa: E501
 
         The latest RepositoryVersion for this Repository will be served.  # noqa: E501
 
         :return: The repository of this ContainerContainerDistribution.  # noqa: E501
         :rtype: str
@@ -151,35 +151,14 @@
         :param repository: The repository of this ContainerContainerDistribution.  # noqa: E501
         :type: str
         """
 
         self._repository = repository
 
     @property
-    def pulp_labels(self):
-        """Gets the pulp_labels of this ContainerContainerDistribution.  # noqa: E501
-
-
-        :return: The pulp_labels of this ContainerContainerDistribution.  # noqa: E501
-        :rtype: object
-        """
-        return self._pulp_labels
-
-    @pulp_labels.setter
-    def pulp_labels(self, pulp_labels):
-        """Sets the pulp_labels of this ContainerContainerDistribution.
-
-
-        :param pulp_labels: The pulp_labels of this ContainerContainerDistribution.  # noqa: E501
-        :type: object
-        """
-
-        self._pulp_labels = pulp_labels
-
-    @property
     def name(self):
         """Gets the name of this ContainerContainerDistribution.  # noqa: E501
 
         A unique name. Ex, `rawhide` and `stable`.  # noqa: E501
 
         :return: The name of this ContainerContainerDistribution.  # noqa: E501
         :rtype: str
@@ -197,14 +176,35 @@
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this ContainerContainerDistribution.  # noqa: E501
+
+
+        :return: The pulp_labels of this ContainerContainerDistribution.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this ContainerContainerDistribution.
+
+
+        :param pulp_labels: The pulp_labels of this ContainerContainerDistribution.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def repository_version(self):
         """Gets the repository_version of this ContainerContainerDistribution.  # noqa: E501
 
         RepositoryVersion to be served  # noqa: E501
 
         :return: The repository_version of this ContainerContainerDistribution.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_distribution_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_distribution_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,73 +31,73 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'pulp_created': 'datetime',
-        'content_guard': 'str',
         'base_path': 'str',
         'pulp_href': 'str',
+        'content_guard': 'str',
         'repository': 'str',
-        'pulp_labels': 'object',
         'name': 'str',
+        'pulp_labels': 'object',
         'repository_version': 'str',
         'registry_path': 'str',
         'namespace': 'str',
         'private': 'bool',
         'description': 'str'
     }
 
     attribute_map = {
         'pulp_created': 'pulp_created',
-        'content_guard': 'content_guard',
         'base_path': 'base_path',
         'pulp_href': 'pulp_href',
+        'content_guard': 'content_guard',
         'repository': 'repository',
-        'pulp_labels': 'pulp_labels',
         'name': 'name',
+        'pulp_labels': 'pulp_labels',
         'repository_version': 'repository_version',
         'registry_path': 'registry_path',
         'namespace': 'namespace',
         'private': 'private',
         'description': 'description'
     }
 
-    def __init__(self, pulp_created=None, content_guard=None, base_path=None, pulp_href=None, repository=None, pulp_labels=None, name=None, repository_version=None, registry_path=None, namespace=None, private=None, description=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_created=None, base_path=None, pulp_href=None, content_guard=None, repository=None, name=None, pulp_labels=None, repository_version=None, registry_path=None, namespace=None, private=None, description=None, local_vars_configuration=None):  # noqa: E501
         """ContainerContainerDistributionResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_created = None
-        self._content_guard = None
         self._base_path = None
         self._pulp_href = None
+        self._content_guard = None
         self._repository = None
-        self._pulp_labels = None
         self._name = None
+        self._pulp_labels = None
         self._repository_version = None
         self._registry_path = None
         self._namespace = None
         self._private = None
         self._description = None
         self.discriminator = None
 
         if pulp_created is not None:
             self.pulp_created = pulp_created
-        if content_guard is not None:
-            self.content_guard = content_guard
         self.base_path = base_path
         if pulp_href is not None:
             self.pulp_href = pulp_href
+        if content_guard is not None:
+            self.content_guard = content_guard
         self.repository = repository
+        self.name = name
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
-        self.name = name
         self.repository_version = repository_version
         if registry_path is not None:
             self.registry_path = registry_path
         if namespace is not None:
             self.namespace = namespace
         if private is not None:
             self.private = private
@@ -123,37 +123,14 @@
         :param pulp_created: The pulp_created of this ContainerContainerDistributionResponse.  # noqa: E501
         :type: datetime
         """
 
         self._pulp_created = pulp_created
 
     @property
-    def content_guard(self):
-        """Gets the content_guard of this ContainerContainerDistributionResponse.  # noqa: E501
-
-        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
-
-        :return: The content_guard of this ContainerContainerDistributionResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._content_guard
-
-    @content_guard.setter
-    def content_guard(self, content_guard):
-        """Sets the content_guard of this ContainerContainerDistributionResponse.
-
-        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
-
-        :param content_guard: The content_guard of this ContainerContainerDistributionResponse.  # noqa: E501
-        :type: str
-        """
-
-        self._content_guard = content_guard
-
-    @property
     def base_path(self):
         """Gets the base_path of this ContainerContainerDistributionResponse.  # noqa: E501
 
         The base (relative) path component of the published url. Avoid paths that                     overlap with other distribution base paths (e.g. \"foo\" and \"foo/bar\")  # noqa: E501
 
         :return: The base_path of this ContainerContainerDistributionResponse.  # noqa: E501
         :rtype: str
@@ -192,14 +169,37 @@
         :param pulp_href: The pulp_href of this ContainerContainerDistributionResponse.  # noqa: E501
         :type: str
         """
 
         self._pulp_href = pulp_href
 
     @property
+    def content_guard(self):
+        """Gets the content_guard of this ContainerContainerDistributionResponse.  # noqa: E501
+
+        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
+
+        :return: The content_guard of this ContainerContainerDistributionResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._content_guard
+
+    @content_guard.setter
+    def content_guard(self, content_guard):
+        """Sets the content_guard of this ContainerContainerDistributionResponse.
+
+        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
+
+        :param content_guard: The content_guard of this ContainerContainerDistributionResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._content_guard = content_guard
+
+    @property
     def repository(self):
         """Gets the repository of this ContainerContainerDistributionResponse.  # noqa: E501
 
         The latest RepositoryVersion for this Repository will be served.  # noqa: E501
 
         :return: The repository of this ContainerContainerDistributionResponse.  # noqa: E501
         :rtype: str
@@ -215,35 +215,14 @@
         :param repository: The repository of this ContainerContainerDistributionResponse.  # noqa: E501
         :type: str
         """
 
         self._repository = repository
 
     @property
-    def pulp_labels(self):
-        """Gets the pulp_labels of this ContainerContainerDistributionResponse.  # noqa: E501
-
-
-        :return: The pulp_labels of this ContainerContainerDistributionResponse.  # noqa: E501
-        :rtype: object
-        """
-        return self._pulp_labels
-
-    @pulp_labels.setter
-    def pulp_labels(self, pulp_labels):
-        """Sets the pulp_labels of this ContainerContainerDistributionResponse.
-
-
-        :param pulp_labels: The pulp_labels of this ContainerContainerDistributionResponse.  # noqa: E501
-        :type: object
-        """
-
-        self._pulp_labels = pulp_labels
-
-    @property
     def name(self):
         """Gets the name of this ContainerContainerDistributionResponse.  # noqa: E501
 
         A unique name. Ex, `rawhide` and `stable`.  # noqa: E501
 
         :return: The name of this ContainerContainerDistributionResponse.  # noqa: E501
         :rtype: str
@@ -261,14 +240,35 @@
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this ContainerContainerDistributionResponse.  # noqa: E501
+
+
+        :return: The pulp_labels of this ContainerContainerDistributionResponse.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this ContainerContainerDistributionResponse.
+
+
+        :param pulp_labels: The pulp_labels of this ContainerContainerDistributionResponse.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def repository_version(self):
         """Gets the repository_version of this ContainerContainerDistributionResponse.  # noqa: E501
 
         RepositoryVersion to be served  # noqa: E501
 
         :return: The repository_version of this ContainerContainerDistributionResponse.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_namespace.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_namespace.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_namespace_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_namespace_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_push_repository.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_push_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,41 +31,41 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'description': 'str',
-        'name': 'str',
         'retain_repo_versions': 'int',
+        'name': 'str',
         'pulp_labels': 'object'
     }
 
     attribute_map = {
         'description': 'description',
-        'name': 'name',
         'retain_repo_versions': 'retain_repo_versions',
+        'name': 'name',
         'pulp_labels': 'pulp_labels'
     }
 
-    def __init__(self, description=None, name=None, retain_repo_versions=None, pulp_labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, description=None, retain_repo_versions=None, name=None, pulp_labels=None, local_vars_configuration=None):  # noqa: E501
         """ContainerContainerPushRepository - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._description = None
-        self._name = None
         self._retain_repo_versions = None
+        self._name = None
         self._pulp_labels = None
         self.discriminator = None
 
         self.description = description
-        self.name = name
         self.retain_repo_versions = retain_repo_versions
+        self.name = name
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
 
     @property
     def description(self):
         """Gets the description of this ContainerContainerPushRepository.  # noqa: E501
 
@@ -85,39 +85,14 @@
         :param description: The description of this ContainerContainerPushRepository.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
-    def name(self):
-        """Gets the name of this ContainerContainerPushRepository.  # noqa: E501
-
-        A unique name for this repository.  # noqa: E501
-
-        :return: The name of this ContainerContainerPushRepository.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ContainerContainerPushRepository.
-
-        A unique name for this repository.  # noqa: E501
-
-        :param name: The name of this ContainerContainerPushRepository.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-
-        self._name = name
-
-    @property
     def retain_repo_versions(self):
         """Gets the retain_repo_versions of this ContainerContainerPushRepository.  # noqa: E501
 
         Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
 
         :return: The retain_repo_versions of this ContainerContainerPushRepository.  # noqa: E501
         :rtype: int
@@ -136,14 +111,39 @@
         if (self.local_vars_configuration.client_side_validation and
                 retain_repo_versions is not None and retain_repo_versions < 1):  # noqa: E501
             raise ValueError("Invalid value for `retain_repo_versions`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._retain_repo_versions = retain_repo_versions
 
     @property
+    def name(self):
+        """Gets the name of this ContainerContainerPushRepository.  # noqa: E501
+
+        A unique name for this repository.  # noqa: E501
+
+        :return: The name of this ContainerContainerPushRepository.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ContainerContainerPushRepository.
+
+        A unique name for this repository.  # noqa: E501
+
+        :param name: The name of this ContainerContainerPushRepository.  # noqa: E501
+        :type: str
+        """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+
+        self._name = name
+
+    @property
     def pulp_labels(self):
         """Gets the pulp_labels of this ContainerContainerPushRepository.  # noqa: E501
 
 
         :return: The pulp_labels of this ContainerContainerPushRepository.  # noqa: E501
         :rtype: object
         """
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_push_repository_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_push_repository_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,63 +31,63 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'pulp_created': 'datetime',
-        'description': 'str',
-        'name': 'str',
-        'retain_repo_versions': 'int',
         'pulp_href': 'str',
-        'pulp_labels': 'object',
+        'latest_version_href': 'str',
+        'description': 'str',
         'versions_href': 'str',
-        'latest_version_href': 'str'
+        'retain_repo_versions': 'int',
+        'name': 'str',
+        'pulp_labels': 'object'
     }
 
     attribute_map = {
         'pulp_created': 'pulp_created',
-        'description': 'description',
-        'name': 'name',
-        'retain_repo_versions': 'retain_repo_versions',
         'pulp_href': 'pulp_href',
-        'pulp_labels': 'pulp_labels',
+        'latest_version_href': 'latest_version_href',
+        'description': 'description',
         'versions_href': 'versions_href',
-        'latest_version_href': 'latest_version_href'
+        'retain_repo_versions': 'retain_repo_versions',
+        'name': 'name',
+        'pulp_labels': 'pulp_labels'
     }
 
-    def __init__(self, pulp_created=None, description=None, name=None, retain_repo_versions=None, pulp_href=None, pulp_labels=None, versions_href=None, latest_version_href=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_created=None, pulp_href=None, latest_version_href=None, description=None, versions_href=None, retain_repo_versions=None, name=None, pulp_labels=None, local_vars_configuration=None):  # noqa: E501
         """ContainerContainerPushRepositoryResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_created = None
+        self._pulp_href = None
+        self._latest_version_href = None
         self._description = None
-        self._name = None
+        self._versions_href = None
         self._retain_repo_versions = None
-        self._pulp_href = None
+        self._name = None
         self._pulp_labels = None
-        self._versions_href = None
-        self._latest_version_href = None
         self.discriminator = None
 
         if pulp_created is not None:
             self.pulp_created = pulp_created
-        self.description = description
-        self.name = name
-        self.retain_repo_versions = retain_repo_versions
         if pulp_href is not None:
             self.pulp_href = pulp_href
-        if pulp_labels is not None:
-            self.pulp_labels = pulp_labels
-        if versions_href is not None:
-            self.versions_href = versions_href
         if latest_version_href is not None:
             self.latest_version_href = latest_version_href
+        self.description = description
+        if versions_href is not None:
+            self.versions_href = versions_href
+        self.retain_repo_versions = retain_repo_versions
+        self.name = name
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
 
     @property
     def pulp_created(self):
         """Gets the pulp_created of this ContainerContainerPushRepositoryResponse.  # noqa: E501
 
         Timestamp of creation.  # noqa: E501
 
@@ -105,14 +105,56 @@
         :param pulp_created: The pulp_created of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :type: datetime
         """
 
         self._pulp_created = pulp_created
 
     @property
+    def pulp_href(self):
+        """Gets the pulp_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+
+
+        :return: The pulp_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._pulp_href
+
+    @pulp_href.setter
+    def pulp_href(self, pulp_href):
+        """Sets the pulp_href of this ContainerContainerPushRepositoryResponse.
+
+
+        :param pulp_href: The pulp_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._pulp_href = pulp_href
+
+    @property
+    def latest_version_href(self):
+        """Gets the latest_version_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+
+
+        :return: The latest_version_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._latest_version_href
+
+    @latest_version_href.setter
+    def latest_version_href(self, latest_version_href):
+        """Sets the latest_version_href of this ContainerContainerPushRepositoryResponse.
+
+
+        :param latest_version_href: The latest_version_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._latest_version_href = latest_version_href
+
+    @property
     def description(self):
         """Gets the description of this ContainerContainerPushRepositoryResponse.  # noqa: E501
 
         An optional description.  # noqa: E501
 
         :return: The description of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :rtype: str
@@ -128,37 +170,33 @@
         :param description: The description of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
-    def name(self):
-        """Gets the name of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+    def versions_href(self):
+        """Gets the versions_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
 
-        A unique name for this repository.  # noqa: E501
 
-        :return: The name of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :return: The versions_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._versions_href
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ContainerContainerPushRepositoryResponse.
+    @versions_href.setter
+    def versions_href(self, versions_href):
+        """Sets the versions_href of this ContainerContainerPushRepositoryResponse.
 
-        A unique name for this repository.  # noqa: E501
 
-        :param name: The name of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :param versions_href: The versions_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._versions_href = versions_href
 
     @property
     def retain_repo_versions(self):
         """Gets the retain_repo_versions of this ContainerContainerPushRepositoryResponse.  # noqa: E501
 
         Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
 
@@ -179,33 +217,37 @@
         if (self.local_vars_configuration.client_side_validation and
                 retain_repo_versions is not None and retain_repo_versions < 1):  # noqa: E501
             raise ValueError("Invalid value for `retain_repo_versions`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._retain_repo_versions = retain_repo_versions
 
     @property
-    def pulp_href(self):
-        """Gets the pulp_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+    def name(self):
+        """Gets the name of this ContainerContainerPushRepositoryResponse.  # noqa: E501
 
+        A unique name for this repository.  # noqa: E501
 
-        :return: The pulp_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :return: The name of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :rtype: str
         """
-        return self._pulp_href
+        return self._name
 
-    @pulp_href.setter
-    def pulp_href(self, pulp_href):
-        """Sets the pulp_href of this ContainerContainerPushRepositoryResponse.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ContainerContainerPushRepositoryResponse.
 
+        A unique name for this repository.  # noqa: E501
 
-        :param pulp_href: The pulp_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
+        :param name: The name of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._pulp_href = pulp_href
+        self._name = name
 
     @property
     def pulp_labels(self):
         """Gets the pulp_labels of this ContainerContainerPushRepositoryResponse.  # noqa: E501
 
 
         :return: The pulp_labels of this ContainerContainerPushRepositoryResponse.  # noqa: E501
@@ -220,56 +262,14 @@
 
         :param pulp_labels: The pulp_labels of this ContainerContainerPushRepositoryResponse.  # noqa: E501
         :type: object
         """
 
         self._pulp_labels = pulp_labels
 
-    @property
-    def versions_href(self):
-        """Gets the versions_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
-
-
-        :return: The versions_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._versions_href
-
-    @versions_href.setter
-    def versions_href(self, versions_href):
-        """Sets the versions_href of this ContainerContainerPushRepositoryResponse.
-
-
-        :param versions_href: The versions_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
-        :type: str
-        """
-
-        self._versions_href = versions_href
-
-    @property
-    def latest_version_href(self):
-        """Gets the latest_version_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
-
-
-        :return: The latest_version_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._latest_version_href
-
-    @latest_version_href.setter
-    def latest_version_href(self, latest_version_href):
-        """Sets the latest_version_href of this ContainerContainerPushRepositoryResponse.
-
-
-        :param latest_version_href: The latest_version_href of this ContainerContainerPushRepositoryResponse.  # noqa: E501
-        :type: str
-        """
-
-        self._latest_version_href = latest_version_href
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_remote.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_remote_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_repository.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_container_repository_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_container_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_content_redirect_content_guard.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_content_redirect_content_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_content_redirect_content_guard_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_content_redirect_content_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_manifest_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_manifest_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/container_tag_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/container_tag_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/content_summary.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/content_summary_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/manifest_copy.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/manifest_copy.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/media_types_enum.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/media_types_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/oci_build_image.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/oci_build_image.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginated_repository_version_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_blob_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_blob_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_distribution_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_namespace_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_namespace_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_push_repository_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_push_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_remote_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_container_repository_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_container_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_content_redirect_content_guard_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_content_redirect_content_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_manifest_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_manifest_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/paginatedcontainer_tag_response_list.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/paginatedcontainer_tag_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_distribution.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,110 +30,110 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'content_guard': 'str',
         'base_path': 'str',
+        'content_guard': 'str',
         'repository': 'str',
-        'pulp_labels': 'object',
         'name': 'str',
+        'pulp_labels': 'object',
         'repository_version': 'str',
         'private': 'bool',
         'description': 'str'
     }
 
     attribute_map = {
-        'content_guard': 'content_guard',
         'base_path': 'base_path',
+        'content_guard': 'content_guard',
         'repository': 'repository',
-        'pulp_labels': 'pulp_labels',
         'name': 'name',
+        'pulp_labels': 'pulp_labels',
         'repository_version': 'repository_version',
         'private': 'private',
         'description': 'description'
     }
 
-    def __init__(self, content_guard=None, base_path=None, repository=None, pulp_labels=None, name=None, repository_version=None, private=None, description=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, base_path=None, content_guard=None, repository=None, name=None, pulp_labels=None, repository_version=None, private=None, description=None, local_vars_configuration=None):  # noqa: E501
         """PatchedcontainerContainerDistribution - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._content_guard = None
         self._base_path = None
+        self._content_guard = None
         self._repository = None
-        self._pulp_labels = None
         self._name = None
+        self._pulp_labels = None
         self._repository_version = None
         self._private = None
         self._description = None
         self.discriminator = None
 
-        if content_guard is not None:
-            self.content_guard = content_guard
         if base_path is not None:
             self.base_path = base_path
+        if content_guard is not None:
+            self.content_guard = content_guard
         self.repository = repository
-        if pulp_labels is not None:
-            self.pulp_labels = pulp_labels
         if name is not None:
             self.name = name
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         self.repository_version = repository_version
         if private is not None:
             self.private = private
         self.description = description
 
     @property
-    def content_guard(self):
-        """Gets the content_guard of this PatchedcontainerContainerDistribution.  # noqa: E501
+    def base_path(self):
+        """Gets the base_path of this PatchedcontainerContainerDistribution.  # noqa: E501
 
-        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
+        The base (relative) path component of the published url. Avoid paths that                     overlap with other distribution base paths (e.g. \"foo\" and \"foo/bar\")  # noqa: E501
 
-        :return: The content_guard of this PatchedcontainerContainerDistribution.  # noqa: E501
+        :return: The base_path of this PatchedcontainerContainerDistribution.  # noqa: E501
         :rtype: str
         """
-        return self._content_guard
+        return self._base_path
 
-    @content_guard.setter
-    def content_guard(self, content_guard):
-        """Sets the content_guard of this PatchedcontainerContainerDistribution.
+    @base_path.setter
+    def base_path(self, base_path):
+        """Sets the base_path of this PatchedcontainerContainerDistribution.
 
-        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
+        The base (relative) path component of the published url. Avoid paths that                     overlap with other distribution base paths (e.g. \"foo\" and \"foo/bar\")  # noqa: E501
 
-        :param content_guard: The content_guard of this PatchedcontainerContainerDistribution.  # noqa: E501
+        :param base_path: The base_path of this PatchedcontainerContainerDistribution.  # noqa: E501
         :type: str
         """
 
-        self._content_guard = content_guard
+        self._base_path = base_path
 
     @property
-    def base_path(self):
-        """Gets the base_path of this PatchedcontainerContainerDistribution.  # noqa: E501
+    def content_guard(self):
+        """Gets the content_guard of this PatchedcontainerContainerDistribution.  # noqa: E501
 
-        The base (relative) path component of the published url. Avoid paths that                     overlap with other distribution base paths (e.g. \"foo\" and \"foo/bar\")  # noqa: E501
+        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
 
-        :return: The base_path of this PatchedcontainerContainerDistribution.  # noqa: E501
+        :return: The content_guard of this PatchedcontainerContainerDistribution.  # noqa: E501
         :rtype: str
         """
-        return self._base_path
+        return self._content_guard
 
-    @base_path.setter
-    def base_path(self, base_path):
-        """Sets the base_path of this PatchedcontainerContainerDistribution.
+    @content_guard.setter
+    def content_guard(self, content_guard):
+        """Sets the content_guard of this PatchedcontainerContainerDistribution.
 
-        The base (relative) path component of the published url. Avoid paths that                     overlap with other distribution base paths (e.g. \"foo\" and \"foo/bar\")  # noqa: E501
+        An optional content-guard. If none is specified, a default one will be used.  # noqa: E501
 
-        :param base_path: The base_path of this PatchedcontainerContainerDistribution.  # noqa: E501
+        :param content_guard: The content_guard of this PatchedcontainerContainerDistribution.  # noqa: E501
         :type: str
         """
 
-        self._base_path = base_path
+        self._content_guard = content_guard
 
     @property
     def repository(self):
         """Gets the repository of this PatchedcontainerContainerDistribution.  # noqa: E501
 
         The latest RepositoryVersion for this Repository will be served.  # noqa: E501
 
@@ -151,35 +151,14 @@
         :param repository: The repository of this PatchedcontainerContainerDistribution.  # noqa: E501
         :type: str
         """
 
         self._repository = repository
 
     @property
-    def pulp_labels(self):
-        """Gets the pulp_labels of this PatchedcontainerContainerDistribution.  # noqa: E501
-
-
-        :return: The pulp_labels of this PatchedcontainerContainerDistribution.  # noqa: E501
-        :rtype: object
-        """
-        return self._pulp_labels
-
-    @pulp_labels.setter
-    def pulp_labels(self, pulp_labels):
-        """Sets the pulp_labels of this PatchedcontainerContainerDistribution.
-
-
-        :param pulp_labels: The pulp_labels of this PatchedcontainerContainerDistribution.  # noqa: E501
-        :type: object
-        """
-
-        self._pulp_labels = pulp_labels
-
-    @property
     def name(self):
         """Gets the name of this PatchedcontainerContainerDistribution.  # noqa: E501
 
         A unique name. Ex, `rawhide` and `stable`.  # noqa: E501
 
         :return: The name of this PatchedcontainerContainerDistribution.  # noqa: E501
         :rtype: str
@@ -195,14 +174,35 @@
         :param name: The name of this PatchedcontainerContainerDistribution.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this PatchedcontainerContainerDistribution.  # noqa: E501
+
+
+        :return: The pulp_labels of this PatchedcontainerContainerDistribution.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this PatchedcontainerContainerDistribution.
+
+
+        :param pulp_labels: The pulp_labels of this PatchedcontainerContainerDistribution.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def repository_version(self):
         """Gets the repository_version of this PatchedcontainerContainerDistribution.  # noqa: E501
 
         RepositoryVersion to be served  # noqa: E501
 
         :return: The repository_version of this PatchedcontainerContainerDistribution.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_push_repository.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_push_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,42 +31,42 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'description': 'str',
-        'name': 'str',
         'retain_repo_versions': 'int',
+        'name': 'str',
         'pulp_labels': 'object'
     }
 
     attribute_map = {
         'description': 'description',
-        'name': 'name',
         'retain_repo_versions': 'retain_repo_versions',
+        'name': 'name',
         'pulp_labels': 'pulp_labels'
     }
 
-    def __init__(self, description=None, name=None, retain_repo_versions=None, pulp_labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, description=None, retain_repo_versions=None, name=None, pulp_labels=None, local_vars_configuration=None):  # noqa: E501
         """PatchedcontainerContainerPushRepository - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._description = None
-        self._name = None
         self._retain_repo_versions = None
+        self._name = None
         self._pulp_labels = None
         self.discriminator = None
 
         self.description = description
+        self.retain_repo_versions = retain_repo_versions
         if name is not None:
             self.name = name
-        self.retain_repo_versions = retain_repo_versions
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
 
     @property
     def description(self):
         """Gets the description of this PatchedcontainerContainerPushRepository.  # noqa: E501
 
@@ -86,37 +86,14 @@
         :param description: The description of this PatchedcontainerContainerPushRepository.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
-    def name(self):
-        """Gets the name of this PatchedcontainerContainerPushRepository.  # noqa: E501
-
-        A unique name for this repository.  # noqa: E501
-
-        :return: The name of this PatchedcontainerContainerPushRepository.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this PatchedcontainerContainerPushRepository.
-
-        A unique name for this repository.  # noqa: E501
-
-        :param name: The name of this PatchedcontainerContainerPushRepository.  # noqa: E501
-        :type: str
-        """
-
-        self._name = name
-
-    @property
     def retain_repo_versions(self):
         """Gets the retain_repo_versions of this PatchedcontainerContainerPushRepository.  # noqa: E501
 
         Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
 
         :return: The retain_repo_versions of this PatchedcontainerContainerPushRepository.  # noqa: E501
         :rtype: int
@@ -135,14 +112,37 @@
         if (self.local_vars_configuration.client_side_validation and
                 retain_repo_versions is not None and retain_repo_versions < 1):  # noqa: E501
             raise ValueError("Invalid value for `retain_repo_versions`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._retain_repo_versions = retain_repo_versions
 
     @property
+    def name(self):
+        """Gets the name of this PatchedcontainerContainerPushRepository.  # noqa: E501
+
+        A unique name for this repository.  # noqa: E501
+
+        :return: The name of this PatchedcontainerContainerPushRepository.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this PatchedcontainerContainerPushRepository.
+
+        A unique name for this repository.  # noqa: E501
+
+        :param name: The name of this PatchedcontainerContainerPushRepository.  # noqa: E501
+        :type: str
+        """
+
+        self._name = name
+
+    @property
     def pulp_labels(self):
         """Gets the pulp_labels of this PatchedcontainerContainerPushRepository.  # noqa: E501
 
 
         :return: The pulp_labels of this PatchedcontainerContainerPushRepository.  # noqa: E501
         :rtype: object
         """
```

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_remote.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_container_repository.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_container_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/patchedcontainer_content_redirect_content_guard.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/patchedcontainer_content_redirect_content_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/policy_enum.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/recursive_manage.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/recursive_manage.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/remove_image.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/remove_image.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/repository_sync_url.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/repository_version.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/repository_version_response.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/tag_copy.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/tag_copy.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/tag_image.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/tag_image.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/models/un_tag_image.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/models/un_tag_image.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/pulpcore/client/pulp_container/rest.py` & `pulp_container-client-2.9.9/pulpcore/client/pulp_container/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/setup.py` & `pulp_container-client-2.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_container-client"
-VERSION = "2.9.8"
+VERSION = "2.9.9"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_container-client-2.9.8/test/test_async_operation_response.py` & `pulp_container-client-2.9.9/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_blob_response.py` & `pulp_container-client-2.9.9/test/test_container_blob_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_container_distribution.py` & `pulp_container-client-2.9.9/test/test_container_container_distribution.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         """Test ContainerContainerDistribution
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_container.models.container_container_distribution.ContainerContainerDistribution()  # noqa: E501
         if include_optional :
             return ContainerContainerDistribution(
-                content_guard = '0', 
                 base_path = '0', 
+                content_guard = '0', 
                 repository = '0', 
-                pulp_labels = None, 
                 name = '0', 
+                pulp_labels = None, 
                 repository_version = '0', 
                 private = True, 
                 description = '0'
             )
         else :
             return ContainerContainerDistribution(
                 base_path = '0',
```

### Comparing `pulp_container-client-2.9.8/test/test_container_container_distribution_response.py` & `pulp_container-client-2.9.9/test/test_container_container_distribution_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,20 +34,20 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_container.models.container_container_distribution_response.ContainerContainerDistributionResponse()  # noqa: E501
         if include_optional :
             return ContainerContainerDistributionResponse(
                 pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                content_guard = '0', 
                 base_path = '0', 
                 pulp_href = '0', 
+                content_guard = '0', 
                 repository = '0', 
-                pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels(), 
                 name = '0', 
+                pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels(), 
                 repository_version = '0', 
                 registry_path = '0', 
                 namespace = '0', 
                 private = True, 
                 description = '0'
             )
         else :
```

### Comparing `pulp_container-client-2.9.8/test/test_container_container_namespace.py` & `pulp_container-client-2.9.9/test/test_container_container_namespace.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_container_namespace_response.py` & `pulp_container-client-2.9.9/test/test_container_container_namespace_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_container_push_repository.py` & `pulp_container-client-2.9.9/test/test_container_container_push_repository.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_container.models.container_container_push_repository.ContainerContainerPushRepository()  # noqa: E501
         if include_optional :
             return ContainerContainerPushRepository(
                 description = '0', 
-                name = '0', 
                 retain_repo_versions = 1, 
+                name = '0', 
                 pulp_labels = None
             )
         else :
             return ContainerContainerPushRepository(
                 name = '0',
         )
```

### Comparing `pulp_container-client-2.9.8/test/test_container_container_push_repository_response.py` & `pulp_container-client-2.9.9/test/test_container_container_push_repository_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,21 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_container.models.container_container_push_repository_response.ContainerContainerPushRepositoryResponse()  # noqa: E501
         if include_optional :
             return ContainerContainerPushRepositoryResponse(
                 pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                description = '0', 
-                name = '0', 
-                retain_repo_versions = 1, 
                 pulp_href = '0', 
-                pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels(), 
+                latest_version_href = '0', 
+                description = '0', 
                 versions_href = '0', 
-                latest_version_href = '0'
+                retain_repo_versions = 1, 
+                name = '0', 
+                pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels()
             )
         else :
             return ContainerContainerPushRepositoryResponse(
                 name = '0',
         )
 
     def testContainerContainerPushRepositoryResponse(self):
```

### Comparing `pulp_container-client-2.9.8/test/test_container_container_remote.py` & `pulp_container-client-2.9.9/test/test_container_container_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_container_remote_response.py` & `pulp_container-client-2.9.9/test/test_container_container_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_container_repository.py` & `pulp_container-client-2.9.9/test/test_container_container_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_container_repository_response.py` & `pulp_container-client-2.9.9/test/test_container_container_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_content_redirect_content_guard.py` & `pulp_container-client-2.9.9/test/test_container_content_redirect_content_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_content_redirect_content_guard_response.py` & `pulp_container-client-2.9.9/test/test_container_content_redirect_content_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_manifest_response.py` & `pulp_container-client-2.9.9/test/test_container_manifest_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_container_tag_response.py` & `pulp_container-client-2.9.9/test/test_container_tag_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_content_blobs_api.py` & `pulp_container-client-2.9.9/test/test_content_blobs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_content_manifests_api.py` & `pulp_container-client-2.9.9/test/test_content_manifests_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_content_summary.py` & `pulp_container-client-2.9.9/test/test_content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_content_summary_response.py` & `pulp_container-client-2.9.9/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_content_tags_api.py` & `pulp_container-client-2.9.9/test/test_content_tags_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_contentguards_content_redirect_api.py` & `pulp_container-client-2.9.9/test/test_contentguards_content_redirect_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_distributions_container_api.py` & `pulp_container-client-2.9.9/test/test_distributions_container_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_manifest_copy.py` & `pulp_container-client-2.9.9/test/test_manifest_copy.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_media_types_enum.py` & `pulp_container-client-2.9.9/test/test_media_types_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_oci_build_image.py` & `pulp_container-client-2.9.9/test/test_oci_build_image.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginated_repository_version_response_list.py` & `pulp_container-client-2.9.9/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_blob_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_blob_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_container_distribution_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_container_distribution_response_list.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,20 +39,20 @@
             return PaginatedcontainerContainerDistributionResponseList(
                 count = 123, 
                 next = 'http://api.example.org/accounts/?offset=400&limit=100', 
                 previous = 'http://api.example.org/accounts/?offset=200&limit=100', 
                 results = [
                     pulpcore.client.pulp_container.models.container/container_distribution_response.container.ContainerDistributionResponse(
                         pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        content_guard = '0', 
                         base_path = '0', 
                         pulp_href = '0', 
+                        content_guard = '0', 
                         repository = '0', 
-                        pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels(), 
                         name = '0', 
+                        pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels(), 
                         repository_version = '0', 
                         registry_path = '0', 
                         namespace = '0', 
                         private = True, 
                         description = '0', )
                     ]
             )
```

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_container_namespace_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_container_namespace_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_container_push_repository_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_container_push_repository_response_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,21 @@
             return PaginatedcontainerContainerPushRepositoryResponseList(
                 count = 123, 
                 next = 'http://api.example.org/accounts/?offset=400&limit=100', 
                 previous = 'http://api.example.org/accounts/?offset=200&limit=100', 
                 results = [
                     pulpcore.client.pulp_container.models.container/container_push_repository_response.container.ContainerPushRepositoryResponse(
                         pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        description = '0', 
-                        name = '0', 
-                        retain_repo_versions = 1, 
                         pulp_href = '0', 
-                        pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels(), 
+                        latest_version_href = '0', 
+                        description = '0', 
                         versions_href = '0', 
-                        latest_version_href = '0', )
+                        retain_repo_versions = 1, 
+                        name = '0', 
+                        pulp_labels = pulpcore.client.pulp_container.models.pulp_labels.pulp_labels(), )
                     ]
             )
         else :
             return PaginatedcontainerContainerPushRepositoryResponseList(
         )
 
     def testPaginatedcontainerContainerPushRepositoryResponseList(self):
```

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_container_remote_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_container_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_container_repository_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_container_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_content_redirect_content_guard_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_content_redirect_content_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_manifest_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_manifest_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_paginatedcontainer_tag_response_list.py` & `pulp_container-client-2.9.9/test/test_paginatedcontainer_tag_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_patchedcontainer_container_distribution.py` & `pulp_container-client-2.9.9/test/test_patchedcontainer_container_distribution.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         """Test PatchedcontainerContainerDistribution
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_container.models.patchedcontainer_container_distribution.PatchedcontainerContainerDistribution()  # noqa: E501
         if include_optional :
             return PatchedcontainerContainerDistribution(
-                content_guard = '0', 
                 base_path = '0', 
+                content_guard = '0', 
                 repository = '0', 
-                pulp_labels = None, 
                 name = '0', 
+                pulp_labels = None, 
                 repository_version = '0', 
                 private = True, 
                 description = '0'
             )
         else :
             return PatchedcontainerContainerDistribution(
         )
```

### Comparing `pulp_container-client-2.9.8/test/test_patchedcontainer_container_push_repository.py` & `pulp_container-client-2.9.9/test/test_patchedcontainer_container_push_repository.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_container.models.patchedcontainer_container_push_repository.PatchedcontainerContainerPushRepository()  # noqa: E501
         if include_optional :
             return PatchedcontainerContainerPushRepository(
                 description = '0', 
-                name = '0', 
                 retain_repo_versions = 1, 
+                name = '0', 
                 pulp_labels = None
             )
         else :
             return PatchedcontainerContainerPushRepository(
         )
 
     def testPatchedcontainerContainerPushRepository(self):
```

### Comparing `pulp_container-client-2.9.8/test/test_patchedcontainer_container_remote.py` & `pulp_container-client-2.9.9/test/test_patchedcontainer_container_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_patchedcontainer_container_repository.py` & `pulp_container-client-2.9.9/test/test_patchedcontainer_container_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_patchedcontainer_content_redirect_content_guard.py` & `pulp_container-client-2.9.9/test/test_patchedcontainer_content_redirect_content_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_policy_enum.py` & `pulp_container-client-2.9.9/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_pulp_container_namespaces_api.py` & `pulp_container-client-2.9.9/test/test_pulp_container_namespaces_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_recursive_manage.py` & `pulp_container-client-2.9.9/test/test_recursive_manage.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_remotes_container_api.py` & `pulp_container-client-2.9.9/test/test_remotes_container_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_remove_image.py` & `pulp_container-client-2.9.9/test/test_remove_image.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_repositories_container_api.py` & `pulp_container-client-2.9.9/test/test_repositories_container_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_repositories_container_push_api.py` & `pulp_container-client-2.9.9/test/test_repositories_container_push_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_repositories_container_push_versions_api.py` & `pulp_container-client-2.9.9/test/test_repositories_container_push_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_repositories_container_versions_api.py` & `pulp_container-client-2.9.9/test/test_repositories_container_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_repository_sync_url.py` & `pulp_container-client-2.9.9/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_repository_version.py` & `pulp_container-client-2.9.9/test/test_repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_repository_version_response.py` & `pulp_container-client-2.9.9/test/test_repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_tag_copy.py` & `pulp_container-client-2.9.9/test/test_tag_copy.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_tag_image.py` & `pulp_container-client-2.9.9/test/test_tag_image.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_token_api.py` & `pulp_container-client-2.9.9/test/test_token_api.py`

 * *Files identical despite different names*

### Comparing `pulp_container-client-2.9.8/test/test_un_tag_image.py` & `pulp_container-client-2.9.9/test/test_un_tag_image.py`

 * *Files identical despite different names*

