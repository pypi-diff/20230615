# Comparing `tmp/edx-enterprise-data-4.6.8.tar.gz` & `tmp/edx-enterprise-data-4.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-data-4.6.8.tar", last modified: Wed Jun 14 18:12:39 2023, max compression
+gzip compressed data, was "edx-enterprise-data-4.6.9.tar", last modified: Wed Jun 14 23:03:23 2023, max compression
```

## Comparing `edx-enterprise-data-4.6.8.tar` & `edx-enterprise-data-4.6.9.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/
--rw-r--r--   0 runner    (1001) docker     (122)    16702 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.758684 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6722 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.758684 edx-enterprise-data-4.6.8/enterprise_data/
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.758684 edx-enterprise-data-4.6.8/enterprise_data/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5945 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    17282 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/clients.py
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_enrollment.json
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_user.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_offer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.766684 edx-enterprise-data-4.6.8/enterprise_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0002_auto_20180430_1358.py
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0003_auto_20180501_0603.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0004_auto_20180501_0928.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0004_auto_20180508_1652.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0005_auto_20180524_2204.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0006_auto_20180612_0336.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0007_auto_20180612_0534.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0008_auto_20180614_0108.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0009_auto_20180628_1152.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0010_enterpriseenrollment_created.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0011_enterpriseuser.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0012_auto_20180831_1930.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0013_auto_20180831_1931.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0014_enterpriseuser_created.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0015_auto_20180907_1757.py
--rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0016_auto_20180924_2138.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0021_auto_20190329_1241.py
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)      635 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0024_auto_20210602_1811.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0025_auto_20210703_1854.py
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0026_auto_20210916_0414.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0029_enterpriseoffer.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0030_auto_20230609_1353.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/settings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    11838 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data_roles/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/vertica.py
--rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/external_resource_link_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/enterprise_customer_reporting.json
--rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/send_enterprise_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_enterprise_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_external_link_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_send_enterprise_reports.py
--rw-r--r--   0 runner    (1001) docker     (122)     8871 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_vertica_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9503 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/reporting.in
--rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/test-reporting.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.804006 edx-enterprise-data-4.6.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    16836 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 23:03:23.804006 edx-enterprise-data-4.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.768004 edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 23:03:23.000000 edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6722 2023-06-14 23:03:23.000000 edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 23:03:23.000000 edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 23:03:23.000000 edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-14 23:03:23.000000 edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-14 23:03:23.000000 edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.768004 edx-enterprise-data-4.6.9/enterprise_data/
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.768004 edx-enterprise-data-4.6.9/enterprise_data/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.768004 edx-enterprise-data-4.6.9/enterprise_data/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v0/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v0/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v0/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.772004 edx-enterprise-data-4.6.9/enterprise_data/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17682 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.780004 edx-enterprise-data-4.6.9/enterprise_data/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/fixtures/enterprise_enrollment.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/fixtures/enterprise_user.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.780004 edx-enterprise-data-4.6.9/enterprise_data/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.780004 edx-enterprise-data-4.6.9/enterprise_data/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_offer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.784005 edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.792005 edx-enterprise-data-4.6.9/enterprise_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0002_auto_20180430_1358.py
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0003_auto_20180501_0603.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0004_auto_20180501_0928.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0004_auto_20180508_1652.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0005_auto_20180524_2204.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0006_auto_20180612_0336.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0007_auto_20180612_0534.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0008_auto_20180614_0108.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0009_auto_20180628_1152.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0010_enterpriseenrollment_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0011_enterpriseuser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0012_auto_20180831_1930.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0013_auto_20180831_1931.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0014_enterpriseuser_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0015_auto_20180907_1757.py
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0016_auto_20180924_2138.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0021_auto_20190329_1241.py
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0024_auto_20210602_1811.py
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0025_auto_20210703_1854.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0026_auto_20210916_0414.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0029_enterpriseoffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/0030_auto_20230609_1353.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.792005 edx-enterprise-data-4.6.9/enterprise_data/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/settings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.792005 edx-enterprise-data-4.6.9/enterprise_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.792005 edx-enterprise-data-4.6.9/enterprise_data/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.792005 edx-enterprise-data-4.6.9/enterprise_data/tests/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/api/v0/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.792005 edx-enterprise-data-4.6.9/enterprise_data/tests/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/api/v1/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/api/v1/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11838 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.796005 edx-enterprise-data-4.6.9/enterprise_data_roles/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.796005 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.796005 edx-enterprise-data-4.6.9/enterprise_data_roles/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_data_roles/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.796005 edx-enterprise-data-4.6.9/enterprise_reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.796005 edx-enterprise-data-4.6.9/enterprise_reporting/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/clients/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/clients/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/clients/vertica.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/external_resource_link_report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.800006 edx-enterprise-data-4.6.9/enterprise_reporting/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/fixtures/enterprise_customer_reporting.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/send_enterprise_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.800006 edx-enterprise-data-4.6.9/enterprise_reporting/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_enterprise_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_external_link_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_send_enterprise_reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8871 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_vertica_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/enterprise_reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:03:23.800006 edx-enterprise-data-4.6.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9503 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/reporting.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/test-reporting.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 23:03:23.804006 edx-enterprise-data-4.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-14 23:03:16.000000 edx-enterprise-data-4.6.9/setup.py
```

### Comparing `edx-enterprise-data-4.6.8/CHANGELOG.rst` & `edx-enterprise-data-4.6.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 =========================
+[4.6.9] - 2023-06-14
+--------------------
+  * Allow querying of offers by either new style UUIDs or old style enterprise ID numbers.
+
 [4.6.8] - 2023-06-14
 --------------------
   * Add to_internal_value method for offer_id translation.
 
 [4.6.7] - 2023-06-14
 --------------------
   * Add support for offer_id to be either an integer or a UUID.
