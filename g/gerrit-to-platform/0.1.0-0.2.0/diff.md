# Comparing `tmp/gerrit-to-platform-0.1.0.tar.gz` & `tmp/gerrit-to-platform-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerrit-to-platform-0.1.0.tar", last modified: Thu Mar 30 16:41:00 2023, max compression
+gzip compressed data, was "gerrit-to-platform-0.2.0.tar", last modified: Thu Jun 15 18:00:54 2023, max compression
```

## Comparing `gerrit-to-platform-0.1.0.tar` & `gerrit-to-platform-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.737861 gerrit-to-platform-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.725861 gerrit-to-platform-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.729861 gerrit-to-platform-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.github/workflows/gerrit-verify.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.gitreview
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-03-30 16:41:00.737861 gerrit-to-platform-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.729861 gerrit-to-platform-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.729861 gerrit-to-platform-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/conf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/license-header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.725861 gerrit-to-platform-0.1.0/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.729861 gerrit-to-platform-0.1.0/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/releasenotes/notes/initial_release-eb04a5f0690afc15.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:41:00.737861 gerrit-to-platform-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.725861 gerrit-to-platform-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.733861 gerrit-to-platform-0.1.0/src/gerrit_to_platform/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/change_merged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/comment_added.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform/patchset_created.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.733861 gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-03-30 16:41:00.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-30 16:41:00.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:41:00.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-30 16:41:00.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-30 16:41:00.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-30 16:41:00.000000 gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.737861 gerrit-to-platform-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:41:00.737861 gerrit-to-platform-0.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/github_workflow_empty_list.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/github_workflow_empty_list_get_workflows_return.json
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/github_workflow_list.json
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/github_workflow_list_filter_workflows_return.json
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/github_workflow_list_filter_workflows_return_merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/github_workflow_list_get_workflows_return.json
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/limited_replication_remotes_return_github.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/limited_replication_remotes_return_gitlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/replication.config
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/replication_remotes_return.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/fixtures/testconfig.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/test_change_merged.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/test_comment_added.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tests/test_patchset_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-30 16:40:45.000000 gerrit-to-platform-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.253065 gerrit-to-platform-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.225065 gerrit-to-platform-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.237065 gerrit-to-platform-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.github/workflows/gerrit-verify.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.gitreview
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-15 18:00:54.253065 gerrit-to-platform-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.241065 gerrit-to-platform-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.241065 gerrit-to-platform-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/onboard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/license-header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.225065 gerrit-to-platform-0.2.0/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.241065 gerrit-to-platform-0.2.0/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/releasenotes/notes/initial_release-eb04a5f0690afc15.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/releasenotes/notes/only-file-names-f0e5c44c8f62bca4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/releasenotes/notes/required_workflows-859326ccaa55da24.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:00:54.253065 gerrit-to-platform-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.225065 gerrit-to-platform-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.245065 gerrit-to-platform-0.2.0/src/gerrit_to_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/change_merged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/comment_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/patchset_created.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.245065 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.249065 gerrit-to-platform-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.249065 gerrit-to-platform-0.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_empty_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_empty_list_get_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_filter_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_filter_workflows_return_merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_get_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_required_filter_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/limited_replication_remotes_return_github.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/limited_replication_remotes_return_gitlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/replication.config
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/replication_remotes_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/testconfig.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_change_merged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_comment_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_patchset_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tox.ini
```

### Comparing `gerrit-to-platform-0.1.0/.coveragerc` & `gerrit-to-platform-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/.github/workflows/gerrit-verify.yaml` & `gerrit-to-platform-0.2.0/.github/workflows/gerrit-verify.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -45,44 +45,82 @@
 
 concurrency:
   group: ${{ github.event.inputs.GERRIT_CHANGE_ID || github.run_id }}
   cancel-in-progress: true
 
 
 jobs:
-  prepare:
+  clear-vote:
     runs-on: ubuntu-latest
-    outputs:
-      wheel-distribution: ${{ steps.wheel-distribution.outputs.path }}
     steps:
       - name: Clear votes
-        uses: lfit/gerrit-review-action@v0.2
+        uses: lfit/gerrit-review-action@v0.3
         with:
-          host: gerrit.linuxfoundation.org
+          host: ${{ vars.LFIT_GERRIT_SERVER }}
           username: ${{ vars.LFIT_GERRIT_SSH_USER }}
-          key: ${{ secrets.LFIT_GERRIT_SSH_PRIVKEY }}
-          passphrase: ${{ secrets.LFIT_GERRIT_SSH_PRIVKEY_PASSPHRASE }}
+          key: ${{ secrets.LFIT_GERRIT_SSH_PRIVKEY_NP }}
+          known_hosts: ${{ vars.LFIT_GERRIT_KNOWN_HOSTS }}
           gerrit-change-number: ${{ inputs.GERRIT_CHANGE_NUMBER }}
           gerrit-patchset-number: ${{ inputs.GERRIT_PATCHSET_NUMBER }}
           vote-type: clear
