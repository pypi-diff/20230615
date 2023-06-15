# Comparing `tmp/django_eveuniverse-1.1.1.tar.gz` & `tmp/django_eveuniverse-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_eveuniverse-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_eveuniverse-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_eveuniverse-1.1.1.tar` & `django_eveuniverse-1.2.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1070 2020-10-23 18:01:44.555775 django_eveuniverse-1.1.1/LICENSE
--rw-r--r--   0        0        0     3082 2023-06-04 09:47:59.298497 django_eveuniverse-1.1.1/README.rst
--rw-r--r--   0        0        0      184 2023-06-04 09:47:59.298497 django_eveuniverse-1.1.1/eveuniverse/__init__.py
--rw-r--r--   0        0        0     1314 2020-10-23 18:01:44.567774 django_eveuniverse-1.1.1/eveuniverse/admin.py
--rw-r--r--   0        0        0     2857 2023-06-03 17:10:19.215764 django_eveuniverse-1.1.1/eveuniverse/app_settings.py
--rw-r--r--   0        0        0      254 2022-03-01 16:54:35.914600 django_eveuniverse-1.1.1/eveuniverse/apps.py
--rw-r--r--   0        0        0      873 2023-05-29 21:04:02.196043 django_eveuniverse-1.1.1/eveuniverse/backends.py
--rw-r--r--   0        0        0      370 2023-04-15 10:37:18.591750 django_eveuniverse-1.1.1/eveuniverse/constants.py
--rw-r--r--   0        0        0        0 2023-06-04 10:02:21.615093 django_eveuniverse-1.1.1/eveuniverse/core/__init__.py
--rw-r--r--   0        0        0     1781 2022-02-11 14:09:07.543015 django_eveuniverse-1.1.1/eveuniverse/core/dotlan.py
--rw-r--r--   0        0        0      423 2022-06-18 12:37:45.694321 django_eveuniverse-1.1.1/eveuniverse/core/esitools.py
--rw-r--r--   0        0        0     5127 2023-05-29 21:04:02.196043 django_eveuniverse-1.1.1/eveuniverse/core/eveimageserver.py
--rw-r--r--   0        0        0      358 2022-01-04 21:23:14.332955 django_eveuniverse-1.1.1/eveuniverse/core/eveitems.py
--rw-r--r--   0        0        0     2598 2023-05-29 21:04:02.196043 django_eveuniverse-1.1.1/eveuniverse/core/evemicros.py
--rw-r--r--   0        0        0     2431 2023-05-29 21:04:02.196043 django_eveuniverse-1.1.1/eveuniverse/core/evesdeapi.py
--rw-r--r--   0        0        0      457 2022-01-04 21:23:14.332955 django_eveuniverse-1.1.1/eveuniverse/core/eveskinserver.py
--rw-r--r--   0        0        0     1145 2023-05-29 21:04:02.196043 django_eveuniverse-1.1.1/eveuniverse/core/evewho.py
--rw-r--r--   0        0        0     2864 2022-02-11 14:41:18.613728 django_eveuniverse-1.1.1/eveuniverse/core/evexml.py
--rw-r--r--   0        0        0     1713 2023-05-29 21:04:02.196043 django_eveuniverse-1.1.1/eveuniverse/core/zkillboard.py
--rw-r--r--   0        0        0     1745 2023-05-30 19:50:16.531702 django_eveuniverse-1.1.1/eveuniverse/helpers.py
--rw-r--r--   0        0        0      365 2023-04-15 10:37:18.591750 django_eveuniverse-1.1.1/eveuniverse/management/commands/__init__.py
--rw-r--r--   0        0        0     4574 2023-04-15 10:37:18.591750 django_eveuniverse-1.1.1/eveuniverse/management/commands/eveuniverse_load_data.py
--rw-r--r--   0        0        0     5348 2023-04-15 10:37:18.591750 django_eveuniverse-1.1.1/eveuniverse/management/commands/eveuniverse_load_types.py
--rw-r--r--   0        0        0     1644 2021-04-16 13:44:19.227872 django_eveuniverse-1.1.1/eveuniverse/management/commands/eveuniverse_purge_data.py
--rw-r--r--   0        0        0    47900 2023-06-03 17:10:19.215764 django_eveuniverse-1.1.1/eveuniverse/managers.py
--rw-r--r--   0        0        0    51659 2023-04-15 17:15:38.755939 django_eveuniverse-1.1.1/eveuniverse/migrations/0001_initial.py
--rw-r--r--   0        0        0      968 2023-04-15 17:15:38.755939 django_eveuniverse-1.1.1/eveuniverse/migrations/0002_load_eveunit.py
--rw-r--r--   0        0        0     1009 2023-04-15 17:15:38.755939 django_eveuniverse-1.1.1/eveuniverse/migrations/0003_evemarketprice.py
--rw-r--r--   0        0        0      478 2023-04-15 17:15:38.755939 django_eveuniverse-1.1.1/eveuniverse/migrations/0004_effect_longer_name.py
--rw-r--r--   0        0        0     2702 2023-04-15 17:15:38.755939 django_eveuniverse-1.1.1/eveuniverse/migrations/0005_type_materials_and_sections.py
--rw-r--r--   0        0        0      429 2023-04-15 17:15:38.759939 django_eveuniverse-1.1.1/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
--rw-r--r--   0        0        0      409 2023-04-15 17:15:38.759939 django_eveuniverse-1.1.1/eveuniverse/migrations/0007_evetype_description.py
--rw-r--r--   0        0        0     7547 2023-06-03 17:10:19.215764 django_eveuniverse-1.1.1/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py
--rw-r--r--   0        0        0      989 2023-06-03 17:10:19.215764 django_eveuniverse-1.1.1/eveuniverse/migrations/0009_load_industry_activities.py
--rw-r--r--   0        0        0     1768 2023-06-03 17:10:19.215764 django_eveuniverse-1.1.1/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py
--rw-r--r--   0        0        0        0 2023-06-04 10:02:21.619093 django_eveuniverse-1.1.1/eveuniverse/migrations/__init__.py
--rw-r--r--   0        0        0     5336 2020-11-20 16:10:16.158594 django_eveuniverse-1.1.1/eveuniverse/migrations/eve_unit.json
--rw-r--r--   0        0        0      934 2023-06-03 17:10:19.215764 django_eveuniverse-1.1.1/eveuniverse/migrations/industry_activities.json
--rw-r--r--   0        0        0    64211 2023-06-04 09:47:59.298497 django_eveuniverse-1.1.1/eveuniverse/models.py
--rw-r--r--   0        0        0      250 2022-06-18 12:37:45.694321 django_eveuniverse-1.1.1/eveuniverse/providers.py
--rw-r--r--   0        0        0    14542 2020-12-18 18:17:56.637925 django_eveuniverse-1.1.1/eveuniverse/static/eveuniverse/skin_generic_128.png
--rw-r--r--   0        0        0     2142 2020-12-18 18:17:56.637925 django_eveuniverse-1.1.1/eveuniverse/static/eveuniverse/skin_generic_32.png
--rw-r--r--   0        0        0     4141 2020-12-18 18:17:56.637925 django_eveuniverse-1.1.1/eveuniverse/static/eveuniverse/skin_generic_64.png
--rw-r--r--   0        0        0   887006 2022-06-18 12:37:45.702321 django_eveuniverse-1.1.1/eveuniverse/swagger.json
--rw-r--r--   0        0        0    10805 2023-05-30 19:50:16.535702 django_eveuniverse-1.1.1/eveuniverse/tasks.py
--rw-r--r--   0        0        0        0 2023-06-04 10:02:21.619093 django_eveuniverse-1.1.1/eveuniverse/tests/__init__.py
--rw-r--r--   0        0        0     1274 2023-04-15 17:15:38.759939 django_eveuniverse-1.1.1/eveuniverse/tests/pilot.py
--rw-r--r--   0        0        0     1046 2023-04-13 02:39:52.214185 django_eveuniverse-1.1.1/eveuniverse/tests/test_backends.py
--rw-r--r--   0        0        0    10286 2023-04-13 19:30:17.215558 django_eveuniverse-1.1.1/eveuniverse/tests/test_commands.py
--rw-r--r--   0        0        0    22736 2023-05-29 21:04:02.204043 django_eveuniverse-1.1.1/eveuniverse/tests/test_core.py
--rw-r--r--   0        0        0     2136 2023-05-29 21:04:02.204043 django_eveuniverse-1.1.1/eveuniverse/tests/test_helpers.py
--rw-r--r--   0        0        0    46495 2023-06-03 17:10:19.219764 django_eveuniverse-1.1.1/eveuniverse/tests/test_models_1.py
--rw-r--r--   0        0        0    28631 2023-04-15 12:19:39.042614 django_eveuniverse-1.1.1/eveuniverse/tests/test_models_2.py
--rw-r--r--   0        0        0    56203 2023-06-03 17:10:19.219764 django_eveuniverse-1.1.1/eveuniverse/tests/test_models_3.py
--rw-r--r--   0        0        0    30849 2023-04-15 12:19:39.042614 django_eveuniverse-1.1.1/eveuniverse/tests/test_models_4.py
--rw-r--r--   0        0        0     6759 2023-04-12 21:38:05.746923 django_eveuniverse-1.1.1/eveuniverse/tests/test_tasks.py
--rw-r--r--   0        0        0     2958 2021-04-16 13:44:19.231871 django_eveuniverse-1.1.1/eveuniverse/tests/test_tools_testdata.py
--rw-r--r--   0        0        0     3975 2023-04-15 17:15:38.759939 django_eveuniverse-1.1.1/eveuniverse/tests/test_utils.py
--rw-r--r--   0        0        0        0 2023-06-04 10:02:21.619093 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/__init__.py
--rw-r--r--   0        0        0     7725 2022-03-08 21:55:48.715606 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/esi.py
--rw-r--r--   0        0        0    81711 2023-06-03 17:10:19.219764 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/esi_data.json
--rw-r--r--   0        0        0     4500 2023-01-18 17:00:28.727344 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/factories.py
--rw-r--r--   0        0        0     1659 2023-06-03 17:10:19.219764 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/fetch_esi_raw_data.py
--rw-r--r--   0        0        0     1183 2023-04-05 13:26:14.320189 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/generate_sde.py
--rw-r--r--   0        0        0      610 2023-06-03 17:10:19.219764 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/sde.py
--rw-r--r--   0        0        0     5187 2023-06-03 17:10:19.219764 django_eveuniverse-1.1.1/eveuniverse/tests/testdata/sde_data.json
--rw-r--r--   0        0        0     4636 2020-11-20 16:10:16.170594 django_eveuniverse-1.1.1/eveuniverse/tests/testdata_example.json
--rw-r--r--   0        0        0        0 2023-06-04 10:02:21.619093 django_eveuniverse-1.1.1/eveuniverse/tests/tools/__init__.py
--rw-r--r--   0        0        0      760 2023-04-15 12:19:39.046614 django_eveuniverse-1.1.1/eveuniverse/tests/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0        0 2023-06-04 10:02:21.619093 django_eveuniverse-1.1.1/eveuniverse/tools/__init__.py
--rw-r--r--   0        0        0     1373 2020-11-20 16:10:16.170594 django_eveuniverse-1.1.1/eveuniverse/tools/drop_tables.sql
--rw-r--r--   0        0        0     5235 2023-04-12 22:26:32.188851 django_eveuniverse-1.1.1/eveuniverse/tools/testdata.py
--rw-r--r--   0        0        0     2817 2023-05-29 21:04:02.204043 django_eveuniverse-1.1.1/eveuniverse/utils.py
--rw-r--r--   0        0        0     1733 2023-06-04 09:47:59.302497 django_eveuniverse-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4432 1970-01-01 00:00:00.000000 django_eveuniverse-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-10-23 18:01:44.555775 django_eveuniverse-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3082 2023-06-04 09:47:59.298497 django_eveuniverse-1.2.0/README.rst
+-rw-r--r--   0        0        0      184 2023-06-15 19:16:53.976714 django_eveuniverse-1.2.0/eveuniverse/__init__.py
+-rw-r--r--   0        0        0     1314 2020-10-23 18:01:44.567774 django_eveuniverse-1.2.0/eveuniverse/admin.py
+-rw-r--r--   0        0        0     2857 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/app_settings.py
+-rw-r--r--   0        0        0      254 2022-03-01 16:54:35.914600 django_eveuniverse-1.2.0/eveuniverse/apps.py
+-rw-r--r--   0        0        0      873 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/backends.py
+-rw-r--r--   0        0        0      370 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/constants.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:51.394095 django_eveuniverse-1.2.0/eveuniverse/core/__init__.py
+-rw-r--r--   0        0        0     1781 2022-02-11 14:09:07.543015 django_eveuniverse-1.2.0/eveuniverse/core/dotlan.py
+-rw-r--r--   0        0        0      423 2022-06-18 12:37:45.694321 django_eveuniverse-1.2.0/eveuniverse/core/esitools.py
+-rw-r--r--   0        0        0     5127 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/eveimageserver.py
+-rw-r--r--   0        0        0      358 2022-01-04 21:23:14.332955 django_eveuniverse-1.2.0/eveuniverse/core/eveitems.py
+-rw-r--r--   0        0        0     2598 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/evemicros.py
+-rw-r--r--   0        0        0     2431 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/evesdeapi.py
+-rw-r--r--   0        0        0      457 2022-01-04 21:23:14.332955 django_eveuniverse-1.2.0/eveuniverse/core/eveskinserver.py
+-rw-r--r--   0        0        0     1145 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/evewho.py
+-rw-r--r--   0        0        0     2864 2022-02-11 14:41:18.613728 django_eveuniverse-1.2.0/eveuniverse/core/evexml.py
+-rw-r--r--   0        0        0     1713 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/zkillboard.py
+-rw-r--r--   0        0        0     1745 2023-05-30 19:50:16.531702 django_eveuniverse-1.2.0/eveuniverse/helpers.py
+-rw-r--r--   0        0        0      365 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/management/commands/__init__.py
+-rw-r--r--   0        0        0     4574 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_data.py
+-rw-r--r--   0        0        0     5348 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_types.py
+-rw-r--r--   0        0        0     1644 2021-04-16 13:44:19.227872 django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_purge_data.py
+-rw-r--r--   0        0        0    47900 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/managers.py
+-rw-r--r--   0        0        0    51659 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0002_load_eveunit.py
+-rw-r--r--   0        0        0     1009 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0003_evemarketprice.py
+-rw-r--r--   0        0        0      478 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0004_effect_longer_name.py
+-rw-r--r--   0        0        0     2702 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0005_type_materials_and_sections.py
+-rw-r--r--   0        0        0      429 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
+-rw-r--r--   0        0        0      409 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/migrations/0007_evetype_description.py
+-rw-r--r--   0        0        0     7547 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py
+-rw-r--r--   0        0        0      989 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/0009_load_industry_activities.py
+-rw-r--r--   0        0        0     1768 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:51.398095 django_eveuniverse-1.2.0/eveuniverse/migrations/__init__.py
+-rw-r--r--   0        0        0     5336 2020-11-20 16:10:16.158594 django_eveuniverse-1.2.0/eveuniverse/migrations/eve_unit.json
+-rw-r--r--   0        0        0      934 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/industry_activities.json
+-rw-r--r--   0        0        0    64475 2023-06-15 19:16:53.976714 django_eveuniverse-1.2.0/eveuniverse/models.py
+-rw-r--r--   0        0        0      250 2022-06-18 12:37:45.694321 django_eveuniverse-1.2.0/eveuniverse/providers.py
+-rw-r--r--   0        0        0    14542 2020-12-18 18:17:56.637925 django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_128.png
+-rw-r--r--   0        0        0     2142 2020-12-18 18:17:56.637925 django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_32.png
+-rw-r--r--   0        0        0     4141 2020-12-18 18:17:56.637925 django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_64.png
+-rw-r--r--   0        0        0   887006 2022-06-18 12:37:45.702321 django_eveuniverse-1.2.0/eveuniverse/swagger.json
+-rw-r--r--   0        0        0    10805 2023-05-30 19:50:16.535702 django_eveuniverse-1.2.0/eveuniverse/tasks.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:51.398095 django_eveuniverse-1.2.0/eveuniverse/tests/__init__.py
+-rw-r--r--   0        0        0     1274 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/tests/pilot.py
+-rw-r--r--   0        0        0     1046 2023-04-13 02:39:52.214185 django_eveuniverse-1.2.0/eveuniverse/tests/test_backends.py
+-rw-r--r--   0        0        0    10286 2023-04-13 19:30:17.215558 django_eveuniverse-1.2.0/eveuniverse/tests/test_commands.py
+-rw-r--r--   0        0        0    22736 2023-05-29 21:04:02.204043 django_eveuniverse-1.2.0/eveuniverse/tests/test_core.py
+-rw-r--r--   0        0        0     2136 2023-05-29 21:04:02.204043 django_eveuniverse-1.2.0/eveuniverse/tests/test_helpers.py
+-rw-r--r--   0        0        0    46753 2023-06-15 19:16:53.980714 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_1.py
+-rw-r--r--   0        0        0    28631 2023-04-15 12:19:39.042614 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_2.py
+-rw-r--r--   0        0        0    56203 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_3.py
+-rw-r--r--   0        0        0    30849 2023-04-15 12:19:39.042614 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_4.py
+-rw-r--r--   0        0        0     6759 2023-04-12 21:38:05.746923 django_eveuniverse-1.2.0/eveuniverse/tests/test_tasks.py
+-rw-r--r--   0        0        0     2958 2021-04-16 13:44:19.231871 django_eveuniverse-1.2.0/eveuniverse/tests/test_tools_testdata.py
+-rw-r--r--   0        0        0     3975 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:51.402095 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     7725 2022-03-08 21:55:48.715606 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi.py
+-rw-r--r--   0        0        0    81711 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0     4500 2023-01-18 17:00:28.727344 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/factories.py
+-rw-r--r--   0        0        0     1659 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py
+-rw-r--r--   0        0        0     1183 2023-04-05 13:26:14.320189 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/generate_sde.py
+-rw-r--r--   0        0        0      610 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde.py
+-rw-r--r--   0        0        0     5187 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde_data.json
+-rw-r--r--   0        0        0     4636 2020-11-20 16:10:16.170594 django_eveuniverse-1.2.0/eveuniverse/tests/testdata_example.json
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:51.402095 django_eveuniverse-1.2.0/eveuniverse/tests/tools/__init__.py
+-rw-r--r--   0        0        0      760 2023-04-15 12:19:39.046614 django_eveuniverse-1.2.0/eveuniverse/tests/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:40:51.402095 django_eveuniverse-1.2.0/eveuniverse/tools/__init__.py
+-rw-r--r--   0        0        0     1373 2020-11-20 16:10:16.170594 django_eveuniverse-1.2.0/eveuniverse/tools/drop_tables.sql
+-rw-r--r--   0        0        0     5235 2023-04-12 22:26:32.188851 django_eveuniverse-1.2.0/eveuniverse/tools/testdata.py
+-rw-r--r--   0        0        0     2817 2023-05-29 21:04:02.204043 django_eveuniverse-1.2.0/eveuniverse/utils.py
+-rw-r--r--   0        0        0     1733 2023-06-04 09:47:59.302497 django_eveuniverse-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4432 1970-01-01 00:00:00.000000 django_eveuniverse-1.2.0/PKG-INFO
```

### Comparing `django_eveuniverse-1.1.1/LICENSE` & `django_eveuniverse-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/README.rst` & `django_eveuniverse-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/admin.py` & `django_eveuniverse-1.2.0/eveuniverse/admin.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/app_settings.py` & `django_eveuniverse-1.2.0/eveuniverse/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/backends.py` & `django_eveuniverse-1.2.0/eveuniverse/backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/core/dotlan.py` & `django_eveuniverse-1.2.0/eveuniverse/core/dotlan.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/core/eveimageserver.py` & `django_eveuniverse-1.2.0/eveuniverse/core/eveimageserver.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/core/evemicros.py` & `django_eveuniverse-1.2.0/eveuniverse/core/evemicros.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/core/evesdeapi.py` & `django_eveuniverse-1.2.0/eveuniverse/core/evesdeapi.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/core/evewho.py` & `django_eveuniverse-1.2.0/eveuniverse/core/evewho.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/core/evexml.py` & `django_eveuniverse-1.2.0/eveuniverse/core/evexml.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/core/zkillboard.py` & `django_eveuniverse-1.2.0/eveuniverse/core/zkillboard.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/helpers.py` & `django_eveuniverse-1.2.0/eveuniverse/helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/management/commands/eveuniverse_load_data.py` & `django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/management/commands/eveuniverse_load_types.py` & `django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_types.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/management/commands/eveuniverse_purge_data.py` & `django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_purge_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/managers.py` & `django_eveuniverse-1.2.0/eveuniverse/managers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/0001_initial.py` & `django_eveuniverse-1.2.0/eveuniverse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/0002_load_eveunit.py` & `django_eveuniverse-1.2.0/eveuniverse/migrations/0002_load_eveunit.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/0003_evemarketprice.py` & `django_eveuniverse-1.2.0/eveuniverse/migrations/0003_evemarketprice.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/0005_type_materials_and_sections.py` & `django_eveuniverse-1.2.0/eveuniverse/migrations/0005_type_materials_and_sections.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py` & `django_eveuniverse-1.2.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/0009_load_industry_activities.py` & `django_eveuniverse-1.2.0/eveuniverse/migrations/0009_load_industry_activities.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py` & `django_eveuniverse-1.2.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/eve_unit.json` & `django_eveuniverse-1.2.0/eveuniverse/migrations/eve_unit.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/migrations/industry_activities.json` & `django_eveuniverse-1.2.0/eveuniverse/migrations/industry_activities.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/models.py` & `django_eveuniverse-1.2.0/eveuniverse/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Eve universe models."""
 
 import enum
 import inspect
 import math
+import re
 import sys
 from collections import namedtuple
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 from bitfield import BitField
 from bravado.exception import HTTPNotFound
 from django.contrib.staticfiles.storage import staticfiles_storage
@@ -1086,14 +1087,22 @@
             "position_x": ("position", "x"),
             "position_y": ("position", "y"),
             "position_z": ("position", "z"),
         }
         children = {"moons": "EveMoon", "asteroid_belts": "EveAsteroidBelt"}
         load_order = 205
 
+    def type_name(self) -> str:
+        """Return shortened name of planet type.
+
+        Note: Accesses the eve_type object.
+        """
+        matches = re.findall(r"Planet \((\S*)\)", self.eve_type.name)
+        return matches[0] if matches else ""
+
     @classmethod
     def _children(cls, enabled_sections: Optional[Iterable[str]] = None) -> dict:
         enabled_sections = cls.determine_effective_sections(enabled_sections)
         children = dict()
         if cls.Section.ASTEROID_BELTS in enabled_sections:
             children["asteroid_belts"] = "EveAsteroidBelt"
         if cls.Section.MOONS in enabled_sections:
```

### Comparing `django_eveuniverse-1.1.1/eveuniverse/static/eveuniverse/skin_generic_128.png` & `django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_128.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/static/eveuniverse/skin_generic_32.png` & `django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_32.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/static/eveuniverse/skin_generic_64.png` & `django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_64.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/swagger.json` & `django_eveuniverse-1.2.0/eveuniverse/swagger.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tasks.py` & `django_eveuniverse-1.2.0/eveuniverse/tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/pilot.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/pilot.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_backends.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_commands.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_core.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_helpers.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_models_1.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -791,14 +791,21 @@
         # action
         EvePlanet.objects.update_or_create_esi(id=40349467, include_children=True)
 
         # validate
         moon.refresh_from_db()
         self.assertNotEqual(moon.name, "Dummy")
 
+    def test_can_return_planet_type_name(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        obj, _ = EvePlanet.objects.update_or_create_esi(id=40349467)
+        # when/then
+        self.assertEqual(obj.type_name(), "Barren")
+
 
 @patch(MANAGERS_PATH + ".esi")
 class TestEveRace(NoSocketsTestCase):
     def test_create_from_esi(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         obj, created = EveRace.objects.update_or_create_esi(id=1)
```

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_models_2.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_2.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_models_3.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_3.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_models_4.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_4.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_tasks.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_tools_testdata.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_tools_testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/test_utils.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata/esi.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata/esi_data.json` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata/factories.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata/fetch_esi_raw_data.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata/generate_sde.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/generate_sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata/sde.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata/sde_data.json` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/testdata_example.json` & `django_eveuniverse-1.2.0/eveuniverse/tests/testdata_example.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tests/tools/clear_celery_once_locks.py` & `django_eveuniverse-1.2.0/eveuniverse/tests/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tools/drop_tables.sql` & `django_eveuniverse-1.2.0/eveuniverse/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/tools/testdata.py` & `django_eveuniverse-1.2.0/eveuniverse/tools/testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/eveuniverse/utils.py` & `django_eveuniverse-1.2.0/eveuniverse/utils.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/pyproject.toml` & `django_eveuniverse-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.1.1/PKG-INFO` & `django_eveuniverse-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-eveuniverse
-Version: 1.1.1
+Version: 1.2.0
 Summary: Complete set of Eve Universe models with on-demand loading from ESI.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