```

### Comparing `edx-enterprise-data-4.6.8/LICENSE` & `edx-enterprise-data-4.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/MANIFEST.in` & `edx-enterprise-data-4.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/PKG-INFO` & `edx-enterprise-data-4.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.6.8
+Version: 4.6.9
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-enterprise-data-4.6.8/README.md` & `edx-enterprise-data-4.6.9/README.md`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/PKG-INFO` & `edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.6.8
+Version: 4.6.9
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/SOURCES.txt` & `edx-enterprise-data-4.6.9/edx_enterprise_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/api/v0/serializers.py` & `edx-enterprise-data-4.6.9/enterprise_data/api/v0/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/api/v0/urls.py` & `edx-enterprise-data-4.6.9/enterprise_data/api/v0/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/api/v0/views.py` & `edx-enterprise-data-4.6.9/enterprise_data/api/v0/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/api/v1/urls.py` & `edx-enterprise-data-4.6.9/enterprise_data/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/api/v1/views.py` & `edx-enterprise-data-4.6.9/enterprise_data/api/v1/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,19 +263,30 @@
     """
     Viewset for enterprise offers.
     """
     serializer_class = serializers.EnterpriseOfferSerializer
     filter_backends = (filters.OrderingFilter, DjangoFilterBackend,)
     ordering_fields = '__all__'
 
+    lookup_field = 'offer_id'
+
     filterset_fields = (
         'offer_id',
         'status'
     )
 
+    def get_object(self):
+        """
+        This ensures that UUIDs with dashes are properly handled when requesting info about offers.
+
+        Related to the work in EnterpriseOfferSerializer with `to_internal_value` and `to_representation`
+        """
+        self.kwargs['offer_id'] = self.kwargs['offer_id'].replace('-', '')
+        return super().get_object()
+
     def get_queryset(self):
         enterprise_customer_uuid = self.kwargs['enterprise_id']
         return EnterpriseOffer.objects.filter(
             enterprise_customer_uuid=enterprise_customer_uuid,
         )
```

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/clients.py` & `edx-enterprise-data-4.6.9/enterprise_data/clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/filters.py` & `edx-enterprise-data-4.6.9/enterprise_data/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_enrollment.json` & `edx-enterprise-data-4.6.9/enterprise_data/fixtures/enterprise_enrollment.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_user.json` & `edx-enterprise-data-4.6.9/enterprise_data/fixtures/enterprise_user.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_dummy_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_enrollment.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_offer.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_offer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_user.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_user.py` & `edx-enterprise-data-4.6.9/enterprise_data/management/commands/tests/test_create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0001_initial.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0002_auto_20180430_1358.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0002_auto_20180430_1358.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0006_auto_20180612_0336.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0006_auto_20180612_0336.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0007_auto_20180612_0534.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0007_auto_20180612_0534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0008_auto_20180614_0108.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0008_auto_20180614_0108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0009_auto_20180628_1152.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0009_auto_20180628_1152.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0011_enterpriseuser.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0011_enterpriseuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0012_auto_20180831_1930.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0012_auto_20180831_1930.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0020_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0020_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0021_auto_20190329_1241.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0021_auto_20190329_1241.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0024_auto_20210602_1811.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0024_auto_20210602_1811.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0026_auto_20210916_0414.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0026_auto_20210916_0414.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0029_enterpriseoffer.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0029_enterpriseoffer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/migrations/0030_auto_20230609_1353.py` & `edx-enterprise-data-4.6.9/enterprise_data/migrations/0030_auto_20230609_1353.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/models.py` & `edx-enterprise-data-4.6.9/enterprise_data/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/settings/test.py` & `edx-enterprise-data-4.6.9/enterprise_data/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/test_serializers.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/api/v0/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_serializers.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/api/v1/test_serializers.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,58 +46,51 @@
 @ddt.ddt
 class TestEnterpriseOfferSerializer(APITransactionTestCase):
     """
     Tests for `enterprise_offer` API serializer.
     """
 
     @ddt.data(
-        ('787f0fa7-f89a-4267-9e2b-fcd299e83918', '787f0fa7-f89a-4267-9e2b-fcd299e83918'),
+        ('787f0fa7-f89a-4267-9e2b-fcd299e83918', '787f0fa7f89a42679e2bfcd299e83918'),
+        ('56a779a5-21ec-4711-830f-6654d3faaa5f', '56a779a521ec4711830f6654d3faaa5f'),
+        ('12345', '12345'),
+    )
+    @ddt.unpack
+    def test_deserialize_offer_id_valid(self, offer_id_request, offer_id_db):
+        data = {
+            'offer_id': offer_id_request,
+            'enterprise_customer_uuid': str(uuid.uuid4()),
+        }
+        serialized_offer = EnterpriseOfferSerializer(data=data)
+        assert serialized_offer.is_valid()
+        assert serialized_offer.validated_data['offer_id'] == offer_id_db
+
+    @ddt.data(
+        # Representations that could be real UUIDs should always be normalized to un-hyphenated UUIDs.
         ('787f0fa7f89a42679e2bfcd299e83918', '787f0fa7-f89a-4267-9e2b-fcd299e83918'),
-        ('11111111111111111111111111111111', '11111111-1111-1111-1111-111111111111'),
-        # fewer or more than 32 characters should serialize into integers.
-        ('1111111111111111111111111111111', '1111111111111111111111111111111'),
-        ('111111111111111111111111111111111', '111111111111111111111111111111111'),
-        # We never want to see the following cases in real life, but at least thye're deterministic and don't crash.
-        ('abc', 'abc'),  # Not exactly 32 characters but also obviously not an integer.
-        ('', ''),
+        ('f0d5fcdbed8e4d408f3b79d1671f967f', 'f0d5fcdb-ed8e-4d40-8f3b-79d1671f967f'),
+        ('c1d39f8a3fd246758bf7f56dd076694d', 'c1d39f8a-3fd2-4675-8bf7-f56dd076694d'),
+        ('12345', '12345'),
     )
     @ddt.unpack