-      - uses: lfit/checkout-gerrit-change-action@v0.2
+      - name: Allow replication
+        run: sleep 10s
+
+  actionlint:
+    needs: clear-vote
+    runs-on: ubuntu-latest
+    steps:
+      - uses: lfit/checkout-gerrit-change-action@v0.3
+        with:
+          gerrit-refspec: ${{ inputs.GERRIT_REFSPEC }}
+          delay: "0s"
+      - name: Download actionlint
+        id: get_actionlint
+        # yamllint disable-line rule:line-length
+        run: bash <(curl https://raw.githubusercontent.com/rhysd/actionlint/main/scripts/download-actionlint.bash)
+        shell: bash
+      - name: Check workflow files
+        run: ${{ steps.get_actionlint.outputs.executable }} -color
+        shell: bash
+
+
+  pre-commit:
+    needs: clear-vote
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout change
+        uses: lfit/checkout-gerrit-change-action@v0.3
         with:
           gerrit-refspec: ${{ inputs.GERRIT_REFSPEC }}
           delay: "0s"
+      - name: Configure Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.11"
+      - name: Run static analysis and format checkers
+        # yamllint disable-line rule:line-length
+        run: SKIP=actionlint pipx run pre-commit run --all-files --show-diff-on-failure
+
+  prepare:
+    runs-on: ubuntu-latest
+    outputs:
+      wheel-distribution: ${{ steps.wheel-distribution.outputs.path }}
+    steps:
+      - uses: lfit/checkout-gerrit-change-action@v0.3
+        with:
+          gerrit-refspec: ${{ inputs.GERRIT_REFSPEC }}
       - uses: actions/setup-python@v4
         with:
           python-version: '3.8'
-      - name: Run static analysis and format checkers
-        run: pipx run pre-commit run --all-files --show-diff-on-failure
       - name: Build package distribution files
         run: >-
           pipx run tox -e clean,build
       - name: Record the path of wheel distribution
         id: wheel-distribution
-        run: echo "path=$(ls dist/*.whl)" >> $GITHUB_OUTPUT
+        run: echo "path=$(ls dist/*.whl)" >> "$GITHUB_OUTPUT"
       - name: Store the distribution files for use in other stages
         # `tests` and `publish` will use the same pre-built distributions,
         # so we make sure to release the exact same package that was tested
         uses: actions/upload-artifact@v3
         with:
           name: python-distribution-files
           path: dist/
@@ -94,60 +132,84 @@
       matrix:
         python:
           - "3.8"
         platform:
           - ubuntu-latest
     runs-on: ${{ matrix.platform }}
     steps:
-      - uses: lfit/checkout-gerrit-change-action@v0.2
+      - uses: lfit/checkout-gerrit-change-action@v0.3
         with:
           gerrit-refspec: ${{ inputs.GERRIT_REFSPEC }}
           delay: "0s"
       - uses: actions/setup-python@v4
         id: setup-python
         with:
           python-version: ${{ matrix.python }}
       - name: Retrieve pre-built distribution files
         uses: actions/download-artifact@v3
         with: {name: python-distribution-files, path: dist/}
       - name: Run tests
         run: >-
+          TOX_SKIP_ENV='(pre-commit)'
           pipx run --python '${{ steps.setup-python.outputs.python-path }}'
           tox --installpkg '${{ needs.prepare.outputs.wheel-distribution }}'
           -- -rFEx --durations 10 --color yes  # pytest args
       - name: Generate coverage report
         run: pipx run coverage lcov -o coverage.lcov
       - name: Upload partial coverage report
         uses: coverallsapp/github-action@master
         with:
           path-to-lcov: coverage.lcov
           github-token: ${{ secrets.github_token }}
           flag-name: ${{ matrix.platform }} - py${{ matrix.python }}
           parallel: true
 
 
+  CodeQL:
+    needs: clear-vote
+    runs-on: ubuntu-latest
+    permissions:
+      security-events: write
+
+    steps:
+      - name: Checkout change
+        uses: lfit/checkout-gerrit-change-action@v0.3
+        with:
+          gerrit-refspec: ${{ inputs.GERRIT_REFSPEC }}
+          delay: "0s"
+      - name: Configure Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.11"
+      - name: Initialize CodeQL
+        uses: github/codeql-action/init@v2
+        with:
+          languages: python
+      - name: Perform CodeQL Analysis
+        uses: github/codeql-action/analyze@v2
+
   finalize:
     needs: test
     runs-on: ubuntu-latest
     steps:
       - name: Finalize coverage report
         uses: coverallsapp/github-action@master
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
           parallel-finished: true
 
   vote:
     if: ${{ always() }}
-    needs: [prepare, test, finalize]
+    needs: [clear-vote, actionlint, pre-commit, prepare, test, finalize, CodeQL]
     runs-on: ubuntu-latest
     steps:
       - uses: technote-space/workflow-conclusion-action@v3
       - name: Set vote
-        uses: lfit/gerrit-review-action@v0.2
+        uses: lfit/gerrit-review-action@v0.3
         with:
-          host: gerrit.linuxfoundation.org
+          host: ${{ vars.LFIT_GERRIT_SERVER }}
           username: ${{ vars.LFIT_GERRIT_SSH_USER }}
-          key: ${{ secrets.LFIT_GERRIT_SSH_PRIVKEY }}
-          passphrase: ${{ secrets.LFIT_GERRIT_SSH_PRIVKEY_PASSPHRASE }}
+          key: ${{ secrets.LFIT_GERRIT_SSH_PRIVKEY_NP }}
+          known_hosts: ${{ vars.LFIT_GERRIT_KNOWN_HOSTS }}
           gerrit-change-number: ${{ inputs.GERRIT_CHANGE_NUMBER }}
           gerrit-patchset-number: ${{ inputs.GERRIT_PATCHSET_NUMBER }}
           vote-type: ${{ env.WORKFLOW_CONCLUSION }}
```

### Comparing `gerrit-to-platform-0.1.0/.github/workflows/release.yaml` & `gerrit-to-platform-0.2.0/.github/workflows/release.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 # yamllint disable-line rule:truthy
 on: push
 
 jobs:
   publish:
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
       - name: Configure Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.8'
       - name: Build package distribution files
         run: >-
           pipx run tox -e clean,build
-      - name: Configure TWINE
-        run: |
-          echo "TWINE_USERNAME=__token__" >> $GITHUB_ENV
-          echo "TWINE_PASSWORD=${{ secrets.PYPI_API_TOKEN }}" >> $GITHUB_ENV
       - name: Publish to PyPI
-        run: >-
-          pipx run tox -e publish -- --repository pypi
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `gerrit-to-platform-0.1.0/.gitignore` & `gerrit-to-platform-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/.gitlint` & `gerrit-to-platform-0.2.0/.gitlint`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/.pre-commit-config.yaml` & `gerrit-to-platform-0.2.0/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 exclude: '^docs/conf.py'
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: f71fa2c1f9cf5cb705f73dffe4b21f7c61470ba9  # frozen: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: check-ast
       - id: check-json
       - id: check-merge-conflict
       - id: check-xml
@@ -22,20 +22,20 @@
           - --branch=dev
           - --branch=master
           - --branch=main
           - --branch=rc
           - --branch=production
 
   - repo: https://github.com/jorisroovers/gitlint
-    rev: v0.19.1
+    rev: acc9d9de6369b76d22cb4167029d2035e8730b98  # frozen: v0.19.1
     hooks:
       - id: gitlint
 
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.30.0
+    rev: b05e028c5881819161d11cb543fd96a30c06cceb  # frozen: v1.32.0
     hooks:
       - id: yamllint
         types: [yaml]
 
   ## If you want to automatically "modernize" your Python code:
   # - repo: https://github.com/asottile/pyupgrade
   #   rev: v3.3.1
@@ -51,47 +51,52 @@
   #     args: [
   #       --in-place,
   #       --remove-all-unused-imports,
   #       --remove-unused-variables,
   #     ]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: dbf82f2dd09ae41d9355bcd7ab69187a19e6bf2f  # frozen: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: bf7a16254ec96b084a6caf3d435ec18f0f245cc7  # frozen: 23.3.0
     hooks:
       - id: black
         language_version: python3
 
   ## If like to embrace black styles even in the docs:
   # - repo: https://github.com/asottile/blacken-docs
   #   rev: v1.13.0
   #   hooks:
   #   - id: blacken-docs
   #     additional_dependencies: [black]
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: c838a5e98878f17889cfce311e1406d252f87ec5  # frozen: 6.0.0
     hooks:
       - id: flake8
         args: ["--max-line-length=120"]
         additional_dependencies: [Flake8-pyproject]
 
   ## Check for misspells in documentation files:
   # - repo: https://github.com/codespell-project/codespell
   #   rev: v2.2.2
   #   hooks:
   #   - id: codespell
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: bd424e49d4f0181d4c8b8909a8cd5ce9eb058044  # frozen: v1.3.0
     hooks:
       - id: mypy
 
   - repo: https://github.com/btford/write-good
-    rev: v1.0.8
+    rev: ab66ce10136dfad5146e69e70f82a3efac8842c1  # frozen: v1.0.8
     hooks:
       - id: write-good
         files: "\\.(rst|md|markdown|mdown|mkdn)$"
+
+  - repo: https://github.com/rhysd/actionlint
+    rev: fd7ba3c382e13dcc0248e425b4cbc3f1185fa3ee  # frozen: v1.6.24
+    hooks:
+      - id: actionlint
```

### Comparing `gerrit-to-platform-0.1.0/.readthedocs.yml` & `gerrit-to-platform-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/CONTRIBUTING.rst` & `gerrit-to-platform-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/LICENSE.txt` & `gerrit-to-platform-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/PKG-INFO` & `gerrit-to-platform-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrit-to-platform
-Version: 0.1.0
+Version: 0.2.0
 Summary: Gerrit to GitHub / GitLab
 Author-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 Maintainer-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -306,34 +306,113 @@
     [gitlab.com]
     token = <a_token_that_allows_triggering_workflows>
 
 
 The ``content-added`` mapping section is a key value pair for comment triggers
 to the corresponding workflow name or filename
 
-.. _Gerrit: https://www.gerritcodereview.com/
-.. _GitHub: https://github.com
-.. _GitLab: https://gitlab.com
-.. _hooks: https://gerrit.googlesource.com/plugins/hooks/+doc/master/src/main/resources/Documentation/about.md
+GitHub Workflow Configuration
+=============================
+
+There are three hooks that gerrit-to-platform handles:
+
+* patchset-created (search filter: verify)
+* change-merged (search filter: merge)
+* comment-added (comment mapping for keyword to search filter)
+
+Configuration for triggered workflows must meet the following requirements:
+
+* The workflow filename must contain 'gerrit'
+* The workflow filename must contain the search filter
+
+Required workflows must be part of the ORGANIZATION/.github magic repository.
+These workflow filenames must also contain 'required'
+
+ex: ``.github/workflows/gerrit-verify.yaml`` or
+``.github/workflows/gerrit-required-verify.yaml``
+
+Standard workflows (non-required ones) must have the following primary configuration::
+
+    ---
+    name: Gerrit Verify
+
+    # yamllint disable-line rule:truthy
+    on:
+      workflow_dispatch:
+        inputs:
+          GERRIT_BRANCH:
+            description: 'Branch that change is against'
+            required: true
+            type: string
+          GERRIT_CHANGE_ID:
+            description: 'The ID for the change'
+            required: true
+            type: string
+          GERRIT_CHANGE_NUMBER:
+            description: 'The Gerrit number'
+            required: true
+            type: string
+          GERRIT_CHANGE_URL:
+            description: 'URL to the change'
+            required: true
+            type: string
+          GERRIT_EVENT_TYPE:
+            description: 'Gerrit event type'
+            required: true
+            type: string
+          GERRIT_PATCHSET_NUMBER:
+            description: 'The patch number for the change'
+            required: true
+            type: string
+          GERRIT_PATCHSET_REVISION:
+            description: 'The revision sha'
+            required: true
+            type: string
+          GERRIT_PROJECT:
+            description: 'Project in Gerrit'
+            required: true
+            type: string
+          GERRIT_REFSPEC:
+            description: 'Gerrit refspec of change'
+            required: true
+            type: string
+
+
+    concurrency:
+      group: ${{ github.event.inputs.GERRIT_CHANGE_ID || github.run_id }}
+      cancel-in-progress: true
+
+    jobs:
+      <your_job_configurations>
+
+Required workflows must have the following extra input::
+
+    TARGET_REPO:
+      description: 'The target GitHub repository needing the required workflow'
+      required: true
+      type: string
 
-.. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
 
 This project uses `pre-commit`_, please make sure to install it before making any
 changes::
 
     pip install pre-commit
     cd gerrit_to_platform
     pre-commit install
     pre-commit install -t commit-msg
 
 Don't forget to tell your contributors to also install and use pre-commit.
 
-.. _pre-commit: https://pre-commit.com/
-
 Note
 ====
 
 PyScaffold 4.4 provided the initial project setup. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
+
+.. _Gerrit: https://www.gerritcodereview.com/
+.. _GitHub: https://github.com
+.. _GitLab: https://gitlab.com
+.. _hooks: https://gerrit.googlesource.com/plugins/hooks/+doc/master/src/main/resources/Documentation/about.md
+.. _pre-commit: https://pre-commit.com/
```

### Comparing `gerrit-to-platform-0.1.0/docs/Makefile` & `gerrit-to-platform-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/docs/_static/logo.png` & `gerrit-to-platform-0.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/docs/conf.py` & `gerrit-to-platform-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/pyproject.toml` & `gerrit-to-platform-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Version Control :: Git"
 ]
 
 dependencies = [
     "ghapi~=1.0.3",
-    "typer[all]~=0.7.0",
+    "typer[all]~=0.9.0",
     "xdg~=5.1.1"
 ]
 
 [project.optional-dependencies]
 testing = [
     "setuptools",
     "pytest",
```

### Comparing `gerrit-to-platform-0.1.0/src/gerrit_to_platform/__init__.py` & `gerrit-to-platform-0.2.0/src/gerrit_to_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/src/gerrit_to_platform/config.py` & `gerrit-to-platform-0.2.0/src/gerrit_to_platform/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     """Platform Dictionary definition."""
 
     github: PlatformType
     gitlab: PlatformType
 
 
 class Platform(Enum):
+    """Enumeration of all platforms recognized by the app."""
+
     GITHUB = "github"
     GITLAB = "gitlab"
 
 
 G2P_CONFIG_FILE = os.path.join(
     XDG_CONFIG_HOME, "gerrit_to_platform", "gerrit_to_platform.ini"
 )
@@ -59,35 +61,59 @@
 CONFIG_FILES = {
     CONFIG: G2P_CONFIG_FILE,
     REPLICATION: GERRIT_REPLICATION_CONFIG,
 }
 
 
 def get_config(config_type: str = DEFAULT_CONFIG) -> ConfigParser:
-    """Get the config object."""
+    """
+    Get the config object.
+
+    Args:
+        config_type (str): Type of configuration file that the parser should use
+
+    Returns:
+        ConfigParser: A loaded ConfigParser object with the requested
+            configuration file
+    """
     config = configparser.ConfigParser()
     conf_file = CONFIG_FILES[config_type]
     with open(conf_file) as config_file:
         config.read_file(config_file, conf_file)
     return config
 
 
 def get_mapping(mapping_section: str) -> Union[Dict[str, str], None]:
-    """Return all of the keyword to job mappings"""
+    """
+    Return all of the keyword to job mappings
+
+    Args:
+        mapping_section (str): the section of the config file to load
+
+    Returns:
+        Optional(Dict[str,str]): The key / value mapping object or None if it
+            does not exist
+    """
     config = get_config()
 
     section = f'mapping "{mapping_section}"'
     if section in config.sections():
         return dict(config.items(section))
 
     return None
 
 
 def get_replication_remotes() -> ReplicationRemotes:
-    """Get the replication remotes available."""
+    """
+    Get the replication remotes available.
+
+    Returns:
+        ReplicationRemotes: All the replication remotes defined the Gerrit
+            configuration file
+    """
     remotes_config = get_config(REPLICATION)
     remotes: ReplicationRemotes = {}
 
     for section in remotes_config.sections():
         if 'remote "' not in section:
             continue
 
@@ -136,20 +162,39 @@
                 }
             }
 
     return remotes
 
 
 def has_section(section: str) -> bool:
-    """Indicate if section exists in config file."""
+    """
+    Indicate if section exists in config file.
+
+    Args:
+        section (str): config section to lookup
+
+    Returns:
+        bool: True if the section exists in configuration, False otherwise
+    """
     config = get_config()
     return config.has_section(section)
 
 
 def get_setting(section: str, option: Optional[str] = None) -> Union[list, str]:
-    """Get all configuration options from a section, or specific option from a section."""
+    """
+    Get all configuration options from a section, or specific option from a
+    section.
+
+    Args:
+        section (str): config section to use
+        option (Optional[str]): a suboption to get from the section
+
+    Returns:
+        list: all of the configuration for a section
+        str: the single sub-option of a section
+    """
     config = get_config()
 
     if option:
         return config.get(section, option)
 
     return config.options(section)
```

### Comparing `gerrit-to-platform-0.1.0/src/gerrit_to_platform/patchset_created.py` & `gerrit-to-platform-0.2.0/src/gerrit_to_platform/patchset_created.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,41 +6,58 @@
 # available under the terms of the Apache-2.0 license which accompanies this
 # distribution, and is available at
 # https://opensource.org/licenses/Apache-2.0
 ##############################################################################
 """Handler for patchset-created events."""
 
 import typer
+from typing_extensions import Annotated
 
 from gerrit_to_platform.helpers import (
     find_and_dispatch,
     get_change_id,
     get_change_number,
     get_change_refspec,
 )
 
 app = typer.Typer()
 
 
 @app.command()
 def patchset_created(
-    change: str = typer.Option(..., help="change id"),
-    kind: str = typer.Option(..., help="change kind"),
-    change_url: str = typer.Option(..., help="change url"),
-    change_owner: str = typer.Option(..., help="change owner"),
-    change_owner_username: str = typer.Option(..., help="username"),
-    project: str = typer.Option(..., help="project name"),
-    branch: str = typer.Option(..., help="branch"),
-    topic: str = typer.Option(..., help="topic"),
-    uploader: str = typer.Option(..., help="uploader"),
-    uploader_username: str = typer.Option(..., help="username"),
-    commit: str = typer.Option(..., help="sha1"),
-    patchset: str = typer.Option(..., help="patchset id"),
+    change: Annotated[str, typer.Option(help="change id")],
+    kind: Annotated[str, typer.Option(help="change kind")],
+    change_url: Annotated[str, typer.Option(help="change url")],
+    change_owner: Annotated[str, typer.Option(help="change owner")],
+    change_owner_username: Annotated[str, typer.Option(help="username")],
+    project: Annotated[str, typer.Option(help="project name")],
+    branch: Annotated[str, typer.Option(help="branch")],
+    topic: Annotated[str, typer.Option(help="topic")],
+    uploader: Annotated[str, typer.Option(help="uploader")],
+    uploader_username: Annotated[str, typer.Option(help="username")],
+    commit: Annotated[str, typer.Option(help="sha1")],
+    patchset: Annotated[str, typer.Option(help="patchset id")],
 ):