-    def test_serialize_offer_id(self, offer_id_db, offer_id_serialized):
+    def test_serialize_offer_id_valid(self, offer_id_db, offer_id_serialized):
         offer = EnterpriseOfferFactory(offer_id=offer_id_db)
         serialized_offer = EnterpriseOfferSerializer(offer)
         assert serialized_offer.data['offer_id'] == offer_id_serialized
 
     @ddt.data(
-        # Representations that could be real UUIDs should always be normalized to un-hyphenated UUIDs.
-        ('787f0fa7-f89a-4267-9e2b-fcd299e83918', '787f0fa7f89a42679e2bfcd299e83918'),
-        ('787f0fa7f89a42679e2bfcd299e83918', '787f0fa7f89a42679e2bfcd299e83918'),
-        # hyphens in the wrong place, but gosh dangit this is a valid UUID!
-        ('787f0fa7-f89a-4267-9e2bfcd299e8391-8', '787f0fa7f89a42679e2bfcd299e83918'),
-        # Representations that are integers should be deserialized verbatim. 31-33 lengths.
-        ('1111111111111111111111111111111', '1111111111111111111111111111111'),
-        ('11111111111111111111111111111111', '11111111111111111111111111111111'),
-        ('111111111111111111111111111111111', '111111111111111111111111111111111'),
+        # The following should fail validation because we want to avoid storing these into the DB.
+        None,  # null values not allowed.
+        '',  # empty values not allowed.
+        'abc',  # Not exactly 36 characters but also obviously not an integer.
+        '787f0fa7f89a42679e2bfcd299e83918',  # Not exactly 36 characters but also obviously not an integer.
+        '11111111111',  # greater than 10 digit integer
+        '111111111111111111111111111111111111',  # 36 digit integer
+        '11111111111111111111111111111111',  # 32 digit integer
     )
-    @ddt.unpack
-    def test_deserialize_offer_id_valid(self, offer_id_request, offer_id_validated):
+    def test_deserialize_offer_id_invalid(self, offer_id_request):
         data = {
             'offer_id': offer_id_request,
             'enterprise_customer_uuid': str(uuid.uuid4()),
         }
         serializer = EnterpriseOfferSerializer(data=data)
-        assert serializer.is_valid()
-        assert serializer.validated_data['offer_id'] == offer_id_validated
-
-    # Commenting out for now, to test a theory on the serializergit sta to_internal_value
-    # @ddt.data(
-    #     # The following should fail validation because we want to avoid storing these into the DB.
-    #     None,  # null values not allowed.
-    #     '',  # empty values not allowed.
-    #     'abc',  # Not exactly 32 characters but also obviously not an integer.
-    # )
-    # def test_deserialize_offer_id_invalid(self, offer_id_request):
-    #     data = {
-    #         'offer_id': offer_id_request,
-    #         'enterprise_customer_uuid': str(uuid.uuid4()),
-    #     }
-    #     serializer = EnterpriseOfferSerializer(data=data)
-    #     assert not serializer.is_valid()
+        assert not serializer.is_valid()
```

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_views.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/api/v1/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,17 +122,17 @@
         self.role_assignment = EnterpriseDataRoleAssignment.objects.create(
             role=role,
             user=self.user
         )
         self.client.force_authenticate(user=self.user)
 
         self.enterprise_customer_uuid_1 = uuid4()
-        self.enterprise_offer_1_offer_id = str(uuid4()).replace('-', '')
+        self.enterprise_offer_1_offer_id = str(uuid4())
         self.enterprise_offer_1 = EnterpriseOfferFactory(
-            offer_id=self.enterprise_offer_1_offer_id,
+            offer_id=self.enterprise_offer_1_offer_id.replace('-', ''),
             enterprise_customer_uuid=self.enterprise_customer_uuid_1
         )
 
         self.enterprise_customer_2_uuid = uuid4()
         self.enterprise_offer_2_offer_id = '11111'
         self.enterprise_offer_2 = EnterpriseOfferFactory(
             offer_id=self.enterprise_offer_2_offer_id,
```

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/mixins.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/test_clients.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/test_filters.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/test_models.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/test_utils.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/tests/test_views.py` & `edx-enterprise-data-4.6.9/enterprise_data/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data/utils.py` & `edx-enterprise-data-4.6.9/enterprise_data/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/admin.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/admin.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0001_initial.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/models.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/rules.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/tests/factories.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_data_roles/tests/test_models.py` & `edx-enterprise-data-4.6.9/enterprise_data_roles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/clients/__init__.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/clients/enterprise.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/clients/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/clients/s3.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/clients/s3.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/clients/snowflake.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/clients/vertica.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/clients/vertica.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/delivery_method.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/external_resource_link_report.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/external_resource_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/enterprise_customer_reporting.json` & `edx-enterprise-data-4.6.9/enterprise_reporting/fixtures/enterprise_customer_reporting.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/reporter.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/send_enterprise_reports.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_clients.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_delivery_method.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_enterprise_client.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_enterprise_client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_external_link_report.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_external_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_reporter.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_send_enterprise_reports.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_utils.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/tests/utils.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/enterprise_reporting/utils.py` & `edx-enterprise-data-4.6.9/enterprise_reporting/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/base.txt` & `edx-enterprise-data-4.6.9/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/ci.txt` & `edx-enterprise-data-4.6.9/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/constraints.txt` & `edx-enterprise-data-4.6.9/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/dev.txt` & `edx-enterprise-data-4.6.9/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/quality.txt` & `edx-enterprise-data-4.6.9/requirements/quality.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/reporting.in` & `edx-enterprise-data-4.6.9/requirements/reporting.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/test-master.txt` & `edx-enterprise-data-4.6.9/requirements/test-master.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/test-reporting.txt` & `edx-enterprise-data-4.6.9/requirements/test-reporting.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/requirements/test.txt` & `edx-enterprise-data-4.6.9/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.8/setup.py` & `edx-enterprise-data-4.6.9/setup.py`

 * *Files identical despite different names*