-    """Handle patcheset-created hook."""
+    """
+    Handle patcheset-created hook.
+
+    Args:
+        change (str): change ID
+        kind (str): type of change
+        change_url (str): change URL
+        change_owner (str): change owner eg: 'Foo <foo@example.com>'
+        change_owner_username (str): change owner username eg: 'foo'
+        project (str): Gerrit project name
+        branch (str): branch change is against
+        topic (str): topic change is part of
+        uploader (str): uploader of change eg: 'Foo <foo@example.com>'
+        uploader_username (str): uploader of change username eg: 'foo'
+        commit (str): SHA1 of commit
+        patchset (str): patchset number
+    """
 
     change_id = get_change_id(change)
     change_number = get_change_number(change_url)
     refspec = get_change_refspec(change_number, patchset)
 
     inputs = {
         "GERRIT_BRANCH": branch,
```

### Comparing `gerrit-to-platform-0.1.0/src/gerrit_to_platform.egg-info/PKG-INFO` & `gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrit-to-platform
-Version: 0.1.0
+Version: 0.2.0
 Summary: Gerrit to GitHub / GitLab
 Author-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 Maintainer-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -306,34 +306,113 @@
     [gitlab.com]
     token = <a_token_that_allows_triggering_workflows>
 
 
 The ``content-added`` mapping section is a key value pair for comment triggers
 to the corresponding workflow name or filename
 
-.. _Gerrit: https://www.gerritcodereview.com/
-.. _GitHub: https://github.com
-.. _GitLab: https://gitlab.com
-.. _hooks: https://gerrit.googlesource.com/plugins/hooks/+doc/master/src/main/resources/Documentation/about.md
+GitHub Workflow Configuration
+=============================
+
+There are three hooks that gerrit-to-platform handles:
+
+* patchset-created (search filter: verify)
+* change-merged (search filter: merge)
+* comment-added (comment mapping for keyword to search filter)
+
+Configuration for triggered workflows must meet the following requirements:
+
+* The workflow filename must contain 'gerrit'
+* The workflow filename must contain the search filter
+
+Required workflows must be part of the ORGANIZATION/.github magic repository.
+These workflow filenames must also contain 'required'
+
+ex: ``.github/workflows/gerrit-verify.yaml`` or
+``.github/workflows/gerrit-required-verify.yaml``
+
+Standard workflows (non-required ones) must have the following primary configuration::
+
+    ---
+    name: Gerrit Verify
+
+    # yamllint disable-line rule:truthy
+    on:
+      workflow_dispatch:
+        inputs:
+          GERRIT_BRANCH:
+            description: 'Branch that change is against'
+            required: true
+            type: string
+          GERRIT_CHANGE_ID:
+            description: 'The ID for the change'
+            required: true
+            type: string
+          GERRIT_CHANGE_NUMBER:
+            description: 'The Gerrit number'
+            required: true
+            type: string
+          GERRIT_CHANGE_URL:
+            description: 'URL to the change'
+            required: true
+            type: string
+          GERRIT_EVENT_TYPE:
+            description: 'Gerrit event type'
+            required: true
+            type: string
+          GERRIT_PATCHSET_NUMBER:
+            description: 'The patch number for the change'
+            required: true
+            type: string
+          GERRIT_PATCHSET_REVISION:
+            description: 'The revision sha'
+            required: true
+            type: string
+          GERRIT_PROJECT:
+            description: 'Project in Gerrit'
+            required: true
+            type: string
+          GERRIT_REFSPEC:
+            description: 'Gerrit refspec of change'
+            required: true
+            type: string
+
+
+    concurrency:
+      group: ${{ github.event.inputs.GERRIT_CHANGE_ID || github.run_id }}
+      cancel-in-progress: true
+
+    jobs:
+      <your_job_configurations>
+
+Required workflows must have the following extra input::
+
+    TARGET_REPO:
+      description: 'The target GitHub repository needing the required workflow'
+      required: true
+      type: string
 
-.. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
 
 This project uses `pre-commit`_, please make sure to install it before making any
 changes::
 
     pip install pre-commit
     cd gerrit_to_platform
     pre-commit install
     pre-commit install -t commit-msg
 
 Don't forget to tell your contributors to also install and use pre-commit.
 
-.. _pre-commit: https://pre-commit.com/
-
 Note
 ====
 
 PyScaffold 4.4 provided the initial project setup. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
+
+.. _Gerrit: https://www.gerritcodereview.com/
+.. _GitHub: https://github.com
+.. _GitLab: https://gitlab.com
+.. _hooks: https://gerrit.googlesource.com/plugins/hooks/+doc/master/src/main/resources/Documentation/about.md
+.. _pre-commit: https://pre-commit.com/
```

### Comparing `gerrit-to-platform-0.1.0/tests/conftest.py` & `gerrit-to-platform-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/tests/fixtures/github_workflow_list.json` & `gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'workflows'": "{insert: [(1, OrderedDict([('id', 20937807), ('node_id', 'W_kwDOFzVD3s4BZnjK'), "*

 * *                "('name', 'Gerrit Verify'), ('path', '.github/workflows/gerrit-verify.yaml'), "*

 * *                "('state', 'active'), ('created_at', '2022-01-18T21:49:30.000-08:00'), "*

 * *                "('updated_at', '2022-01-18T21:56:17.000-08:00'), ('url', "*

 * *                "'https://api.github.com/repos/example/example/actions/workflows/18525370'), "*

 * *                "('html_url', "*

 * *                "'https:/ […]*

```diff
@@ -10,14 +10,38 @@
             "node_id": "W_kwDOFzVD3s4BFfHK",
             "path": ".github/workflows/codeql-analysis.yaml",
             "state": "disabled_manually",
             "updated_at": "2022-01-18T21:56:17.000-08:00",
             "url": "https://api.github.com/repos/example/example/actions/workflows/18215370"
         },
         {
+            "badge_url": "https://github.com/example/example/workflows/gerrit-verify/badge.svg",
+            "created_at": "2022-01-18T21:49:30.000-08:00",
+            "html_url": "https://github.com/example/example/blob/main/.github/workflows/gerrit-verify.yaml",
+            "id": 20937807,
+            "name": "Gerrit Verify",
+            "node_id": "W_kwDOFzVD3s4BZnjK",
+            "path": ".github/workflows/gerrit-verify.yaml",
+            "state": "active",
+            "updated_at": "2022-01-18T21:56:17.000-08:00",
+            "url": "https://api.github.com/repos/example/example/actions/workflows/18525370"
+        },
+        {
+            "badge_url": "https://github.com/example/example/workflows/gerrit-required-verify/badge.svg",
+            "created_at": "2022-01-18T21:49:30.000-08:00",
+            "html_url": "https://github.com/example/example/blob/main/.github/workflows/gerrit-required-verify.yaml",
+            "id": 20937808,
+            "name": "Required Gerrit Verify",
+            "node_id": "W_kwDOFzVD3s5BZnjK",
+            "path": ".github/workflows/gerrit-required-verify.yaml",
+            "state": "active",
+            "updated_at": "2022-01-18T21:56:17.000-08:00",
+            "url": "https://api.github.com/repos/example/example/actions/workflows/20937808"
+        },
+        {
             "badge_url": "https://github.com/example/example/workflows/verify/badge.svg",
             "created_at": "2022-01-18T21:49:30.000-08:00",
             "html_url": "https://github.com/example/example/blob/main/.github/workflows/verify.yaml",
             "id": 18525370,
             "name": "Verify",
             "node_id": "W_kwDOFzVD3s4BYhHK",
             "path": ".github/workflows/verify.yaml",
```

### Comparing `gerrit-to-platform-0.1.0/tests/fixtures/replication.config` & `gerrit-to-platform-0.2.0/tests/fixtures/replication.config`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/tests/test_change_merged.py` & `gerrit-to-platform-0.2.0/tests/test_change_merged.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/tests/test_comment_added.py` & `gerrit-to-platform-0.2.0/tests/test_comment_added.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/tests/test_config.py` & `gerrit-to-platform-0.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/tests/test_github.py` & `gerrit-to-platform-0.2.0/tests/test_github.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from fastcore.net import HTTP404NotFoundError  # type: ignore
 
 import gerrit_to_platform.config  # type: ignore
 import gerrit_to_platform.github  # type: ignore
 from gerrit_to_platform.config import CONFIG, REPLICATION
 from gerrit_to_platform.github import (  # type: ignore
     dispatch_workflow,
+    filter_path,
     filter_workflows,
     get_workflows,
 )
 
 FIXTURE_DIR = os.path.join(
     os.path.dirname(os.path.realpath(__file__)),
     "fixtures",
@@ -49,14 +50,18 @@
     FIXTURE_DIR, "github_workflow_empty_list_get_workflows_return.json"
 )
 
 GITHUB_FILTERED_LIST = os.path.join(
     FIXTURE_DIR, "github_workflow_list_filter_workflows_return.json"
 )
 
+GITHUB_REQUIRED_FILTERED_LIST = os.path.join(
+    FIXTURE_DIR, "github_workflow_list_required_filter_workflows_return.json"
+)
+
 
 def test_dispatch_workflow(mocker):
     """Test workflow triggering."""
     mocker.patch.object(
         gerrit_to_platform.config,
         "CONFIG_FILES",
         MOCK_CONFIG_FILES,
@@ -121,20 +126,39 @@
     assert expected == actual
 
     mock_GhApi.actions.list_repo_workflows = mock_list_repo_workflows_exception
     actual = get_workflows("example", "repository")
     assert expected == actual
 
 
+def test_filter_path(mocker):
+    """Test filter_path"""
+    # use upper case to validate that filter works case insensitive
+    workflow = {"path": ".GITHUB/WORKFLOWS/GERRIT-VERIFY.yaml"}
+
+    expected = True
+    actual = filter_path("verify", workflow)
+    assert actual == expected
+
+    expected = False
+    actual = filter_path("merge", workflow)
+    assert actual == expected
+
+
 def test_filter_workflows(mocker):
     """Return workflows that match filter."""
     with open(GITHUB_WORKFLOW_LIST_RETURN) as list_file:
         get_workflows_return = json.load(list_file)
     with open(GITHUB_FILTERED_LIST) as list_file:
         expected = json.load(list_file)
 
     mocker.patch(
         "gerrit_to_platform.github.get_workflows", return_value=get_workflows_return
     )
 
     actual = filter_workflows("example", "repository", "verify")
     assert expected == actual
+
+    with open(GITHUB_REQUIRED_FILTERED_LIST) as list_file:
+        expected = json.load(list_file)
+    actual = filter_workflows("example", "repository", "verify", True)
+    assert expected == actual
```

### Comparing `gerrit-to-platform-0.1.0/tests/test_helpers.py` & `gerrit-to-platform-0.2.0/tests/test_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     choose_dispatch,
     choose_filter_workflows,
     convert_repo_name,
     find_and_dispatch,
     get_change_id,
     get_change_number,
     get_change_refspec,
+    get_magic_repo,
 )
 
 FIXTURE_DIR = os.path.join(
     os.path.dirname(os.path.realpath(__file__)),
     "fixtures",
 )
 
@@ -45,24 +46,37 @@
     FIXTURE_DIR, "limited_replication_remotes_return_github.json"
 )
 
 REPLICATION_REMOTES_GITLAB = os.path.join(
     FIXTURE_DIR, "limited_replication_remotes_return_gitlab.json"
 )
 
+REQUIRED_VERIFY_FILTERED_WORKFLOWS = os.path.join(
+    FIXTURE_DIR, "github_workflow_list_required_filter_workflows_return.json"
+)
+
+PATCH1_GERRIT_VERIFY = (
+    "Dispatching workflow 'Gerrit Verify', id 20937807 on "
+    + "github:example/example-project for change 1 patch 1"
+)
 PATCH1_VERIFY = (
     "Dispatching workflow 'Verify', id 18525370 on "
     + "github:example/example-project for change 1 patch 1"
 )
+PATCH1_REQUIRED_VERIFY = (
+    "Dispatching required workflow 'Required Gerrit Verify', id 20937808 on "
+    + "github:example/.github for change 1 patch 1 against "
+    + "github:example/example-project"
+)
 PATCH1_CHECK_MAIN = (
     "Dispatching workflow 'Check Main', id 17098575 on "
     + "github:example/example-project for change 1 patch 1"
 )
 CHANGE2_MERGE = (
-    "Dispatching workflow 'Merge', id 18525370 on "
+    "Dispatching workflow 'Gerrit Merge', id 18525370 on "
     + "github:example/example-project for change 1 patch 1"
 )
 
 
 def test_choose_dispatch(mocker):
     """Test choose_dispatch."""
     expected = github.dispatch_workflow
@@ -127,18 +141,22 @@
 
     mocker.patch(
         "gerrit_to_platform.helpers.get_replication_remotes",
         return_value=replication_remotes,
     )
 
     def mock_filter_workflows(
-        owner: str, repo: str, search_filter: str
+        owner: str, repo: str, search_filter: str, search_required: bool = False
     ) -> List[Dict[str, str]]:
         """Mock of filter_workflows."""
         filter_file = VERIFY_FILTERED_WORKFLOWS
+
+        if search_required:
+            filter_file = REQUIRED_VERIFY_FILTERED_WORKFLOWS
+
         if search_filter == "merge":
             filter_file = MERGE_FILTERED_WORKFLOWS
 
         with open(filter_file) as workflows:
             return json.load(workflows)
 
     def mock_choose_filter_workflows(platform: Platform) -> Union[Callable, None]:
@@ -171,30 +189,34 @@
         gerrit_to_platform.helpers,
         "choose_dispatch",
         mock_choose_dispatch,
     )
 
     find_and_dispatch("example-project", "verify", inputs)
     actual = capfd.readouterr().out
-    assert PATCH1_VERIFY in actual
-    assert PATCH1_CHECK_MAIN in actual
+    assert PATCH1_GERRIT_VERIFY in actual
+    assert PATCH1_VERIFY not in actual
+    assert PATCH1_REQUIRED_VERIFY in actual
+    assert PATCH1_CHECK_MAIN not in actual
 
     find_and_dispatch("example-project", "merge", inputs)
     actual = capfd.readouterr().out
     assert CHANGE2_MERGE in actual
 
     with open(REPLICATION_REMOTES_GITLAB) as remotes:
         replication_remotes = json.load(remotes)
     mocker.patch(
         "gerrit_to_platform.helpers.get_replication_remotes",
         return_value=replication_remotes,
     )
     find_and_dispatch("example-project", "verify", inputs)
     actual = capfd.readouterr().out
+    assert PATCH1_GERRIT_VERIFY not in actual
     assert PATCH1_VERIFY not in actual
+    assert PATCH1_REQUIRED_VERIFY not in actual
     assert PATCH1_CHECK_MAIN not in actual
     assert actual == ""
 
 
 def test_get_change_id(mocker):
     """Test get_change_id"""
     expected = "Ibaz"
@@ -218,7 +240,18 @@
     expected = "refs/changes/01/1/2"
     actual = get_change_refspec("1", "2")
     assert expected == actual
 
     expected = "refs/changes/02/202/1"
     actual = get_change_refspec("202", "1")
     assert expected == actual
+
+
+def test_get_magic_repo(mocker):
+    """Test get_magic_repo"""
+    expected = ".github"
+    actual = get_magic_repo(Platform.GITHUB)
+    assert expected == actual
+
+    expected = None
+    actual = get_magic_repo(Platform.GITLAB)
+    assert expected == actual
```

### Comparing `gerrit-to-platform-0.1.0/tests/test_patchset_created.py` & `gerrit-to-platform-0.2.0/tests/test_patchset_created.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.1.0/tox.ini` & `gerrit-to-platform-0.2.0/tox.ini`

 * *Files identical despite different names*

