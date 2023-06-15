# Comparing `tmp/simpl-cloud-1.2.4.tar.gz` & `tmp/simpl-cloud-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpl-cloud-1.2.4.tar", last modified: Tue Nov 15 10:06:21 2022, max compression
+gzip compressed data, was "simpl-cloud-1.3.0.tar", last modified: Thu Jun 15 15:00:24 2023, max compression
```

## Comparing `simpl-cloud-1.2.4.tar` & `simpl-cloud-1.3.0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/
--rw-rw-r--   0 chris     (1000) chris     (1000)     7574 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/CHANGELOG.md
--rw-rw-r--   0 chris     (1000) chris     (1000)    18092 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      118 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/MANIFEST.in
--rw-rw-r--   0 chris     (1000) chris     (1000)     6029 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     4939 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/README.rst
--rw-rw-r--   0 chris     (1000) chris     (1000)     1702 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)       60 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1203 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1158 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/admin.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      695 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/apps.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/auth0.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/conf/
--rw-rw-r--   0 chris     (1000) chris     (1000)      222 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/conf/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2905 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/conf/app_settings.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       85 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/constants.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4980 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/managers.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/migrations/
--rw-rw-r--   0 chris     (1000) chris     (1000)    10093 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0001_initial.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      512 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0002_run_data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1442 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0003_auto_20210701_1047.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      329 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0004_rename_token_apitoken.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      756 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0005_auto_20210707_0934.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      593 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0005_auto_20210712_0038.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1073 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0006_auto_20210712_0240.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      383 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0007_shorten_lobby_name.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      265 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0008_merge_20210727_1117.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      388 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0009_player_inactive.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      727 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0010_class.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      405 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0011_gameexperience_experience_id.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      332 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0012_remove_lobby_ready.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      594 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0013_gameexperience_multiplayer.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      625 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0014_auto_20210903_1514.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      530 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0015_lobby_instance.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      834 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0016_link_lobby_instances.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      404 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0017_run_date_continuous_end.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      398 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0018_apitoken_name.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1629 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0019_auto_20211027_1812.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      832 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/0020_auto_20211109_2056.py
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/migrations/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    20034 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2623 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/nav.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1752 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/receivers.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/schema/
--rw-rw-r--   0 chris     (1000) chris     (1000)      616 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/schema/external/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/external/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1508 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/external/auth0.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4433 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/external/mutations.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3832 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/external/query.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7842 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/external/types.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2897 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/external/utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3005 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/mutations.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1515 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/query.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1723 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/schema/types.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.580268 simpl-cloud-1.2.4/simpl/static/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/static/simpl/
--rw-rw-r--   0 chris     (1000) chris     (1000)   240548 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/static/simpl/simpl.es.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   241011 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/static/simpl/simpl.umd.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   159126 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/static/simpl/style.css
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.580268 simpl-cloud-1.2.4/simpl/templates/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/templates/simpl/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1957 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/base.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/templates/simpl/includes/
--rw-rw-r--   0 chris     (1000) chris     (1000)      379 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/dropdown-item.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      289 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/dropdown.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      501 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/form-card.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1630 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/form_debrief.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1285 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/form_end.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1354 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/form_prepare.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/templates/simpl/includes/forms/
--rw-rw-r--   0 chris     (1000) chris     (1000)       71 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/forms/field.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      457 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/messages.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1770 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/page-header.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      344 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/player.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/
--rw-rw-r--   0 chris     (1000) chris     (1000)      414 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/active_player_in_setup.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      484 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/inactive_player.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1428 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/instructions.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      103 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/invite.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      186 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/list_header_togglers.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      274 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/multiplayer_in_play.html
--rw-rw-r--   0 chris     (1000) chris     (1000)       42 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/multiplayer_in_setup.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      274 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/singleplayer_in_play.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1125 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/search_form.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1088 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/site-header.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      926 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/site-subheader.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1622 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/includes/status-arrows.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      207 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_config.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      437 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_debrief.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      439 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_end_gameplay.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     8213 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_players.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      457 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_prepare.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      324 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_start.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      575 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_status.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      664 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templates/simpl/run_team.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/templatetags/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templatetags/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4999 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templatetags/includecontents.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      737 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/templatetags/simpl.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      888 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/tests/settings.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10830 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/tests/test_models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11059 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/tests/test_simpl.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1058 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/urls.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl/utils/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/utils/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2925 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/utils/models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4455 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/utils/name_faker.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10869 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl/views.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-15 10:06:21.584268 simpl-cloud-1.2.4/simpl_cloud.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6029 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl_cloud.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     3631 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl_cloud.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl_cloud.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl_cloud.egg-info/not-zip-safe
--rw-rw-r--   0 chris     (1000) chris     (1000)      254 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl_cloud.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        6 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/simpl_cloud.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      987 2022-11-15 10:06:21.000000 simpl-cloud-1.2.4/tox.ini
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.097108 simpl-cloud-1.3.0/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     7773 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/CHANGELOG.md
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    18092 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/LICENSE
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      118 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/MANIFEST.in
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     6049 2023-06-15 15:00:24.101108 simpl-cloud-1.3.0/PKG-INFO
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     4939 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/README.rst
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1709 2023-06-15 15:00:24.101108 simpl-cloud-1.3.0/setup.cfg
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)       60 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/setup.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.085108 simpl-cloud-1.3.0/simpl/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1203 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/__init__.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1158 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/admin.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      695 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/apps.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      882 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/auth0.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.085108 simpl-cloud-1.3.0/simpl/conf/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      222 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/conf/__init__.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     2905 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/conf/app_settings.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)       85 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/constants.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     4980 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/managers.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.089108 simpl-cloud-1.3.0/simpl/migrations/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    10093 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0001_initial.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      512 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0002_run_data.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1442 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0003_auto_20210701_1047.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      329 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0004_rename_token_apitoken.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      756 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0005_auto_20210707_0934.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      593 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0005_auto_20210712_0038.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1073 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0006_auto_20210712_0240.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      383 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0007_shorten_lobby_name.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      265 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0008_merge_20210727_1117.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      388 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0009_player_inactive.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      727 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0010_class.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      405 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0011_gameexperience_experience_id.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      332 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0012_remove_lobby_ready.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      594 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0013_gameexperience_multiplayer.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      625 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0014_auto_20210903_1514.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      530 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0015_lobby_instance.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      834 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0016_link_lobby_instances.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      404 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0017_run_date_continuous_end.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      398 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0018_apitoken_name.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1629 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0019_auto_20211027_1812.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      832 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/0020_auto_20211109_2056.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/migrations/__init__.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    20034 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/models.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     2623 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/nav.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1752 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/receivers.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.089108 simpl-cloud-1.3.0/simpl/schema/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      616 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/__init__.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.089108 simpl-cloud-1.3.0/simpl/schema/external/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/external/__init__.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1508 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/external/auth0.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     4433 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/external/mutations.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     3832 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/external/query.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    10162 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/external/types.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     6161 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/external/utils.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     3005 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/mutations.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1515 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/query.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1723 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/schema/types.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.081108 simpl-cloud-1.3.0/simpl/static/
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.093108 simpl-cloud-1.3.0/simpl/static/simpl/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)   242358 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/static/simpl/simpl.es.js
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)   242764 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/static/simpl/simpl.umd.js
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)   159204 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/static/simpl/style.css
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.081108 simpl-cloud-1.3.0/simpl/templates/
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.093108 simpl-cloud-1.3.0/simpl/templates/simpl/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1957 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/base.html
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.093108 simpl-cloud-1.3.0/simpl/templates/simpl/includes/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      379 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/dropdown-item.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      289 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/dropdown.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      501 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/form-card.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1630 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/form_debrief.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1285 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/form_end.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1354 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/form_prepare.html
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.093108 simpl-cloud-1.3.0/simpl/templates/simpl/includes/forms/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)       71 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/forms/field.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      457 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/messages.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1770 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/page-header.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      344 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/player.html
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.097108 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      414 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/active_player_in_setup.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      484 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/inactive_player.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1428 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/instructions.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      103 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/invite.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      186 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/list_header_togglers.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      274 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/multiplayer_in_play.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)       42 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/multiplayer_in_setup.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      274 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/singleplayer_in_play.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1125 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/search_form.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1088 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/site-header.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      926 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/site-subheader.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1622 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/includes/status-arrows.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      207 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_config.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      437 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_debrief.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      439 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_end_gameplay.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     8213 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_players.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      457 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_prepare.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      324 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_start.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      575 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_status.html
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      664 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templates/simpl/run_team.html
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.097108 simpl-cloud-1.3.0/simpl/templatetags/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templatetags/__init__.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     4999 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templatetags/includecontents.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      737 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/templatetags/simpl.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.097108 simpl-cloud-1.3.0/simpl/tests/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/tests/__init__.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      909 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/tests/settings.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    17763 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/tests/test_external_schema.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    10850 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/tests/test_models.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    11091 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/tests/test_simpl.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    11482 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/tests/test_utils.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     1058 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/urls.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.097108 simpl-cloud-1.3.0/simpl/utils/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/utils/__init__.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     2925 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/utils/models.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     4455 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/utils/name_faker.py
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)    10869 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl/views.py
+drwxrwxr-x   0 jacobtm   (1000) jacobtm   (1000)        0 2023-06-15 15:00:24.097108 simpl-cloud-1.3.0/simpl_cloud.egg-info/
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     6049 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl_cloud.egg-info/PKG-INFO
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)     3693 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl_cloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        1 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl_cloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        1 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl_cloud.egg-info/not-zip-safe
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      261 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl_cloud.egg-info/requires.txt
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)        6 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/simpl_cloud.egg-info/top_level.txt
+-rw-rw-r--   0 jacobtm   (1000) jacobtm   (1000)      987 2023-06-15 15:00:23.000000 simpl-cloud-1.3.0/tox.ini
```

### Comparing `simpl-cloud-1.2.4/CHANGELOG.md` & `simpl-cloud-1.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 Change log for Simpl Cloud
 ==========================
 
 A list of notable changes to the Simpl-Cloud library included in each release.
 
+1.3.0 (15 June 2023)
+====================
+
+- Optimise `instance` and `run` queries
+- Replace CSS dropdown with JS, to fix issue with dropdown not opening on Safari, and improve keyboard navigation
+
+
 1.2.4 (15 November 2022)
 ========================
 
 - Use `__str__` to calculate the BaseInstance display name
   This enables BaseInstance subclasses to customise how names are displayed more easily
```

### Comparing `simpl-cloud-1.2.4/LICENSE` & `simpl-cloud-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/PKG-INFO` & `simpl-cloud-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: simpl-cloud
-Version: 1.2.4
+Version: 1.3.0
 Summary: Base models and API for Django-based simulations.
 Home-page: https://github.com/Wharton-Interactive/simpl-cloud
 Author: Chris Beaven
 Author-email: smileychris@gmail.com
 License: GPL2
 Keywords: api simulation administration
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -200,7 +201,9 @@
 
 If using Auth0 for social authentication, add the following Django settings to
 make sure users are correctly logged out of Auth0 and (optionally) redirected after logout::
 
 
   ACCOUNT_ADAPTER = "simpl.auth0.Auth0LogoutAdapter"
   AUTH0_LOGOUT_RETURN_TO = "some.url"
+
+
```

### Comparing `simpl-cloud-1.2.4/README.rst` & `simpl-cloud-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/setup.cfg` & `simpl-cloud-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = simpl-cloud
-version = 1.2.4
+version = 1.3.0
 description = Base models and API for Django-based simulations.
 long_description = file: README.rst
 author = Chris Beaven
 author_email = smileychris@gmail.com
 url = https://github.com/Wharton-Interactive/simpl-cloud
 keywords = api simulation administration
 license = GPL2
@@ -31,33 +31,33 @@
 packages = find:
 install_requires = 
 	Faker
 	mmh3
 	murmurhash3
 	graphene-django<3
 	django-allauth
-	packaging
+	packaging<21
 
 [options.extras_require]
 api = 
-	auth0-python
+	auth0-python<4
 maintainer = 
 	zest.releaser[recommended]
 dev = 
 	tox
 	black
 	django
 	pytest
 	pytest-django
 test = 
 	pytest
 	pytest-django
 	pytest-cov
 	model-bakery
-	auth0-python
+	auth0-python<4
 	psycopg2-binary
 
 [bdist_wheel]
 universal = 0
 
 [flake8]
 exclude =
```

### Comparing `simpl-cloud-1.2.4/simpl/__init__.py` & `simpl-cloud-1.3.0/simpl/__init__.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/admin.py` & `simpl-cloud-1.3.0/simpl/admin.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/apps.py` & `simpl-cloud-1.3.0/simpl/apps.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/auth0.py` & `simpl-cloud-1.3.0/simpl/auth0.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/conf/app_settings.py` & `simpl-cloud-1.3.0/simpl/conf/app_settings.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/managers.py` & `simpl-cloud-1.3.0/simpl/managers.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0001_initial.py` & `simpl-cloud-1.3.0/simpl/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0002_run_data.py` & `simpl-cloud-1.3.0/simpl/migrations/0002_run_data.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0003_auto_20210701_1047.py` & `simpl-cloud-1.3.0/simpl/migrations/0003_auto_20210701_1047.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0005_auto_20210707_0934.py` & `simpl-cloud-1.3.0/simpl/migrations/0005_auto_20210707_0934.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0005_auto_20210712_0038.py` & `simpl-cloud-1.3.0/simpl/migrations/0005_auto_20210712_0038.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0006_auto_20210712_0240.py` & `simpl-cloud-1.3.0/simpl/migrations/0006_auto_20210712_0240.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0010_class.py` & `simpl-cloud-1.3.0/simpl/migrations/0010_class.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0013_gameexperience_multiplayer.py` & `simpl-cloud-1.3.0/simpl/migrations/0013_gameexperience_multiplayer.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0014_auto_20210903_1514.py` & `simpl-cloud-1.3.0/simpl/migrations/0014_auto_20210903_1514.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0015_lobby_instance.py` & `simpl-cloud-1.3.0/simpl/migrations/0015_lobby_instance.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0016_link_lobby_instances.py` & `simpl-cloud-1.3.0/simpl/migrations/0016_link_lobby_instances.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0019_auto_20211027_1812.py` & `simpl-cloud-1.3.0/simpl/migrations/0019_auto_20211027_1812.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/migrations/0020_auto_20211109_2056.py` & `simpl-cloud-1.3.0/simpl/migrations/0020_auto_20211109_2056.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/models.py` & `simpl-cloud-1.3.0/simpl/models.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/nav.py` & `simpl-cloud-1.3.0/simpl/nav.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/receivers.py` & `simpl-cloud-1.3.0/simpl/receivers.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/schema/__init__.py` & `simpl-cloud-1.3.0/simpl/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/schema/external/auth0.py` & `simpl-cloud-1.3.0/simpl/schema/external/auth0.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/schema/external/mutations.py` & `simpl-cloud-1.3.0/simpl/schema/external/mutations.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/schema/external/query.py` & `simpl-cloud-1.3.0/simpl/schema/external/query.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/schema/mutations.py` & `simpl-cloud-1.3.0/simpl/schema/mutations.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/schema/query.py` & `simpl-cloud-1.3.0/simpl/schema/query.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/schema/types.py` & `simpl-cloud-1.3.0/simpl/schema/types.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/static/simpl/simpl.es.js` & `simpl-cloud-1.3.0/simpl/static/simpl/simpl.es.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -17,29 +17,29 @@
         return e
     },
     s = (e, i) => t(e, n(i));
 
 function c() {}
 const u = e => e;
 
-function A(e, t) {
+function d(e, t) {
     for (const n in t) e[n] = t[n];
     return e
 }
 
-function d(e) {
+function A(e) {
     return e()
 }
 
 function f() {
     return Object.create(null)
 }
 
 function h(e) {
-    e.forEach(d)
+    e.forEach(A)
 }
 
 function m(e) {
     return "function" == typeof e
 }
 
 function p(e, t) {
@@ -61,15 +61,15 @@
     if (e) {
         const a = b(e, t, n, i);
         return e[0](a)
     }
 }
 
 function b(e, t, n, i) {
-    return e[1] && i ? A(n.ctx.slice(), e[1](i(t))) : n.ctx
+    return e[1] && i ? d(n.ctx.slice(), e[1](i(t))) : n.ctx
 }
 
 function I(e, t, n, i) {
     if (e[2] && i) {
         const a = e[2](i(n));
         if (void 0 === t.dirty) return a;
         if ("object" == typeof a) {
@@ -339,68 +339,68 @@
     const s = 16.666 / i;
     let c = "{\n";
     for (let p = 0; p <= 1; p += s) {
         const e = t + (n - t) * r(p);
         c += 100 * p + `%{${l(e,1-e)}}\n`
     }
     const u = c + `100% {${l(n,1-n)}}\n}`,
-        A = `__svelte_${function(e){let t=5381,n=e.length;for(;n--;)t=(t<<5)-t^e.charCodeAt(n);return t>>>0}(u)}_${o}`,
-        d = F(e);
-    oe.add(d);
-    const f = d.__svelte_stylesheet || (d.__svelte_stylesheet = U(e).sheet),
-        h = d.__svelte_rules || (d.__svelte_rules = {});
-    h[A] || (h[A] = !0, f.insertRule(`@keyframes ${A} ${u}`, f.cssRules.length));
+        d = `__svelte_${function(e){let t=5381,n=e.length;for(;n--;)t=(t<<5)-t^e.charCodeAt(n);return t>>>0}(u)}_${o}`,
+        A = F(e);
+    oe.add(A);
+    const f = A.__svelte_stylesheet || (A.__svelte_stylesheet = U(e).sheet),
+        h = A.__svelte_rules || (A.__svelte_rules = {});
+    h[d] || (h[d] = !0, f.insertRule(`@keyframes ${d} ${u}`, f.cssRules.length));
     const m = e.style.animation || "";
-    return e.style.animation = `${m?`${m}, `:""}${A} ${i}ms linear ${a}ms 1 both`, ce += 1, A
+    return e.style.animation = `${m?`${m}, `:""}${d} ${i}ms linear ${a}ms 1 both`, ce += 1, d
 }
 
-function Ae(e, t) {
+function de(e, t) {
     const n = (e.style.animation || "").split(", "),
         i = n.filter(t ? e => e.indexOf(t) < 0 : e => -1 === e.indexOf("__svelte")),
         a = n.length - i.length;
     a && (e.style.animation = i.join(", "), ce -= a, ce || x((() => {
         ce || (oe.forEach((e => {
             const t = e.__svelte_stylesheet;
             let n = t.cssRules.length;
             for (; n--;) t.deleteRule(n);
             e.__svelte_rules = {}
         })), oe.clear())
     })))
 }
 
-function de(e, t, n, i) {
+function Ae(e, t, n, i) {
     if (!t) return c;
     const a = e.getBoundingClientRect();
     if (t.left === a.left && t.right === a.right && t.top === a.top && t.bottom === a.bottom) return c;
     const {
         delay: r = 0,
         duration: l = 300,
         easing: o = u,
         start: s = P() + r,
-        end: A = s + l,
-        tick: d = c,
+        end: d = s + l,
+        tick: A = c,
         css: f
     } = n(e, {
         from: t,
         to: a
     }, i);
     let h, m = !0,
         p = !1;
 
     function g() {
-        f && Ae(e, h), m = !1
+        f && de(e, h), m = !1
     }
     return V((e => {
-        if (!p && e >= s && (p = !0), p && e >= A && (d(1, 0), g()), !m) return !1;
+        if (!p && e >= s && (p = !0), p && e >= d && (A(1, 0), g()), !m) return !1;
         if (p) {
             const t = 0 + 1 * o((e - s) / l);
-            d(t, 1 - t)
+            A(t, 1 - t)
         }
         return !0
-    })), f && (h = ue(e, 0, 1, l, r, o, f)), r || (p = !0), d(0, 1), g
+    })), f && (h = ue(e, 0, 1, l, r, o, f)), r || (p = !0), A(0, 1), g
 }
 
 function fe(e) {
     const t = getComputedStyle(e);
     if ("absolute" !== t.position && "fixed" !== t.position) {
         const {
             width: n,
@@ -428,210 +428,214 @@
     return se
 }
 
 function ge(e) {
     pe().$$.on_mount.push(e)
 }
 
-function ve() {
+function ve(e) {
+    pe().$$.on_destroy.push(e)
+}
+
+function ye() {
     const e = pe();
     return (t, n) => {
         const i = e.$$.callbacks[t];
         if (i) {
             const a = le(t, n);
             i.slice().forEach((t => {
                 t.call(e, a)
             }))
         }
     }
 }
 
-function ye(e, t) {
+function Ee(e, t) {
     const n = e.$$.callbacks[t.type];
     n && n.slice().forEach((e => e.call(this, t)))
 }
-const Ee = [],
-    be = [],
+const be = [],
     Ie = [],
     we = [],
-    Ce = Promise.resolve();
-let Be = !1;
-
-function Se(e) {
-    Ie.push(e)
-}
+    Ce = [],
+    Be = Promise.resolve();
+let Se = !1;
 
 function Le(e) {
     we.push(e)
 }
-let Pe = !1;
-const xe = new Set;
 
-function ke() {
-    if (!Pe) {
-        Pe = !0;
+function Pe(e) {
+    Ce.push(e)
+}
+let xe = !1;
+const ke = new Set;
+
+function Re() {
+    if (!xe) {
+        xe = !0;
         do {
-            for (let e = 0; e < Ee.length; e += 1) {
-                const t = Ee[e];
-                me(t), Re(t.$$)
+            for (let e = 0; e < be.length; e += 1) {
+                const t = be[e];
+                me(t), Ve(t.$$)
             }
-            for (me(null), Ee.length = 0; be.length;) be.pop()();
-            for (let e = 0; e < Ie.length; e += 1) {
-                const t = Ie[e];
-                xe.has(t) || (xe.add(t), t())
+            for (me(null), be.length = 0; Ie.length;) Ie.pop()();
+            for (let e = 0; e < we.length; e += 1) {
+                const t = we[e];
+                ke.has(t) || (ke.add(t), t())
             }
-            Ie.length = 0
-        } while (Ee.length);
-        for (; we.length;) we.pop()();
-        Be = !1, Pe = !1, xe.clear()
+            we.length = 0
+        } while (be.length);
+        for (; Ce.length;) Ce.pop()();
+        Se = !1, xe = !1, ke.clear()
     }
 }
 
-function Re(e) {
+function Ve(e) {
     if (null !== e.fragment) {
         e.update(), h(e.before_update);
         const t = e.dirty;
-        e.dirty = [-1], e.fragment && e.fragment.p(e.ctx, t), e.after_update.forEach(Se)
+        e.dirty = [-1], e.fragment && e.fragment.p(e.ctx, t), e.after_update.forEach(Le)
     }
 }
-let Ve;
+let Xe;
 
-function Xe() {
-    return Ve || (Ve = Promise.resolve(), Ve.then((() => {
-        Ve = null
-    }))), Ve
+function Oe() {
+    return Xe || (Xe = Promise.resolve(), Xe.then((() => {
+        Xe = null
+    }))), Xe
 }
 
-function Oe(e, t, n) {
+function Fe(e, t, n) {
     e.dispatchEvent(le(`${t?"intro":"outro"}${n}`))
 }
-const Fe = new Set;
-let Ue;
+const Ue = new Set;
+let ze;
 
-function ze() {
-    Ue = {
+function Te() {
+    ze = {
         r: 0,
         c: [],
-        p: Ue
+        p: ze
     }
 }
 
-function Te() {
-    Ue.r || h(Ue.c), Ue = Ue.p
+function De() {
+    ze.r || h(ze.c), ze = ze.p
 }
 
-function De(e, t) {
-    e && e.i && (Fe.delete(e), e.i(t))
+function He(e, t) {
+    e && e.i && (Ue.delete(e), e.i(t))
 }
 
-function He(e, t, n, i) {
+function Ne(e, t, n, i) {
     if (e && e.o) {
-        if (Fe.has(e)) return;
-        Fe.add(e), Ue.c.push((() => {
-            Fe.delete(e), i && (n && e.d(1), i())
+        if (Ue.has(e)) return;
+        Ue.add(e), ze.c.push((() => {
+            Ue.delete(e), i && (n && e.d(1), i())
         })), e.o(t)
     }
 }
-const Ne = {
+const Qe = {
     duration: 0
 };
 
-function Qe(e, t, n) {
+function We(e, t, n) {
     let i, a, r = t(e, n),
         l = !1,
         o = 0;
 
     function s() {
-        i && Ae(e, i)
+        i && de(e, i)
     }
 
-    function A() {
+    function d() {
         const {
             delay: t = 0,
             duration: n = 300,
-            easing: A = u,
-            tick: d = c,
+            easing: d = u,
+            tick: A = c,
             css: f
-        } = r || Ne;
-        f && (i = ue(e, 0, 1, n, t, A, f, o++)), d(0, 1);
+        } = r || Qe;
+        f && (i = ue(e, 0, 1, n, t, d, f, o++)), A(0, 1);
         const h = P() + t,
             m = h + n;
-        a && a.abort(), l = !0, Se((() => Oe(e, !0, "start"))), a = V((t => {
+        a && a.abort(), l = !0, Le((() => Fe(e, !0, "start"))), a = V((t => {
             if (l) {
-                if (t >= m) return d(1, 0), Oe(e, !0, "end"), s(), l = !1;
+                if (t >= m) return A(1, 0), Fe(e, !0, "end"), s(), l = !1;
                 if (t >= h) {
-                    const e = A((t - h) / n);
-                    d(e, 1 - e)
+                    const e = d((t - h) / n);
+                    A(e, 1 - e)
                 }
             }
             return l
         }))
     }
-    let d = !1;
+    let A = !1;
     return {
         start() {
-            d || (d = !0, Ae(e), m(r) ? (r = r(), Xe().then(A)) : A())
+            A || (A = !0, de(e), m(r) ? (r = r(), Oe().then(d)) : d())
         },
         invalidate() {
-            d = !1
+            A = !1
         },
         end() {
             l && (s(), l = !1)
         }
     }
 }
 
-function We(e, t, n) {
+function Je(e, t, n) {
     let i, a = t(e, n),
         r = !0;
-    const l = Ue;
+    const l = ze;
 
     function o() {
         const {
             delay: t = 0,
             duration: n = 300,
             easing: o = u,
             tick: s = c,
-            css: A
-        } = a || Ne;
-        A && (i = ue(e, 1, 0, n, t, o, A));
-        const d = P() + t,
-            f = d + n;
-        Se((() => Oe(e, !1, "start"))), V((t => {
+            css: d
+        } = a || Qe;
+        d && (i = ue(e, 1, 0, n, t, o, d));
+        const A = P() + t,
+            f = A + n;
+        Le((() => Fe(e, !1, "start"))), V((t => {
             if (r) {
-                if (t >= f) return s(0, 1), Oe(e, !1, "end"), --l.r || h(l.c), !1;
-                if (t >= d) {
-                    const e = o((t - d) / n);
+                if (t >= f) return s(0, 1), Fe(e, !1, "end"), --l.r || h(l.c), !1;
+                if (t >= A) {
+                    const e = o((t - A) / n);
                     s(1 - e, e)
                 }
             }
             return r
         }))
     }
-    return l.r += 1, m(a) ? Xe().then((() => {
+    return l.r += 1, m(a) ? Oe().then((() => {
         a = a(), o()
     })) : o(), {
         end(t) {
-            t && a.tick && a.tick(1, 0), r && (i && Ae(e, i), r = !1)
+            t && a.tick && a.tick(1, 0), r && (i && de(e, i), r = !1)
         }
     }
 }
 
-function Je(e, t, n, i) {
+function je(e, t, n, i) {
     let a = t(e, n),
         r = i ? 0 : 1,
         l = null,
         o = null,
         s = null;
 
-    function A() {
-        s && Ae(e, s)
+    function d() {
+        s && de(e, s)
     }
 
-    function d(e, t) {
+    function A(e, t) {
         const n = e.b - r;
         return t *= Math.abs(n), {
             a: r,
             b: e.b,
             d: n,
             duration: t,
             start: e.start,
@@ -643,127 +647,127 @@
     function f(t) {
         const {
             delay: n = 0,
             duration: i = 300,
             easing: f = u,
             tick: m = c,
             css: p
-        } = a || Ne, g = {
+        } = a || Qe, g = {
             start: P() + n,
             b: t
         };
-        t || (g.group = Ue, Ue.r += 1), l || o ? o = g : (p && (A(), s = ue(e, r, t, i, n, f, p)), t && m(0, 1), l = d(g, i), Se((() => Oe(e, t, "start"))), V((t => {
-            if (o && t > o.start && (l = d(o, i), o = null, Oe(e, l.b, "start"), p && (A(), s = ue(e, r, l.b, l.duration, 0, f, a.css))), l)
-                if (t >= l.end) m(r = l.b, 1 - r), Oe(e, l.b, "end"), o || (l.b ? A() : --l.group.r || h(l.group.c)), l = null;
+        t || (g.group = ze, ze.r += 1), l || o ? o = g : (p && (d(), s = ue(e, r, t, i, n, f, p)), t && m(0, 1), l = A(g, i), Le((() => Fe(e, t, "start"))), V((t => {
+            if (o && t > o.start && (l = A(o, i), o = null, Fe(e, l.b, "start"), p && (d(), s = ue(e, r, l.b, l.duration, 0, f, a.css))), l)
+                if (t >= l.end) m(r = l.b, 1 - r), Fe(e, l.b, "end"), o || (l.b ? d() : --l.group.r || h(l.group.c)), l = null;
                 else if (t >= l.start) {
                 const e = t - l.start;
                 r = l.a + l.d * f(e / l.duration), m(r, 1 - r)
             }
             return !(!l && !o)
         })))
     }
     return {
         run(e) {
-            m(a) ? Xe().then((() => {
+            m(a) ? Oe().then((() => {
                 a = a(), f(e)
             })) : f(e)
         },
         end() {
-            A(), l = o = null
+            d(), l = o = null
         }
     }
 }
-const je = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : global;
+const qe = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : global;
 
-function qe(e, t) {
+function Me(e, t) {
     e.d(1), t.delete(e.key)
 }
 
-function Me(e, t) {
-    He(e, 1, 1, (() => {
+function Ke(e, t) {
+    Ne(e, 1, 1, (() => {
         t.delete(e.key)
     }))
 }
 
-function Ke(e, t) {
-    e.f(), Me(e, t)
+function Ze(e, t) {
+    e.f(), Ke(e, t)
 }
 
-function Ze(e, t, n, i, a, r, l, o, s, c, u, A) {
-    let d = e.length,
+function Ye(e, t, n, i, a, r, l, o, s, c, u, d) {
+    let A = e.length,
         f = r.length,
-        h = d;
+        h = A;
     const m = {};
     for (; h--;) m[e[h].key] = h;
     const p = [],
         g = new Map,
         v = new Map;
     for (h = f; h--;) {
-        const e = A(a, r, h),
+        const e = d(a, r, h),
             o = n(e);
         let s = l.get(o);
         s ? i && s.p(e, t) : (s = c(o, e), s.c()), g.set(o, p[h] = s), o in m && v.set(o, Math.abs(h - m[o]))
     }
     const y = new Set,
         E = new Set;
 
     function b(e) {
-        De(e, 1), e.m(o, u), l.set(e.key, e), u = e.first, f--
+        He(e, 1), e.m(o, u), l.set(e.key, e), u = e.first, f--
     }
-    for (; d && f;) {
+    for (; A && f;) {
         const t = p[f - 1],
-            n = e[d - 1],
+            n = e[A - 1],
             i = t.key,
             a = n.key;
-        t === n ? (u = t.first, d--, f--) : g.has(a) ? !l.has(i) || y.has(i) ? b(t) : E.has(a) ? d-- : v.get(i) > v.get(a) ? (E.add(i), b(t)) : (y.add(a), d--) : (s(n, l), d--)
+        t === n ? (u = t.first, A--, f--) : g.has(a) ? !l.has(i) || y.has(i) ? b(t) : E.has(a) ? A-- : v.get(i) > v.get(a) ? (E.add(i), b(t)) : (y.add(a), A--) : (s(n, l), A--)
     }
-    for (; d--;) {
-        const t = e[d];
+    for (; A--;) {
+        const t = e[A];
         g.has(t.key) || s(t, l)
     }
     for (; f;) b(p[f - 1]);
     return p
 }
 
-function Ye(e, t, n) {
+function Ge(e, t, n) {
     const i = e.$$.props[t];
     void 0 !== i && (e.$$.bound[i] = n, n(e.$$.ctx[i]))
 }
 
-function Ge(e) {
+function $e(e) {
     e && e.c()
 }
 
-function $e(e, t) {
+function _e(e, t) {
     e && e.l(t)
 }
 
-function _e(e, t, n, i) {
+function et(e, t, n, i) {
     const {
         fragment: a,
         on_mount: r,
         on_destroy: l,
         after_update: o
     } = e.$$;
-    a && a.m(t, n), i || Se((() => {
-        const t = r.map(d).filter(m);
+    a && a.m(t, n), i || Le((() => {
+        const t = r.map(A).filter(m);
         l ? l.push(...t) : h(t), e.$$.on_mount = []
-    })), o.forEach(Se)
+    })), o.forEach(Le)
 }
 
-function et(e, t) {
+function tt(e, t) {
     const n = e.$$;
     null !== n.fragment && (h(n.on_destroy), n.fragment && n.fragment.d(t), n.on_destroy = n.fragment = null, n.ctx = [])
 }
 
-function tt(e, t) {
-    -1 === e.$$.dirty[0] && (Ee.push(e), Be || (Be = !0, Ce.then(ke)), e.$$.dirty.fill(0)), e.$$.dirty[t / 31 | 0] |= 1 << t % 31
+function nt(e, t) {
+    -1 === e.$$.dirty[0] && (be.push(e), Se || (Se = !0, Be.then(Re)), e.$$.dirty.fill(0)), e.$$.dirty[t / 31 | 0] |= 1 << t % 31
 }
 
-function nt(e, t, n, i, a, r, l, o = [-1]) {
+function it(e, t, n, i, a, r, l, o = [-1]) {
     const s = se;
     me(e);
     const u = e.$$ = {
         fragment: null,
         ctx: null,
         props: r,
         update: c,
@@ -777,56 +781,56 @@
         context: new Map(s ? s.$$.context : t.context || []),
         callbacks: f(),
         dirty: o,
         skip_bound: !1,
         root: t.target || s.$$.root
     };
     l && l(u.root);
-    let A = !1;
+    let d = !1;
     if (u.ctx = n ? n(e, t.props || {}, ((t, n, ...i) => {
             const r = i.length ? i[0] : n;
-            return u.ctx && a(u.ctx[t], u.ctx[t] = r) && (!u.skip_bound && u.bound[t] && u.bound[t](r), A && tt(e, t)), n
-        })) : [], u.update(), A = !0, h(u.before_update), u.fragment = !!i && i(u.ctx), t.target) {
+            return u.ctx && a(u.ctx[t], u.ctx[t] = r) && (!u.skip_bound && u.bound[t] && u.bound[t](r), d && nt(e, t)), n
+        })) : [], u.update(), d = !0, h(u.before_update), u.fragment = !!i && i(u.ctx), t.target) {
         if (t.hydrate) {
             X = !0;
             const e = G(t.target);
             u.fragment && u.fragment.l(e), e.forEach(D)
         } else u.fragment && u.fragment.c();
-        t.intro && De(e.$$.fragment), _e(e, t.target, t.anchor, t.customElement), X = !1, ke()
+        t.intro && He(e.$$.fragment), et(e, t.target, t.anchor, t.customElement), X = !1, Re()
     }
     me(s)
 }
-class it {
+class at {
     $destroy() {
-        et(this, 1), this.$destroy = c
+        tt(this, 1), this.$destroy = c
     }
     $on(e, t) {
         const n = this.$$.callbacks[e] || (this.$$.callbacks[e] = []);
         return n.push(t), () => {
             const e = n.indexOf(t); - 1 !== e && n.splice(e, 1)
         }
     }
     $set(e) {
         var t;
         this.$$set && (t = e, 0 !== Object.keys(t).length) && (this.$$.skip_bound = !0, this.$$set(e), this.$$.skip_bound = !1)
     }
 }
-const at = [];
+const rt = [];
 
-function rt(e, t = c) {
+function lt(e, t = c) {
     let n;
     const i = new Set;
 
     function a(t) {
         if (p(e, t) && (e = t, n)) {
-            const t = !at.length;
-            for (const n of i) n[1](), at.push(n, e);
+            const t = !rt.length;
+            for (const n of i) n[1](), rt.push(n, e);
             if (t) {
-                for (let e = 0; e < at.length; e += 2) at[e][0](at[e + 1]);
-                at.length = 0
+                for (let e = 0; e < rt.length; e += 2) rt[e][0](rt[e + 1]);
+                rt.length = 0
             }
         }
     }
     return {
         set: a,
         update: function(t) {
             a(t(e))
@@ -835,103 +839,103 @@
             const o = [r, l];
             return i.add(o), 1 === i.size && (n = t(a) || c), r(e), () => {
                 i.delete(o), 0 === i.size && (n(), n = null)
             }
         }
     }
 }
-const lt = rt({
+const ot = lt({
         sessions: [],
         teams: [],
         players: null,
         minimumPlayers: null,
         maximumPlayers: null
     }),
-    ot = rt(!1);
-const st = function() {
+    st = lt(!1);
+const ct = function() {
     const e = new Set;
     return {
         subscribe: t => (e.add(t), () => {
             e.delete(t)
         }),
         notify: t => {
             e.forEach((e => e(t)))
         }
     }
 }();
-var ct = window.CustomEvent;
+var ut = window.CustomEvent;
 
-function ut(e, t) {
+function dt(e, t) {
     var n = "on" + t.type.toLowerCase();
     return "function" == typeof e[n] && e[n](t), e.dispatchEvent(t)
 }
 
 function At(e) {
     for (; e;) {
         if ("dialog" === e.localName) return e;
         e = e.parentElement ? e.parentElement : e.parentNode ? e.parentNode.host : null
     }
     return null
 }
 
-function dt(e) {
+function ft(e) {
     for (; e && e.shadowRoot && e.shadowRoot.activeElement;) e = e.shadowRoot.activeElement;
     e && e.blur && e !== document.body && e.blur()
 }
 
-function ft(e, t) {
+function ht(e, t) {
     for (var n = 0; n < e.length; ++n)
         if (e[n] === t) return !0;
     return !1
 }
 
-function ht(e) {
+function mt(e) {
     return !(!e || !e.hasAttribute("method")) && "dialog" === e.getAttribute("method").toLowerCase()
 }
 
-function mt(e) {
+function pt(e) {
     var t = ["button", "input", "keygen", "select", "textarea"].map((function(e) {
         return e + ":not([disabled])"
     }));
     t.push('[tabindex]:not([disabled]):not([tabindex=""])');
     var n = e.querySelector(t.join(", "));
     if (!n && "attachShadow" in Element.prototype)
-        for (var i = e.querySelectorAll("*"), a = 0; a < i.length && !(i[a].tagName && i[a].shadowRoot && (n = mt(i[a].shadowRoot))); a++);
+        for (var i = e.querySelectorAll("*"), a = 0; a < i.length && !(i[a].tagName && i[a].shadowRoot && (n = pt(i[a].shadowRoot))); a++);
     return n
 }
 
-function pt(e) {
+function gt(e) {
     return e.isConnected || document.body.contains(e)
 }
 
-function gt(e) {
+function vt(e) {
     if (e.submitter) return e.submitter;
     var t = e.target;
     if (!(t instanceof HTMLFormElement)) return null;
-    var n = Et.formSubmitter;
+    var n = bt.formSubmitter;
     if (!n) {
         var i = e.target;
         n = ("getRootNode" in i && i.getRootNode() || document).activeElement
     }
     return n && n.form === t ? n : null
 }
 
-function vt(e) {
+function yt(e) {
     if (!e.defaultPrevented) {
         var t = e.target,
-            n = Et.imagemapUseValue,
-            i = gt(e);
+            n = bt.imagemapUseValue,
+            i = vt(e);
         null === n && i && (n = i.value);
         var a = At(t);
         if (a) "dialog" === (i && i.getAttribute("formmethod") || t.getAttribute("method")) && (e.preventDefault(), null != n ? a.close(n) : a.close())
     }
 }
 
-function yt(e) {
-    if (this.dialog_ = e, this.replacedStyleTop_ = !1, this.openAsModal_ = !1, e.hasAttribute("role") || e.setAttribute("role", "dialog"), e.show = this.show.bind(this), e.showModal = this.showModal.bind(this), e.close = this.close.bind(this), e.addEventListener("submit", vt, !1), "returnValue" in e || (e.returnValue = ""), "MutationObserver" in window) {
+function Et(e) {
+    if (this.dialog_ = e, this.replacedStyleTop_ = !1, this.openAsModal_ = !1, e.hasAttribute("role") || e.setAttribute("role", "dialog"), e.show = this.show.bind(this), e.showModal = this.showModal.bind(this), e.close = this.close.bind(this), e.addEventListener("submit", yt, !1), "returnValue" in e || (e.returnValue = ""), "MutationObserver" in window) {
         new MutationObserver(this.maybeHideModal.bind(this)).observe(e, {
             attributes: !0,
             attributeFilter: ["open"]
         })
     } else {
         var t, n = !1,
             i = function() {
@@ -948,27 +952,27 @@
         }))
     }
     Object.defineProperty(e, "open", {
         set: this.setOpen.bind(this),
         get: e.hasAttribute.bind(e, "open")
     }), this.backdrop_ = document.createElement("div"), this.backdrop_.className = "backdrop", this.backdrop_.addEventListener("mouseup", this.backdropMouseEvent_.bind(this)), this.backdrop_.addEventListener("mousedown", this.backdropMouseEvent_.bind(this)), this.backdrop_.addEventListener("click", this.backdropMouseEvent_.bind(this))
 }
-ct && "object" != typeof ct || ((ct = function(e, t) {
+ut && "object" != typeof ut || ((ut = function(e, t) {
     t = t || {};
     var n = document.createEvent("CustomEvent");
     return n.initCustomEvent(e, !!t.bubbles, !!t.cancelable, t.detail || null), n
-}).prototype = window.Event.prototype), yt.prototype = {
+}).prototype = window.Event.prototype), Et.prototype = {
     get dialog() {
         return this.dialog_
     },
     maybeHideModal: function() {
-        this.dialog_.hasAttribute("open") && pt(this.dialog_) || this.downgradeModal()
+        this.dialog_.hasAttribute("open") && gt(this.dialog_) || this.downgradeModal()
     },
     downgradeModal: function() {
-        this.openAsModal_ && (this.openAsModal_ = !1, this.dialog_.style.zIndex = "", this.replacedStyleTop_ && (this.dialog_.style.top = "", this.replacedStyleTop_ = !1), this.backdrop_.parentNode && this.backdrop_.parentNode.removeChild(this.backdrop_), Et.dm.removeDialog(this))
+        this.openAsModal_ && (this.openAsModal_ = !1, this.dialog_.style.zIndex = "", this.replacedStyleTop_ && (this.dialog_.style.top = "", this.replacedStyleTop_ = !1), this.backdrop_.parentNode && this.backdrop_.parentNode.removeChild(this.backdrop_), bt.dm.removeDialog(this))
     },
     setOpen: function(e) {
         e ? this.dialog_.hasAttribute("open") || this.dialog_.setAttribute("open", "") : (this.dialog_.removeAttribute("open"), this.maybeHideModal())
     },
     backdropMouseEvent_: function(e) {
         if (this.dialog_.hasAttribute("tabindex")) this.dialog_.focus();
         else {
@@ -976,50 +980,50 @@
             this.dialog_.insertBefore(t, this.dialog_.firstChild), t.tabIndex = -1, t.focus(), this.dialog_.removeChild(t)
         }
         var n = document.createEvent("MouseEvents");
         n.initMouseEvent(e.type, e.bubbles, e.cancelable, window, e.detail, e.screenX, e.screenY, e.clientX, e.clientY, e.ctrlKey, e.altKey, e.shiftKey, e.metaKey, e.button, e.relatedTarget), this.dialog_.dispatchEvent(n), e.stopPropagation()
     },
     focus_: function() {
         var e = this.dialog_.querySelector("[autofocus]:not([disabled])");
-        !e && this.dialog_.tabIndex >= 0 && (e = this.dialog_), e || (e = mt(this.dialog_)), dt(document.activeElement), e && e.focus()
+        !e && this.dialog_.tabIndex >= 0 && (e = this.dialog_), e || (e = pt(this.dialog_)), ft(document.activeElement), e && e.focus()
     },
     updateZIndex: function(e, t) {
         if (e < t) throw new Error("dialogZ should never be < backdropZ");
         this.dialog_.style.zIndex = e, this.backdrop_.style.zIndex = t
     },
     show: function() {
         this.dialog_.open || (this.setOpen(!0), this.focus_())
     },
     showModal: function() {
         if (this.dialog_.hasAttribute("open")) throw new Error("Failed to execute 'showModal' on dialog: The element is already open, and therefore cannot be opened modally.");
-        if (!pt(this.dialog_)) throw new Error("Failed to execute 'showModal' on dialog: The element is not in a Document.");
-        if (!Et.dm.pushDialog(this)) throw new Error("Failed to execute 'showModal' on dialog: There are too many open modal dialogs.");
+        if (!gt(this.dialog_)) throw new Error("Failed to execute 'showModal' on dialog: The element is not in a Document.");
+        if (!bt.dm.pushDialog(this)) throw new Error("Failed to execute 'showModal' on dialog: There are too many open modal dialogs.");
         (function(e) {
             for (; e && e !== document.body;) {
                 var t = window.getComputedStyle(e),
                     n = function(e, n) {
                         return !(void 0 === t[e] || t[e] === n)
                     };
                 if (t.opacity < 1 || n("zIndex", "auto") || n("transform", "none") || n("mixBlendMode", "normal") || n("filter", "none") || n("perspective", "none") || "isolate" === t.isolation || "fixed" === t.position || "touch" === t.webkitOverflowScrolling) return !0;
                 e = e.parentElement
             }
             return !1
-        })(this.dialog_.parentElement) && console.warn("A dialog is being shown inside a stacking context. This may cause it to be unusable. For more information, see this link: https://github.com/GoogleChrome/dialog-polyfill/#stacking-context"), this.setOpen(!0), this.openAsModal_ = !0, Et.needsCentering(this.dialog_) ? (Et.reposition(this.dialog_), this.replacedStyleTop_ = !0) : this.replacedStyleTop_ = !1, this.dialog_.parentNode.insertBefore(this.backdrop_, this.dialog_.nextSibling), this.focus_()
+        })(this.dialog_.parentElement) && console.warn("A dialog is being shown inside a stacking context. This may cause it to be unusable. For more information, see this link: https://github.com/GoogleChrome/dialog-polyfill/#stacking-context"), this.setOpen(!0), this.openAsModal_ = !0, bt.needsCentering(this.dialog_) ? (bt.reposition(this.dialog_), this.replacedStyleTop_ = !0) : this.replacedStyleTop_ = !1, this.dialog_.parentNode.insertBefore(this.backdrop_, this.dialog_.nextSibling), this.focus_()
     },
     close: function(e) {
         if (!this.dialog_.hasAttribute("open")) throw new Error("Failed to execute 'close' on dialog: The element does not have an 'open' attribute, and therefore cannot be closed.");
         this.setOpen(!1), void 0 !== e && (this.dialog_.returnValue = e);
-        var t = new ct("close", {
+        var t = new ut("close", {
             bubbles: !1,
             cancelable: !1
         });
-        ut(this.dialog_, t)
+        dt(this.dialog_, t)
     }
 };
-var Et = {
+var bt = {
     reposition: function(e) {
         var t = document.body.scrollTop || document.documentElement.scrollTop,
             n = t + (window.innerHeight - e.offsetHeight) / 2;
         e.style.top = Math.max(t, n) + "px"
     },
     isInlinePositionSetByStylesheet: function(e) {
         for (var t = 0; t < document.styleSheets.length; ++t) {
@@ -1031,138 +1035,138 @@
             if (i)
                 for (var a = 0; a < i.length; ++a) {
                     var r = i[a],
                         l = null;
                     try {
                         l = document.querySelectorAll(r.selectorText)
                     } catch (c) {}
-                    if (l && ft(l, e)) {
+                    if (l && ht(l, e)) {
                         var o = r.style.getPropertyValue("top"),
                             s = r.style.getPropertyValue("bottom");
                         if (o && "auto" !== o || s && "auto" !== s) return !0
                     }
                 }
         }
         return !1
     },
     needsCentering: function(e) {
-        return "absolute" === window.getComputedStyle(e).position && (!("auto" !== e.style.top && "" !== e.style.top || "auto" !== e.style.bottom && "" !== e.style.bottom) && !Et.isInlinePositionSetByStylesheet(e))
+        return "absolute" === window.getComputedStyle(e).position && (!("auto" !== e.style.top && "" !== e.style.top || "auto" !== e.style.bottom && "" !== e.style.bottom) && !bt.isInlinePositionSetByStylesheet(e))
     },
     forceRegisterDialog: function(e) {
         if ((window.HTMLDialogElement || e.showModal) && console.warn("This browser already supports <dialog>, the polyfill may not work correctly", e), "dialog" !== e.localName) throw new Error("Failed to register dialog: The element is not a dialog.");
-        new yt(e)
+        new Et(e)
     },
     registerDialog: function(e) {
-        e.showModal || Et.forceRegisterDialog(e)
+        e.showModal || bt.forceRegisterDialog(e)
     },
     DialogManager: function() {
         this.pendingDialogStack = [];
         var e = this.checkDOM_.bind(this);
         this.overlay = document.createElement("div"), this.overlay.className = "_dialog_overlay", this.overlay.addEventListener("click", function(t) {
             this.forwardTab_ = void 0, t.stopPropagation(), e([])
         }.bind(this)), this.handleKey_ = this.handleKey_.bind(this), this.handleFocus_ = this.handleFocus_.bind(this), this.zIndexLow_ = 1e5, this.zIndexHigh_ = 100150, this.forwardTab_ = void 0, "MutationObserver" in window && (this.mo_ = new MutationObserver((function(t) {
             var n = [];
             t.forEach((function(e) {
                 for (var t, i = 0; t = e.removedNodes[i]; ++i) t instanceof Element && ("dialog" === t.localName && n.push(t), n = n.concat(t.querySelectorAll("dialog")))
             })), n.length && e(n)
         })))
     }
 };
-if (Et.DialogManager.prototype.blockDocument = function() {
+if (bt.DialogManager.prototype.blockDocument = function() {
         document.documentElement.addEventListener("focus", this.handleFocus_, !0), document.addEventListener("keydown", this.handleKey_), this.mo_ && this.mo_.observe(document, {
             childList: !0,
             subtree: !0
         })
-    }, Et.DialogManager.prototype.unblockDocument = function() {
+    }, bt.DialogManager.prototype.unblockDocument = function() {
         document.documentElement.removeEventListener("focus", this.handleFocus_, !0), document.removeEventListener("keydown", this.handleKey_), this.mo_ && this.mo_.disconnect()
-    }, Et.DialogManager.prototype.updateStacking = function() {
+    }, bt.DialogManager.prototype.updateStacking = function() {
         for (var e, t = this.zIndexHigh_, n = 0; e = this.pendingDialogStack[n]; ++n) e.updateZIndex(--t, --t), 0 === n && (this.overlay.style.zIndex = --t);
         var i = this.pendingDialogStack[0];
         i ? (i.dialog.parentNode || document.body).appendChild(this.overlay) : this.overlay.parentNode && this.overlay.parentNode.removeChild(this.overlay)
-    }, Et.DialogManager.prototype.containedByTopDialog_ = function(e) {
+    }, bt.DialogManager.prototype.containedByTopDialog_ = function(e) {
         for (; e = At(e);) {
             for (var t, n = 0; t = this.pendingDialogStack[n]; ++n)
                 if (t.dialog === e) return 0 === n;
             e = e.parentElement
         }
         return !1
-    }, Et.DialogManager.prototype.handleFocus_ = function(e) {
+    }, bt.DialogManager.prototype.handleFocus_ = function(e) {
         var t = e.composedPath ? e.composedPath()[0] : e.target;
-        if (!this.containedByTopDialog_(t) && document.activeElement !== document.documentElement && (e.preventDefault(), e.stopPropagation(), dt(t), void 0 !== this.forwardTab_)) {
+        if (!this.containedByTopDialog_(t) && document.activeElement !== document.documentElement && (e.preventDefault(), e.stopPropagation(), ft(t), void 0 !== this.forwardTab_)) {
             var n = this.pendingDialogStack[0];
             return n.dialog.compareDocumentPosition(t) & Node.DOCUMENT_POSITION_PRECEDING && (this.forwardTab_ ? n.focus_() : t !== document.documentElement && document.documentElement.focus()), !1
         }
-    }, Et.DialogManager.prototype.handleKey_ = function(e) {
+    }, bt.DialogManager.prototype.handleKey_ = function(e) {
         if (this.forwardTab_ = void 0, 27 === e.keyCode) {
             e.preventDefault(), e.stopPropagation();
-            var t = new ct("cancel", {
+            var t = new ut("cancel", {
                     bubbles: !1,
                     cancelable: !0
                 }),
                 n = this.pendingDialogStack[0];
-            n && ut(n.dialog, t) && n.dialog.close()
+            n && dt(n.dialog, t) && n.dialog.close()
         } else 9 === e.keyCode && (this.forwardTab_ = !e.shiftKey)
-    }, Et.DialogManager.prototype.checkDOM_ = function(e) {
+    }, bt.DialogManager.prototype.checkDOM_ = function(e) {
         this.pendingDialogStack.slice().forEach((function(t) {
             -1 !== e.indexOf(t.dialog) ? t.downgradeModal() : t.maybeHideModal()
         }))
-    }, Et.DialogManager.prototype.pushDialog = function(e) {
+    }, bt.DialogManager.prototype.pushDialog = function(e) {
         var t = (this.zIndexHigh_ - this.zIndexLow_) / 2 - 1;
         return !(this.pendingDialogStack.length >= t) && (1 === this.pendingDialogStack.unshift(e) && this.blockDocument(), this.updateStacking(), !0)
-    }, Et.DialogManager.prototype.removeDialog = function(e) {
+    }, bt.DialogManager.prototype.removeDialog = function(e) {
         var t = this.pendingDialogStack.indexOf(e); - 1 !== t && (this.pendingDialogStack.splice(t, 1), 0 === this.pendingDialogStack.length && this.unblockDocument(), this.updateStacking())
-    }, Et.dm = new Et.DialogManager, Et.formSubmitter = null, Et.imagemapUseValue = null, void 0 === window.HTMLDialogElement) {
-    var bt = document.createElement("form");
-    if (bt.setAttribute("method", "dialog"), "dialog" !== bt.method) {
-        var It = Object.getOwnPropertyDescriptor(HTMLFormElement.prototype, "method");
-        if (It) {
-            var wt = It.get;
-            It.get = function() {
-                return ht(this) ? "dialog" : wt.call(this)
+    }, bt.dm = new bt.DialogManager, bt.formSubmitter = null, bt.imagemapUseValue = null, void 0 === window.HTMLDialogElement) {
+    var It = document.createElement("form");
+    if (It.setAttribute("method", "dialog"), "dialog" !== It.method) {
+        var wt = Object.getOwnPropertyDescriptor(HTMLFormElement.prototype, "method");
+        if (wt) {
+            var Ct = wt.get;
+            wt.get = function() {
+                return mt(this) ? "dialog" : Ct.call(this)
             };
-            var Ct = It.set;
-            It.set = function(e) {
-                return "string" == typeof e && "dialog" === e.toLowerCase() ? this.setAttribute("method", e) : Ct.call(this, e)
-            }, Object.defineProperty(HTMLFormElement.prototype, "method", It)
+            var Bt = wt.set;
+            wt.set = function(e) {
+                return "string" == typeof e && "dialog" === e.toLowerCase() ? this.setAttribute("method", e) : Bt.call(this, e)
+            }, Object.defineProperty(HTMLFormElement.prototype, "method", wt)
         }
     }
     document.addEventListener("click", (function(e) {
-        if (Et.formSubmitter = null, Et.imagemapUseValue = null, !e.defaultPrevented) {
+        if (bt.formSubmitter = null, bt.imagemapUseValue = null, !e.defaultPrevented) {
             var t = e.target;
             if ("composedPath" in e) t = e.composedPath().shift() || t;
-            if (t && ht(t.form)) {
+            if (t && mt(t.form)) {
                 if (!("submit" === t.type && ["button", "input"].indexOf(t.localName) > -1)) {
                     if ("input" !== t.localName || "image" !== t.type) return;
-                    Et.imagemapUseValue = e.offsetX + "," + e.offsetY
+                    bt.imagemapUseValue = e.offsetX + "," + e.offsetY
                 }
-                At(t) && (Et.formSubmitter = t)
+                At(t) && (bt.formSubmitter = t)
             }
         }
     }), !1), document.addEventListener("submit", (function(e) {
         var t = e.target;
         if (!At(t)) {
-            var n = gt(e);
+            var n = vt(e);
             "dialog" === (n && n.getAttribute("formmethod") || t.getAttribute("method")) && e.preventDefault()
         }
     }));
-    var Bt = HTMLFormElement.prototype.submit;
+    var St = HTMLFormElement.prototype.submit;
     HTMLFormElement.prototype.submit = function() {
-        if (!ht(this)) return Bt.call(this);
+        if (!mt(this)) return St.call(this);
         var e = At(this);
         e && e.close()
     }
 }
 
-function St(e) {
+function Lt(e) {
     let t, n, i, a, r, l, o, s, c;
     const u = e[3].default,
-        A = E(u, e, e[2], null);
+        d = E(u, e, e[2], null);
     return {
         c() {
-            t = N("dialog"), n = N("button"), i = Q("svg"), a = Q("path"), r = J(), l = N("div"), A && A.c(), this.h()
+            t = N("dialog"), n = N("button"), i = Q("svg"), a = Q("path"), r = J(), l = N("div"), d && d.c(), this.h()
         },
         l(e) {
             t = _(e, "DIALOG", {
                 class: !0
             });
             var o = G(t);
             n = _(o, "BUTTON", {
@@ -1178,69 +1182,69 @@
             a = _(c, "path", {
                 fill: !0,
                 d: !0
             }, 1), G(a).forEach(D), c.forEach(D), s.forEach(D), r = te(o), l = _(o, "DIV", {
                 class: !0
             });
             var u = G(l);
-            A && A.l(u), u.forEach(D), o.forEach(D), this.h()
+            d && d.l(u), u.forEach(D), o.forEach(D), this.h()
         },
         h() {
             Z(a, "fill", "currentColor"), Z(a, "d", "M11.38 7.75L16 3.14a1.86 1.86 0 00.25-2.38 1.79 1.79 0 00-2.74-.23L8.83 5.2a.76.76 0 01-1.08 0L3.14.6A1.86 1.86 0 00.76.33a1.79 1.79 0 00-.23 2.74L5.2 7.75a.76.76 0 010 1.08L.6 13.44a1.88 1.88 0 00-.27 2.39 1.81 1.81 0 002.74.23l4.68-4.68a.76.76 0 011.08 0L13.44 16a1.87 1.87 0 002.39.26 1.81 1.81 0 00.23-2.74l-4.68-4.69a.76.76 0 010-1.08z"), Z(i, "class", "icon"), Z(i, "viewBox", "0 0 16.59 16.59"), Z(i, "xmlns", "http://www.w3.org/2000/svg"), Z(n, "class", "close-button"), Z(l, "class", "scroll-wrap"), Z(t, "class", "modal")
         },
-        m(u, d) {
-            T(u, t, d), z(t, n), z(n, i), z(i, a), z(t, r), z(t, l), A && A.m(l, null), e[5](t), o = !0, s || (c = q(n, "click", e[4]), s = !0)
+        m(u, A) {
+            T(u, t, A), z(t, n), z(n, i), z(i, a), z(t, r), z(t, l), d && d.m(l, null), e[5](t), o = !0, s || (c = q(n, "click", e[4]), s = !0)
         },
         p(e, [t]) {
-            A && A.p && (!o || 4 & t) && w(A, u, e, e[2], o ? I(u, e[2], t, null) : C(e[2]), null)
+            d && d.p && (!o || 4 & t) && w(d, u, e, e[2], o ? I(u, e[2], t, null) : C(e[2]), null)
         },
         i(e) {
-            o || (De(A, e), o = !0)
+            o || (He(d, e), o = !0)
         },
         o(e) {
-            He(A, e), o = !1
+            Ne(d, e), o = !1
         },
         d(n) {
-            n && D(t), A && A.d(n), e[5](null), s = !1, c()
+            n && D(t), d && d.d(n), e[5](null), s = !1, c()
         }
     }
 }
 
-function Lt(e, t, n) {
+function Pt(e, t, n) {
     let i, {
             $$slots: a = {},
             $$scope: r
         } = t,
         {
             open: l = !1
         } = t;
     ge((() => {
-        Et.registerDialog(i)
+        bt.registerDialog(i)
     }));
     return e.$$set = e => {
         "open" in e && n(0, l = e.open), "$$scope" in e && n(2, r = e.$$scope)
     }, e.$$.update = () => {
         3 & e.$$.dirty && (l ? null == i || i.showModal() : i && i.open && i.close())
     }, [l, i, r, a, () => {
         n(0, l = !1)
     }, function(e) {
-        be[e ? "unshift" : "push"]((() => {
+        Ie[e ? "unshift" : "push"]((() => {
             i = e, n(1, i)
         }))
     }]
 }
-class Pt extends it {
+class xt extends at {
     constructor(e) {
-        super(), nt(this, e, Lt, St, p, {
+        super(), it(this, e, Pt, Lt, p, {
             open: 0
         })
     }
 }
 
-function xt(e) {
+function kt(e) {
     let t, n, i, a, r;
     return {
         c() {
             t = N("input"), this.h()
         },
         l(e) {
             t = _(e, "INPUT", {
@@ -1262,15 +1266,15 @@
         },
         d(e) {
             e && D(t), a = !1, r()
         }
     }
 }
 
-function kt(e) {
+function Rt(e) {
     let t;
     return {
         c() {
             t = W(e[3])
         },
         l(n) {
             t = ee(n, e[3])
@@ -1283,19 +1287,19 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Rt(e) {
+function Vt(e) {
     let t;
 
     function n(e, t) {
-        return e[2].minimumPlayers > 1 && e[2].maximumPlayers ? Ot : e[2].minimumPlayers > 1 ? Xt : e[2].maximumPlayers ? Vt : void 0
+        return e[2].minimumPlayers > 1 && e[2].maximumPlayers ? Ft : e[2].minimumPlayers > 1 ? Ot : e[2].maximumPlayers ? Xt : void 0
     }
     let i = n(e),
         a = i && i(e);
     return {
         c() {
             a && a.c(), t = j()
         },
@@ -1310,15 +1314,15 @@
         },
         d(e) {
             a && a.d(e), e && D(t)
         }
     }
 }
 
-function Vt(e) {
+function Xt(e) {
     let t, n, i, a, r = e[2].maximumPlayers + "";
     return {
         c() {
             t = N("em"), n = W("(at most "), i = W(r), a = W(")")
         },
         l(e) {
             t = _(e, "EM", {});
@@ -1333,15 +1337,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Xt(e) {
+function Ot(e) {
     let t, n, i, a, r = e[2].minimumPlayers + "";
     return {
         c() {
             t = N("em"), n = W("(at least "), i = W(r), a = W(")")
         },
         l(e) {
             t = _(e, "EM", {});
@@ -1356,15 +1360,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Ot(e) {
+function Ft(e) {
     let t, n, i, a, r, l, o = e[2].minimumPlayers + "",
         s = e[2].maximumPlayers + "";
     return {
         c() {
             t = N("em"), n = W("(between "), i = W(o), a = W(" and\n              "), r = W(s), l = W(")")
         },
         l(e) {
@@ -1380,120 +1384,120 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Ft(e) {
-    let t, n, i, a, r, l, o, s, c, u, A, d, f, h, m, p, g, v, y = 1 == e[3] ? "player" : "players",
+function Ut(e) {
+    let t, n, i, a, r, l, o, s, c, u, d, A, f, h, m, p, g, v, y = 1 == e[3] ? "player" : "players",
         E = e[1].length + "";
 
     function b(e, t) {
-        return e[2].minimumPlayers && e[2].maximumPlayers && e[2].minimumPlayers === e[2].maximumPlayers ? kt : xt
+        return e[2].minimumPlayers && e[2].maximumPlayers && e[2].minimumPlayers === e[2].maximumPlayers ? Rt : kt
     }
     let I = b(e),
         w = I(e),
-        C = e[2].minimumPlayers !== e[2].maximumPlayers && Rt(e);
+        C = e[2].minimumPlayers !== e[2].maximumPlayers && Vt(e);
     return {
         c() {
-            t = N("div"), n = N("form"), i = N("h2"), a = W("Auto Assign"), r = J(), l = N("p"), o = W("Fill or create teams of up to "), w.c(), s = J(), c = W(y), u = J(), C && C.c(), A = J(), d = N("div"), f = N("button"), h = W("Assign "), m = W(E), p = W(" Players"), this.h()
+            t = N("div"), n = N("form"), i = N("h2"), a = W("Auto Assign"), r = J(), l = N("p"), o = W("Fill or create teams of up to "), w.c(), s = J(), c = W(y), u = J(), C && C.c(), d = J(), A = N("div"), f = N("button"), h = W("Assign "), m = W(E), p = W(" Players"), this.h()
         },
         l(e) {
             t = _(e, "DIV", {
                 class: !0
             });
             var g = G(t);
             n = _(g, "FORM", {});
             var v = G(n);
             i = _(v, "H2", {
                 class: !0
             });
             var b = G(i);
             a = ee(b, "Auto Assign"), b.forEach(D), r = te(v), l = _(v, "P", {});
             var I = G(l);
-            o = ee(I, "Fill or create teams of up to "), w.l(I), s = te(I), c = ee(I, y), u = te(I), C && C.l(I), I.forEach(D), A = te(v), d = _(v, "DIV", {
+            o = ee(I, "Fill or create teams of up to "), w.l(I), s = te(I), c = ee(I, y), u = te(I), C && C.l(I), I.forEach(D), d = te(v), A = _(v, "DIV", {
                 class: !0
             });
-            var B = G(d);
+            var B = G(A);
             f = _(B, "BUTTON", {
                 class: !0
             });
             var S = G(f);
             h = ee(S, "Assign "), m = ee(S, E), p = ee(S, " Players"), S.forEach(D), B.forEach(D), v.forEach(D), g.forEach(D), this.h()
         },
         h() {
-            Z(i, "class", "modal-heading"), Z(f, "class", "button"), Z(d, "class", "button-wrap align-center"), Z(t, "class", "text-center")
+            Z(i, "class", "modal-heading"), Z(f, "class", "button"), Z(A, "class", "button-wrap align-center"), Z(t, "class", "text-center")
         },
         m(y, E) {
-            T(y, t, E), z(t, n), z(n, i), z(i, a), z(n, r), z(n, l), z(l, o), w.m(l, null), z(l, s), z(l, c), z(l, u), C && C.m(l, null), z(n, A), z(n, d), z(d, f), z(f, h), z(f, m), z(f, p), g || (v = q(n, "submit", M(e[6])), g = !0)
+            T(y, t, E), z(t, n), z(n, i), z(i, a), z(n, r), z(n, l), z(l, o), w.m(l, null), z(l, s), z(l, c), z(l, u), C && C.m(l, null), z(n, d), z(n, A), z(A, f), z(f, h), z(f, m), z(f, p), g || (v = q(n, "submit", M(e[6])), g = !0)
         },
         p(e, t) {
-            I === (I = b(e)) && w ? w.p(e, t) : (w.d(1), w = I(e), w && (w.c(), w.m(l, s))), 8 & t && y !== (y = 1 == e[3] ? "player" : "players") && ne(c, y), e[2].minimumPlayers !== e[2].maximumPlayers ? C ? C.p(e, t) : (C = Rt(e), C.c(), C.m(l, null)) : C && (C.d(1), C = null), 2 & t && E !== (E = e[1].length + "") && ne(m, E)
+            I === (I = b(e)) && w ? w.p(e, t) : (w.d(1), w = I(e), w && (w.c(), w.m(l, s))), 8 & t && y !== (y = 1 == e[3] ? "player" : "players") && ne(c, y), e[2].minimumPlayers !== e[2].maximumPlayers ? C ? C.p(e, t) : (C = Vt(e), C.c(), C.m(l, null)) : C && (C.d(1), C = null), 2 & t && E !== (E = e[1].length + "") && ne(m, E)
         },
         d(e) {
             e && D(t), w.d(), C && C.d(), g = !1, v()
         }
     }
 }
 
-function Ut(e) {
+function zt(e) {
     let t, n, i;
 
     function a(t) {
         e[7](t)
     }
     let r = {
         $$slots: {
-            default: [Ft]
+            default: [Ut]
         },
         $$scope: {
             ctx: e
         }
     };
-    return void 0 !== e[0] && (r.open = e[0]), t = new Pt({
+    return void 0 !== e[0] && (r.open = e[0]), t = new xt({
         props: r
-    }), be.push((() => Ye(t, "open", a))), {
+    }), Ie.push((() => Ge(t, "open", a))), {
         c() {
-            Ge(t.$$.fragment)
+            $e(t.$$.fragment)
         },
         l(e) {
-            $e(t.$$.fragment, e)
+            _e(t.$$.fragment, e)
         },
         m(e, n) {
-            _e(t, e, n), i = !0
+            et(t, e, n), i = !0
         },
         p(e, [i]) {
             const a = {};
             527 & i && (a.$$scope = {
                 dirty: i,
                 ctx: e
-            }), !n && 1 & i && (n = !0, a.open = e[0], Le((() => n = !1))), t.$set(a)
+            }), !n && 1 & i && (n = !0, a.open = e[0], Pe((() => n = !1))), t.$set(a)
         },
         i(e) {
-            i || (De(t.$$.fragment, e), i = !0)
+            i || (He(t.$$.fragment, e), i = !0)
         },
         o(e) {
-            He(t.$$.fragment, e), i = !1
+            Ne(t.$$.fragment, e), i = !1
         },
         d(e) {
-            et(t, e)
+            tt(t, e)
         }
     }
 }
 
-function zt(e, t, n) {
+function Tt(e, t, n) {
     let i, a;
-    y(e, lt, (e => n(2, i = e)));
+    y(e, ot, (e => n(2, i = e)));
     let {
         open: r
     } = t, {
         unassigned: l
     } = t;
-    const o = ve();
+    const o = ye();
     return e.$$set = e => {
         "open" in e && n(0, r = e.open), "unassigned" in e && n(1, l = e.unassigned)
     }, e.$$.update = () => {
         var t, r;
         4 & e.$$.dirty && (t = i.minimumPlayers, r = i.maximumPlayers, n(3, a = t && r ? Math.floor((r + t) / 2) : t ? Math.max(t, 3) : r ? Math.min(r, 3) : 3))
     }, [r, l, i, a, o, function() {
         a = Y(this.value), n(3, a)
@@ -1501,24 +1505,24 @@
         o("submit", {
             fillCount: a
         }), n(0, r = !1)
     }, function(e) {
         r = e, n(0, r)
     }]
 }
-class Tt extends it {
+class Dt extends at {
     constructor(e) {
-        super(), nt(this, e, zt, Ut, p, {
+        super(), it(this, e, Tt, zt, p, {
             open: 0,
             unassigned: 1
         })
     }
 }
 
-function Dt(e) {
+function Ht(e) {
     let t, n, i;
     const a = e[1].default,
         r = E(a, e, e[0], null);
     return {
         c() {
             t = N("div"), n = N("ul"), r && r.c(), this.h()
         },
@@ -1540,41 +1544,41 @@
         m(e, a) {
             T(e, t, a), z(t, n), r && r.m(n, null), i = !0
         },
         p(e, [t]) {
             r && r.p && (!i || 1 & t) && w(r, a, e, e[0], i ? I(a, e[0], t, null) : C(e[0]), null)
         },
         i(e) {
-            i || (De(r, e), i = !0)
+            i || (He(r, e), i = !0)
         },
         o(e) {
-            He(r, e), i = !1
+            Ne(r, e), i = !1
         },
         d(e) {
             e && D(t), r && r.d(e)
         }
     }
 }
 
-function Ht(e, t, n) {
+function Nt(e, t, n) {
     let {
         $$slots: i = {},
         $$scope: a
     } = t;
     return e.$$set = e => {
         "$$scope" in e && n(0, a = e.$$scope)
     }, [a, i]
 }
-class Nt extends it {
+class Qt extends at {
     constructor(e) {
-        super(), nt(this, e, Ht, Dt, p, {})
+        super(), it(this, e, Nt, Ht, p, {})
     }
 }
 
-function Qt(e) {
+function Wt(e) {
     let t, n, i, a, r, l;
     const o = e[6].default,
         s = E(o, e, e[5], null);
     return {
         c() {
             t = N("li"), n = N("button"), s && s.c(), this.h()
         },
@@ -1597,26 +1601,26 @@
         m(i, o) {
             T(i, t, o), z(t, n), s && s.m(n, null), a = !0, r || (l = [S(e[4].call(null, n)), q(n, "click", e[7])], r = !0)
         },
         p(e, [t]) {
             s && s.p && (!a || 32 & t) && w(s, o, e, e[5], a ? I(o, e[5], t, null) : C(e[5]), null), (!a || 3 & t && i !== (i = e[0] === e[1])) && Z(n, "aria-selected", i), (!a || 4 & t) && Z(n, "data-notification-badge", e[2]), 12 & t && re(n, "outline", e[3] || e[2])
         },
         i(e) {
-            a || (De(s, e), a = !0)
+            a || (He(s, e), a = !0)
         },
         o(e) {
-            He(s, e), a = !1
+            Ne(s, e), a = !1
         },
         d(e) {
             e && D(t), s && s.d(e), r = !1, h(l)
         }
     }
 }
 
-function Wt(e, t, n) {
+function Jt(e, t, n) {
     let {
         $$slots: i = {},
         $$scope: a
     } = t, {
         state: r
     } = t, {
         value: l = null
@@ -1627,52 +1631,52 @@
     } = t;
     return e.$$set = e => {
         "state" in e && n(0, r = e.state), "value" in e && n(1, l = e.value), "badge" in e && n(2, o = e.badge), "outline" in e && n(3, s = e.outline), "$$scope" in e && n(5, a = e.$$scope)
     }, [r, l, o, s, e => {
         l || n(1, l = e.innerText)
     }, a, i, () => n(0, r = l)]
 }
-class Jt extends it {
+class jt extends at {
     constructor(e) {
-        super(), nt(this, e, Wt, Qt, p, {
+        super(), it(this, e, Jt, Wt, p, {
             state: 0,
             value: 1,
             badge: 2,
             outline: 3
         })
     }
 }
 
-function jt(e) {
+function qt(e) {
     const t = e - 1;
     return t * t * t + 1
 }
 
-function qt(e, t, n = {}) {
+function Mt(e, t, n = {}) {
     const i = getComputedStyle(e),
         a = "none" === i.transform ? "" : i.transform,
         r = t.from.width / e.clientWidth,
         l = t.from.height / e.clientHeight,
         o = (t.from.left - t.to.left) / r,
         s = (t.from.top - t.to.top) / l,
         c = Math.sqrt(o * o + s * s),
         {
             delay: u = 0,
-            duration: A = (e => 120 * Math.sqrt(e)),
-            easing: d = jt
+            duration: d = (e => 120 * Math.sqrt(e)),
+            easing: A = qt
         } = n;
     return {
         delay: u,
-        duration: m(A) ? A(c) : A,
-        easing: d,
+        duration: m(d) ? d(c) : d,
+        easing: A,
         css: (e, t) => `transform: ${a} translate(${t*o}px, ${t*s}px);`
     }
 }
 
-function Mt(e, t = 41, n = 24) {
+function Kt(e, t = 41, n = 24) {
     const i = function(e, t) {
         var n, i, a, r, l, o, s, c;
         for (n = 3 & e.length, i = e.length - n, a = t, l = 3432918353, o = 461845907, c = 0; c < i;) s = 255 & e.charCodeAt(c) | (255 & e.charCodeAt(++c)) << 8 | (255 & e.charCodeAt(++c)) << 16 | (255 & e.charCodeAt(++c)) << 24, ++c, a = 27492 + (65535 & (r = 5 * (65535 & (a = (a ^= s = (65535 & (s = (s = (65535 & s) * l + (((s >>> 16) * l & 65535) << 16) & 4294967295) << 15 | s >>> 17)) * o + (((s >>> 16) * o & 65535) << 16) & 4294967295) << 13 | a >>> 19)) + ((5 * (a >>> 16) & 65535) << 16) & 4294967295)) + ((58964 + (r >>> 16) & 65535) << 16);
         switch (s = 0, n) {
             case 3:
                 s ^= (255 & e.charCodeAt(c + 2)) << 16;
                 break;
@@ -1687,51 +1691,153 @@
     let a = i % 360,
         r = (i >>> 11) % 100,
         l = (i >>> 17) % 100;
     r = Math.floor(r / 100 * t + (100 - t) / 2), l = Math.floor(l / 100 * n + (100 - n) / 2.5);
     return `hsl(${a},${r}%,${l}%)`
 }
 
-function Kt(e, t, n) {
+function Zt(e) {
+    let t, n, i, a, r, l, o, s;
+    const c = e[6].default,
+        u = E(c, e, e[5], null);
+    return {
+        c() {
+            t = N("div"), n = N("a"), i = W(e[1]), a = J(), r = N("div"), u && u.c(), this.h()
+        },
+        l(l) {
+            t = _(l, "DIV", {
+                class: !0
+            });
+            var o = G(t);
+            n = _(o, "A", {
+                href: !0,
+                class: !0,
+                "aria-expanded": !0
+            });
+            var s = G(n);
+            i = ee(s, e[1]), s.forEach(D), a = te(o), r = _(o, "DIV", {
+                class: !0
+            });
+            var c = G(r);
+            u && u.l(c), c.forEach(D), o.forEach(D), this.h()
+        },
+        h() {
+            Z(n, "href", "#"), Z(n, "class", "button dropdown-button hollow small"), Z(n, "aria-expanded", e[0]), Z(r, "class", "dropdown"), Z(t, "class", "has-dropdown narrow-dropdown"), re(t, "is-expanded", e[0])
+        },
+        m(c, d) {
+            T(c, t, d), z(t, n), z(n, i), z(t, a), z(t, r), u && u.m(r, null), e[8](r), e[9](t), l = !0, o || (s = [q(n, "click", M(e[7])), q(n, "click", e[4])], o = !0)
+        },
+        p(e, [a]) {
+            (!l || 2 & a) && ne(i, e[1]), (!l || 1 & a) && Z(n, "aria-expanded", e[0]), u && u.p && (!l || 32 & a) && w(u, c, e, e[5], l ? I(c, e[5], a, null) : C(e[5]), null), 1 & a && re(t, "is-expanded", e[0])
+        },
+        i(e) {
+            l || (He(u, e), l = !0)
+        },
+        o(e) {
+            Ne(u, e), l = !1
+        },
+        d(n) {
+            n && D(t), u && u.d(n), e[8](null), e[9](null), o = !1, h(s)
+        }
+    }
+}
+
+function Yt(e, t, n) {
+    let i, a, {
+            $$slots: r = {},
+            $$scope: l
+        } = t,
+        {
+            placeholderText: o = "Select"
+        } = t,
+        {
+            expanded: s = !1
+        } = t;
+    const c = () => {
+            const e = e => {
+                i.contains(null == e ? void 0 : e.target) || d()
+            };
+            return document.addEventListener("click", e), {
+                destroy() {
+                    document.removeEventListener("click", e)
+                }
+            }
+        },
+        u = e => {
+            i.contains(e.relatedTarget) || d()
+        },
+        d = () => {
+            n(0, s = !1)
+        };
+    return ge((() => {
+        document.addEventListener("click", c), i.addEventListener("focusout", u)
+    })), ve((() => {
+        document.removeEventListener("click", c), i.removeEventListener("focusout", u)
+    })), e.$$set = e => {
+        "placeholderText" in e && n(1, o = e.placeholderText), "expanded" in e && n(0, s = e.expanded), "$$scope" in e && n(5, l = e.$$scope)
+    }, [s, o, i, a, () => {
+        n(0, s = !s)
+    }, l, r, function(t) {
+        Ee.call(this, e, t)
+    }, function(e) {
+        Ie[e ? "unshift" : "push"]((() => {
+            a = e, n(3, a)
+        }))
+    }, function(e) {
+        Ie[e ? "unshift" : "push"]((() => {
+            i = e, n(2, i)
+        }))
+    }]
+}
+class Gt extends at {
+    constructor(e) {
+        super(), it(this, e, Yt, Zt, p, {
+            placeholderText: 1,
+            expanded: 0
+        })
+    }
+}
+
+function $t(e, t, n) {
     const i = e.slice();
-    return i[18] = t[n], i
+    return i[17] = t[n], i
 }
 
-function Zt(e) {
+function _t(e) {
     var t;
-    let n, i, a = (null == (t = e[8](e[18].session)) ? void 0 : t.name) + "";
+    let n, i, a = (null == (t = e[8](e[17].session)) ? void 0 : t.name) + "";
     return {
         c() {
             n = N("small"), i = W(a)
         },
         l(e) {
             n = _(e, "SMALL", {});
             var t = G(n);
             i = ee(t, a), t.forEach(D)
         },
         m(e, t) {
             T(e, n, t), z(n, i)
         },
         p(e, t) {
             var n;
-            16 & t && a !== (a = (null == (n = e[8](e[18].session)) ? void 0 : n.name) + "") && ne(i, a)
+            16 & t && a !== (a = (null == (n = e[8](e[17].session)) ? void 0 : n.name) + "") && ne(i, a)
         },
         d(e) {
             e && D(n)
         }
     }
 }
 
-function Yt(e) {
-    let t, n, i, a, r, l, o = e[18].name + "",
-        s = e[8](e[18].session),
-        c = s && Zt(e);
+function en(e) {
+    let t, n, i, a, r, l, o = e[17].name + "",
+        s = e[8](e[17].session),
+        c = s && _t(e);
 
     function u() {
-        return e[11](e[18])
+        return e[10](e[17])
     }
     return {
         c() {
             t = N("li"), n = N("a"), i = W(o), a = J(), c && c.c(), this.h()
         },
         l(e) {
             t = _(e, "LI", {
@@ -1748,23 +1854,23 @@
         h() {
             Z(n, "class", "dropdown-link"), Z(n, "href", "."), Z(t, "class", "dropdown-item")
         },
         m(e, o) {
             T(e, t, o), z(t, n), z(n, i), z(n, a), c && c.m(n, null), r || (l = q(n, "click", K(M(u))), r = !0)
         },
         p(t, a) {
-            e = t, 16 & a && o !== (o = e[18].name + "") && ne(i, o), 16 & a && (s = e[8](e[18].session)), s ? c ? c.p(e, a) : (c = Zt(e), c.c(), c.m(n, null)) : c && (c.d(1), c = null)
+            e = t, 16 & a && o !== (o = e[17].name + "") && ne(i, o), 16 & a && (s = e[8](e[17].session)), s ? c ? c.p(e, a) : (c = _t(e), c.c(), c.m(n, null)) : c && (c.d(1), c = null)
         },
         d(e) {
             e && D(t), c && c.d(), r = !1, l()
         }
     }
 }
 
-function Gt(e) {
+function tn(e) {
     let t, n, i, a, r, l, o;
     return {
         c() {
             t = N("li"), n = N("a"), i = Q("svg"), a = Q("path"), r = W("\n              Mark inactive"), this.h()
         },
         l(e) {
             t = _(e, "LI", {
@@ -1788,24 +1894,24 @@
                 stroke: !0
             }, 1), G(a).forEach(D), s.forEach(D), r = ee(o, "\n              Mark inactive"), o.forEach(D), l.forEach(D), this.h()
         },
         h() {
             Z(a, "d", "M4.91 9.541h3.272c1.164 0 2.283.48 3.111 1.337a4.68 4.68 0 0 1 1.298 3.25v1.13c0 .023-.01.042-.02.052a.037.037 0 0 1-.025.012h-12a.037.037 0 0 1-.027-.012.076.076 0 0 1-.019-.053v-1.13a4.68 4.68 0 0 1 1.298-3.249 4.324 4.324 0 0 1 3.111-1.337ZM3.226 3.956c0-.922.354-1.804.978-2.45A3.253 3.253 0 0 1 6.545.5c.875 0 1.717.36 2.34 1.006a3.53 3.53 0 0 1 .979 2.45 3.53 3.53 0 0 1-.978 2.45 3.253 3.253 0 0 1-2.34 1.005c-.875 0-1.717-.36-2.34-1.005a3.53 3.53 0 0 1-.979-2.45Z"), Z(a, "stroke", "currentColor"), Z(i, "class", "icon theme-alert-color"), Z(i, "viewBox", "0 0 14 16"), Z(i, "fill", "none"), Z(i, "xmlns", "http://www.w3.org/2000/svg"), Z(n, "class", "dropdown-link"), Z(n, "href", "."), Z(t, "class", "dropdown-item")
         },
         m(s, c) {
-            T(s, t, c), z(t, n), z(n, i), z(i, a), z(n, r), l || (o = q(n, "click", K(M(e[14]))), l = !0)
+            T(s, t, c), z(t, n), z(n, i), z(i, a), z(n, r), l || (o = q(n, "click", K(M(e[13]))), l = !0)
         },
         p: c,
         d(e) {
             e && D(t), l = !1, o()
         }
     }
 }
 
-function $t(e) {
+function nn(e) {
     let t, n, i, a, r;
     return {
         c() {
             t = N("li"), n = N("a"), i = W("Mark active"), this.h()
         },
         l(e) {
             t = _(e, "LI", {
@@ -1819,24 +1925,24 @@
             var r = G(n);
             i = ee(r, "Mark active"), r.forEach(D), a.forEach(D), this.h()
         },
         h() {
             Z(n, "class", "dropdown-link"), Z(n, "href", "."), Z(t, "class", "dropdown-item")
         },
         m(l, o) {
-            T(l, t, o), z(t, n), z(n, i), a || (r = q(n, "click", K(M(e[13]))), a = !0)
+            T(l, t, o), z(t, n), z(n, i), a || (r = q(n, "click", K(M(e[12]))), a = !0)
         },
         p: c,
         d(e) {
             e && D(t), a = !1, r()
         }
     }
 }
 
-function _t(e) {
+function an(e) {
     let t, n, i, a, r, l, o;
     return {
         c() {
             t = N("li"), n = N("a"), i = Q("svg"), a = Q("path"), r = W("\n              Unassign"), this.h()
         },
         l(e) {
             t = _(e, "LI", {
@@ -1860,203 +1966,230 @@
                 fill: !0
             }, 1), G(a).forEach(D), s.forEach(D), r = ee(o, "\n              Unassign"), o.forEach(D), l.forEach(D), this.h()
         },
         h() {
             Z(a, "d", "M4.91 9.541h3.272c1.164 0 2.283.48 3.111 1.337a4.68 4.68 0 0 1 1.298 3.25v1.13c0 .023-.01.042-.02.052a.037.037 0 0 1-.025.012h-12a.037.037 0 0 1-.027-.012.076.076 0 0 1-.019-.053v-1.13a4.68 4.68 0 0 1 1.298-3.249 4.324 4.324 0 0 1 3.111-1.337ZM3.226 3.956c0-.922.354-1.804.978-2.45A3.253 3.253 0 0 1 6.545.5c.875 0 1.717.36 2.34 1.006a3.53 3.53 0 0 1 .979 2.45 3.53 3.53 0 0 1-.978 2.45 3.253 3.253 0 0 1-2.34 1.005c-.875 0-1.717-.36-2.34-1.005a3.53 3.53 0 0 1-.979-2.45Z"), Z(a, "fill", "currentColor"), Z(i, "class", "icon theme-info-color"), Z(i, "viewBox", "0 0 14 16"), Z(i, "fill", "none"), Z(i, "xmlns", "http://www.w3.org/2000/svg"), Z(n, "class", "dropdown-link"), Z(n, "href", "."), Z(t, "class", "dropdown-item")
         },
         m(s, c) {
-            T(s, t, c), z(t, n), z(n, i), z(i, a), z(n, r), l || (o = q(n, "click", K(M(e[15]))), l = !0)
+            T(s, t, c), z(t, n), z(n, i), z(i, a), z(n, r), l || (o = q(n, "click", K(M(e[14]))), l = !0)
         },
         p: c,
         d(e) {
             e && D(t), l = !1, o()
         }
     }
 }
 
-function en(e) {
-    let t, n, i, a, r, l, o, s, u, A, d, f, m, p, g, v, y, E, b, I, w, C, B, S, L, P, x, k, R, V, X = e[0].name + "",
-        O = e[4],
-        F = [];
-    for (let c = 0; c < O.length; c += 1) F[c] = Yt(Kt(e, O, c));
+function rn(e) {
+    let t, n, i, a, r, l, o, s, c, u, d, A, f, h, m = e[4],
+        p = [];
+    for (let b = 0; b < m.length; b += 1) p[b] = en($t(e, m, b));
 
-    function U(e, t) {
-        return e[0].inactive ? $t : Gt
+    function g(e, t) {
+        return e[0].inactive ? nn : tn
     }
-    let j = U(e),
-        Y = j(e),
-        $ = e[3] && _t(e);
+    let v = g(e),
+        y = v(e),
+        E = e[3] && an(e);
     return {
         c() {
-            t = N("div"), n = N("div"), i = N("div"), a = N("div"), r = W(e[7]), l = J(), o = N("p"), s = W(X), u = J(), A = N("div"), d = N("a"), f = W("Assign to…"), m = J(), p = N("div"), g = N("ul");
-            for (let e = 0; e < F.length; e += 1) F[e].c();
-            v = J(), y = N("li"), E = N("a"), b = Q("svg"), I = Q("g"), w = Q("path"), C = Q("path"), B = Q("path"), S = W("\n            New Team"), L = J(), Y.c(), P = J(), $ && $.c(), x = J(), k = N("input"), this.h()
+            t = N("ul");
+            for (let e = 0; e < p.length; e += 1) p[e].c();
+            n = J(), i = N("li"), a = N("a"), r = Q("svg"), l = Q("g"), o = Q("path"), s = Q("path"), c = Q("path"), u = W("\n            New Team"), d = J(), y.c(), A = J(), E && E.c(), this.h()
         },
-        l(c) {
-            t = _(c, "DIV", {
-                class: !0,
-                "aria-readonly": !0
-            });
-            var h = G(t);
-            n = _(h, "DIV", {
-                class: !0
-            });
-            var R = G(n);
-            i = _(R, "DIV", {
-                class: !0,
-                style: !0
-            });
-            var V = G(i);
-            a = _(V, "DIV", {
-                class: !0
-            });
-            var O = G(a);
-            r = ee(O, e[7]), O.forEach(D), V.forEach(D), l = te(R), o = _(R, "P", {
-                class: !0
-            });
-            var U = G(o);
-            s = ee(U, X), U.forEach(D), R.forEach(D), u = te(h), A = _(h, "DIV", {
-                class: !0
-            });
-            var z = G(A);
-            d = _(z, "A", {
-                href: !0,
-                class: !0
-            });
-            var T = G(d);
-            f = ee(T, "Assign to…"), T.forEach(D), m = te(z), p = _(z, "DIV", {
-                class: !0
-            });
-            var H = G(p);
-            g = _(H, "UL", {
+        l(e) {
+            t = _(e, "UL", {
                 class: !0
             });
-            var N = G(g);
-            for (let e = 0; e < F.length; e += 1) F[e].l(N);
-            v = te(N), y = _(N, "LI", {
+            var f = G(t);
+            for (let t = 0; t < p.length; t += 1) p[t].l(f);
+            n = te(f), i = _(f, "LI", {
                 class: !0
             });
-            var Q = G(y);
-            E = _(Q, "A", {
+            var h = G(i);
+            a = _(h, "A", {
                 class: !0,
                 href: !0
             });
-            var W = G(E);
-            b = _(W, "svg", {
+            var m = G(a);
+            r = _(m, "svg", {
                 class: !0,
                 viewBox: !0,
                 id: !0,
                 xmlns: !0
             }, 1);
-            var J = G(b);
-            I = _(J, "g", {
+            var g = G(r);
+            l = _(g, "g", {
                 fill: !0
             }, 1);
-            var j = G(I);
-            w = _(j, "path", {
+            var v = G(l);
+            o = _(v, "path", {
                 d: !0
-            }, 1), G(w).forEach(D), C = _(j, "path", {
+            }, 1), G(o).forEach(D), s = _(v, "path", {
                 d: !0
-            }, 1), G(C).forEach(D), B = _(j, "path", {
+            }, 1), G(s).forEach(D), c = _(v, "path", {
                 d: !0
-            }, 1), G(B).forEach(D), j.forEach(D), J.forEach(D), S = ee(W, "\n            New Team"), W.forEach(D), Q.forEach(D), L = te(N), Y.l(N), P = te(N), $ && $.l(N), N.forEach(D), H.forEach(D), z.forEach(D), x = te(h), k = _(h, "INPUT", {
+            }, 1), G(c).forEach(D), v.forEach(D), g.forEach(D), u = ee(m, "\n            New Team"), m.forEach(D), h.forEach(D), d = te(f), y.l(f), A = te(f), E && E.l(f), f.forEach(D), this.h()
+        },
+        h() {
+            Z(o, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), Z(s, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), Z(c, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), Z(l, "fill", "currentColor"), Z(r, "class", "icon theme-info-color"), Z(r, "viewBox", "0 0 17.928 22.481"), Z(r, "id", "people"), Z(r, "xmlns", "http://www.w3.org/2000/svg"), Z(a, "class", "dropdown-link is-new"), Z(a, "href", "."), Z(i, "class", "dropdown-item"), Z(t, "class", "dropdown-list")
+        },
+        m(m, g) {
+            T(m, t, g);
+            for (let e = 0; e < p.length; e += 1) p[e].m(t, null);
+            z(t, n), z(t, i), z(i, a), z(a, r), z(r, l), z(l, o), z(l, s), z(l, c), z(a, u), z(t, d), y.m(t, null), z(t, A), E && E.m(t, null), f || (h = q(a, "click", K(M(e[11]))), f = !0)
+        },
+        p(e, i) {
+            if (337 & i) {
+                let a;
+                for (m = e[4], a = 0; a < m.length; a += 1) {
+                    const r = $t(e, m, a);
+                    p[a] ? p[a].p(r, i) : (p[a] = en(r), p[a].c(), p[a].m(t, n))
+                }
+                for (; a < p.length; a += 1) p[a].d(1);
+                p.length = m.length
+            }
+            v === (v = g(e)) && y ? y.p(e, i) : (y.d(1), y = v(e), y && (y.c(), y.m(t, A))), e[3] ? E ? E.p(e, i) : (E = an(e), E.c(), E.m(t, null)) : E && (E.d(1), E = null)
+        },
+        d(e) {
+            e && D(t), H(p, e), y.d(), E && E.d(), f = !1, h()
+        }
+    }
+}
+
+function ln(e) {
+    let t, n, i, a, r, l, o, s, c, u, d, A, f, h, m, p = e[0].name + "";
+    return u = new Gt({
+        props: {
+            placeholderText: "Assign to…",
+            $$slots: {
+                default: [rn]
+            },
+            $$scope: {
+                ctx: e
+            }
+        }
+    }), {
+        c() {
+            t = N("div"), n = N("div"), i = N("div"), a = N("div"), r = W(e[7]), l = J(), o = N("p"), s = W(p), c = J(), $e(u.$$.fragment), d = J(), A = N("input"), this.h()
+        },
+        l(f) {
+            t = _(f, "DIV", {
+                class: !0,
+                "aria-readonly": !0
+            });
+            var h = G(t);
+            n = _(h, "DIV", {
+                class: !0
+            });
+            var m = G(n);
+            i = _(m, "DIV", {
+                class: !0,
+                style: !0
+            });
+            var g = G(i);
+            a = _(g, "DIV", {
+                class: !0
+            });
+            var v = G(a);
+            r = ee(v, e[7]), v.forEach(D), g.forEach(D), l = te(m), o = _(m, "P", {
+                class: !0
+            });
+            var y = G(o);
+            s = ee(y, p), y.forEach(D), m.forEach(D), c = te(h), _e(u.$$.fragment, h), d = te(h), A = _(h, "INPUT", {
                 class: !0,
                 type: !0
             }), h.forEach(D), this.h()
         },
         h() {
-            Z(a, "class", "avatar-inner"), Z(i, "class", "avatar"), ae(i, "background", Mt(e[0].name)), Z(o, "class", "avatar-detail-meta"), Z(n, "class", "avatar-detail"), Z(d, "href", "."), Z(d, "class", "button dropdown-button hollow small"), Z(w, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), Z(C, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), Z(B, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), Z(I, "fill", "currentColor"), Z(b, "class", "icon theme-info-color"), Z(b, "viewBox", "0 0 17.928 22.481"), Z(b, "id", "people"), Z(b, "xmlns", "http://www.w3.org/2000/svg"), Z(E, "class", "dropdown-link is-new"), Z(E, "href", "."), Z(y, "class", "dropdown-item"), Z(g, "class", "dropdown-list"), Z(p, "class", "dropdown"), Z(A, "class", "has-dropdown narrow-dropdown"), Z(k, "class", "show-for-sr-only svelte-hxuor6"), Z(k, "type", "checkbox"), k.checked = e[1], Z(t, "class", "player-item svelte-hxuor6"), Z(t, "aria-readonly", e[2]), re(t, "is-selected", e[1])
+            Z(a, "class", "avatar-inner"), Z(i, "class", "avatar"), ae(i, "background", Kt(e[0].name)), Z(o, "class", "avatar-detail-meta"), Z(n, "class", "avatar-detail"), Z(A, "class", "show-for-sr-only svelte-hxuor6"), Z(A, "type", "checkbox"), A.checked = e[1], Z(t, "class", "player-item svelte-hxuor6"), Z(t, "aria-readonly", e[2]), re(t, "is-selected", e[1])
         },
-        m(c, h) {
-            T(c, t, h), z(t, n), z(n, i), z(i, a), z(a, r), z(n, l), z(n, o), z(o, s), z(t, u), z(t, A), z(A, d), z(d, f), z(A, m), z(A, p), z(p, g);
-            for (let e = 0; e < F.length; e += 1) F[e].m(g, null);
-            z(g, v), z(g, y), z(y, E), z(E, b), z(b, I), z(I, w), z(I, C), z(I, B), z(E, S), z(g, L), Y.m(g, null), z(g, P), $ && $.m(g, null), z(t, x), z(t, k), R || (V = [q(d, "click", K(M(e[10]))), q(E, "click", K(M(e[12]))), q(t, "click", e[16])], R = !0)
+        m(p, g) {
+            T(p, t, g), z(t, n), z(n, i), z(i, a), z(a, r), z(n, l), z(n, o), z(o, s), z(t, c), et(u, t, null), z(t, d), z(t, A), f = !0, h || (m = q(t, "click", e[15]), h = !0)
         },
         p(e, [n]) {
-            if (1 & n && ae(i, "background", Mt(e[0].name)), 1 & n && X !== (X = e[0].name + "") && ne(s, X), 337 & n) {
-                let t;
-                for (O = e[4], t = 0; t < O.length; t += 1) {
-                    const i = Kt(e, O, t);
-                    F[t] ? F[t].p(i, n) : (F[t] = Yt(i), F[t].c(), F[t].m(g, v))
-                }
-                for (; t < F.length; t += 1) F[t].d(1);
-                F.length = O.length
-            }
-            j === (j = U(e)) && Y ? Y.p(e, n) : (Y.d(1), Y = j(e), Y && (Y.c(), Y.m(g, P))), e[3] ? $ ? $.p(e, n) : ($ = _t(e), $.c(), $.m(g, null)) : $ && ($.d(1), $ = null), 2 & n && (k.checked = e[1]), 4 & n && Z(t, "aria-readonly", e[2]), 2 & n && re(t, "is-selected", e[1])
+            (!f || 1 & n) && ae(i, "background", Kt(e[0].name)), (!f || 1 & n) && p !== (p = e[0].name + "") && ne(s, p);
+            const a = {};
+            1048635 & n && (a.$$scope = {
+                dirty: n,
+                ctx: e
+            }), u.$set(a), (!f || 2 & n) && (A.checked = e[1]), (!f || 4 & n) && Z(t, "aria-readonly", e[2]), 2 & n && re(t, "is-selected", e[1])
+        },
+        i(e) {
+            f || (He(u.$$.fragment, e), f = !0)
+        },
+        o(e) {
+            Ne(u.$$.fragment, e), f = !1
         },
-        i: c,
-        o: c,
         d(e) {
-            e && D(t), H(F, e), Y.d(), $ && $.d(), R = !1, h(V)
+            e && D(t), tt(u), h = !1, m()
         }
     }
 }
 
-function tn(e, t, n) {
+function on(e, t, n) {
     let i;
-    y(e, lt, (e => n(5, i = e)));
+    y(e, ot, (e => n(5, i = e)));
     let {
         isSelected: a = !1
     } = t, {
         player: r
     } = t, {
         currentTeam: l = null
     } = t, {
         readOnly: o = !1
     } = t, {
         assigned: s = !1
     } = t;
-    const c = ve(),
+    const c = ye(),
         u = r.name.replace(/(\w)[^ ]+/g, "$1").replace(/[^\w]/g, "");
-    var A = u[0] + u[u.length - 1];
-    let d;
+    var d = u[0] + u[u.length - 1];
+    let A;
     return e.$$set = e => {
         "isSelected" in e && n(1, a = e.isSelected), "player" in e && n(0, r = e.player), "currentTeam" in e && n(9, l = e.currentTeam), "readOnly" in e && n(2, o = e.readOnly), "assigned" in e && n(3, s = e.assigned)
     }, e.$$.update = () => {
-        561 & e.$$.dirty && (n(4, d = i.teams), r.session && i.sessions.find((e => e.id === r.session)) && n(4, d = d.filter((e => e.session === r.session))), l && n(4, d = d.filter((e => e !== l))))
-    }, [r, a, o, s, d, i, c, A, e => e ? i.sessions.length <= 1 ? null : i.sessions.find((t => t.id === e)) : null, l, function(t) {
-        ye.call(this, e, t)
-    }, e => {
+        561 & e.$$.dirty && (n(4, A = i.teams), r.session && i.sessions.find((e => e.id === r.session)) && n(4, A = A.filter((e => e.session === r.session))), l && n(4, A = A.filter((e => e !== l))))
+    }, [r, a, o, s, A, i, c, d, e => e ? i.sessions.length <= 1 ? null : i.sessions.find((t => t.id === e)) : null, l, e => {
         c("addPlayers", {
             team: e,
             adding: [r.id]
         })
     }, () => {
         c("addPlayers", {
             team: null,
             adding: [r.id],
             session: r.session
         })
     }, () => {
-        st.notify({
+        ct.notify({
             playerId: r.id,
             active: !0
-        }), n(0, r.inactive = !1, r), lt.set(i)
+        }), n(0, r.inactive = !1, r), ot.set(i)
     }, () => {
-        st.notify({
+        ct.notify({
             playerId: r.id,
             active: !1
         }), a && c("selectPlayer", {
             id: r.id
         }), s && c("unassignPlayer", {
             id: r.id
-        }), n(0, r.inactive = !0, r), lt.set(i)
+        }), n(0, r.inactive = !0, r), ot.set(i)
     }, () => {
         c("unassignPlayer", {
             id: r.id
         })
     }, () => {
         o || c("selectPlayer", {
             id: r.id
         })
     }]
 }
-class nn extends it {
+class sn extends at {
     constructor(e) {
-        super(), nt(this, e, tn, en, p, {
+        super(), it(this, e, on, ln, p, {
             isSelected: 1,
             player: 0,
             currentTeam: 9,
             readOnly: 2,
             assigned: 3
         })
     }
@@ -2071,50 +2204,50 @@
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
 AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
 INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
 LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
 OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
 PERFORMANCE OF THIS SOFTWARE.
 ***************************************************************************** */
-function an(e, {
+function cn(e, {
     delay: t = 0,
     duration: n = 400,
     easing: i = u
 } = {}) {
     const a = +getComputedStyle(e).opacity;
     return {
         delay: t,
         duration: n,
         easing: i,
         css: e => "opacity: " + e * a
     }
 }
 
-function rn(e, {
+function un(e, {
     delay: t = 0,
     duration: n = 400,
-    easing: i = jt
+    easing: i = qt
 } = {}) {
     const a = getComputedStyle(e),
         r = +a.opacity,
         l = parseFloat(a.height),
         o = parseFloat(a.paddingTop),
         s = parseFloat(a.paddingBottom),
         c = parseFloat(a.marginTop),
         u = parseFloat(a.marginBottom),
-        A = parseFloat(a.borderTopWidth),
-        d = parseFloat(a.borderBottomWidth);
+        d = parseFloat(a.borderTopWidth),
+        A = parseFloat(a.borderBottomWidth);
     return {
         delay: t,
         duration: n,
         easing: i,
-        css: e => `overflow: hidden;opacity: ${Math.min(20*e,1)*r};height: ${e*l}px;padding-top: ${e*o}px;padding-bottom: ${e*s}px;margin-top: ${e*c}px;margin-bottom: ${e*u}px;border-top-width: ${e*A}px;border-bottom-width: ${e*d}px;`
+        css: e => `overflow: hidden;opacity: ${Math.min(20*e,1)*r};height: ${e*l}px;padding-top: ${e*o}px;padding-bottom: ${e*s}px;margin-top: ${e*c}px;margin-bottom: ${e*u}px;border-top-width: ${e*d}px;border-bottom-width: ${e*A}px;`
     }
 }
-const [ln, on] = function(e) {
+const [dn, An] = function(e) {
     var {
         fallback: t
     } = e, n = function(e, t) {
         var n = {};
         for (var i in e) Object.prototype.hasOwnProperty.call(e, i) && t.indexOf(i) < 0 && (n[i] = e[i]);
         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
             var a = 0;
@@ -2134,21 +2267,21 @@
                     rect: e
                 } = i.get(l.key);
                 return i.delete(l.key),
                     function(e, t, i) {
                         const {
                             delay: a = 0,
                             duration: r = (e => 30 * Math.sqrt(e)),
-                            easing: l = jt
-                        } = A(A({}, n), i), o = t.getBoundingClientRect(), s = e.left - o.left, c = e.top - o.top, u = e.width / o.width, d = e.height / o.height, f = Math.sqrt(s * s + c * c), h = getComputedStyle(t), p = "none" === h.transform ? "" : h.transform, g = +h.opacity;
+                            easing: l = qt
+                        } = d(d({}, n), i), o = t.getBoundingClientRect(), s = e.left - o.left, c = e.top - o.top, u = e.width / o.width, A = e.height / o.height, f = Math.sqrt(s * s + c * c), h = getComputedStyle(t), p = "none" === h.transform ? "" : h.transform, g = +h.opacity;
                         return {
                             delay: a,
                             duration: m(r) ? r(f) : r,
                             easing: l,
-                            css: (e, t) => `\n\t\t\t\topacity: ${e*g};\n\t\t\t\ttransform-origin: top left;\n\t\t\t\ttransform: ${p} translate(${t*s}px,${t*c}px) scale(${e+(1-e)*u}, ${e+(1-e)*d});\n\t\t\t`
+                            css: (e, t) => `\n\t\t\t\topacity: ${e*g};\n\t\t\t\ttransform-origin: top left;\n\t\t\t\ttransform: ${p} translate(${t*s}px,${t*c}px) scale(${e+(1-e)*u}, ${e+(1-e)*A});\n\t\t\t`
                         }
                     }(e, r, l)
             }
             return e.delete(l.key), t && t(r, l, a)
         })
     }
     return [r(a, i, !1), r(i, a, !0)]
@@ -2160,20 +2293,20 @@
         return {
             duration: 600,
             css: e => `\n        transform: ${n} scale(${e});\n        opacity: ${e}\n      `
         }
     }
 });
 
-function sn(e, t, n) {
+function fn(e, t, n) {
     const i = e.slice();
     return i[6] = t[n], i
 }
 
-function cn(e) {
+function hn(e) {
     let t;
     return {
         c() {
             t = W("Inactive Players")
         },
         l(e) {
             t = ee(e, "Inactive Players")
@@ -2183,15 +2316,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function un(e) {
+function mn(e) {
     let t;
     return {
         c() {
             t = W("Unassigned Players")
         },
         l(e) {
             t = ee(e, "Unassigned Players")
@@ -2201,15 +2334,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function An(e) {
+function pn(e) {
     let t, n, i, a, r, l;
     return {
         c() {
             t = N("span"), n = Q("svg"), i = Q("path"), a = J(), r = N("div"), l = W("Inactive players will not be able to participate or follow along once the game is set to play."), this.h()
         },
         l(e) {
             t = _(e, "SPAN", {
@@ -2242,92 +2375,92 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function dn(e, t) {
+function gn(e, t) {
     let n, i, a, r, l, o, s, u = c;
-    return i = new nn({
+    return i = new sn({
         props: {
             isSelected: t[0].includes(t[6].id),
             player: t[6]
         }
     }), i.$on("selectPlayer", t[4]), i.$on("addPlayers", t[5]), {
         key: e,
         first: null,
         c() {
-            n = N("div"), Ge(i.$$.fragment), a = J(), this.h()
+            n = N("div"), $e(i.$$.fragment), a = J(), this.h()
         },
         l(e) {
             n = _(e, "DIV", {});
             var t = G(n);
-            $e(i.$$.fragment, t), a = te(t), t.forEach(D), this.h()
+            _e(i.$$.fragment, t), a = te(t), t.forEach(D), this.h()
         },
         h() {
             this.first = n
         },
         m(e, t) {
-            T(e, n, t), _e(i, n, null), z(n, a), s = !0
+            T(e, n, t), et(i, n, null), z(n, a), s = !0
         },
         p(e, n) {
             t = e;
             const a = {};
             3 & n && (a.isSelected = t[0].includes(t[6].id)), 2 & n && (a.player = t[6]), i.$set(a)
         },
         r() {
             o = n.getBoundingClientRect()
         },
         f() {
             fe(n), u(), he(n, o)
         },
         a() {
-            u(), u = de(n, o, qt, {})
+            u(), u = Ae(n, o, Mt, {})
         },
         i(e) {
-            s || (De(i.$$.fragment, e), e && Se((() => {
-                l && l.end(1), r = Qe(n, on, {
+            s || (He(i.$$.fragment, e), e && Le((() => {
+                l && l.end(1), r = We(n, An, {
                     key: t[6].id
                 }), r.start()
             })), s = !0)
         },
         o(e) {
-            He(i.$$.fragment, e), r && r.invalidate(), e && (l = We(n, ln, {
+            Ne(i.$$.fragment, e), r && r.invalidate(), e && (l = Je(n, dn, {
                 key: t[6].id
             })), s = !1
         },
         d(e) {
-            e && D(n), et(i), e && l && l.end()
+            e && D(n), tt(i), e && l && l.end()
         }
     }
 }
 
-function fn(e) {
+function vn(e) {
     let t, n, i, a, r, l, o, s, c, u = e[1].length + "",
-        A = [],
-        d = new Map;
+        d = [],
+        A = new Map;
 
     function f(e, t) {
-        return e[3] ? cn : un
+        return e[3] ? hn : mn
     }
     let h = f(e),
         m = h(e),
-        p = e[3] && An(),
+        p = e[3] && pn(),
         g = e[1];
     const v = e => e[6].id;
     for (let y = 0; y < g.length; y += 1) {
-        let t = sn(e, g, y),
+        let t = fn(e, g, y),
             n = v(t);
-        d.set(n, A[y] = dn(n, t))
+        A.set(n, d[y] = gn(n, t))
     }
     return {
         c() {
             t = N("div"), n = N("p"), m.c(), i = W("\n    ("), a = W(u), r = W(")\n    "), p && p.c(), o = J(), s = N("div");
-            for (let e = 0; e < A.length; e += 1) A[e].c();
+            for (let e = 0; e < d.length; e += 1) d[e].c();
             this.h()
         },
         l(e) {
             t = _(e, "DIV", {
                 class: !0
             });
             var l = G(t);
@@ -2337,88 +2470,88 @@
             });
             var c = G(n);
             m.l(c), i = ee(c, "\n    ("), a = ee(c, u), r = ee(c, ")\n    "), p && p.l(c), c.forEach(D), l.forEach(D), o = te(e), s = _(e, "DIV", {
                 class: !0,
                 role: !0,
                 "aria-labelledby": !0
             });
-            var d = G(s);
-            for (let t = 0; t < A.length; t += 1) A[t].l(d);
-            d.forEach(D), this.h()
+            var A = G(s);
+            for (let t = 0; t < d.length; t += 1) d[t].l(A);
+            A.forEach(D), this.h()
         },
         h() {
             Z(n, "class", "walkthrough-chapter-heading"), Z(n, "id", l = e[3] ? "inactive-players" : "unassigned-players"), re(n, "note", !e[3] && e[1].length && e[2]), re(n, "theme-alert-color", !e[3] && e[1].length && e[2]), Z(t, "class", "player-header"), re(t, "pad-top", e[3]), Z(s, "class", "card player-card tab-pane"), Z(s, "role", "tabpanel"), Z(s, "aria-labelledby", "tabby-toggle_active"), re(s, "glow-shadow", !e[3]), re(s, "is-inactive-player", e[3])
         },
         m(e, l) {
             T(e, t, l), z(t, n), m.m(n, null), z(n, i), z(n, a), z(n, r), p && p.m(n, null), T(e, o, l), T(e, s, l);
-            for (let t = 0; t < A.length; t += 1) A[t].m(s, null);
+            for (let t = 0; t < d.length; t += 1) d[t].m(s, null);
             c = !0
         },
         p(e, [r]) {
-            if (h !== (h = f(e)) && (m.d(1), m = h(e), m && (m.c(), m.m(n, i))), (!c || 2 & r) && u !== (u = e[1].length + "") && ne(a, u), e[3] ? p || (p = An(), p.c(), p.m(n, null)) : p && (p.d(1), p = null), (!c || 8 & r && l !== (l = e[3] ? "inactive-players" : "unassigned-players")) && Z(n, "id", l), 14 & r && re(n, "note", !e[3] && e[1].length && e[2]), 14 & r && re(n, "theme-alert-color", !e[3] && e[1].length && e[2]), 8 & r && re(t, "pad-top", e[3]), 3 & r) {
-                g = e[1], ze();
-                for (let e = 0; e < A.length; e += 1) A[e].r();
-                A = Ze(A, r, v, 1, e, g, d, s, Ke, dn, null, sn);
-                for (let e = 0; e < A.length; e += 1) A[e].a();
-                Te()
+            if (h !== (h = f(e)) && (m.d(1), m = h(e), m && (m.c(), m.m(n, i))), (!c || 2 & r) && u !== (u = e[1].length + "") && ne(a, u), e[3] ? p || (p = pn(), p.c(), p.m(n, null)) : p && (p.d(1), p = null), (!c || 8 & r && l !== (l = e[3] ? "inactive-players" : "unassigned-players")) && Z(n, "id", l), 14 & r && re(n, "note", !e[3] && e[1].length && e[2]), 14 & r && re(n, "theme-alert-color", !e[3] && e[1].length && e[2]), 8 & r && re(t, "pad-top", e[3]), 3 & r) {
+                g = e[1], Te();
+                for (let e = 0; e < d.length; e += 1) d[e].r();
+                d = Ye(d, r, v, 1, e, g, A, s, Ze, gn, null, fn);
+                for (let e = 0; e < d.length; e += 1) d[e].a();
+                De()
             }
             8 & r && re(s, "glow-shadow", !e[3]), 8 & r && re(s, "is-inactive-player", e[3])
         },
         i(e) {
             if (!c) {
-                for (let e = 0; e < g.length; e += 1) De(A[e]);
+                for (let e = 0; e < g.length; e += 1) He(d[e]);
                 c = !0
             }
         },
         o(e) {
-            for (let t = 0; t < A.length; t += 1) He(A[t]);
+            for (let t = 0; t < d.length; t += 1) Ne(d[t]);
             c = !1
         },
         d(e) {
             e && D(t), m.d(), p && p.d(), e && D(o), e && D(s);
-            for (let t = 0; t < A.length; t += 1) A[t].d()
+            for (let t = 0; t < d.length; t += 1) d[t].d()
         }
     }
 }
 
-function hn(e, t, n) {
+function yn(e, t, n) {
     let {
         selected: i
     } = t, {
         players: a
     } = t, {
         unassignedIsError: r = !1
     } = t, {
         inactive: l = !1
     } = t;
     return e.$$set = e => {
         "selected" in e && n(0, i = e.selected), "players" in e && n(1, a = e.players), "unassignedIsError" in e && n(2, r = e.unassignedIsError), "inactive" in e && n(3, l = e.inactive)
     }, [i, a, r, l, function(t) {
-        ye.call(this, e, t)
+        Ee.call(this, e, t)
     }, function(t) {
-        ye.call(this, e, t)
+        Ee.call(this, e, t)
     }]
 }
-class mn extends it {
+class En extends at {
     constructor(e) {
-        super(), nt(this, e, hn, fn, p, {
+        super(), it(this, e, yn, vn, p, {
             selected: 0,
             players: 1,
             unassignedIsError: 2,
             inactive: 3
         })
     }
 }
 
-function pn(e, t, n) {
+function bn(e, t, n) {
     const i = e.slice();
     return i[14] = t[n], i
 }
 
-function gn(e) {
+function In(e) {
     let t;
     return {
         c() {
             t = W("Inactive Players")
         },
         l(e) {
             t = ee(e, "Inactive Players")
@@ -2429,15 +2562,15 @@
         p: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function vn(e) {
+function wn(e) {
     let t, n, i, a = 1 != e[4] ? "s" : "";
     return {
         c() {
             t = N("a"), n = W("Inactive Player"), i = W(a), this.h()
         },
         l(e) {
             t = _(e, "A", {
@@ -2457,15 +2590,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function yn(e) {
+function Cn(e) {
     let t, n, i, a, r;
     return {
         c() {
             t = N("h3"), n = W("Create your first team"), i = J(), a = N("p"), r = W("Teams may be created manually now. Alternatively once players arrive, you\n      may randomly distribute players into teams."), this.h()
         },
         l(e) {
             t = _(e, "H3", {
@@ -2487,24 +2620,24 @@
         p: c,
         d(e) {
             e && D(t), e && D(i), e && D(a)
         }
     }
 }
 
-function En(e) {
+function Bn(e) {
     let t, n, i = [],
         a = new Map,
-        r = e[6] && bn(e),
+        r = e[6] && Sn(e),
         l = e[7];
     const o = e => e[14].internalId || e[14].id;
     for (let s = 0; s < l.length; s += 1) {
-        let t = pn(e, l, s),
+        let t = bn(e, l, s),
             n = o(t);
-        a.set(n, i[s] = wn(n, t))
+        a.set(n, i[s] = Pn(n, t))
     }
     return {
         c() {
             r && r.c(), t = J(), n = N("ul");
             for (let e = 0; e < i.length; e += 1) i[e].c();
             this.h()
         },
@@ -2520,24 +2653,24 @@
             Z(n, "class", "pill-list is-large")
         },
         m(e, a) {
             r && r.m(e, a), T(e, t, a), T(e, n, a);
             for (let t = 0; t < i.length; t += 1) i[t].m(n, null)
         },
         p(e, s) {
-            e[6] ? r ? r.p(e, s) : (r = bn(e), r.c(), r.m(t.parentNode, t)) : r && (r.d(1), r = null), 641 & s && (l = e[7], i = Ze(i, s, o, 1, e, l, a, n, qe, wn, null, pn))
+            e[6] ? r ? r.p(e, s) : (r = Sn(e), r.c(), r.m(t.parentNode, t)) : r && (r.d(1), r = null), 641 & s && (l = e[7], i = Ye(i, s, o, 1, e, l, a, n, Me, Pn, null, bn))
         },
         d(e) {
             r && r.d(e), e && D(t), e && D(n);
             for (let t = 0; t < i.length; t += 1) i[t].d()
         }
     }
 }
 
-function bn(e) {
+function Sn(e) {
     let t, n;
     return {
         c() {
             t = N("a"), n = W("Download CSV"), this.h()
         },
         l(e) {
             t = _(e, "A", {
@@ -2558,15 +2691,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function In(e) {
+function Ln(e) {
     let t, n, i, a, r = e[9](e[14].session).name + "";
     return {
         c() {
             t = N("small"), n = W("("), i = W(r), a = W(")")
         },
         l(e) {
             t = _(e, "SMALL", {});
@@ -2581,117 +2714,117 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function wn(e, t) {
-    let n, i, a, r, l, o, s, c, u, A, d, f, h = t[14].players.length + "",
+function Pn(e, t) {
+    let n, i, a, r, l, o, s, c, u, d, A, f, h = t[14].players.length + "",
         m = t[14].name + "",
         p = t[9](t[14].session);
 
     function g() {
         return t[11](t[14])
     }
-    let v = p && In(t);
+    let v = p && Ln(t);
     return {
         key: e,
         first: null,
         c() {
-            n = N("li"), i = N("span"), a = W(h), r = J(), l = N("span"), o = N("a"), s = W(m), u = J(), v && v.c(), A = J(), this.h()
+            n = N("li"), i = N("span"), a = W(h), r = J(), l = N("span"), o = N("a"), s = W(m), u = J(), v && v.c(), d = J(), this.h()
         },
         l(e) {
             n = _(e, "LI", {
                 class: !0
             });
             var t = G(n);
             i = _(t, "SPAN", {
                 class: !0
             });
             var c = G(i);
             a = ee(c, h), c.forEach(D), r = te(t), l = _(t, "SPAN", {
                 class: !0
             });
-            var d = G(l);
-            o = _(d, "A", {
+            var A = G(l);
+            o = _(A, "A", {
                 href: !0
             });
             var f = G(o);
-            s = ee(f, m), f.forEach(D), u = te(d), v && v.l(d), d.forEach(D), A = te(t), t.forEach(D), this.h()
+            s = ee(f, m), f.forEach(D), u = te(A), v && v.l(A), A.forEach(D), d = te(t), t.forEach(D), this.h()
         },
         h() {
             Z(i, "class", "pill-var"), Z(o, "href", c = "#" + (t[14].internalId || t[14].id)), Z(l, "class", "pill-label"), Z(n, "class", "pill-item"), this.first = n
         },
         m(e, t) {
-            T(e, n, t), z(n, i), z(i, a), z(n, r), z(n, l), z(l, o), z(o, s), z(l, u), v && v.m(l, null), z(n, A), d || (f = q(o, "click", g), d = !0)
+            T(e, n, t), z(n, i), z(i, a), z(n, r), z(n, l), z(l, o), z(o, s), z(l, u), v && v.m(l, null), z(n, d), A || (f = q(o, "click", g), A = !0)
         },
         p(e, n) {
-            t = e, 128 & n && h !== (h = t[14].players.length + "") && ne(a, h), 128 & n && m !== (m = t[14].name + "") && ne(s, m), 128 & n && c !== (c = "#" + (t[14].internalId || t[14].id)) && Z(o, "href", c), 128 & n && (p = t[9](t[14].session)), p ? v ? v.p(t, n) : (v = In(t), v.c(), v.m(l, null)) : v && (v.d(1), v = null)
+            t = e, 128 & n && h !== (h = t[14].players.length + "") && ne(a, h), 128 & n && m !== (m = t[14].name + "") && ne(s, m), 128 & n && c !== (c = "#" + (t[14].internalId || t[14].id)) && Z(o, "href", c), 128 & n && (p = t[9](t[14].session)), p ? v ? v.p(t, n) : (v = Ln(t), v.c(), v.m(l, null)) : v && (v.d(1), v = null)
         },
         d(e) {
-            e && D(n), v && v.d(), d = !1, f()
+            e && D(n), v && v.d(), A = !1, f()
         }
     }
 }
 
-function Cn(e) {
-    let t, n, i, a, r, l, o, s, c, u, A, d = e[1] && Bn(e);
+function xn(e) {
+    let t, n, i, a, r, l, o, s, c, u, d, A = e[1] && kn(e);
     return {
         c() {
-            t = N("button"), n = Q("svg"), i = Q("g"), a = Q("path"), r = Q("path"), l = Q("path"), o = W("\n        Create New Team"), s = J(), d && d.c(), c = j(), this.h()
+            t = N("button"), n = Q("svg"), i = Q("g"), a = Q("path"), r = Q("path"), l = Q("path"), o = W("\n        Create New Team"), s = J(), A && A.c(), c = j(), this.h()
         },
         l(e) {
             t = _(e, "BUTTON", {
                 class: !0
             });
             var u = G(t);
             n = _(u, "svg", {
                 class: !0,
                 style: !0,
                 viewBox: !0,
                 id: !0,
                 xmlns: !0
             }, 1);
-            var A = G(n);
-            i = _(A, "g", {
+            var d = G(n);
+            i = _(d, "g", {
                 fill: !0
             }, 1);
             var f = G(i);
             a = _(f, "path", {
                 d: !0
             }, 1), G(a).forEach(D), r = _(f, "path", {
                 d: !0
             }, 1), G(r).forEach(D), l = _(f, "path", {
                 d: !0
-            }, 1), G(l).forEach(D), f.forEach(D), A.forEach(D), o = ee(u, "\n        Create New Team"), u.forEach(D), s = te(e), d && d.l(e), c = j(), this.h()
+            }, 1), G(l).forEach(D), f.forEach(D), d.forEach(D), o = ee(u, "\n        Create New Team"), u.forEach(D), s = te(e), A && A.l(e), c = j(), this.h()
         },
         h() {
             Z(a, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), Z(r, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), Z(l, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), Z(i, "fill", "currentColor"), Z(n, "class", "icon"), ae(n, "margin-left", "-8px"), Z(n, "viewBox", "0 0 17.928 22.481"), Z(n, "id", "people"), Z(n, "xmlns", "http://www.w3.org/2000/svg"), Z(t, "class", "button")
         },
         m(f, h) {
-            T(f, t, h), z(t, n), z(n, i), z(i, a), z(i, r), z(i, l), z(t, o), T(f, s, h), d && d.m(f, h), T(f, c, h), u || (A = q(t, "click", e[12]), u = !0)
+            T(f, t, h), z(t, n), z(n, i), z(i, a), z(i, r), z(i, l), z(t, o), T(f, s, h), A && A.m(f, h), T(f, c, h), u || (d = q(t, "click", e[12]), u = !0)
         },
         p(e, t) {
-            e[1] ? d ? d.p(e, t) : (d = Bn(e), d.c(), d.m(c.parentNode, c)) : d && (d.d(1), d = null)
+            e[1] ? A ? A.p(e, t) : (A = kn(e), A.c(), A.m(c.parentNode, c)) : A && (A.d(1), A = null)
         },
         d(e) {
-            e && D(t), e && D(s), d && d.d(e), e && D(c), u = !1, A()
+            e && D(t), e && D(s), A && A.d(e), e && D(c), u = !1, d()
         }
     }
 }
 
-function Bn(e) {
-    let t, n, i, a, r, l, o, s, c, u, A, d, f, h = 1 !== e[1] ? "s" : "";
+function kn(e) {
+    let t, n, i, a, r, l, o, s, c, u, d, A, f, h = 1 !== e[1] ? "s" : "";
     return {
         c() {
-            t = N("button"), n = Q("svg"), i = Q("g"), a = Q("path"), r = Q("path"), l = Q("path"), o = W("\n          Auto-assign "), s = W(e[1]), c = W(" player"), u = W(h), A = W("\n          to teams"), this.h()
+            t = N("button"), n = Q("svg"), i = Q("g"), a = Q("path"), r = Q("path"), l = Q("path"), o = W("\n          Auto-assign "), s = W(e[1]), c = W(" player"), u = W(h), d = W("\n          to teams"), this.h()
         },
-        l(d) {
-            t = _(d, "BUTTON", {
+        l(A) {
+            t = _(A, "BUTTON", {
                 class: !0
             });
             var f = G(t);
             n = _(f, "svg", {
                 class: !0,
                 style: !0,
                 viewBox: !0,
@@ -2705,51 +2838,51 @@
             var p = G(i);
             a = _(p, "path", {
                 d: !0
             }, 1), G(a).forEach(D), r = _(p, "path", {
                 d: !0
             }, 1), G(r).forEach(D), l = _(p, "path", {
                 d: !0
-            }, 1), G(l).forEach(D), p.forEach(D), m.forEach(D), o = ee(f, "\n          Auto-assign "), s = ee(f, e[1]), c = ee(f, " player"), u = ee(f, h), A = ee(f, "\n          to teams"), f.forEach(D), this.h()
+            }, 1), G(l).forEach(D), p.forEach(D), m.forEach(D), o = ee(f, "\n          Auto-assign "), s = ee(f, e[1]), c = ee(f, " player"), u = ee(f, h), d = ee(f, "\n          to teams"), f.forEach(D), this.h()
         },
         h() {
             Z(a, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), Z(r, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), Z(l, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), Z(i, "fill", "currentColor"), Z(n, "class", "icon"), ae(n, "margin-left", "-8px"), Z(n, "viewBox", "0 0 17.928 22.481"), Z(n, "id", "people"), Z(n, "xmlns", "http://www.w3.org/2000/svg"), Z(t, "class", "button")
         },
         m(h, m) {
-            T(h, t, m), z(t, n), z(n, i), z(i, a), z(i, r), z(i, l), z(t, o), z(t, s), z(t, c), z(t, u), z(t, A), d || (f = q(t, "click", e[13]), d = !0)
+            T(h, t, m), z(t, n), z(n, i), z(i, a), z(i, r), z(i, l), z(t, o), z(t, s), z(t, c), z(t, u), z(t, d), A || (f = q(t, "click", e[13]), A = !0)
         },
         p(e, t) {
             2 & t && ne(s, e[1]), 2 & t && h !== (h = 1 !== e[1] ? "s" : "") && ne(u, h)
         },
         d(e) {
-            e && D(t), d = !1, f()
+            e && D(t), A = !1, f()
         }
     }
 }
 
-function Sn(e) {
-    let t, n, i, a, r, l, o, s, u, A, d, f, h, m, p, g, v, y, E, b, I, w, C, B, S, L, P, x, k = 1 != e[2] ? "s" : "",
+function Rn(e) {
+    let t, n, i, a, r, l, o, s, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, L, P, x, k = 1 != e[2] ? "s" : "",
         R = e[7].length + "",
         V = 1 != e[7].length ? "s" : "";
 
     function X(e, t) {
-        return e[4] ? vn : gn
+        return e[4] ? wn : In
     }
     let O = X(e),
         F = O(e);
 
     function U(e, t) {
-        return e[7].length ? En : yn
+        return e[7].length ? Bn : Cn
     }
     let H = U(e),
         Q = H(e),
-        j = e[5] && Cn(e);
+        j = e[5] && xn(e);
     return {
         c() {
-            t = N("ul"), n = N("li"), i = N("span"), a = W(e[2]), r = J(), l = N("span"), o = W("Unassigned Player"), s = W(k), u = J(), A = N("li"), d = N("span"), f = W(R), h = J(), m = N("span"), p = N("a"), g = W("Team"), v = W(V), y = J(), E = N("li"), b = N("span"), I = W(e[4]), w = J(), C = N("span"), F.c(), B = J(), S = N("div"), Q.c(), L = J(), P = N("div"), j && j.c(), this.h()
+            t = N("ul"), n = N("li"), i = N("span"), a = W(e[2]), r = J(), l = N("span"), o = W("Unassigned Player"), s = W(k), u = J(), d = N("li"), A = N("span"), f = W(R), h = J(), m = N("span"), p = N("a"), g = W("Team"), v = W(V), y = J(), E = N("li"), b = N("span"), I = W(e[4]), w = J(), C = N("span"), F.c(), B = J(), S = N("div"), Q.c(), L = J(), P = N("div"), j && j.c(), this.h()
         },
         l(c) {
             t = _(c, "UL", {
                 class: !0
             });
             var x = G(t);
             n = _(x, "LI", {
@@ -2760,22 +2893,22 @@
                 class: !0
             });
             var O = G(i);
             a = ee(O, e[2]), O.forEach(D), r = te(X), l = _(X, "SPAN", {
                 class: !0
             });
             var U = G(l);
-            o = ee(U, "Unassigned Player"), s = ee(U, k), U.forEach(D), X.forEach(D), u = te(x), A = _(x, "LI", {
+            o = ee(U, "Unassigned Player"), s = ee(U, k), U.forEach(D), X.forEach(D), u = te(x), d = _(x, "LI", {
                 class: !0
             });
-            var z = G(A);
-            d = _(z, "SPAN", {
+            var z = G(d);
+            A = _(z, "SPAN", {
                 class: !0
             });
-            var T = G(d);
+            var T = G(A);
             f = ee(T, R), T.forEach(D), h = te(z), m = _(z, "SPAN", {
                 class: !0
             });
             var H = G(m);
             p = _(H, "A", {
                 href: !0
             });
@@ -2800,75 +2933,75 @@
                 class: !0,
                 style: !0
             });
             var K = G(P);
             j && j.l(K), K.forEach(D), M.forEach(D), this.h()
         },
         h() {
-            Z(i, "class", "pill-var"), Z(l, "class", "pill-label"), Z(n, "class", "pill-item"), Z(d, "class", "pill-var"), Z(p, "href", "#teams"), Z(m, "class", "pill-label"), Z(A, "class", "pill-item"), Z(b, "class", "pill-var"), Z(C, "class", "pill-label"), Z(E, "class", "pill-item"), Z(t, "class", "pill-list is-horizontal"), Z(P, "class", x = e[7].length ? "button-wrap" : "button-wrap align-center"), ae(P, "padding-bottom", "0"), Z(S, "class", "team-status-box well")
+            Z(i, "class", "pill-var"), Z(l, "class", "pill-label"), Z(n, "class", "pill-item"), Z(A, "class", "pill-var"), Z(p, "href", "#teams"), Z(m, "class", "pill-label"), Z(d, "class", "pill-item"), Z(b, "class", "pill-var"), Z(C, "class", "pill-label"), Z(E, "class", "pill-item"), Z(t, "class", "pill-list is-horizontal"), Z(P, "class", x = e[7].length ? "button-wrap" : "button-wrap align-center"), ae(P, "padding-bottom", "0"), Z(S, "class", "team-status-box well")
         },
         m(e, c) {
-            T(e, t, c), z(t, n), z(n, i), z(i, a), z(n, r), z(n, l), z(l, o), z(l, s), z(t, u), z(t, A), z(A, d), z(d, f), z(A, h), z(A, m), z(m, p), z(p, g), z(p, v), z(t, y), z(t, E), z(E, b), z(b, I), z(E, w), z(E, C), F.m(C, null), T(e, B, c), T(e, S, c), Q.m(S, null), z(S, L), z(S, P), j && j.m(P, null)
+            T(e, t, c), z(t, n), z(n, i), z(i, a), z(n, r), z(n, l), z(l, o), z(l, s), z(t, u), z(t, d), z(d, A), z(A, f), z(d, h), z(d, m), z(m, p), z(p, g), z(p, v), z(t, y), z(t, E), z(E, b), z(b, I), z(E, w), z(E, C), F.m(C, null), T(e, B, c), T(e, S, c), Q.m(S, null), z(S, L), z(S, P), j && j.m(P, null)
         },
         p(e, [t]) {
-            4 & t && ne(a, e[2]), 4 & t && k !== (k = 1 != e[2] ? "s" : "") && ne(s, k), 128 & t && R !== (R = e[7].length + "") && ne(f, R), 128 & t && V !== (V = 1 != e[7].length ? "s" : "") && ne(v, V), 16 & t && ne(I, e[4]), O === (O = X(e)) && F ? F.p(e, t) : (F.d(1), F = O(e), F && (F.c(), F.m(C, null))), H === (H = U(e)) && Q ? Q.p(e, t) : (Q.d(1), Q = H(e), Q && (Q.c(), Q.m(S, L))), e[5] ? j ? j.p(e, t) : (j = Cn(e), j.c(), j.m(P, null)) : j && (j.d(1), j = null), 128 & t && x !== (x = e[7].length ? "button-wrap" : "button-wrap align-center") && Z(P, "class", x)
+            4 & t && ne(a, e[2]), 4 & t && k !== (k = 1 != e[2] ? "s" : "") && ne(s, k), 128 & t && R !== (R = e[7].length + "") && ne(f, R), 128 & t && V !== (V = 1 != e[7].length ? "s" : "") && ne(v, V), 16 & t && ne(I, e[4]), O === (O = X(e)) && F ? F.p(e, t) : (F.d(1), F = O(e), F && (F.c(), F.m(C, null))), H === (H = U(e)) && Q ? Q.p(e, t) : (Q.d(1), Q = H(e), Q && (Q.c(), Q.m(S, L))), e[5] ? j ? j.p(e, t) : (j = xn(e), j.c(), j.m(P, null)) : j && (j.d(1), j = null), 128 & t && x !== (x = e[7].length ? "button-wrap" : "button-wrap align-center") && Z(P, "class", x)
         },
         i: c,
         o: c,
         d(e) {
             e && D(t), F.d(), e && D(B), e && D(S), Q.d(), j && j.d()
         }
     }
 }
 
-function Ln(e, t, n) {
+function Vn(e, t, n) {
     let i, a, r = c,
         l = () => (r(), r = v(u, (e => n(10, a = e))), u);
     e.$$.on_destroy.push((() => r()));
     let {
         showAutoBalance: o
     } = t, {
         unassigned: s
     } = t, {
         data: u
     } = t;
     l();
     let {
-        inactive: A
+        inactive: d
     } = t, {
-        currentSession: d
+        currentSession: A
     } = t, {
         allowCreate: f = !0
     } = t, {
         downloadPlayersUrl: h
     } = t;
-    const m = ve();
+    const m = ye();
     return e.$$set = e => {
-        "showAutoBalance" in e && n(1, o = e.showAutoBalance), "unassigned" in e && n(2, s = e.unassigned), "data" in e && l(n(3, u = e.data)), "inactive" in e && n(4, A = e.inactive), "currentSession" in e && n(0, d = e.currentSession), "allowCreate" in e && n(5, f = e.allowCreate), "downloadPlayersUrl" in e && n(6, h = e.downloadPlayersUrl)
+        "showAutoBalance" in e && n(1, o = e.showAutoBalance), "unassigned" in e && n(2, s = e.unassigned), "data" in e && l(n(3, u = e.data)), "inactive" in e && n(4, d = e.inactive), "currentSession" in e && n(0, A = e.currentSession), "allowCreate" in e && n(5, f = e.allowCreate), "downloadPlayersUrl" in e && n(6, h = e.downloadPlayersUrl)
     }, e.$$.update = () => {
         1024 & e.$$.dirty && n(7, i = a.teams)
-    }, [d, o, s, u, A, f, h, i, m, e => a.sessions.length <= 1 ? null : a.sessions.find((t => t.id === e)), a, e => {
-        e.session && d && n(0, d = e.session)
+    }, [A, o, s, u, d, f, h, i, m, e => a.sessions.length <= 1 ? null : a.sessions.find((t => t.id === e)), a, e => {
+        e.session && A && n(0, A = e.session)
     }, () => m("clickCreateTeam"), () => m("openAutoBalance")]
 }
-class Pn extends it {
+class Xn extends at {
     constructor(e) {
-        super(), nt(this, e, Ln, Sn, p, {
+        super(), it(this, e, Vn, Rn, p, {
             showAutoBalance: 1,
             unassigned: 2,
             data: 3,
             inactive: 4,
             currentSession: 0,
             allowCreate: 5,
             downloadPlayersUrl: 6
         })
     }
 }
 
-function xn(e) {
+function On(e) {
     let t, n, i, a, r, l, o, s, u;
     return {
         c() {
             t = N("p"), n = W("Choose\n    "), i = N("button"), a = Q("svg"), r = Q("path"), l = W("\n      Auto Balance"), o = W("\n    to randomly distribute players into teams."), this.h()
         },
         l(e) {
             t = _(e, "P", {});
@@ -2888,25 +3021,25 @@
                 d: !0,
                 fill: !0
             }, 1), G(r).forEach(D), u.forEach(D), l = ee(c, "\n      Auto Balance"), c.forEach(D), o = ee(s, "\n    to randomly distribute players into teams."), s.forEach(D), this.h()
         },
         h() {
             Z(r, "d", "M18.857 0H3.143A3.143 3.143 0 000 3.143v15.714A3.143 3.143 0 003.143 22h15.714A3.143 3.143 0 0022 18.857V3.143A3.143 3.143 0 0018.857 0zm0 9.429h-6.286V3.143h6.286v6.286zM3.143 3.143h6.286v6.286H3.143V3.143zm0 15.714v-6.286h6.286v6.286H3.143zm9.428 0v-6.286h6.286v6.286h-6.286z"), Z(r, "fill", "#0C66B8"), Z(a, "fill", "none"), Z(a, "class", "icon"), Z(a, "xmlns", "http://www.w3.org/2000/svg"), Z(a, "viewBox", "0 0 22 22"), Z(i, "class", "button no-border strong theme-info-color inline-help-button")
         },
-        m(c, A) {
-            T(c, t, A), z(t, n), z(t, i), z(i, a), z(a, r), z(i, l), z(t, o), s || (u = q(i, "click", e[2]), s = !0)
+        m(c, d) {
+            T(c, t, d), z(t, n), z(t, i), z(i, a), z(a, r), z(i, l), z(t, o), s || (u = q(i, "click", e[2]), s = !0)
         },
         p: c,
         d(e) {
             e && D(t), s = !1, u()
         }
     }
 }
 
-function kn(e) {
+function Fn(e) {
     let t;
     return {
         c() {
             t = W("Option 2: ")
         },
         l(e) {
             t = ee(e, "Option 2: ")
@@ -2916,37 +3049,37 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Rn(e) {
-    let t, n, i, a, r, l, o, s, u, A, d, f, h, m, p, v, y, E, b, I, w, C, B, S, L, P, x, k, R, V, X, O, F, U, H, j, M, K, Y, $, ne, ie, ae, re, le, oe, se = e[0] && xn(e),
-        ce = e[0] && kn();
+function Un(e) {
+    let t, n, i, a, r, l, o, s, u, d, A, f, h, m, p, v, y, E, b, I, w, C, B, S, L, P, x, k, R, V, X, O, F, U, H, j, M, K, Y, $, ne, ie, ae, re, le, oe, se = e[0] && On(e),
+        ce = e[0] && Fn();
     return {
         c() {
-            t = N("div"), se && se.c(), n = J(), i = N("h3"), ce && ce.c(), a = W("Build teams manually"), r = J(), l = N("img"), s = J(), u = N("ol"), A = N("li"), d = W("Select one or more players from the ’Unassigned Players’ list by hovering over their name and clicking the check box."), f = J(), h = N("li"), m = W("Click\n      "), p = N("button"), v = Q("svg"), y = Q("circle"), E = Q("g"), b = Q("path"), I = Q("defs"), w = Q("clipPath"), C = Q("rect"), B = W("\n\n        Add Team"), S = W("\n      to start a new team with the selected players, and repeat until all players are assigned."), L = J(), P = N("div"), x = Q("svg"), k = Q("path"), R = J(), V = N("div"), X = N("p"), O = W("You may "), F = N("strong"), U = W("rearrange teams"), H = W(" as much as you’d like before the game is in play."), j = J(), M = N("p"), K = W("All players must be "), Y = N("em"), $ = W("assigned"), ne = W(" or marked "), ie = N("em"), ae = W("inactive"), re = W(" before the game can start."), this.h()
+            t = N("div"), se && se.c(), n = J(), i = N("h3"), ce && ce.c(), a = W("Build teams manually"), r = J(), l = N("img"), s = J(), u = N("ol"), d = N("li"), A = W("Select one or more players from the ’Unassigned Players’ list by hovering over their name and clicking the check box."), f = J(), h = N("li"), m = W("Click\n      "), p = N("button"), v = Q("svg"), y = Q("circle"), E = Q("g"), b = Q("path"), I = Q("defs"), w = Q("clipPath"), C = Q("rect"), B = W("\n\n        Add Team"), S = W("\n      to start a new team with the selected players, and repeat until all players are assigned."), L = J(), P = N("div"), x = Q("svg"), k = Q("path"), R = J(), V = N("div"), X = N("p"), O = W("You may "), F = N("strong"), U = W("rearrange teams"), H = W(" as much as you’d like before the game is in play."), j = J(), M = N("p"), K = W("All players must be "), Y = N("em"), $ = W("assigned"), ne = W(" or marked "), ie = N("em"), ae = W("inactive"), re = W(" before the game can start."), this.h()
         },
         l(e) {
             t = _(e, "DIV", {});
             var o = G(t);
             se && se.l(o), n = te(o), i = _(o, "H3", {
                 class: !0
             });
             var c = G(i);
             ce && ce.l(c), a = ee(c, "Build teams manually"), c.forEach(D), r = te(o), l = _(o, "IMG", {
                 class: !0,
                 src: !0,
                 alt: !0
             }), s = te(o), u = _(o, "OL", {});
             var g = G(u);
-            A = _(g, "LI", {});
-            var z = G(A);
-            d = ee(z, "Select one or more players from the ’Unassigned Players’ list by hovering over their name and clicking the check box."), z.forEach(D), f = te(g), h = _(g, "LI", {});
+            d = _(g, "LI", {});
+            var z = G(d);
+            A = ee(z, "Select one or more players from the ’Unassigned Players’ list by hovering over their name and clicking the check box."), z.forEach(D), f = te(g), h = _(g, "LI", {});
             var T = G(h);
             m = ee(T, "Click\n      "), p = _(T, "BUTTON", {
                 class: !0
             });
             var N = G(p);
             v = _(N, "svg", {
                 width: !0,
@@ -2998,63 +3131,63 @@
             }, 1), G(k).forEach(D), le.forEach(D), R = te(Z), V = _(Z, "DIV", {
                 class: !0
             });
             var oe = G(V);
             X = _(oe, "P", {});
             var ue = G(X);
             O = ee(ue, "You may "), F = _(ue, "STRONG", {});
-            var Ae = G(F);
-            U = ee(Ae, "rearrange teams"), Ae.forEach(D), H = ee(ue, " as much as you’d like before the game is in play."), ue.forEach(D), j = te(oe), M = _(oe, "P", {});
-            var de = G(M);
-            K = ee(de, "All players must be "), Y = _(de, "EM", {});
+            var de = G(F);
+            U = ee(de, "rearrange teams"), de.forEach(D), H = ee(ue, " as much as you’d like before the game is in play."), ue.forEach(D), j = te(oe), M = _(oe, "P", {});
+            var Ae = G(M);
+            K = ee(Ae, "All players must be "), Y = _(Ae, "EM", {});
             var fe = G(Y);
-            $ = ee(fe, "assigned"), fe.forEach(D), ne = ee(de, " or marked "), ie = _(de, "EM", {});
+            $ = ee(fe, "assigned"), fe.forEach(D), ne = ee(Ae, " or marked "), ie = _(Ae, "EM", {});
             var he = G(ie);
-            ae = ee(he, "inactive"), he.forEach(D), re = ee(de, " before the game can start."), de.forEach(D), oe.forEach(D), Z.forEach(D), o.forEach(D), this.h()
+            ae = ee(he, "inactive"), he.forEach(D), re = ee(Ae, " before the game can start."), Ae.forEach(D), oe.forEach(D), Z.forEach(D), o.forEach(D), this.h()
         },
         h() {
             var e, t;
             Z(i, "class", "player-help-header"), Z(l, "class", "player-help-img"), e = l.src, t = o = "data:image/png;base64,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", g || (g = document.createElement("a")), g.href = t, e !== g.href && Z(l, "src", "data:image/png;base64,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"), Z(l, "alt", "Player Management Examples"), Z(y, "cx", "13"), Z(y, "cy", "13"), Z(y, "r", "12"), Z(y, "stroke", "currentColor"), Z(y, "stroke-width", "2"), Z(b, "d", "M17.9653 11.6049H15.1504C14.9504 11.6049 14.7585 11.5254 14.6171 11.384C14.4757 11.2426 14.3962 11.0507 14.3962 10.8507H14.3952V8.00958C14.3885 7.81386 14.3061 7.62837 14.1652 7.49226C14.0244 7.35615 13.8363 7.28005 13.6404 7.28003H12.3612C12.262 7.27989 12.1637 7.29931 12.072 7.33717C11.9803 7.37503 11.8969 7.43059 11.8267 7.50068C11.7564 7.57077 11.7007 7.65402 11.6626 7.74565C11.6246 7.83729 11.605 7.93553 11.6049 8.03476V10.8497C11.6049 11.2666 11.2666 11.6039 10.8507 11.6039H8.0227C7.82453 11.6076 7.63572 11.6889 7.49685 11.8303C7.35798 11.9717 7.28013 12.162 7.28003 12.3602V13.6394C7.28003 14.0516 7.61098 14.3878 8.0227 14.3936H10.8507V14.3946C11.2677 14.3946 11.6049 14.7329 11.6049 15.1488V17.9774C11.6083 18.1753 11.6894 18.364 11.8305 18.5028C11.9717 18.6416 12.1617 18.7194 12.3596 18.7195H13.6394C14.0521 18.7195 14.3873 18.3886 14.3936 17.9774V15.1488H14.3946C14.3946 14.7319 14.7329 14.3946 15.1488 14.3946V14.3936H17.9894C18.1852 14.3872 18.3708 14.3049 18.5071 14.1642C18.6433 14.0234 18.7195 13.8353 18.7195 13.6394V12.3602C18.7196 12.261 18.7002 12.1628 18.6624 12.0712C18.6246 11.9796 18.569 11.8963 18.499 11.8262C18.4289 11.756 18.3457 11.7004 18.2542 11.6624C18.1626 11.6245 18.0644 11.6049 17.9653 11.6049Z"), Z(b, "fill", "currentColor"), Z(E, "clip-path", "url(#clip0)"), Z(C, "width", "11.44"), Z(C, "height", "11.44"), Z(C, "fill", "white"), Z(C, "transform", "translate(7.28003 7.28003)"), Z(w, "id", "clip0"), Z(v, "width", "26"), Z(v, "height", "26"), Z(v, "viewBox", "0 0 26 26"), Z(v, "fill", "none"), Z(v, "xmlns", "http://www.w3.org/2000/svg"), Z(v, "class", "icon"), Z(p, "class", "button no-border strong theme-info-color inline-help-button"), Z(k, "d", "M26.115 11.345 15.639.86a3.094 3.094 0 0 0-4.278 0L.885 11.345a3.029 3.029 0 0 0 0 4.28l10.476 10.487a3.02 3.02 0 0 0 4.278 0l10.476-10.489a3.029 3.029 0 0 0 0-4.28v.002ZM12.054 6.73A1.449 1.449 0 0 1 13.5 5.282a1.446 1.446 0 0 1 1.446 1.447v5.792A1.449 1.449 0 0 1 13.5 13.97a1.446 1.446 0 0 1-1.446-1.448V6.73ZM13.5 20.243a1.928 1.928 0 0 1-1.892-2.307 1.931 1.931 0 0 1 2.63-1.407 1.93 1.93 0 0 1 .626 3.149 1.928 1.928 0 0 1-1.364.565Z"), Z(k, "fill", "#FFBE15"), Z(x, "class", "icon"), Z(x, "fill", "none"), Z(x, "xmlns", "http://www.w3.org/2000/svg"), Z(x, "viewBox", "0 0 27 27"), Z(V, "class", "note-content"), Z(P, "class", "note border-theme theme-caution-color")
         },
         m(o, c) {
-            T(o, t, c), se && se.m(t, null), z(t, n), z(t, i), ce && ce.m(i, null), z(i, a), z(t, r), z(t, l), z(t, s), z(t, u), z(u, A), z(A, d), z(u, f), z(u, h), z(h, m), z(h, p), z(p, v), z(v, y), z(v, E), z(E, b), z(v, I), z(I, w), z(w, C), z(p, B), z(h, S), z(t, L), z(t, P), z(P, x), z(x, k), z(P, R), z(P, V), z(V, X), z(X, O), z(X, F), z(F, U), z(X, H), z(V, j), z(V, M), z(M, K), z(M, Y), z(Y, $), z(M, ne), z(M, ie), z(ie, ae), z(M, re), le || (oe = q(p, "click", e[3]), le = !0)
+            T(o, t, c), se && se.m(t, null), z(t, n), z(t, i), ce && ce.m(i, null), z(i, a), z(t, r), z(t, l), z(t, s), z(t, u), z(u, d), z(d, A), z(u, f), z(u, h), z(h, m), z(h, p), z(p, v), z(v, y), z(v, E), z(E, b), z(v, I), z(I, w), z(w, C), z(p, B), z(h, S), z(t, L), z(t, P), z(P, x), z(x, k), z(P, R), z(P, V), z(V, X), z(X, O), z(X, F), z(F, U), z(X, H), z(V, j), z(V, M), z(M, K), z(M, Y), z(Y, $), z(M, ne), z(M, ie), z(ie, ae), z(M, re), le || (oe = q(p, "click", e[3]), le = !0)
         },
         p(e, [r]) {
-            e[0] ? se ? se.p(e, r) : (se = xn(e), se.c(), se.m(t, n)) : se && (se.d(1), se = null), e[0] ? ce || (ce = kn(), ce.c(), ce.m(i, a)) : ce && (ce.d(1), ce = null)
+            e[0] ? se ? se.p(e, r) : (se = On(e), se.c(), se.m(t, n)) : se && (se.d(1), se = null), e[0] ? ce || (ce = Fn(), ce.c(), ce.m(i, a)) : ce && (ce.d(1), ce = null)
         },
         i: c,
         o: c,
         d(e) {
             e && D(t), se && se.d(), ce && ce.d(), le = !1, oe()
         }
     }
 }
 
-function Vn(e, t, n) {
+function zn(e, t, n) {
     let {
         showAutoBalance: i
     } = t;
-    const a = ve();
+    const a = ye();
     return e.$$set = e => {
         "showAutoBalance" in e && n(0, i = e.showAutoBalance)
     }, [i, a, () => a("openAutoBalance"), () => a("clickCreateTeam")]
 }
-class Xn extends it {
+class Tn extends at {
     constructor(e) {
-        super(), nt(this, e, Vn, Rn, p, {
+        super(), it(this, e, zn, Un, p, {
             showAutoBalance: 0
         })
     }
 }
 
-function On(e) {
-    let t, n, i, a, r, l, o, s, u, A, d, f, m, p, g, v, y, E;
+function Dn(e) {
+    let t, n, i, a, r, l, o, s, u, d, A, f, m, p, g, v, y, E;
     return {
         c() {
-            t = N("dialog"), n = N("button"), i = Q("svg"), a = Q("path"), r = J(), l = N("div"), o = N("form"), s = N("h2"), u = W("Rename Team"), A = J(), d = N("p"), f = N("input"), m = J(), p = N("div"), g = N("button"), v = W("Rename Team"), this.h()
+            t = N("dialog"), n = N("button"), i = Q("svg"), a = Q("path"), r = J(), l = N("div"), o = N("form"), s = N("h2"), u = W("Rename Team"), d = J(), A = N("p"), f = N("input"), m = J(), p = N("div"), g = N("button"), v = W("Rename Team"), this.h()
         },
         l(e) {
             t = _(e, "DIALOG", {
                 class: !0
             });
             var c = G(t);
             n = _(c, "BUTTON", {
@@ -3076,57 +3209,57 @@
             var E = G(l);
             o = _(E, "FORM", {});
             var b = G(o);
             s = _(b, "H2", {
                 class: !0
             });
             var I = G(s);
-            u = ee(I, "Rename Team"), I.forEach(D), A = te(b), d = _(b, "P", {});
-            var w = G(d);
+            u = ee(I, "Rename Team"), I.forEach(D), d = te(b), A = _(b, "P", {});
+            var w = G(A);
             f = _(w, "INPUT", {}), w.forEach(D), m = te(b), p = _(b, "DIV", {
                 class: !0
             });
             var C = G(p);
             g = _(C, "BUTTON", {
                 class: !0
             });
             var B = G(g);
             v = ee(B, "Rename Team"), B.forEach(D), C.forEach(D), b.forEach(D), E.forEach(D), c.forEach(D), this.h()
         },
         h() {
             Z(a, "fill", "currentColor"), Z(a, "d", "M11.38 7.75L16 3.14a1.86 1.86 0 00.25-2.38 1.79 1.79 0 00-2.74-.23L8.83 5.2a.76.76 0 01-1.08 0L3.14.6A1.86 1.86 0 00.76.33a1.79 1.79 0 00-.23 2.74L5.2 7.75a.76.76 0 010 1.08L.6 13.44a1.88 1.88 0 00-.27 2.39 1.81 1.81 0 002.74.23l4.68-4.68a.76.76 0 011.08 0L13.44 16a1.87 1.87 0 002.39.26 1.81 1.81 0 00.23-2.74l-4.68-4.69a.76.76 0 010-1.08z"), Z(i, "class", "icon"), Z(i, "viewBox", "0 0 16.59 16.59"), Z(i, "xmlns", "http://www.w3.org/2000/svg"), Z(n, "class", "close-button"), Z(s, "class", "modal-heading"), Z(g, "class", "button"), Z(p, "class", "button-wrap align-center"), Z(l, "class", "scroll-wrap text-center"), Z(t, "class", "modal large-pad")
         },
         m(c, h) {
-            T(c, t, h), z(t, n), z(n, i), z(i, a), z(t, r), z(t, l), z(l, o), z(o, s), z(s, u), z(o, A), z(o, d), z(d, f), ie(f, e[2]), z(o, m), z(o, p), z(p, g), z(g, v), e[9](t), y || (E = [q(n, "click", e[5]), q(f, "input", e[6]), S(Fn.call(null, f)), q(f, "keyup", e[7]), q(o, "submit", M(e[8]))], y = !0)
+            T(c, t, h), z(t, n), z(n, i), z(i, a), z(t, r), z(t, l), z(l, o), z(o, s), z(s, u), z(o, d), z(o, A), z(A, f), ie(f, e[2]), z(o, m), z(o, p), z(p, g), z(g, v), e[9](t), y || (E = [q(n, "click", e[5]), q(f, "input", e[6]), S(Hn.call(null, f)), q(f, "keyup", e[7]), q(o, "submit", M(e[8]))], y = !0)
         },
         p(e, [t]) {
             4 & t && f.value !== e[2] && ie(f, e[2])
         },
         i: c,
         o: c,
         d(n) {
             n && D(t), e[9](null), y = !1, h(E)
         }
     }
 }
 
-function Fn(e) {
+function Hn(e) {
     e.focus()
 }
 
-function Un(e, t, n) {
+function Nn(e, t, n) {
     let {
         team: i
     } = t, {
         open: a = !1
     } = t;
-    const r = ve();
+    const r = ye();
     let l, o = i.name;
     ge((() => {
-        Et.registerDialog(l)
+        bt.registerDialog(l)
     }));
     return e.$$set = e => {
         "team" in e && n(4, i = e.team), "open" in e && n(0, a = e.open)
     }, e.$$.update = () => {
         3 & e.$$.dirty && l && (a ? l.showModal() : (null == l ? void 0 : l.open) && l.close(), document.body.classList.toggle("modal-is-open", a))
     }, [a, l, o, r, i, () => {
         n(0, a = !1)
@@ -3135,38 +3268,38 @@
     }, e => {
         "Escape" === e.key && r("close")
     }, () => {
         r("rename", {
             name: o
         }), n(0, a = !1)
     }, function(e) {
-        be[e ? "unshift" : "push"]((() => {
+        Ie[e ? "unshift" : "push"]((() => {
             l = e, n(1, l)
         }))
     }]
 }
-class zn extends it {
+class Qn extends at {
     constructor(e) {
-        super(), nt(this, e, Un, On, p, {
+        super(), it(this, e, Nn, Dn, p, {
             team: 4,
             open: 0
         })
     }
 }
 
-function Tn(e, t, n) {
+function Wn(e, t, n) {
     const i = e.slice();
     return i[19] = t[n], i
 }
 
-function Dn(e) {
+function Jn(e) {
     let t, n, i, a;
 
     function r(e, t) {
-        return e[7].length > 1 ? Nn : Hn
+        return e[7].length > 1 ? qn : jn
     }
     let l = r(e),
         o = l(e);
     return {
         c() {
             t = N("button"), n = W("Add "), o.c(), this.h()
         },
@@ -3188,15 +3321,15 @@
         },
         d(e) {
             e && D(t), o.d(), i = !1, a()
         }
     }
 }
 
-function Hn(e) {
+function jn(e) {
     let t;
     return {
         c() {
             t = W("player")
         },
         l(e) {
             t = ee(e, "player")
@@ -3207,15 +3340,15 @@
         p: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Nn(e) {
+function qn(e) {
     let t, n, i = e[7].length + "";
     return {
         c() {
             t = W(i), n = W(" players")
         },
         l(e) {
             t = ee(e, i), n = ee(e, " players")
@@ -3228,19 +3361,19 @@
         },
         d(e) {
             e && D(t), e && D(n)
         }
     }
 }
 
-function Qn(e) {
+function Mn(e) {
     let t;
 
     function n(e, t) {
-        return !e[4].minimumPlayers || e[4].maximumPlayers && e[4].minimumPlayers !== e[4].maximumPlayers ? e[4].minimumPlayers && e[4].maximumPlayers ? Jn : e[4].maximumPlayers ? Wn : void 0 : jn
+        return !e[4].minimumPlayers || e[4].maximumPlayers && e[4].minimumPlayers !== e[4].maximumPlayers ? e[4].minimumPlayers && e[4].maximumPlayers ? Zn : e[4].maximumPlayers ? Kn : void 0 : Yn
     }
     let i = n(e),
         a = i && i(e);
     return {
         c() {
             a && a.c(), t = j()
         },
@@ -3255,15 +3388,15 @@
         },
         d(e) {
             a && a.d(e), e && D(t)
         }
     }
 }
 
-function Wn(e) {
+function Kn(e) {
     let t, n, i, a, r = e[4].maximumPlayers + "";
     return {
         c() {
             t = N("em"), n = W("("), i = W(r), a = W(" maximum)")
         },
         l(e) {
             t = _(e, "EM", {});
@@ -3278,15 +3411,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Jn(e) {
+function Zn(e) {
     let t, n, i, a, r, l, o = e[4].minimumPlayers + "",
         s = e[4].maximumPlayers + "";
     return {
         c() {
             t = N("em"), n = W("("), i = W(o), a = W(" to "), r = W(s), l = W(" required)")
         },
         l(e) {
@@ -3302,15 +3435,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function jn(e) {
+function Yn(e) {
     let t, n, i, a, r = e[4].minimumPlayers + "";
     return {
         c() {
             t = N("em"), n = W("("), i = W(r), a = W(" required)")
         },
         l(e) {
             t = _(e, "EM", {});
@@ -3325,15 +3458,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function qn(e) {
+function Gn(e) {
     let t, n, i;
     return {
         c() {
             t = N("div"), n = N("p"), i = W("Assign players to this team to get started."), this.h()
         },
         l(e) {
             t = _(e, "DIV", {
@@ -3354,106 +3487,106 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Mn(e, t) {
+function $n(e, t) {
     let n, i, a, r, l, o, s, u = c;
-    return i = new nn({
+    return i = new sn({
         props: {
             isSelected: t[2].includes(t[19].id),
             player: t[19],
             assigned: !0,
             readOnly: t[3],
             currentTeam: t[0]
         }
     }), i.$on("selectPlayer", t[13]), i.$on("unassignPlayer", t[14]), i.$on("addPlayers", t[15]), {
         key: e,
         first: null,
         c() {
-            n = N("div"), Ge(i.$$.fragment), a = J(), this.h()
+            n = N("div"), $e(i.$$.fragment), a = J(), this.h()
         },
         l(e) {
             n = _(e, "DIV", {});
             var t = G(n);
-            $e(i.$$.fragment, t), a = te(t), t.forEach(D), this.h()
+            _e(i.$$.fragment, t), a = te(t), t.forEach(D), this.h()
         },
         h() {
             this.first = n
         },
         m(e, t) {
-            T(e, n, t), _e(i, n, null), z(n, a), s = !0
+            T(e, n, t), et(i, n, null), z(n, a), s = !0
         },
         p(e, n) {
             t = e;
             const a = {};
             6 & n && (a.isSelected = t[2].includes(t[19].id)), 2 & n && (a.player = t[19]), 8 & n && (a.readOnly = t[3]), 1 & n && (a.currentTeam = t[0]), i.$set(a)
         },
         r() {
             o = n.getBoundingClientRect()
         },
         f() {
             fe(n), u(), he(n, o)
         },
         a() {
-            u(), u = de(n, o, qt, {})
+            u(), u = Ae(n, o, Mt, {})
         },
         i(e) {
-            s || (De(i.$$.fragment, e), e && Se((() => {
-                l && l.end(1), r = Qe(n, on, {
+            s || (He(i.$$.fragment, e), e && Le((() => {
+                l && l.end(1), r = We(n, An, {
                     key: t[19].id
                 }), r.start()
             })), s = !0)
         },
         o(e) {
-            He(i.$$.fragment, e), r && r.invalidate(), e && (l = We(n, ln, {
+            Ne(i.$$.fragment, e), r && r.invalidate(), e && (l = Je(n, dn, {
                 key: t[19].id
             })), s = !1
         },
         d(e) {
-            e && D(n), et(i), e && l && l.end()
+            e && D(n), tt(i), e && l && l.end()
         }
     }
 }
 
-function Kn(e) {
-    let t, n, i, a, r, l, o, s, c, u, A, d, f, m, p, g, v, y, E, b, I, w, C, B, S, L, P, x, k, R, V = e[0].name + "",
+function _n(e) {
+    let t, n, i, a, r, l, o, s, c, u, d, A, f, m, p, g, v, y, E, b, I, w, C, B, S, L, P, x, k, R, V = e[0].name + "",
         X = (e[1].length || "No") + "",
         O = 1 === e[1].length ? "player" : "players",
         F = [],
         U = new Map,
-        H = e[7].length && Dn(e),
-        j = e[6] && Qn(e),
-        K = 0 == e[1].length && qn(),
+        H = e[7].length && Jn(e),
+        j = e[6] && Mn(e),
+        K = 0 == e[1].length && Gn(),
         Y = e[1];
     const $ = e => {
         var t;
         return null == (t = e[19]) ? void 0 : t.id
     };
     for (let h = 0; h < Y.length; h += 1) {
-        let t = Tn(e, Y, h),
+        let t = Wn(e, Y, h),
             n = $(t);
-        U.set(n, F[h] = Mn(n, t))
+        U.set(n, F[h] = $n(n, t))
     }
 
     function ie(t) {
         e[16](t)
     }
     let ae = {
         team: e[0]
     };
-    return void 0 !== e[5] && (ae.open = e[5]), L = new zn({
+    return void 0 !== e[5] && (ae.open = e[5]), L = new Qn({
         props: ae
-    }), be.push((() => Ye(L, "open", ie))), L.$on("close", e[17]), L.$on("rename", e[18]), {
+    }), Ie.push((() => Ge(L, "open", ie))), L.$on("close", e[17]), L.$on("rename", e[18]), {
         c() {
-            t = N("div"), n = N("h2"), i = W(V), a = J(), H && H.c(), r = J(), l = N("p"), o = W(X), s = J(), c = W(O), u = J(), j && j.c(), A = J(), d = N("div"), f = N("a"), m = Q("svg"), p = Q("path"), g = J(), v = N("a"), y = Q("svg"), E = Q("path"), I = J(), w = N("div"), K && K.c(), C = J();
+            t = N("div"), n = N("h2"), i = W(V), a = J(), H && H.c(), r = J(), l = N("p"), o = W(X), s = J(), c = W(O), u = J(), j && j.c(), d = J(), A = N("div"), f = N("a"), m = Q("svg"), p = Q("path"), g = J(), v = N("a"), y = Q("svg"), E = Q("path"), I = J(), w = N("div"), K && K.c(), C = J();
             for (let e = 0; e < F.length; e += 1) F[e].c();
-            S = J(), Ge(L.$$.fragment), this.h()
+            S = J(), $e(L.$$.fragment), this.h()
         },
         l(e) {
             t = _(e, "DIV", {
                 class: !0,
                 id: !0
             });
             var h = G(t);
@@ -3461,18 +3594,18 @@
                 class: !0
             });
             var b = G(n);
             i = ee(b, V), b.forEach(D), a = te(h), H && H.l(h), r = te(h), l = _(h, "P", {
                 class: !0
             });
             var B = G(l);
-            o = ee(B, X), s = te(B), c = ee(B, O), u = te(B), j && j.l(B), B.forEach(D), A = te(h), d = _(h, "DIV", {
+            o = ee(B, X), s = te(B), c = ee(B, O), u = te(B), j && j.l(B), B.forEach(D), d = te(h), A = _(h, "DIV", {
                 class: !0
             });
-            var P = G(d);
+            var P = G(A);
             f = _(P, "A", {
                 class: !0,
                 href: !0
             });
             var x = G(f);
             m = _(x, "svg", {
                 class: !0,
@@ -3499,133 +3632,133 @@
             E = _(U, "path", {
                 d: !0,
                 fill: !0
             }, 1), G(E).forEach(D), U.forEach(D), R.forEach(D), P.forEach(D), h.forEach(D), I = te(e), w = _(e, "DIV", {});
             var z = G(w);
             K && K.l(z), C = te(z);
             for (let t = 0; t < F.length; t += 1) F[t].l(z);
-            z.forEach(D), S = te(e), $e(L.$$.fragment, e), this.h()
+            z.forEach(D), S = te(e), _e(L.$$.fragment, e), this.h()
         },
         h() {
-            Z(n, "class", "player-card-heading"), Z(l, "class", "player-card-summary"), Z(p, "d", "M23.323 2.883L20.861.422a1.44 1.44 0 00-2.036 0l-2.122 2.122a.64.64 0 000 .905l3.593 3.593c.25.25.655.25.905 0l2.122-2.122a1.441 1.441 0 000-2.037zm-7.39 1.336a.639.639 0 00-.905 0l-11.75 11.75a.639.639 0 000 .905l3.593 3.593c.25.25.655.25.905 0l11.75-11.75a.64.64 0 000-.905l-3.593-3.593zM2.597 17.732a.48.48 0 00-.775.138l-.032.095-1.746 5.099-.032.093a.48.48 0 00.576.576l.093-.033 5.099-1.746.095-.032a.48.48 0 00.138-.775l-3.416-3.415z"), Z(p, "fill", "currentColor"), Z(m, "class", "icon"), Z(m, "viewBox", "0 0 23.744 23.745"), Z(m, "id", "pencil"), Z(m, "xmlns", "http://www.w3.org/2000/svg"), Z(f, "class", "button icon-button circle "), Z(f, "href", "."), Z(E, "d", "M15.67 4.446l-.057-.215-.409-1.545a.876.876 0 00-.692-.588l-.034-.005a51.6 51.6 0 00-3.453-.33l-.04.002a.638.638 0 01-.614-.46C10.234.993 9.978.311 9.663.184A1.438 1.438 0 009.448.12C9.39.11 9.331.103 9.272.095a10.745 10.745 0 00-2.867 0C6.348.103 6.288.11 6.23.12a1.225 1.225 0 00-.213.065C5.709.308 5.459.98 5.32 1.28a.634.634 0 01-.62.485c-.011 0-.021 0-.032-.002-1.146.071-2.28.18-3.404.325l-.142.018a.876.876 0 00-.648.581L.065 4.231l-.057.215a.904.904 0 00.874 1.027h13.915a.905.905 0 00.873-1.027zm-1.695 2.69H1.704a.906.906 0 00-.812.859l.02.232 1.005 12.18a.88.88 0 00.869.762h10.107c.44 0 .812-.326.869-.762l1.007-12.18.019-.232a.908.908 0 00-.813-.859z"), Z(E, "fill", "currentColor"), Z(y, "class", "icon"), Z(y, "viewBox", "0 0 15.679 21.169"), Z(y, "id", "trash"), Z(y, "xmlns", "http://www.w3.org/2000/svg"), Z(v, "class", "button icon-button circle "), Z(v, "href", "."), Z(d, "class", "player-card-actions"), Z(t, "class", "player-item is-header theme-caution-color"), Z(t, "id", b = e[0].internalId || e[0].id), re(t, "theme-caution-color", e[6])
+            Z(n, "class", "player-card-heading"), Z(l, "class", "player-card-summary"), Z(p, "d", "M23.323 2.883L20.861.422a1.44 1.44 0 00-2.036 0l-2.122 2.122a.64.64 0 000 .905l3.593 3.593c.25.25.655.25.905 0l2.122-2.122a1.441 1.441 0 000-2.037zm-7.39 1.336a.639.639 0 00-.905 0l-11.75 11.75a.639.639 0 000 .905l3.593 3.593c.25.25.655.25.905 0l11.75-11.75a.64.64 0 000-.905l-3.593-3.593zM2.597 17.732a.48.48 0 00-.775.138l-.032.095-1.746 5.099-.032.093a.48.48 0 00.576.576l.093-.033 5.099-1.746.095-.032a.48.48 0 00.138-.775l-3.416-3.415z"), Z(p, "fill", "currentColor"), Z(m, "class", "icon"), Z(m, "viewBox", "0 0 23.744 23.745"), Z(m, "id", "pencil"), Z(m, "xmlns", "http://www.w3.org/2000/svg"), Z(f, "class", "button icon-button circle "), Z(f, "href", "."), Z(E, "d", "M15.67 4.446l-.057-.215-.409-1.545a.876.876 0 00-.692-.588l-.034-.005a51.6 51.6 0 00-3.453-.33l-.04.002a.638.638 0 01-.614-.46C10.234.993 9.978.311 9.663.184A1.438 1.438 0 009.448.12C9.39.11 9.331.103 9.272.095a10.745 10.745 0 00-2.867 0C6.348.103 6.288.11 6.23.12a1.225 1.225 0 00-.213.065C5.709.308 5.459.98 5.32 1.28a.634.634 0 01-.62.485c-.011 0-.021 0-.032-.002-1.146.071-2.28.18-3.404.325l-.142.018a.876.876 0 00-.648.581L.065 4.231l-.057.215a.904.904 0 00.874 1.027h13.915a.905.905 0 00.873-1.027zm-1.695 2.69H1.704a.906.906 0 00-.812.859l.02.232 1.005 12.18a.88.88 0 00.869.762h10.107c.44 0 .812-.326.869-.762l1.007-12.18.019-.232a.908.908 0 00-.813-.859z"), Z(E, "fill", "currentColor"), Z(y, "class", "icon"), Z(y, "viewBox", "0 0 15.679 21.169"), Z(y, "id", "trash"), Z(y, "xmlns", "http://www.w3.org/2000/svg"), Z(v, "class", "button icon-button circle "), Z(v, "href", "."), Z(A, "class", "player-card-actions"), Z(t, "class", "player-item is-header theme-caution-color"), Z(t, "id", b = e[0].internalId || e[0].id), re(t, "theme-caution-color", e[6])
         },
         m(h, b) {
-            T(h, t, b), z(t, n), z(n, i), z(t, a), H && H.m(t, null), z(t, r), z(t, l), z(l, o), z(l, s), z(l, c), z(l, u), j && j.m(l, null), z(t, A), z(t, d), z(d, f), z(f, m), z(m, p), z(d, g), z(d, v), z(v, y), z(y, E), T(h, I, b), T(h, w, b), K && K.m(w, null), z(w, C);
+            T(h, t, b), z(t, n), z(n, i), z(t, a), H && H.m(t, null), z(t, r), z(t, l), z(l, o), z(l, s), z(l, c), z(l, u), j && j.m(l, null), z(t, d), z(t, A), z(A, f), z(f, m), z(m, p), z(A, g), z(A, v), z(v, y), z(y, E), T(h, I, b), T(h, w, b), K && K.m(w, null), z(w, C);
             for (let e = 0; e < F.length; e += 1) F[e].m(w, null);
-            T(h, S, b), _e(L, h, b), x = !0, k || (R = [q(n, "dblclick", e[9]), q(f, "click", M(e[11])), q(v, "click", M(e[12]))], k = !0)
+            T(h, S, b), et(L, h, b), x = !0, k || (R = [q(n, "dblclick", e[9]), q(f, "click", M(e[11])), q(v, "click", M(e[12]))], k = !0)
         },
         p(e, [n]) {
-            if ((!x || 1 & n) && V !== (V = e[0].name + "") && ne(i, V), e[7].length ? H ? H.p(e, n) : (H = Dn(e), H.c(), H.m(t, r)) : H && (H.d(1), H = null), (!x || 2 & n) && X !== (X = (e[1].length || "No") + "") && ne(o, X), (!x || 2 & n) && O !== (O = 1 === e[1].length ? "player" : "players") && ne(c, O), e[6] ? j ? j.p(e, n) : (j = Qn(e), j.c(), j.m(l, null)) : j && (j.d(1), j = null), (!x || 1 & n && b !== (b = e[0].internalId || e[0].id)) && Z(t, "id", b), 64 & n && re(t, "theme-caution-color", e[6]), 0 == e[1].length ? K || (K = qn(), K.c(), K.m(w, C)) : K && (K.d(1), K = null), 15 & n) {
-                Y = e[1], ze();
+            if ((!x || 1 & n) && V !== (V = e[0].name + "") && ne(i, V), e[7].length ? H ? H.p(e, n) : (H = Jn(e), H.c(), H.m(t, r)) : H && (H.d(1), H = null), (!x || 2 & n) && X !== (X = (e[1].length || "No") + "") && ne(o, X), (!x || 2 & n) && O !== (O = 1 === e[1].length ? "player" : "players") && ne(c, O), e[6] ? j ? j.p(e, n) : (j = Mn(e), j.c(), j.m(l, null)) : j && (j.d(1), j = null), (!x || 1 & n && b !== (b = e[0].internalId || e[0].id)) && Z(t, "id", b), 64 & n && re(t, "theme-caution-color", e[6]), 0 == e[1].length ? K || (K = Gn(), K.c(), K.m(w, C)) : K && (K.d(1), K = null), 15 & n) {
+                Y = e[1], Te();
                 for (let e = 0; e < F.length; e += 1) F[e].r();
-                F = Ze(F, n, $, 1, e, Y, U, w, Ke, Mn, null, Tn);
+                F = Ye(F, n, $, 1, e, Y, U, w, Ze, $n, null, Wn);
                 for (let e = 0; e < F.length; e += 1) F[e].a();
-                Te()
+                De()
             }
             const a = {};
-            1 & n && (a.team = e[0]), !P && 32 & n && (P = !0, a.open = e[5], Le((() => P = !1))), L.$set(a)
+            1 & n && (a.team = e[0]), !P && 32 & n && (P = !0, a.open = e[5], Pe((() => P = !1))), L.$set(a)
         },
         i(e) {
             if (!x) {
-                for (let e = 0; e < Y.length; e += 1) De(F[e]);
-                e && Se((() => {
-                    B || (B = Je(w, rn, {}, !0)), B.run(1)
-                })), De(L.$$.fragment, e), x = !0
+                for (let e = 0; e < Y.length; e += 1) He(F[e]);
+                e && Le((() => {
+                    B || (B = je(w, un, {}, !0)), B.run(1)
+                })), He(L.$$.fragment, e), x = !0
             }
         },
         o(e) {
-            for (let t = 0; t < F.length; t += 1) He(F[t]);
-            e && (B || (B = Je(w, rn, {}, !1)), B.run(0)), He(L.$$.fragment, e), x = !1
+            for (let t = 0; t < F.length; t += 1) Ne(F[t]);
+            e && (B || (B = je(w, un, {}, !1)), B.run(0)), Ne(L.$$.fragment, e), x = !1
         },
         d(e) {
             e && D(t), H && H.d(), j && j.d(), e && D(I), e && D(w), K && K.d();
             for (let t = 0; t < F.length; t += 1) F[t].d();
-            e && B && B.end(), e && D(S), et(L, e), k = !1, h(R)
+            e && B && B.end(), e && D(S), tt(L, e), k = !1, h(R)
         }
     }
 }
 
-function Zn(e, t, n) {
+function ei(e, t, n) {
     let i, a, r;
-    y(e, lt, (e => n(4, r = e)));
+    y(e, ot, (e => n(4, r = e)));
     let {
         team: l
     } = t, {
         players: o
     } = t, {
         selected: s = []
     } = t, {
         readOnly: c = !1
     } = t, u = !1;
-    const A = ve();
+    const d = ye();
     console.log(l.length);
     return e.$$set = e => {
         "team" in e && n(0, l = e.team), "players" in e && n(1, o = e.players), "selected" in e && n(2, s = e.selected), "readOnly" in e && n(3, c = e.readOnly)
     }, e.$$.update = () => {
         5 & e.$$.dirty && n(7, i = s.filter((e => !l.players.includes(e)))), 18 & e.$$.dirty && n(6, a = o.length && (r.minimumPlayers && o.length < r.minimumPlayers || r.maximumPlayers && o.length > r.maximumPlayers))
-    }, [l, o, s, c, r, u, a, i, A, () => {
+    }, [l, o, s, c, r, u, a, i, d, () => {
         n(5, u = !0)
     }, () => {
-        A("addPlayers")
+        d("addPlayers")
     }, () => {
         n(5, u = !0)
     }, () => {
-        A("delete")
+        d("delete")
     }, function(t) {
-        ye.call(this, e, t)
+        Ee.call(this, e, t)
     }, function(t) {
-        ye.call(this, e, t)
+        Ee.call(this, e, t)
     }, function(t) {
-        ye.call(this, e, t)
+        Ee.call(this, e, t)
     }, function(e) {
         u = e, n(5, u)
     }, () => {
         n(5, u = !1)
     }, e => {
-        A("rename", e.detail), n(5, u = !1)
+        d("rename", e.detail), n(5, u = !1)
     }]
 }
-class Yn extends it {
+class ti extends at {
     constructor(e) {
-        super(), nt(this, e, Zn, Kn, p, {
+        super(), it(this, e, ei, _n, p, {
             team: 0,
             players: 1,
             selected: 2,
             readOnly: 3
         })
     }
 }
 const {
-    Map: Gn
-} = je;
+    Map: ni
+} = qe;
 
-function $n(e, t, n) {
+function ii(e, t, n) {
     const i = e.slice();
     return i[33] = t[n][0], i[34] = t[n][1], i
 }
 
-function _n(e, t, n) {
+function ai(e, t, n) {
     const i = e.slice();
     return i[30] = t[n], i[37] = t, i[38] = n, i
 }
 
-function ei(e, t, n) {
+function ri(e, t, n) {
     const i = e.slice();
     return i[30] = t[n], i[31] = t, i[32] = n, i
 }
 
-function ti(e) {
+function li(e) {
     let t, n, i = [],
-        a = new Gn,
+        a = new ni,
         r = [...e[6]];
     const l = e => e[33];
     for (let o = 0; o < r.length; o += 1) {
-        let t = $n(e, r, o),
+        let t = ii(e, r, o),
             n = l(t);
-        a.set(n, i[o] = oi(n, t))
+        a.set(n, i[o] = Ai(n, t))
     }
     return {
         c() {
             for (let e = 0; e < i.length; e += 1) i[e].c();
             t = j()
         },
         l(e) {
@@ -3633,43 +3766,43 @@
             t = j()
         },
         m(e, a) {
             for (let t = 0; t < i.length; t += 1) i[t].m(e, a);
             T(e, t, a), n = !0
         },
         p(e, n) {
-            31297 & n[0] && (r = [...e[6]], ze(), i = Ze(i, n, l, 1, e, r, a, t.parentNode, Me, oi, t, $n), Te())
+            31297 & n[0] && (r = [...e[6]], Te(), i = Ye(i, n, l, 1, e, r, a, t.parentNode, Ke, Ai, t, ii), De())
         },
         i(e) {
             if (!n) {
-                for (let e = 0; e < r.length; e += 1) De(i[e]);
+                for (let e = 0; e < r.length; e += 1) He(i[e]);
                 n = !0
             }
         },
         o(e) {
-            for (let t = 0; t < i.length; t += 1) He(i[t]);
+            for (let t = 0; t < i.length; t += 1) Ne(i[t]);
             n = !1
         },
         d(e) {
             for (let t = 0; t < i.length; t += 1) i[t].d(e);
             e && D(t)
         }
     }
 }
 
-function ni(e) {
+function oi(e) {
     let t, n, i, a, r, l, o, s, c = e[7].length + "",
         u = [],
-        A = new Gn,
-        d = e[7];
+        d = new ni,
+        A = e[7];
     const f = e => e[30].internalId || e[30].id;
-    for (let h = 0; h < d.length; h += 1) {
-        let t = ei(e, d, h),
+    for (let h = 0; h < A.length; h += 1) {
+        let t = ri(e, A, h),
             n = f(t);
-        A.set(n, u[h] = si(n, t))
+        d.set(n, u[h] = fi(n, t))
     }
     return {
         c() {
             t = N("div"), n = N("p"), i = W("Teams ("), a = W(c), r = W(")"), l = J(), o = N("div");
             for (let e = 0; e < u.length; e += 1) u[e].c();
             this.h()
         },
@@ -3678,134 +3811,134 @@
                 class: !0,
                 id: !0
             });
             var s = G(t);
             n = _(s, "P", {
                 class: !0
             });
-            var A = G(n);
-            i = ee(A, "Teams ("), a = ee(A, c), r = ee(A, ")"), A.forEach(D), s.forEach(D), l = te(e), o = _(e, "DIV", {
+            var d = G(n);
+            i = ee(d, "Teams ("), a = ee(d, c), r = ee(d, ")"), d.forEach(D), s.forEach(D), l = te(e), o = _(e, "DIV", {
                 class: !0
             });
-            var d = G(o);
-            for (let t = 0; t < u.length; t += 1) u[t].l(d);
-            d.forEach(D), this.h()
+            var A = G(o);
+            for (let t = 0; t < u.length; t += 1) u[t].l(A);
+            A.forEach(D), this.h()
         },
         h() {
             Z(n, "class", "walkthrough-chapter-heading"), Z(t, "class", "player-header pad-top"), Z(t, "id", "teams"), Z(o, "class", "team-grid-wrap")
         },
         m(e, c) {
             T(e, t, c), z(t, n), z(n, i), z(n, a), z(n, r), T(e, l, c), T(e, o, c);
             for (let t = 0; t < u.length; t += 1) u[t].m(o, null);
             s = !0
         },
         p(e, t) {
             if ((!s || 128 & t[0]) && c !== (c = e[7].length + "") && ne(a, c), 14984 & t[0]) {
-                d = e[7], ze();
+                A = e[7], Te();
                 for (let e = 0; e < u.length; e += 1) u[e].r();
-                u = Ze(u, t, f, 1, e, d, A, o, Ke, si, null, ei);
+                u = Ye(u, t, f, 1, e, A, d, o, Ze, fi, null, ri);
                 for (let e = 0; e < u.length; e += 1) u[e].a();
-                Te()
+                De()
             }
         },
         i(e) {
             if (!s) {
-                for (let e = 0; e < d.length; e += 1) De(u[e]);
+                for (let e = 0; e < A.length; e += 1) He(u[e]);
                 s = !0
             }
         },
         o(e) {
-            for (let t = 0; t < u.length; t += 1) He(u[t]);
+            for (let t = 0; t < u.length; t += 1) Ne(u[t]);
             s = !1
         },
         d(e) {
             e && D(t), e && D(l), e && D(o);
             for (let t = 0; t < u.length; t += 1) u[t].d()
         }
     }
 }
 
-function ii(e) {
-    let t, n, i, a, r, l, o, s, c, u, A, d, f, h = e[34].length + "",
+function si(e) {
+    let t, n, i, a, r, l, o, s, c, u, d, A, f, h = e[34].length + "",
         m = 1 == e[34].length ? "team" : "teams",
         p = [],
-        g = new Gn;
+        g = new ni;
 
     function v(e, t) {
-        return e[33] ? ri : ai
+        return e[33] ? ui : ci
     }
     let y = v(e),
         E = y(e),
         b = e[34];
     const I = e => e[30].internalId || e[30].id;
     for (let w = 0; w < b.length; w += 1) {
-        let t = _n(e, b, w),
+        let t = ai(e, b, w),
             n = I(t);
-        g.set(n, p[w] = li(n, t))
+        g.set(n, p[w] = di(n, t))
     }
     return {
         c() {
             t = N("div"), n = N("div"), i = N("h3"), E.c(), a = W("\n          ("), r = W(h), l = J(), o = W(m), s = W(")"), u = J();
             for (let e = 0; e < p.length; e += 1) p[e].c();
-            A = J(), this.h()
+            d = J(), this.h()
         },
         l(e) {
             t = _(e, "DIV", {
                 class: !0
             });
             var c = G(t);
             n = _(c, "DIV", {
                 id: !0,
                 class: !0
             });
-            var d = G(n);
-            i = _(d, "H3", {
+            var A = G(n);
+            i = _(A, "H3", {
                 class: !0
             });
             var f = G(i);
-            E.l(f), f.forEach(D), a = ee(d, "\n          ("), r = ee(d, h), l = te(d), o = ee(d, m), s = ee(d, ")"), d.forEach(D), u = te(c);
+            E.l(f), f.forEach(D), a = ee(A, "\n          ("), r = ee(A, h), l = te(A), o = ee(A, m), s = ee(A, ")"), A.forEach(D), u = te(c);
             for (let t = 0; t < p.length; t += 1) p[t].l(c);
-            A = te(c), c.forEach(D), this.h()
+            d = te(c), c.forEach(D), this.h()
         },
         h() {
             Z(i, "class", "svelte-gwov2v"), Z(n, "id", c = `session-${e[33]}`), Z(n, "class", "card-header"), Z(t, "class", "card well")
         },
         m(e, c) {
             T(e, t, c), z(t, n), z(n, i), E.m(i, null), z(n, a), z(n, r), z(n, l), z(n, o), z(n, s), z(t, u);
             for (let n = 0; n < p.length; n += 1) p[n].m(t, null);
-            z(t, A), f = !0
+            z(t, d), f = !0
         },
         p(e, a) {
-            y === (y = v(e)) && E ? E.p(e, a) : (E.d(1), E = y(e), E && (E.c(), E.m(i, null))), (!f || 64 & a[0]) && h !== (h = e[34].length + "") && ne(r, h), (!f || 64 & a[0]) && m !== (m = 1 == e[34].length ? "team" : "teams") && ne(o, m), (!f || 64 & a[0] && c !== (c = `session-${e[33]}`)) && Z(n, "id", c), 14912 & a[0] && (b = e[34], ze(), p = Ze(p, a, I, 1, e, b, g, t, Me, li, A, _n), Te())
+            y === (y = v(e)) && E ? E.p(e, a) : (E.d(1), E = y(e), E && (E.c(), E.m(i, null))), (!f || 64 & a[0]) && h !== (h = e[34].length + "") && ne(r, h), (!f || 64 & a[0]) && m !== (m = 1 == e[34].length ? "team" : "teams") && ne(o, m), (!f || 64 & a[0] && c !== (c = `session-${e[33]}`)) && Z(n, "id", c), 14912 & a[0] && (b = e[34], Te(), p = Ye(p, a, I, 1, e, b, g, t, Ke, di, d, ai), De())
         },
         i(e) {
             if (!f) {
-                for (let e = 0; e < b.length; e += 1) De(p[e]);
-                e && Se((() => {
-                    d || (d = Je(t, rn, {
+                for (let e = 0; e < b.length; e += 1) He(p[e]);
+                e && Le((() => {
+                    A || (A = je(t, un, {
                         duration: 200
-                    }, !0)), d.run(1)
+                    }, !0)), A.run(1)
                 })), f = !0
             }
         },
         o(e) {
-            for (let t = 0; t < p.length; t += 1) He(p[t]);
-            e && (d || (d = Je(t, rn, {
+            for (let t = 0; t < p.length; t += 1) Ne(p[t]);
+            e && (A || (A = je(t, un, {
                 duration: 200
-            }, !1)), d.run(0)), f = !1
+            }, !1)), A.run(0)), f = !1
         },
         d(e) {
             e && D(t), E.d();
             for (let t = 0; t < p.length; t += 1) p[t].d();
-            e && d && d.end()
+            e && A && A.end()
         }
     }
 }
 
-function ai(e) {
+function ci(e) {
     let t, n;
     return {
         c() {
             t = N("em"), n = W("No Session Group")
         },
         l(e) {
             t = _(e, "EM", {});
@@ -3818,15 +3951,15 @@
         p: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function ri(e) {
+function ui(e) {
     let t, n, i, a, r = e[14](e[33]) + "";
 
     function l() {
         return e[21](e[33])
     }
     return {
         c() {
@@ -3850,17 +3983,17 @@
         },
         d(e) {
             e && D(t), i = !1, a()
         }
     }
 }
 
-function li(e, t) {
+function di(e, t) {
     let n, i, a, r;
-    return i = new Yn({
+    return i = new ti({
         props: {
             team: t[30],
             players: t[30].players.map(t[22]),
             readOnly: !0
         }
     }), i.$on("delete", (function() {
         return t[23](t[30])
@@ -3870,54 +4003,54 @@
         return t[25](t[30], ...e)
     })), i.$on("unassignPlayer", (function(...e) {
         return t[26](t[30], t[37], t[38], ...e)
     })), {
         key: e,
         first: null,
         c() {
-            n = N("div"), Ge(i.$$.fragment), this.h()
+            n = N("div"), $e(i.$$.fragment), this.h()
         },
         l(e) {
             n = _(e, "DIV", {
                 class: !0
             });
             var t = G(n);
-            $e(i.$$.fragment, t), t.forEach(D), this.h()
+            _e(i.$$.fragment, t), t.forEach(D), this.h()
         },
         h() {
             Z(n, "class", "card player-card team-card"), this.first = n
         },
         m(e, t) {
-            T(e, n, t), _e(i, n, null), r = !0
+            T(e, n, t), et(i, n, null), r = !0
         },
         p(e, n) {
             t = e;
             const a = {};
             64 & n[0] && (a.team = t[30]), 576 & n[0] && (a.players = t[30].players.map(t[22])), i.$set(a)
         },
         i(e) {
-            r || (De(i.$$.fragment, e), e && Se((() => {
-                a || (a = Je(n, an, {
+            r || (He(i.$$.fragment, e), e && Le((() => {
+                a || (a = je(n, cn, {
                     duration: 200
                 }, !0)), a.run(1)
             })), r = !0)
         },
         o(e) {
-            He(i.$$.fragment, e), e && (a || (a = Je(n, an, {
+            Ne(i.$$.fragment, e), e && (a || (a = je(n, cn, {
                 duration: 200
             }, !1)), a.run(0)), r = !1
         },
         d(e) {
-            e && D(n), et(i), e && a && a.end()
+            e && D(n), tt(i), e && a && a.end()
         }
     }
 }
 
-function oi(e, t) {
-    let n, i, a, r = t[34].length && ii(t);
+function Ai(e, t) {
+    let n, i, a, r = t[34].length && si(t);
     return {
         key: e,
         first: null,
         c() {
             n = j(), r && r.c(), i = j(), this.h()
         },
         l(e) {
@@ -3926,33 +4059,33 @@
         h() {
             this.first = n
         },
         m(e, t) {
             T(e, n, t), r && r.m(e, t), T(e, i, t), a = !0
         },
         p(e, n) {
-            (t = e)[34].length ? r ? (r.p(t, n), 64 & n[0] && De(r, 1)) : (r = ii(t), r.c(), De(r, 1), r.m(i.parentNode, i)) : r && (ze(), He(r, 1, 1, (() => {
+            (t = e)[34].length ? r ? (r.p(t, n), 64 & n[0] && He(r, 1)) : (r = si(t), r.c(), He(r, 1), r.m(i.parentNode, i)) : r && (Te(), Ne(r, 1, 1, (() => {
                 r = null
-            })), Te())
+            })), De())
         },
         i(e) {
-            a || (De(r), a = !0)
+            a || (He(r), a = !0)
         },
         o(e) {
-            He(r), a = !1
+            Ne(r), a = !1
         },
         d(e) {
             e && D(n), r && r.d(e), e && D(i)
         }
     }
 }
 
-function si(e, t) {
+function fi(e, t) {
     let n, i, a, r, l, o, s = c;
-    return i = new Yn({
+    return i = new ti({
         props: {
             team: t[30],
             players: t[30].players.map(t[15]).filter(Boolean),
             selected: t[3]
         }
     }), i.$on("selectPlayer", t[16]), i.$on("delete", (function() {
         return t[17](t[30])
@@ -3962,188 +4095,188 @@
         return t[19](t[30], ...e)
     })), i.$on("unassignPlayer", (function(...e) {
         return t[20](t[30], t[31], t[32], ...e)
     })), {
         key: e,
         first: null,
         c() {
-            n = N("div"), Ge(i.$$.fragment), a = J(), this.h()
+            n = N("div"), $e(i.$$.fragment), a = J(), this.h()
         },
         l(e) {
             n = _(e, "DIV", {
                 class: !0
             });
             var t = G(n);
-            $e(i.$$.fragment, t), a = te(t), t.forEach(D), this.h()
+            _e(i.$$.fragment, t), a = te(t), t.forEach(D), this.h()
         },
         h() {
             Z(n, "class", "card player-card glow-shadow team-card"), this.first = n
         },
         m(e, t) {
-            T(e, n, t), _e(i, n, null), z(n, a), o = !0
+            T(e, n, t), et(i, n, null), z(n, a), o = !0
         },
         p(e, n) {
             t = e;
             const a = {};
             128 & n[0] && (a.team = t[30]), 640 & n[0] && (a.players = t[30].players.map(t[15]).filter(Boolean)), 8 & n[0] && (a.selected = t[3]), i.$set(a)
         },
         r() {
             l = n.getBoundingClientRect()
         },
         f() {
             fe(n), s(), he(n, l)
         },
         a() {
-            s(), s = de(n, l, qt, {
+            s(), s = Ae(n, l, Mt, {
                 duration: 400
             })
         },
         i(e) {
-            o || (De(i.$$.fragment, e), e && Se((() => {
-                r || (r = Je(n, an, {
+            o || (He(i.$$.fragment, e), e && Le((() => {
+                r || (r = je(n, cn, {
                     duration: 200
                 }, !0)), r.run(1)
             })), o = !0)
         },
         o(e) {
-            He(i.$$.fragment, e), e && (r || (r = Je(n, an, {
+            Ne(i.$$.fragment, e), e && (r || (r = je(n, cn, {
                 duration: 200
             }, !1)), r.run(0)), o = !1
         },
         d(e) {
-            e && D(n), et(i), e && r && r.end()
+            e && D(n), tt(i), e && r && r.end()
         }
     }
 }
 
-function ci(e) {
+function hi(e) {
     let t, n;
-    return t = new Xn({
+    return t = new Tn({
         props: {
             showAutoBalance: e[5]
         }
     }), t.$on("clickCreateTeam", e[27]), t.$on("openAutoBalance", e[28]), {
         c() {
-            Ge(t.$$.fragment)
+            $e(t.$$.fragment)
         },
         l(e) {
-            $e(t.$$.fragment, e)
+            _e(t.$$.fragment, e)
         },
         m(e, i) {
-            _e(t, e, i), n = !0
+            et(t, e, i), n = !0
         },
         p(e, n) {
             const i = {};
             32 & n[0] && (i.showAutoBalance = e[5]), t.$set(i)
         },
         i(e) {
-            n || (De(t.$$.fragment, e), n = !0)
+            n || (He(t.$$.fragment, e), n = !0)
         },
         o(e) {
-            He(t.$$.fragment, e), n = !1
+            Ne(t.$$.fragment, e), n = !1
         },
         d(e) {
-            et(t, e)
+            tt(t, e)
         }
     }
 }
 
-function ui(e) {
+function mi(e) {
     let t, n, i, a, r, l;
-    const o = [ni, ti],
+    const o = [oi, li],
         s = [];
 
     function c(e, t) {
         return e[8] ? 1 : 0
     }
 
     function u(t) {
         e[29](t)
     }
     t = c(e), n = s[t] = o[t](e);
-    let A = {
+    let d = {
         $$slots: {
-            default: [ci]
+            default: [hi]
         },
         $$scope: {
             ctx: e
         }
     };
-    return void 0 !== e[10] && (A.open = e[10]), a = new Pt({
-        props: A
-    }), be.push((() => Ye(a, "open", u))), {
+    return void 0 !== e[10] && (d.open = e[10]), a = new xt({
+        props: d
+    }), Ie.push((() => Ge(a, "open", u))), {
         c() {
-            n.c(), i = J(), Ge(a.$$.fragment)
+            n.c(), i = J(), $e(a.$$.fragment)
         },
         l(e) {
-            n.l(e), i = te(e), $e(a.$$.fragment, e)
+            n.l(e), i = te(e), _e(a.$$.fragment, e)
         },
         m(e, n) {
-            s[t].m(e, n), T(e, i, n), _e(a, e, n), l = !0
+            s[t].m(e, n), T(e, i, n), et(a, e, n), l = !0
         },
         p(e, l) {
             let u = t;
-            t = c(e), t === u ? s[t].p(e, l) : (ze(), He(s[u], 1, 1, (() => {
+            t = c(e), t === u ? s[t].p(e, l) : (Te(), Ne(s[u], 1, 1, (() => {
                 s[u] = null
-            })), Te(), n = s[t], n ? n.p(e, l) : (n = s[t] = o[t](e), n.c()), De(n, 1), n.m(i.parentNode, i));
-            const A = {};
-            1586 & l[0] | 256 & l[1] && (A.$$scope = {
+            })), De(), n = s[t], n ? n.p(e, l) : (n = s[t] = o[t](e), n.c()), He(n, 1), n.m(i.parentNode, i));
+            const d = {};
+            1586 & l[0] | 256 & l[1] && (d.$$scope = {
                 dirty: l,
                 ctx: e
-            }), !r && 1024 & l[0] && (r = !0, A.open = e[10], Le((() => r = !1))), a.$set(A)
+            }), !r && 1024 & l[0] && (r = !0, d.open = e[10], Pe((() => r = !1))), a.$set(d)
         },
         i(e) {
-            l || (De(n), De(a.$$.fragment, e), l = !0)
+            l || (He(n), He(a.$$.fragment, e), l = !0)
         },
         o(e) {
-            He(n), He(a.$$.fragment, e), l = !1
+            Ne(n), Ne(a.$$.fragment, e), l = !1
         },
         d(e) {
-            s[t].d(e), e && D(i), et(a, e)
+            s[t].d(e), e && D(i), tt(a, e)
         }
     }
 }
 
-function Ai(e, t, n) {
+function pi(e, t, n) {
     let i, a, r, l = c,
         o = () => (l(), l = v(s, (e => n(9, r = e))), s);
     e.$$.on_destroy.push((() => l()));
     let {
         data: s
     } = t;
     o();
     let {
         currentSession: u
     } = t, {
-        currentSessionSelected: A
+        currentSessionSelected: d
     } = t, {
-        createTeam: d
+        createTeam: A
     } = t, {
         showDialog: f
     } = t, {
         showAutoBalance: h
     } = t;
-    const m = ve();
+    const m = ye();
     let p, g = new Map;
 
     function y(e) {
         B(s, r.teams = r.teams.filter((t => t !== e)), r)
     }
 
     function E(e, t) {
         e.detail.name && (t.name = e.detail.name, s.set(r))
     }
     return e.$$set = e => {
-        "data" in e && o(n(2, s = e.data)), "currentSession" in e && n(0, u = e.currentSession), "currentSessionSelected" in e && n(3, A = e.currentSessionSelected), "createTeam" in e && n(4, d = e.createTeam), "showDialog" in e && n(1, f = e.showDialog), "showAutoBalance" in e && n(5, h = e.showAutoBalance)
+        "data" in e && o(n(2, s = e.data)), "currentSession" in e && n(0, u = e.currentSession), "currentSessionSelected" in e && n(3, d = e.currentSessionSelected), "createTeam" in e && n(4, A = e.createTeam), "showDialog" in e && n(1, f = e.showDialog), "showAutoBalance" in e && n(5, h = e.showAutoBalance)
     }, e.$$.update = () => {
         1 & e.$$.dirty[0] && n(8, i = null === u), 769 & e.$$.dirty[0] && n(7, a = i ? r.teams : r.teams.filter((e => !e.session || e.session === u || void 0 === u))), 960 & e.$$.dirty[0] && i && (n(6, g = new Map), r.sessions.forEach((e => g.set(e, []))), a.forEach((e => {
             e.players.length && (g.has(e.session) || g.set(e.session, []), g.get(e.session).push(e))
         })))
-    }, [u, f, s, A, d, h, g, a, i, r, p, m, y, E, e => r.sessions.find((t => t.id === e)).name, e => r.players.find((t => t.id === e)), function(t) {
-        ye.call(this, e, t)
+    }, [u, f, s, d, A, h, g, a, i, r, p, m, y, E, e => r.sessions.find((t => t.id === e)).name, e => r.players.find((t => t.id === e)), function(t) {
+        Ee.call(this, e, t)
     }, e => {
         y(e)
     }, (e, t) => {
         E(t, e)
     }, (e, t) => {
         const n = t.detail || {
             team: e
@@ -4161,94 +4294,94 @@
         const n = t.detail || {
             team: e
         };
         m("addPlayers", n)
     }, (e, t, i, a) => {
         n(6, t[i].players = e.players.filter((e => e !== a.detail.id)), g), s.set(r)
     }, () => {
-        const e = d();
+        const e = A();
         m("addPlayers", {
             team: e,
             onlyUnassigned: !0
         }), B(s, r.teams = [e, ...r.teams], r), n(10, p = !1)
     }, () => {
         n(1, f = !0), n(10, p = !1)
     }, function(e) {
         p = e, n(10, p)
     }]
 }
-class di extends it {
+class gi extends at {
     constructor(e) {
-        super(), nt(this, e, Ai, ui, p, {
+        super(), it(this, e, pi, mi, p, {
             data: 2,
             currentSession: 0,
             currentSessionSelected: 3,
             createTeam: 4,
             showDialog: 1,
             showAutoBalance: 5
         }, null, [-1, -1])
     }
 }
 
-function fi(e, t, n) {
+function vi(e, t, n) {
     const i = e.slice();
     return i[36] = t[n], i
 }
 
-function hi(e, t, n) {
+function yi(e, t, n) {
     const i = e.slice();
     return i[39] = t[n], i
 }
 
-function mi(e, t, n) {
+function Ei(e, t, n) {
     const i = e.slice();
     return i[42] = t[n], i
 }
 
-function pi(e) {
+function bi(e) {
     let t, n;
-    return t = new Nt({
+    return t = new Qt({
         props: {
             $$slots: {
-                default: [yi]
+                default: [Ci]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), {
         c() {
-            Ge(t.$$.fragment)
+            $e(t.$$.fragment)
         },
         l(e) {
-            $e(t.$$.fragment, e)
+            _e(t.$$.fragment, e)
         },
         m(e, i) {
-            _e(t, e, i), n = !0
+            et(t, e, i), n = !0
         },
         p(e, n) {
             const i = {};
             8206 & n[0] | 16384 & n[1] && (i.$$scope = {
                 dirty: n,
                 ctx: e
             }), t.$set(i)
         },
         i(e) {
-            n || (De(t.$$.fragment, e), n = !0)
+            n || (He(t.$$.fragment, e), n = !0)
         },
         o(e) {
-            He(t.$$.fragment, e), n = !1
+            Ne(t.$$.fragment, e), n = !1
         },
         d(e) {
-            et(t, e)
+            tt(t, e)
         }
     }
 }
 
-function gi(e) {
+function Ii(e) {
     let t, n = (e[42] ? e[42].name : "Summary") + "";
     return {
         c() {
             t = W(n)
         },
         l(e) {
             t = ee(e, n)
@@ -4261,82 +4394,82 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function vi(e, t) {
+function wi(e, t) {
     var n, i, a;
     let r, l, o, s;
 
     function c(e) {
         t[20](e)
     }
     let u = {
-        badge: t[2][null == (n = t[42]) ? void 0 : n.id] && t[2][null == (i = t[42]) ? void 0 : i.id].filter(Fi).length || null,
+        badge: t[2][null == (n = t[42]) ? void 0 : n.id] && t[2][null == (i = t[42]) ? void 0 : i.id].filter(Hi).length || null,
         outline: !t[42] && !t[3].length,
         value: (null == (a = t[42]) ? void 0 : a.id) || null,
         $$slots: {
-            default: [gi]
+            default: [Ii]
         },
         $$scope: {
             ctx: t
         }
     };
-    return void 0 !== t[1] && (u.state = t[1]), l = new Jt({
+    return void 0 !== t[1] && (u.state = t[1]), l = new jt({
         props: u
-    }), be.push((() => Ye(l, "state", c))), {
+    }), Ie.push((() => Ge(l, "state", c))), {
         key: e,
         first: null,
         c() {
-            r = j(), Ge(l.$$.fragment), this.h()
+            r = j(), $e(l.$$.fragment), this.h()
         },
         l(e) {
-            r = j(), $e(l.$$.fragment, e), this.h()
+            r = j(), _e(l.$$.fragment, e), this.h()
         },
         h() {
             this.first = r
         },
         m(e, t) {
-            T(e, r, t), _e(l, e, t), s = !0
+            T(e, r, t), et(l, e, t), s = !0
         },
         p(e, n) {
             var i, a, r;
             t = e;
             const s = {};
-            8196 & n[0] && (s.badge = t[2][null == (i = t[42]) ? void 0 : i.id] && t[2][null == (a = t[42]) ? void 0 : a.id].filter(Fi).length || null), 8200 & n[0] && (s.outline = !t[42] && !t[3].length), 8192 & n[0] && (s.value = (null == (r = t[42]) ? void 0 : r.id) || null), 8192 & n[0] | 16384 & n[1] && (s.$$scope = {
+            8196 & n[0] && (s.badge = t[2][null == (i = t[42]) ? void 0 : i.id] && t[2][null == (a = t[42]) ? void 0 : a.id].filter(Hi).length || null), 8200 & n[0] && (s.outline = !t[42] && !t[3].length), 8192 & n[0] && (s.value = (null == (r = t[42]) ? void 0 : r.id) || null), 8192 & n[0] | 16384 & n[1] && (s.$$scope = {
                 dirty: n,
                 ctx: t
-            }), !o && 2 & n[0] && (o = !0, s.state = t[1], Le((() => o = !1))), l.$set(s)
+            }), !o && 2 & n[0] && (o = !0, s.state = t[1], Pe((() => o = !1))), l.$set(s)
         },
         i(e) {
-            s || (De(l.$$.fragment, e), s = !0)
+            s || (He(l.$$.fragment, e), s = !0)
         },
         o(e) {
-            He(l.$$.fragment, e), s = !1
+            Ne(l.$$.fragment, e), s = !1
         },
         d(e) {
-            e && D(r), et(l, e)
+            e && D(r), tt(l, e)
         }
     }
 }
 
-function yi(e) {
+function Ci(e) {
     let t, n, i = [],
         a = new Map,
         r = e[13];
     const l = e => {
         var t;
         return null == (t = e[42]) ? void 0 : t.id
     };
     for (let o = 0; o < r.length; o += 1) {
-        let t = mi(e, r, o),
+        let t = Ei(e, r, o),
             n = l(t);
-        a.set(n, i[o] = vi(n, t))
+        a.set(n, i[o] = wi(n, t))
     }
     return {
         c() {
             for (let e = 0; e < i.length; e += 1) i[e].c();
             t = j()
         },
         l(e) {
@@ -4344,38 +4477,38 @@
             t = j()
         },
         m(e, a) {
             for (let t = 0; t < i.length; t += 1) i[t].m(e, a);
             T(e, t, a), n = !0
         },
         p(e, n) {
-            8206 & n[0] && (r = e[13], ze(), i = Ze(i, n, l, 1, e, r, a, t.parentNode, Me, vi, t, mi), Te())
+            8206 & n[0] && (r = e[13], Te(), i = Ye(i, n, l, 1, e, r, a, t.parentNode, Ke, wi, t, Ei), De())
         },
         i(e) {
             if (!n) {
-                for (let e = 0; e < r.length; e += 1) De(i[e]);
+                for (let e = 0; e < r.length; e += 1) He(i[e]);
                 n = !0
             }
         },
         o(e) {
-            for (let t = 0; t < i.length; t += 1) He(i[t]);
+            for (let t = 0; t < i.length; t += 1) Ne(i[t]);
             n = !1
         },
         d(e) {
             for (let t = 0; t < i.length; t += 1) i[t].d(e);
             e && D(t)
         }
     }
 }
 
-function Ei(e) {
+function Bi(e) {
     let t, n, i, a, r;
 
     function l(e, t) {
-        return e[5] && null !== e[1] ? Ci : Bi
+        return e[5] && null !== e[1] ? xi : ki
     }
     let o = l(e),
         s = o(e);
     return {
         c() {
             t = N("div"), n = Q("svg"), i = Q("path"), a = J(), r = N("p"), s.c(), this.h()
         },
@@ -4412,34 +4545,34 @@
         o: c,
         d(e) {
             e && D(t), s.d()
         }
     }
 }
 
-function bi(e) {
+function Si(e) {
     let t, n, i, a, r, l, o, s, u;
     return {
         c() {
             t = N("div"), n = N("h3"), i = W("There are no players registered."), a = J(), r = N("p"), l = W("Once players have accepted their invitation from the marketplace, they\n          will appear in this list."), o = J(), s = N("p"), u = W("All unassigned players must either be assigned to teams or made\n          inactive before the game may begin."), this.h()
         },
         l(e) {
             t = _(e, "DIV", {
                 class: !0
             });
             var c = G(t);
             n = _(c, "H3", {
                 class: !0
             });
-            var A = G(n);
-            i = ee(A, "There are no players registered."), A.forEach(D), a = te(c), r = _(c, "P", {
+            var d = G(n);
+            i = ee(d, "There are no players registered."), d.forEach(D), a = te(c), r = _(c, "P", {
                 class: !0
             });
-            var d = G(r);
-            l = ee(d, "Once players have accepted their invitation from the marketplace, they\n          will appear in this list."), d.forEach(D), o = te(c), s = _(c, "P", {
+            var A = G(r);
+            l = ee(A, "Once players have accepted their invitation from the marketplace, they\n          will appear in this list."), A.forEach(D), o = te(c), s = _(c, "P", {
                 class: !0
             });
             var f = G(s);
             u = ee(f, "All unassigned players must either be assigned to teams or made\n          inactive before the game may begin."), f.forEach(D), c.forEach(D), this.h()
         },
         h() {
             Z(n, "class", "card-heading text-center"), Z(r, "class", "text-center"), Z(s, "class", "text-center"), Z(t, "class", "all-players-managed")
@@ -4452,18 +4585,18 @@
         o: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Ii(e) {
+function Li(e) {
     let t, n, i, a, r = e[11],
         l = [];
-    for (let o = 0; o < r.length; o += 1) l[o] = Ri(hi(e, r, o));
+    for (let o = 0; o < r.length; o += 1) l[o] = Ui(yi(e, r, o));
     return {
         c() {
             t = N("div"), n = Q("svg"), i = Q("path"), a = J();
             for (let e = 0; e < l.length; e += 1) l[e].c();
             this.h()
         },
         l(e) {
@@ -4494,71 +4627,71 @@
             T(e, t, r), z(t, n), z(n, i), z(t, a);
             for (let n = 0; n < l.length; n += 1) l[n].m(t, null)
         },
         p(e, n) {
             if (2112 & n[0]) {
                 let i;
                 for (r = e[11], i = 0; i < r.length; i += 1) {
-                    const a = hi(e, r, i);
-                    l[i] ? l[i].p(a, n) : (l[i] = Ri(a), l[i].c(), l[i].m(t, null))
+                    const a = yi(e, r, i);
+                    l[i] ? l[i].p(a, n) : (l[i] = Ui(a), l[i].c(), l[i].m(t, null))
                 }
                 for (; i < l.length; i += 1) l[i].d(1);
                 l.length = r.length
             }
         },
         i: c,
         o: c,
         d(e) {
             e && D(t), H(l, e)
         }
     }
 }
 
-function wi(e) {
+function Pi(e) {
     let t, n, i;
-    return n = new mn({
+    return n = new En({
         props: {
             selected: e[4],
             players: e[12],
             unassignedIsError: e[5] && null === e[1]
         }
     }), n.$on("selectPlayer", e[23]), n.$on("addPlayers", e[24]), {
         c() {
-            t = N("div"), Ge(n.$$.fragment), this.h()
+            t = N("div"), $e(n.$$.fragment), this.h()
         },
         l(e) {
             t = _(e, "DIV", {
                 class: !0
             });
             var i = G(t);
-            $e(n.$$.fragment, i), i.forEach(D), this.h()
+            _e(n.$$.fragment, i), i.forEach(D), this.h()
         },
         h() {
             Z(t, "class", "player-col")
         },
         m(e, a) {
-            T(e, t, a), _e(n, t, null), i = !0
+            T(e, t, a), et(n, t, null), i = !0
         },
         p(e, t) {
             const i = {};
             16 & t[0] && (i.selected = e[4]), 4096 & t[0] && (i.players = e[12]), 34 & t[0] && (i.unassignedIsError = e[5] && null === e[1]), n.$set(i)
         },
         i(e) {
-            i || (De(n.$$.fragment, e), i = !0)
+            i || (He(n.$$.fragment, e), i = !0)
         },
         o(e) {
-            He(n.$$.fragment, e), i = !1
+            Ne(n.$$.fragment, e), i = !1
         },
         d(e) {
-            e && D(t), et(n)
+            e && D(t), tt(n)
         }
     }
 }
 
-function Ci(e) {
+function xi(e) {
     let t;
     return {
         c() {
             t = W("All players are assigned for this session group.")
         },
         l(e) {
             t = ee(e, "All players are assigned for this session group.")
@@ -4569,19 +4702,19 @@
         p: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Bi(e) {
+function ki(e) {
     let t;
 
     function n(e, t) {
-        return e[10].length ? Li : Si
+        return e[10].length ? Vi : Ri
     }
     let i = n(e),
         a = i(e);
     return {
         c() {
             a.c(), t = j()
         },
@@ -4596,15 +4729,15 @@
         },
         d(e) {
             a.d(e), e && D(t)
         }
     }
 }
 
-function Si(e) {
+function Ri(e) {
     let t;
     return {
         c() {
             t = W("All players are assigned to teams.")
         },
         l(e) {
             t = ee(e, "All players are assigned to teams.")
@@ -4614,15 +4747,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Li(e) {
+function Vi(e) {
     let t, n, i, a;
     return {
         c() {
             t = W("All players are assigned to teams or marked "), n = N("a"), i = W("Inactive"), a = W("."), this.h()
         },
         l(e) {
             t = ee(e, "All players are assigned to teams or marked "), n = _(e, "A", {
@@ -4639,15 +4772,15 @@
         },
         d(e) {
             e && D(t), e && D(n), e && D(a)
         }
     }
 }
 
-function Pi(e) {
+function Xi(e) {
     let t, n, i, a, r, l, o = e[39].name + "",
         s = e[6].maximumPlayers + "";
     return {
         c() {
             t = N("strong"), n = W(o), i = W(" must have\n              "), a = N("strong"), r = W(s), l = W(" players to begin.")
         },
         l(e) {
@@ -4665,44 +4798,44 @@
         },
         d(e) {
             e && D(t), e && D(i), e && D(a), e && D(l)
         }
     }
 }
 
-function xi(e) {
+function Oi(e) {
     let t, n, i, a, r, l, o, s, c, u = e[39].name + "",
-        A = e[6].minimumPlayers + "",
-        d = e[6].maximumPlayers + "";
+        d = e[6].minimumPlayers + "",
+        A = e[6].maximumPlayers + "";
     return {
         c() {
-            t = N("strong"), n = W(u), i = W(" must have\n              "), a = N("strong"), r = W(A), l = W("\n              to\n              "), o = N("strong"), s = W(d), c = W(" players to begin.")
+            t = N("strong"), n = W(u), i = W(" must have\n              "), a = N("strong"), r = W(d), l = W("\n              to\n              "), o = N("strong"), s = W(A), c = W(" players to begin.")
         },
         l(e) {
             t = _(e, "STRONG", {});
             var f = G(t);
             n = ee(f, u), f.forEach(D), i = ee(e, " must have\n              "), a = _(e, "STRONG", {});
             var h = G(a);
-            r = ee(h, A), h.forEach(D), l = ee(e, "\n              to\n              "), o = _(e, "STRONG", {});
+            r = ee(h, d), h.forEach(D), l = ee(e, "\n              to\n              "), o = _(e, "STRONG", {});
             var m = G(o);
-            s = ee(m, d), m.forEach(D), c = ee(e, " players to begin.")
+            s = ee(m, A), m.forEach(D), c = ee(e, " players to begin.")
         },
         m(e, u) {
             T(e, t, u), z(t, n), T(e, i, u), T(e, a, u), z(a, r), T(e, l, u), T(e, o, u), z(o, s), T(e, c, u)
         },
         p(e, t) {
-            2048 & t[0] && u !== (u = e[39].name + "") && ne(n, u), 64 & t[0] && A !== (A = e[6].minimumPlayers + "") && ne(r, A), 64 & t[0] && d !== (d = e[6].maximumPlayers + "") && ne(s, d)
+            2048 & t[0] && u !== (u = e[39].name + "") && ne(n, u), 64 & t[0] && d !== (d = e[6].minimumPlayers + "") && ne(r, d), 64 & t[0] && A !== (A = e[6].maximumPlayers + "") && ne(s, A)
         },
         d(e) {
             e && D(t), e && D(i), e && D(a), e && D(l), e && D(o), e && D(c)
         }
     }
 }
 
-function ki(e) {
+function Fi(e) {
     let t, n, i, a, r, l, o = e[39].name + "",
         s = e[6].minimumPlayers + "";
     return {
         c() {
             t = N("strong"), n = W(o), i = W(" must have\n              "), a = N("strong"), r = W(s), l = W(" players to begin.")
         },
         l(e) {
@@ -4720,19 +4853,19 @@
         },
         d(e) {
             e && D(t), e && D(i), e && D(a), e && D(l)
         }
     }
 }
 
-function Ri(e) {
+function Ui(e) {
     let t, n;
 
     function i(e, t) {
-        return !e[6].minimumPlayers || e[6].maximumPlayers && e[6].maximumPlayers !== e[6].minimumPlayers ? e[6].minimumPlayers && e[6].maximumPlayers ? xi : Pi : ki
+        return !e[6].minimumPlayers || e[6].maximumPlayers && e[6].maximumPlayers !== e[6].minimumPlayers ? e[6].minimumPlayers && e[6].maximumPlayers ? Oi : Xi : Fi
     }
     let a = i(e),
         r = a(e);
     return {
         c() {
             t = N("p"), r.c(), n = J(), this.h()
         },
@@ -4754,227 +4887,227 @@
         },
         d(e) {
             e && D(t), r.d()
         }
     }
 }
 
-function Vi(e) {
+function zi(e) {
     let t, n, i, a, r;
-    return i = new mn({
+    return i = new En({
         props: {
             inactive: !0,
             selected: e[4],
             players: e[10],
             unassignedIsError: e[5] && null === e[1]
         }
     }), i.$on("selectPlayer", e[33]), i.$on("addPlayers", e[34]), {
         c() {
-            t = N("div"), n = N("div"), Ge(i.$$.fragment), a = J(), this.h()
+            t = N("div"), n = N("div"), $e(i.$$.fragment), a = J(), this.h()
         },
         l(e) {
             t = _(e, "DIV", {
                 class: !0
             });
             var r = G(t);
             n = _(r, "DIV", {
                 class: !0
             });
             var l = G(n);
-            $e(i.$$.fragment, l), l.forEach(D), a = te(r), r.forEach(D), this.h()
+            _e(i.$$.fragment, l), l.forEach(D), a = te(r), r.forEach(D), this.h()
         },
         h() {
             Z(n, "class", "player-col"), Z(t, "class", "player-grid")
         },
         m(e, l) {
-            T(e, t, l), z(t, n), _e(i, n, null), z(t, a), r = !0
+            T(e, t, l), z(t, n), et(i, n, null), z(t, a), r = !0
         },
         p(e, t) {
             const n = {};
             16 & t[0] && (n.selected = e[4]), 1024 & t[0] && (n.players = e[10]), 34 & t[0] && (n.unassignedIsError = e[5] && null === e[1]), i.$set(n)
         },
         i(e) {
-            r || (De(i.$$.fragment, e), r = !0)
+            r || (He(i.$$.fragment, e), r = !0)
         },
         o(e) {
-            He(i.$$.fragment, e), r = !1
+            Ne(i.$$.fragment, e), r = !1
         },
         d(e) {
-            e && D(t), et(i)
+            e && D(t), tt(i)
         }
     }
 }
 
-function Xi(e, t) {
-    let n, i, a, r, l, o, s, c, u, A, d, f, h, m;
-    const p = [wi, Ii, bi, Ei],
+function Ti(e, t) {
+    let n, i, a, r, l, o, s, c, u, d, A, f, h, m;
+    const p = [Pi, Li, Si, Bi],
         g = [];
 
     function v(e, t) {
         var n, i;
         return e[12].length ? 0 : e[11].length ? 1 : (null == (i = null == (n = e[6]) ? void 0 : n.players) ? void 0 : i.length) ? 3 : 2
     }
 
     function y(e) {
         t[25](e)
     }
     i = v(t), a = g[i] = p[i](t);
     let E = {
         unassigned: t[3].length,
-        data: lt,
+        data: ot,
         inactive: t[10].length,
         downloadPlayersUrl: t[0],
         showAutoBalance: t[9],
         allowCreate: !t[5] || null !== t[1]
     };
 
     function b(e) {
         t[28](e)
     }
 
     function I(e) {
         t[29](e)
     }
-    void 0 !== t[1] && (E.currentSession = t[1]), o = new Pn({
+    void 0 !== t[1] && (E.currentSession = t[1]), o = new Xn({
         props: E
-    }), be.push((() => Ye(o, "currentSession", y))), o.$on("clickCreateTeam", t[26]), o.$on("openAutoBalance", t[27]);
+    }), Ie.push((() => Ge(o, "currentSession", y))), o.$on("clickCreateTeam", t[26]), o.$on("openAutoBalance", t[27]);
     let w = {
-        data: lt,
+        data: ot,
         currentSessionSelected: t[8],
         createTeam: t[14],
         showAutoBalance: t[9]
     };
-    void 0 !== t[1] && (w.currentSession = t[1]), void 0 !== t[7] && (w.showDialog = t[7]), u = new di({
+    void 0 !== t[1] && (w.currentSession = t[1]), void 0 !== t[7] && (w.showDialog = t[7]), u = new gi({
         props: w
-    }), be.push((() => Ye(u, "currentSession", b))), be.push((() => Ye(u, "showDialog", I))), u.$on("selectPlayer", t[30]), u.$on("unassignPlayer", t[31]), u.$on("addPlayers", t[32]);
-    let C = t[10].length && Vi(t);
+    }), Ie.push((() => Ge(u, "currentSession", b))), Ie.push((() => Ge(u, "showDialog", I))), u.$on("selectPlayer", t[30]), u.$on("unassignPlayer", t[31]), u.$on("addPlayers", t[32]);
+    let C = t[10].length && zi(t);
     return {
         key: e,
         first: null,
         c() {
-            n = N("div"), a.c(), r = J(), l = N("div"), Ge(o.$$.fragment), c = J(), Ge(u.$$.fragment), f = J(), C && C.c(), h = j(), this.h()
+            n = N("div"), a.c(), r = J(), l = N("div"), $e(o.$$.fragment), c = J(), $e(u.$$.fragment), f = J(), C && C.c(), h = j(), this.h()
         },
         l(e) {
             n = _(e, "DIV", {
                 class: !0
             });
             var t = G(n);
             a.l(t), r = te(t), l = _(t, "DIV", {
                 class: !0
             });
             var i = G(l);
-            $e(o.$$.fragment, i), i.forEach(D), t.forEach(D), c = te(e), $e(u.$$.fragment, e), f = te(e), C && C.l(e), h = j(), this.h()
+            _e(o.$$.fragment, i), i.forEach(D), t.forEach(D), c = te(e), _e(u.$$.fragment, e), f = te(e), C && C.l(e), h = j(), this.h()
         },
         h() {
             Z(l, "class", "player-col"), Z(n, "class", "player-grid"), this.first = n
         },
         m(e, t) {
-            T(e, n, t), g[i].m(n, null), z(n, r), z(n, l), _e(o, l, null), T(e, c, t), _e(u, e, t), T(e, f, t), C && C.m(e, t), T(e, h, t), m = !0
+            T(e, n, t), g[i].m(n, null), z(n, r), z(n, l), et(o, l, null), T(e, c, t), et(u, e, t), T(e, f, t), C && C.m(e, t), T(e, h, t), m = !0
         },
         p(e, l) {
             let c = i;
-            i = v(t = e), i === c ? g[i].p(t, l) : (ze(), He(g[c], 1, 1, (() => {
+            i = v(t = e), i === c ? g[i].p(t, l) : (Te(), Ne(g[c], 1, 1, (() => {
                 g[c] = null
-            })), Te(), a = g[i], a ? a.p(t, l) : (a = g[i] = p[i](t), a.c()), De(a, 1), a.m(n, r));
+            })), De(), a = g[i], a ? a.p(t, l) : (a = g[i] = p[i](t), a.c()), He(a, 1), a.m(n, r));
             const f = {};
-            8 & l[0] && (f.unassigned = t[3].length), 1024 & l[0] && (f.inactive = t[10].length), 1 & l[0] && (f.downloadPlayersUrl = t[0]), 512 & l[0] && (f.showAutoBalance = t[9]), 34 & l[0] && (f.allowCreate = !t[5] || null !== t[1]), !s && 2 & l[0] && (s = !0, f.currentSession = t[1], Le((() => s = !1))), o.$set(f);
+            8 & l[0] && (f.unassigned = t[3].length), 1024 & l[0] && (f.inactive = t[10].length), 1 & l[0] && (f.downloadPlayersUrl = t[0]), 512 & l[0] && (f.showAutoBalance = t[9]), 34 & l[0] && (f.allowCreate = !t[5] || null !== t[1]), !s && 2 & l[0] && (s = !0, f.currentSession = t[1], Pe((() => s = !1))), o.$set(f);
             const m = {};
-            256 & l[0] && (m.currentSessionSelected = t[8]), 512 & l[0] && (m.showAutoBalance = t[9]), !A && 2 & l[0] && (A = !0, m.currentSession = t[1], Le((() => A = !1))), !d && 128 & l[0] && (d = !0, m.showDialog = t[7], Le((() => d = !1))), u.$set(m), t[10].length ? C ? (C.p(t, l), 1024 & l[0] && De(C, 1)) : (C = Vi(t), C.c(), De(C, 1), C.m(h.parentNode, h)) : C && (ze(), He(C, 1, 1, (() => {
+            256 & l[0] && (m.currentSessionSelected = t[8]), 512 & l[0] && (m.showAutoBalance = t[9]), !d && 2 & l[0] && (d = !0, m.currentSession = t[1], Pe((() => d = !1))), !A && 128 & l[0] && (A = !0, m.showDialog = t[7], Pe((() => A = !1))), u.$set(m), t[10].length ? C ? (C.p(t, l), 1024 & l[0] && He(C, 1)) : (C = zi(t), C.c(), He(C, 1), C.m(h.parentNode, h)) : C && (Te(), Ne(C, 1, 1, (() => {
                 C = null
-            })), Te())
+            })), De())
         },
         i(e) {
-            m || (De(a), De(o.$$.fragment, e), De(u.$$.fragment, e), De(C), m = !0)
+            m || (He(a), He(o.$$.fragment, e), He(u.$$.fragment, e), He(C), m = !0)
         },
         o(e) {
-            He(a), He(o.$$.fragment, e), He(u.$$.fragment, e), He(C), m = !1
+            Ne(a), Ne(o.$$.fragment, e), Ne(u.$$.fragment, e), Ne(C), m = !1
         },
         d(e) {
-            e && D(n), g[i].d(), et(o), e && D(c), et(u, e), e && D(f), C && C.d(e), e && D(h)
+            e && D(n), g[i].d(), tt(o), e && D(c), tt(u, e), e && D(f), C && C.d(e), e && D(h)
         }
     }
 }
 
-function Oi(e) {
+function Di(e) {
     var t;
     let n, i, a, r, l, o, s = [],
         c = new Map,
-        u = e[6].sessions && e[5] && pi(e);
+        u = e[6].sessions && e[5] && bi(e);
 
-    function A(t) {
+    function d(t) {
         e[21](t)
     }
-    let d = {
-        unassigned: (null == (t = e[2][e[1]]) ? void 0 : t.filter(Ui)) || []
+    let A = {
+        unassigned: (null == (t = e[2][e[1]]) ? void 0 : t.filter(Ni)) || []
     };
-    void 0 !== e[7] && (d.open = e[7]), i = new Tt({
-        props: d
-    }), be.push((() => Ye(i, "open", A))), i.$on("submit", e[22]);
+    void 0 !== e[7] && (A.open = e[7]), i = new Dt({
+        props: A
+    }), Ie.push((() => Ge(i, "open", d))), i.$on("submit", e[22]);
     let f = [e[1]];
     const h = e => e[36];
     for (let m = 0; m < 1; m += 1) {
-        let t = fi(e, f, m),
+        let t = vi(e, f, m),
             n = h(t);
-        c.set(n, s[m] = Xi(n, t))
+        c.set(n, s[m] = Ti(n, t))
     }
     return {
         c() {
-            u && u.c(), n = J(), Ge(i.$$.fragment), r = J();
+            u && u.c(), n = J(), $e(i.$$.fragment), r = J();
             for (let e = 0; e < 1; e += 1) s[e].c();
             l = j()
         },
         l(e) {
-            u && u.l(e), n = te(e), $e(i.$$.fragment, e), r = te(e);
+            u && u.l(e), n = te(e), _e(i.$$.fragment, e), r = te(e);
             for (let t = 0; t < 1; t += 1) s[t].l(e);
             l = j()
         },
         m(e, t) {
-            u && u.m(e, t), T(e, n, t), _e(i, e, t), T(e, r, t);
+            u && u.m(e, t), T(e, n, t), et(i, e, t), T(e, r, t);
             for (let n = 0; n < 1; n += 1) s[n].m(e, t);
             T(e, l, t), o = !0
         },
         p(e, t) {
             var r;
-            e[6].sessions && e[5] ? u ? (u.p(e, t), 96 & t[0] && De(u, 1)) : (u = pi(e), u.c(), De(u, 1), u.m(n.parentNode, n)) : u && (ze(), He(u, 1, 1, (() => {
+            e[6].sessions && e[5] ? u ? (u.p(e, t), 96 & t[0] && He(u, 1)) : (u = bi(e), u.c(), He(u, 1), u.m(n.parentNode, n)) : u && (Te(), Ne(u, 1, 1, (() => {
                 u = null
-            })), Te());
+            })), De());
             const o = {};
-            6 & t[0] && (o.unassigned = (null == (r = e[2][e[1]]) ? void 0 : r.filter(Ui)) || []), !a && 128 & t[0] && (a = !0, o.open = e[7], Le((() => a = !1))), i.$set(o), 253947 & t[0] && (f = [e[1]], ze(), s = Ze(s, t, h, 1, e, f, c, l.parentNode, Me, Xi, l, fi), Te())
+            6 & t[0] && (o.unassigned = (null == (r = e[2][e[1]]) ? void 0 : r.filter(Ni)) || []), !a && 128 & t[0] && (a = !0, o.open = e[7], Pe((() => a = !1))), i.$set(o), 253947 & t[0] && (f = [e[1]], Te(), s = Ye(s, t, h, 1, e, f, c, l.parentNode, Ke, Ti, l, vi), De())
         },
         i(e) {
             if (!o) {
-                De(u), De(i.$$.fragment, e);
-                for (let e = 0; e < 1; e += 1) De(s[e]);
+                He(u), He(i.$$.fragment, e);
+                for (let e = 0; e < 1; e += 1) He(s[e]);
                 o = !0
             }
         },
         o(e) {
-            He(u), He(i.$$.fragment, e);
-            for (let t = 0; t < 1; t += 1) He(s[t]);
+            Ne(u), Ne(i.$$.fragment, e);
+            for (let t = 0; t < 1; t += 1) Ne(s[t]);
             o = !1
         },
         d(e) {
-            u && u.d(e), e && D(n), et(i, e), e && D(r);
+            u && u.d(e), e && D(n), tt(i, e), e && D(r);
             for (let t = 0; t < 1; t += 1) s[t].d(e);
             e && D(l)
         }
     }
 }
-const Fi = e => !e.inactive,
-    Ui = e => !e.inactive;
+const Hi = e => !e.inactive,
+    Ni = e => !e.inactive;
 
-function zi(e, t, n) {
+function Qi(e, t, n) {
     let i, a, r, l, o, s, c;
-    y(e, lt, (e => n(6, c = e)));
+    y(e, ot, (e => n(6, c = e)));
     let u = !1,
         {
-            nextStep: A = null
+            nextStep: d = null
         } = t,
         {
-            downloadPlayersUrl: d = null
+            downloadPlayersUrl: A = null
         } = t;
     const f = {
         sessions: [{
             id: "10:00:00",
             name: "10 a.m."
         }, {
             id: "14:00:00",
@@ -5027,15 +5160,15 @@
         minimumPlayers: 2,
         maximumPlayers: 4
     };
     f.players.map((e => e.email = `${e.name.replace(" ",".").toLowerCase()}@wharton.edu`));
     let h, {
         example: m = null
     } = t;
-    m && B(lt, c = f, c);
+    m && B(ot, c = f, c);
     let p = {},
         g = [];
     const v = ({
         name: e = null,
         session: t = null
     } = {}) => {
         if (!e) {
@@ -5052,57 +5185,57 @@
     let E = [];
     const b = e => {
         E.includes(e) ? n(4, E = E.filter((t => t !== e))) : n(4, E = [...E, e])
     };
     let I = [];
     const w = e => {
             for (const t of c.teams) t.players = t.players.filter((t => t !== e));
-            lt.set(c)
+            ot.set(c)
         },
         C = ({
             team: e,
             onlyUnassigned: t = !1,
             adding: i = null,
             session: a = null
         }) => {
             const l = c.teams;
             if (e || (e = v({
                     session: a
-                }), B(lt, c.teams = [...c.teams, e], c)), null === i && (i = I, t)) {
+                }), B(ot, c.teams = [...c.teams, e], c)), null === i && (i = I, t)) {
                 const e = l.flatMap((e => e.players)),
                     t = i.filter((t => e.includes(t)));
                 i = i.filter((e => !t.includes(e) && !r.map((e => e.id)).includes(e)))
             }
             e.players = [...e.players, ...i.filter((t => !e.players.includes(t)))];
             for (const n of l.filter((t => t !== e))) n.players = n.players.filter((e => !i.includes(e)));
             r.filter((e => i.includes(e.id))).map((e => {
                 e.inactive = !1
-            })), lt.set(c), n(4, E = E.filter((t => !e.players.includes(t)))), a && h && n(1, h = a)
+            })), ot.set(c), n(4, E = E.filter((t => !e.players.includes(t)))), a && h && n(1, h = a)
         };
     return e.$$set = e => {
-        "nextStep" in e && n(18, A = e.nextStep), "downloadPlayersUrl" in e && n(0, d = e.downloadPlayersUrl), "example" in e && n(19, m = e.example)
+        "nextStep" in e && n(18, d = e.nextStep), "downloadPlayersUrl" in e && n(0, A = e.downloadPlayersUrl), "example" in e && n(19, m = e.example)
     }, e.$$.update = () => {
-        var t, u, A, d;
+        var t, u, d, A;
         if (64 & e.$$.dirty[0] && n(5, i = (null == (t = null == c ? void 0 : c.sessions) ? void 0 : t.length) > 1), 96 & e.$$.dirty[0] && n(13, a = i ? [...c.sessions, null] : c.sessions), 106 & e.$$.dirty[0] && (null == c ? void 0 : c.players)) {
             const e = c.teams.flatMap((e => e.players));
             if (n(3, g = c.players.filter((t => !e.includes(t.id) && !t.inactive))), n(2, p = {}), i)
                 for (const t of c.sessions) n(2, p[t.id] = g.filter((e => !(e.inactive || e.session && e.session !== t.id))), p);
             else 1 === (null == (u = null == c ? void 0 : c.sessions) ? void 0 : u.length) && n(1, h = c.sessions[0].id), n(2, p[h] = g, p);
             i && void 0 === h && n(1, h = e && !g.length ? null : c.sessions[0].id)
         }
-        if (64 & e.$$.dirty[0] && n(10, r = (null == (A = null == c ? void 0 : c.players) ? void 0 : A.filter((e => e.inactive))) || []), 14 & e.$$.dirty[0] && n(12, l = (null === h ? g : p[h] || []).filter((e => !e.inactive))), 64 & e.$$.dirty[0] && n(11, o = c.teams.filter((e => {
+        if (64 & e.$$.dirty[0] && n(10, r = (null == (d = null == c ? void 0 : c.players) ? void 0 : d.filter((e => e.inactive))) || []), 14 & e.$$.dirty[0] && n(12, l = (null === h ? g : p[h] || []).filter((e => !e.inactive))), 64 & e.$$.dirty[0] && n(11, o = c.teams.filter((e => {
                 const t = e.players;
                 return !!e.players.length && (t.length < c.minimumPlayers || t.length > c.maximumPlayers)
             }))), 114 & e.$$.dirty[0])
             if (i) {
                 const e = c.players.filter((e => null !== h && (!e.session || e.session === h))).map((e => e.id));
                 n(8, I = E.filter((t => e.includes(t))))
             } else n(8, I = E);
-        6 & e.$$.dirty[0] && n(9, s = ((null == (d = p[h]) ? void 0 : d.filter((e => !e.inactive))) || []).length)
-    }, [d, h, p, g, E, i, c, u, I, s, r, o, l, a, v, b, w, C, A, m, function(e) {
+        6 & e.$$.dirty[0] && n(9, s = ((null == (A = p[h]) ? void 0 : A.filter((e => !e.inactive))) || []).length)
+    }, [A, h, p, g, E, i, c, u, I, s, r, o, l, a, v, b, w, C, d, m, function(e) {
         h = e, n(1, h), n(6, c), n(5, i), n(3, g)
     }, function(e) {
         u = e, n(7, u)
     }, e => {
         const t = e.detail.fillCount,
             i = c.teams.filter((e => (!e.session || e.session === h) && e.players.length < t));
         let a, r = p[h].filter((e => !e.inactive));
@@ -5112,24 +5245,24 @@
                     i = e[t];
                 e[t] = e[n], e[n] = i
             }
         }(r);
         for (const n of r) i.length ? a = i.shift() : (a = v(), c.teams.unshift(a)), a.players.push(n.id), a.players.length < t && i.unshift(a);
         c.teams.forEach((e => {
             delete e.ready
-        })), lt.set(c), n(4, E = [])
+        })), ot.set(c), n(4, E = [])
     }, e => {
         b(e.detail.id)
     }, e => {
         C(e.detail)
     }, function(e) {
         h = e, n(1, h), n(6, c), n(5, i), n(3, g)
     }, () => {
         const e = v();
-        B(lt, c.teams = [...c.teams, e], c), C({
+        B(ot, c.teams = [...c.teams, e], c), C({
             team: e,
             onlyUnassigned: !0
         })
     }, () => {
         n(7, u = !0)
     }, function(e) {
         h = e, n(1, h), n(6, c), n(5, i), n(3, g)
@@ -5143,46 +5276,46 @@
         C(e.detail)
     }, e => {
         b(e.detail.id)
     }, e => {
         C(e.detail)
     }]
 }
-class Ti extends it {
+class Wi extends at {
     constructor(e) {
-        super(), nt(this, e, zi, Oi, p, {
+        super(), it(this, e, Qi, Di, p, {
             nextStep: 18,
             downloadPlayersUrl: 0,
             example: 19
         }, null, [-1, -1])
     }
 }
-var Di = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
+var Ji = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
 
-function Hi(e) {
+function ji(e) {
     if (e.__esModule) return e;
     var t = Object.defineProperty({}, "__esModule", {
         value: !0
     });
     return Object.keys(e).forEach((function(n) {
         var i = Object.getOwnPropertyDescriptor(e, n);
         Object.defineProperty(t, n, i.get ? i : {
             enumerable: !0,
             get: function() {
                 return e[n]
             }
         })
     })), t
 }
-var Ni = {},
-    Qi = {
+var qi = {},
+    Mi = {
         exports: {}
     };
 ! function(e, t) {
-    var n, i = "undefined" != typeof self ? self : Di,
+    var n, i = "undefined" != typeof self ? self : Ji,
         a = function() {
             function e() {
                 this.fetch = !1, this.DOMException = i.DOMException
             }
             return e.prototype = i, new e
         }();
     n = a,
@@ -5208,31 +5341,31 @@
                 return e.toLowerCase()
             }
 
             function u(e) {
                 return "string" != typeof e && (e = String(e)), e
             }
 
-            function A(e) {
+            function d(e) {
                 var t = {
                     next: function() {
                         var t = e.shift();
                         return {
                             done: void 0 === t,
                             value: t
                         }
                     }
                 };
                 return i && (t[Symbol.iterator] = function() {
                     return t
                 }), t
             }
 
-            function d(e) {
-                this.map = {}, e instanceof d ? e.forEach((function(e, t) {
+            function A(e) {
+                this.map = {}, e instanceof A ? e.forEach((function(e, t) {
                     this.append(t, e)
                 }), this) : Array.isArray(e) ? e.forEach((function(e) {
                     this.append(e[0], e[1])
                 }), this) : e && Object.getOwnPropertyNames(e).forEach((function(t) {
                     this.append(t, e[t])
                 }), this)
             }
@@ -5289,53 +5422,53 @@
                     return Promise.resolve(this._bodyText)
                 }, r && (this.formData = function() {
                     return this.text().then(E)
                 }), this.json = function() {
                     return this.text().then(JSON.parse)
                 }, this
             }
-            d.prototype.append = function(e, t) {
+            A.prototype.append = function(e, t) {
                 e = c(e), t = u(t);
                 var n = this.map[e];
                 this.map[e] = n ? n + ", " + t : t
-            }, d.prototype.delete = function(e) {
+            }, A.prototype.delete = function(e) {
                 delete this.map[c(e)]
-            }, d.prototype.get = function(e) {
+            }, A.prototype.get = function(e) {
                 return e = c(e), this.has(e) ? this.map[e] : null
-            }, d.prototype.has = function(e) {
+            }, A.prototype.has = function(e) {
                 return this.map.hasOwnProperty(c(e))
-            }, d.prototype.set = function(e, t) {
+            }, A.prototype.set = function(e, t) {
                 this.map[c(e)] = u(t)
-            }, d.prototype.forEach = function(e, t) {
+            }, A.prototype.forEach = function(e, t) {
                 for (var n in this.map) this.map.hasOwnProperty(n) && e.call(t, this.map[n], n, this)
-            }, d.prototype.keys = function() {
+            }, A.prototype.keys = function() {
                 var e = [];
                 return this.forEach((function(t, n) {
                     e.push(n)
-                })), A(e)
-            }, d.prototype.values = function() {
+                })), d(e)
+            }, A.prototype.values = function() {
                 var e = [];
                 return this.forEach((function(t) {
                     e.push(t)
-                })), A(e)
-            }, d.prototype.entries = function() {
+                })), d(e)
+            }, A.prototype.entries = function() {
                 var e = [];
                 return this.forEach((function(t, n) {
                     e.push([n, t])
-                })), A(e)
-            }, i && (d.prototype[Symbol.iterator] = d.prototype.entries);
+                })), d(e)
+            }, i && (A.prototype[Symbol.iterator] = A.prototype.entries);
             var v = ["DELETE", "GET", "HEAD", "OPTIONS", "POST", "PUT"];
 
             function y(e, t) {
                 var n, i, a = (t = t || {}).body;
                 if (e instanceof y) {
                     if (e.bodyUsed) throw new TypeError("Already read");
-                    this.url = e.url, this.credentials = e.credentials, t.headers || (this.headers = new d(e.headers)), this.method = e.method, this.mode = e.mode, this.signal = e.signal, a || null == e._bodyInit || (a = e._bodyInit, e.bodyUsed = !0)
+                    this.url = e.url, this.credentials = e.credentials, t.headers || (this.headers = new A(e.headers)), this.method = e.method, this.mode = e.mode, this.signal = e.signal, a || null == e._bodyInit || (a = e._bodyInit, e.bodyUsed = !0)
                 } else this.url = String(e);
-                if (this.credentials = t.credentials || this.credentials || "same-origin", !t.headers && this.headers || (this.headers = new d(t.headers)), this.method = (n = t.method || this.method || "GET", i = n.toUpperCase(), v.indexOf(i) > -1 ? i : n), this.mode = t.mode || this.mode || null, this.signal = t.signal || this.signal, this.referrer = null, ("GET" === this.method || "HEAD" === this.method) && a) throw new TypeError("Body not allowed for GET or HEAD requests");
+                if (this.credentials = t.credentials || this.credentials || "same-origin", !t.headers && this.headers || (this.headers = new A(t.headers)), this.method = (n = t.method || this.method || "GET", i = n.toUpperCase(), v.indexOf(i) > -1 ? i : n), this.mode = t.mode || this.mode || null, this.signal = t.signal || this.signal, this.referrer = null, ("GET" === this.method || "HEAD" === this.method) && a) throw new TypeError("Body not allowed for GET or HEAD requests");
                 this._initBody(a)
             }
 
             function E(e) {
                 var t = new FormData;
                 return e.trim().split("&").forEach((function(e) {
                     if (e) {
@@ -5344,25 +5477,25 @@
                             a = n.join("=").replace(/\+/g, " ");
                         t.append(decodeURIComponent(i), decodeURIComponent(a))
                     }
                 })), t
             }
 
             function b(e, t) {
-                t || (t = {}), this.type = "default", this.status = void 0 === t.status ? 200 : t.status, this.ok = this.status >= 200 && this.status < 300, this.statusText = "statusText" in t ? t.statusText : "OK", this.headers = new d(t.headers), this.url = t.url || "", this._initBody(e)
+                t || (t = {}), this.type = "default", this.status = void 0 === t.status ? 200 : t.status, this.ok = this.status >= 200 && this.status < 300, this.statusText = "statusText" in t ? t.statusText : "OK", this.headers = new A(t.headers), this.url = t.url || "", this._initBody(e)
             }
             y.prototype.clone = function() {
                 return new y(this, {
                     body: this._bodyInit
                 })
             }, g.call(y.prototype), g.call(b.prototype), b.prototype.clone = function() {
                 return new b(this._bodyInit, {
                     status: this.status,
                     statusText: this.statusText,
-                    headers: new d(this.headers),
+                    headers: new A(this.headers),
                     url: this.url
                 })
             }, b.error = function() {
                 var e = new b(null, {
                     status: 0,
                     statusText: ""
                 });
@@ -5397,15 +5530,15 @@
                     function s() {
                         o.abort()
                     }
                     o.onload = function() {
                         var e, t, n = {
                             status: o.status,
                             statusText: o.statusText,
-                            headers: (e = o.getAllResponseHeaders() || "", t = new d, e.replace(/\r?\n[\t ]+/g, " ").split(/\r?\n/).forEach((function(e) {
+                            headers: (e = o.getAllResponseHeaders() || "", t = new A, e.replace(/\r?\n[\t ]+/g, " ").split(/\r?\n/).forEach((function(e) {
                                 var n = e.split(":"),
                                     i = n.shift().trim();
                                 if (i) {
                                     var a = n.join(":").trim();
                                     t.append(i, a)
                                 }
                             })), t)
@@ -5422,57 +5555,57 @@
                     }, o.open(l.method, l.url, !0), "include" === l.credentials ? o.withCredentials = !0 : "omit" === l.credentials && (o.withCredentials = !1), "responseType" in o && a && (o.responseType = "blob"), l.headers.forEach((function(e, t) {
                         o.setRequestHeader(t, e)
                     })), l.signal && (l.signal.addEventListener("abort", s), o.onreadystatechange = function() {
                         4 === o.readyState && l.signal.removeEventListener("abort", s)
                     }), o.send(void 0 === l._bodyInit ? null : l._bodyInit)
                 }))
             }
-            w.polyfill = !0, n.fetch || (n.fetch = w, n.Headers = d, n.Request = y, n.Response = b), e.Headers = d, e.Request = y, e.Response = b, e.fetch = w, Object.defineProperty(e, "__esModule", {
+            w.polyfill = !0, n.fetch || (n.fetch = w, n.Headers = A, n.Request = y, n.Response = b), e.Headers = A, e.Request = y, e.Response = b, e.fetch = w, Object.defineProperty(e, "__esModule", {
                 value: !0
             })
         }({}), a.fetch.ponyfill = !0, delete a.fetch.polyfill;
     var r = a;
     (t = r.fetch).default = r.fetch, t.fetch = r.fetch, t.Headers = r.Headers, t.Request = r.Request, t.Response = r.Response, e.exports = t
-}(Qi, Qi.exports);
-var Wi = "function" == typeof Symbol && "function" == typeof Symbol.for ? Symbol.for("nodejs.util.inspect.custom") : void 0;
+}(Mi, Mi.exports);
+var Ki = "function" == typeof Symbol && "function" == typeof Symbol.for ? Symbol.for("nodejs.util.inspect.custom") : void 0;
 
-function Ji(e) {
-    return (Ji = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+function Zi(e) {
+    return (Zi = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
         return typeof e
     } : function(e) {
         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
     })(e)
 }
 
-function ji(e) {
-    return qi(e, [])
+function Yi(e) {
+    return Gi(e, [])
 }
 
-function qi(e, t) {
-    switch (Ji(e)) {
+function Gi(e, t) {
+    switch (Zi(e)) {
         case "string":
             return JSON.stringify(e);
         case "function":
             return e.name ? "[function ".concat(e.name, "]") : "[function]";
         case "object":
             return null === e ? "null" : function(e, t) {
                 if (-1 !== t.indexOf(e)) return "[Circular]";
                 var n = [].concat(t, [e]),
                     i = function(e) {
-                        var t = e[String(Wi)];
+                        var t = e[String(Ki)];
                         if ("function" == typeof t) return t;
                         if ("function" == typeof e.inspect) return e.inspect
                     }(e);
                 if (void 0 !== i) {
                     var a = i.call(e);
-                    if (a !== e) return "string" == typeof a ? a : qi(a, n)
+                    if (a !== e) return "string" == typeof a ? a : Gi(a, n)
                 } else if (Array.isArray(e)) return function(e, t) {
                     if (0 === e.length) return "[]";
                     if (t.length > 2) return "[Array]";
-                    for (var n = Math.min(10, e.length), i = e.length - n, a = [], r = 0; r < n; ++r) a.push(qi(e[r], t));
+                    for (var n = Math.min(10, e.length), i = e.length - n, a = [], r = 0; r < n; ++r) a.push(Gi(e[r], t));
                     1 === i ? a.push("... 1 more item") : i > 1 && a.push("... ".concat(i, " more items"));
                     return "[" + a.join(", ") + "]"
                 }(e, n);
                 return function(e, t) {
                     var n = Object.keys(e);
                     if (0 === n.length) return "{}";
                     if (t.length > 2) return "[" + function(e) {
@@ -5480,57 +5613,57 @@
                         if ("Object" === t && "function" == typeof e.constructor) {
                             var n = e.constructor.name;
                             if ("string" == typeof n && "" !== n) return n
                         }
                         return t
                     }(e) + "]";
                     return "{ " + n.map((function(n) {
-                        return n + ": " + qi(e[n], t)
+                        return n + ": " + Gi(e[n], t)
                     })).join(", ") + " }"
                 }(e, n)
             }(e, t);
         default:
             return String(e)
     }
 }
 
-function Mi(e) {
+function $i(e) {
     var t = e.prototype.toJSON;
     "function" == typeof t || function(e, t) {
         if (!Boolean(e)) throw new Error(null != t ? t : "Unexpected invariant triggered.")
-    }(0), e.prototype.inspect = t, Wi && (e.prototype[Wi] = t)
+    }(0), e.prototype.inspect = t, Ki && (e.prototype[Ki] = t)
 }
 
-function Ki(e) {
+function _i(e) {
     return null != e && "string" == typeof e.kind
 }
-Mi(function() {
+$i(function() {
     function e(e, t, n) {
         this.start = e.start, this.end = t.end, this.startToken = e, this.endToken = t, this.source = n
     }
     return e.prototype.toJSON = function() {
         return {
             start: this.start,
             end: this.end
         }
     }, e
-}()), Mi(function() {
+}()), $i(function() {
     function e(e, t, n, i, a, r, l) {
         this.kind = e, this.start = t, this.end = n, this.line = i, this.column = a, this.value = l, this.prev = r, this.next = null
     }
     return e.prototype.toJSON = function() {
         return {
             kind: this.kind,
             value: this.value,
             line: this.line,
             column: this.column
         }
     }, e
 }());
-var Zi = {
+var ea = {
         Name: [],
         Document: ["definitions"],
         OperationDefinition: ["name", "variableDefinitions", "directives", "selectionSet"],
         VariableDefinition: ["variable", "type", "defaultValue", "directives"],
         Variable: ["name"],
         SelectionSet: ["selections"],
         Field: ["alias", "name", "arguments", "directives", "selectionSet"],
@@ -5567,88 +5700,88 @@
         ScalarTypeExtension: ["name", "directives"],
         ObjectTypeExtension: ["name", "interfaces", "directives", "fields"],
         InterfaceTypeExtension: ["name", "interfaces", "directives", "fields"],
         UnionTypeExtension: ["name", "directives", "types"],
         EnumTypeExtension: ["name", "directives", "values"],
         InputObjectTypeExtension: ["name", "directives", "fields"]
     },
-    Yi = Object.freeze({});
+    ta = Object.freeze({});
 
-function Gi(e, t, n) {
+function na(e, t, n) {
     var i = e[t];
     if (i) {
         if (!n && "function" == typeof i) return i;
         var a = n ? i.leave : i.enter;
         if ("function" == typeof a) return a
     } else {
         var r = n ? e.leave : e.enter;
         if (r) {
             if ("function" == typeof r) return r;
             var l = r[t];
             if ("function" == typeof l) return l
         }
     }
 }
-var $i = {
+var ia = {
     Name: function(e) {
         return e.value
     },
     Variable: function(e) {
         return "$" + e.name
     },
     Document: function(e) {
-        return ea(e.definitions, "\n\n") + "\n"
+        return ra(e.definitions, "\n\n") + "\n"
     },
     OperationDefinition: function(e) {
         var t = e.operation,
             n = e.name,
-            i = na("(", ea(e.variableDefinitions, ", "), ")"),
-            a = ea(e.directives, " "),
+            i = oa("(", ra(e.variableDefinitions, ", "), ")"),
+            a = ra(e.directives, " "),
             r = e.selectionSet;
-        return n || a || i || "query" !== t ? ea([t, ea([n, i]), a, r], " ") : r
+        return n || a || i || "query" !== t ? ra([t, ra([n, i]), a, r], " ") : r
     },
     VariableDefinition: function(e) {
         var t = e.variable,
             n = e.type,
             i = e.defaultValue,
             a = e.directives;
-        return t + ": " + n + na(" = ", i) + na(" ", ea(a, " "))
+        return t + ": " + n + oa(" = ", i) + oa(" ", ra(a, " "))
     },
     SelectionSet: function(e) {
-        return ta(e.selections)
+        return la(e.selections)
     },
     Field: function(e) {
         var t = e.alias,
             n = e.name,
             i = e.arguments,
             a = e.directives,
             r = e.selectionSet,
-            l = na("", t, ": ") + n,
-            o = l + na("(", ea(i, ", "), ")");
-        return o.length > 80 && (o = l + na("(\n", ia(ea(i, "\n")), "\n)")), ea([o, ea(a, " "), r], " ")
+            l = oa("", t, ": ") + n,
+            o = l + oa("(", ra(i, ", "), ")");
+        return o.length > 80 && (o = l + oa("(\n", sa(ra(i, "\n")), "\n)")), ra([o, ra(a, " "), r], " ")
     },
     Argument: function(e) {
         return e.name + ": " + e.value
     },
     FragmentSpread: function(e) {
-        return "..." + e.name + na(" ", ea(e.directives, " "))
+        return "..." + e.name + oa(" ", ra(e.directives, " "))
     },
     InlineFragment: function(e) {
         var t = e.typeCondition,
             n = e.directives,
             i = e.selectionSet;
-        return ea(["...", na("on ", t), ea(n, " "), i], " ")
+        return ra(["...", oa("on ", t), ra(n, " "), i], " ")
     },
     FragmentDefinition: function(e) {
         var t = e.name,
             n = e.typeCondition,
             i = e.variableDefinitions,
             a = e.directives,
             r = e.selectionSet;
-        return "fragment ".concat(t).concat(na("(", ea(i, ", "), ")"), " ") + "on ".concat(n, " ").concat(na("", ea(a, " "), " ")) + r
+        return "fragment ".concat(t).concat(oa("(", ra(i, ", "), ")"), " ") + "on ".concat(n, " ").concat(oa("", ra(a, " "), " ")) + r
     },
     IntValue: function(e) {
         return e.value
     },
     FloatValue: function(e) {
         return e.value
     },
@@ -5672,198 +5805,198 @@
     NullValue: function() {
         return "null"
     },
     EnumValue: function(e) {
         return e.value
     },
     ListValue: function(e) {
-        return "[" + ea(e.values, ", ") + "]"
+        return "[" + ra(e.values, ", ") + "]"
     },
     ObjectValue: function(e) {
-        return "{" + ea(e.fields, ", ") + "}"
+        return "{" + ra(e.fields, ", ") + "}"
     },
     ObjectField: function(e) {
         return e.name + ": " + e.value
     },
     Directive: function(e) {
-        return "@" + e.name + na("(", ea(e.arguments, ", "), ")")
+        return "@" + e.name + oa("(", ra(e.arguments, ", "), ")")
     },
     NamedType: function(e) {
         return e.name
     },
     ListType: function(e) {
         return "[" + e.type + "]"
     },
     NonNullType: function(e) {
         return e.type + "!"
     },
-    SchemaDefinition: _i((function(e) {
+    SchemaDefinition: aa((function(e) {
         var t = e.directives,
             n = e.operationTypes;
-        return ea(["schema", ea(t, " "), ta(n)], " ")
+        return ra(["schema", ra(t, " "), la(n)], " ")
     })),
     OperationTypeDefinition: function(e) {
         return e.operation + ": " + e.type
     },
-    ScalarTypeDefinition: _i((function(e) {
-        return ea(["scalar", e.name, ea(e.directives, " ")], " ")
+    ScalarTypeDefinition: aa((function(e) {
+        return ra(["scalar", e.name, ra(e.directives, " ")], " ")
     })),
-    ObjectTypeDefinition: _i((function(e) {
+    ObjectTypeDefinition: aa((function(e) {
         var t = e.name,
             n = e.interfaces,
             i = e.directives,
             a = e.fields;
-        return ea(["type", t, na("implements ", ea(n, " & ")), ea(i, " "), ta(a)], " ")
+        return ra(["type", t, oa("implements ", ra(n, " & ")), ra(i, " "), la(a)], " ")
     })),
-    FieldDefinition: _i((function(e) {
+    FieldDefinition: aa((function(e) {
         var t = e.name,
             n = e.arguments,
             i = e.type,
             a = e.directives;
-        return t + (ra(n) ? na("(\n", ia(ea(n, "\n")), "\n)") : na("(", ea(n, ", "), ")")) + ": " + i + na(" ", ea(a, " "))
+        return t + (ua(n) ? oa("(\n", sa(ra(n, "\n")), "\n)") : oa("(", ra(n, ", "), ")")) + ": " + i + oa(" ", ra(a, " "))
     })),
-    InputValueDefinition: _i((function(e) {
+    InputValueDefinition: aa((function(e) {
         var t = e.name,
             n = e.type,
             i = e.defaultValue,
             a = e.directives;
-        return ea([t + ": " + n, na("= ", i), ea(a, " ")], " ")
+        return ra([t + ": " + n, oa("= ", i), ra(a, " ")], " ")
     })),
-    InterfaceTypeDefinition: _i((function(e) {
+    InterfaceTypeDefinition: aa((function(e) {
         var t = e.name,
             n = e.interfaces,
             i = e.directives,
             a = e.fields;
-        return ea(["interface", t, na("implements ", ea(n, " & ")), ea(i, " "), ta(a)], " ")
+        return ra(["interface", t, oa("implements ", ra(n, " & ")), ra(i, " "), la(a)], " ")
     })),
-    UnionTypeDefinition: _i((function(e) {
+    UnionTypeDefinition: aa((function(e) {
         var t = e.name,
             n = e.directives,
             i = e.types;
-        return ea(["union", t, ea(n, " "), i && 0 !== i.length ? "= " + ea(i, " | ") : ""], " ")
+        return ra(["union", t, ra(n, " "), i && 0 !== i.length ? "= " + ra(i, " | ") : ""], " ")
     })),
-    EnumTypeDefinition: _i((function(e) {
+    EnumTypeDefinition: aa((function(e) {
         var t = e.name,
             n = e.directives,
             i = e.values;
-        return ea(["enum", t, ea(n, " "), ta(i)], " ")
+        return ra(["enum", t, ra(n, " "), la(i)], " ")
     })),
-    EnumValueDefinition: _i((function(e) {
-        return ea([e.name, ea(e.directives, " ")], " ")
+    EnumValueDefinition: aa((function(e) {
+        return ra([e.name, ra(e.directives, " ")], " ")
     })),
-    InputObjectTypeDefinition: _i((function(e) {
+    InputObjectTypeDefinition: aa((function(e) {
         var t = e.name,
             n = e.directives,
             i = e.fields;
-        return ea(["input", t, ea(n, " "), ta(i)], " ")
+        return ra(["input", t, ra(n, " "), la(i)], " ")
     })),
-    DirectiveDefinition: _i((function(e) {
+    DirectiveDefinition: aa((function(e) {
         var t = e.name,
             n = e.arguments,
             i = e.repeatable,
             a = e.locations;
-        return "directive @" + t + (ra(n) ? na("(\n", ia(ea(n, "\n")), "\n)") : na("(", ea(n, ", "), ")")) + (i ? " repeatable" : "") + " on " + ea(a, " | ")
+        return "directive @" + t + (ua(n) ? oa("(\n", sa(ra(n, "\n")), "\n)") : oa("(", ra(n, ", "), ")")) + (i ? " repeatable" : "") + " on " + ra(a, " | ")
     })),
     SchemaExtension: function(e) {
         var t = e.directives,
             n = e.operationTypes;
-        return ea(["extend schema", ea(t, " "), ta(n)], " ")
+        return ra(["extend schema", ra(t, " "), la(n)], " ")
     },
     ScalarTypeExtension: function(e) {
-        return ea(["extend scalar", e.name, ea(e.directives, " ")], " ")
+        return ra(["extend scalar", e.name, ra(e.directives, " ")], " ")
     },
     ObjectTypeExtension: function(e) {
         var t = e.name,
             n = e.interfaces,
             i = e.directives,
             a = e.fields;
-        return ea(["extend type", t, na("implements ", ea(n, " & ")), ea(i, " "), ta(a)], " ")
+        return ra(["extend type", t, oa("implements ", ra(n, " & ")), ra(i, " "), la(a)], " ")
     },
     InterfaceTypeExtension: function(e) {
         var t = e.name,
             n = e.interfaces,
             i = e.directives,
             a = e.fields;
-        return ea(["extend interface", t, na("implements ", ea(n, " & ")), ea(i, " "), ta(a)], " ")
+        return ra(["extend interface", t, oa("implements ", ra(n, " & ")), ra(i, " "), la(a)], " ")
     },
     UnionTypeExtension: function(e) {
         var t = e.name,
             n = e.directives,
             i = e.types;
-        return ea(["extend union", t, ea(n, " "), i && 0 !== i.length ? "= " + ea(i, " | ") : ""], " ")
+        return ra(["extend union", t, ra(n, " "), i && 0 !== i.length ? "= " + ra(i, " | ") : ""], " ")
     },
     EnumTypeExtension: function(e) {
         var t = e.name,
             n = e.directives,
             i = e.values;
-        return ea(["extend enum", t, ea(n, " "), ta(i)], " ")
+        return ra(["extend enum", t, ra(n, " "), la(i)], " ")
     },
     InputObjectTypeExtension: function(e) {
         var t = e.name,
             n = e.directives,
             i = e.fields;
-        return ea(["extend input", t, ea(n, " "), ta(i)], " ")
+        return ra(["extend input", t, ra(n, " "), la(i)], " ")
     }
 };
 
-function _i(e) {
+function aa(e) {
     return function(t) {
-        return ea([t.description, e(t)], "\n")
+        return ra([t.description, e(t)], "\n")
     }
 }
 
-function ea(e) {
+function ra(e) {
     var t, n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
     return null !== (t = null == e ? void 0 : e.filter((function(e) {
         return e
     })).join(n)) && void 0 !== t ? t : ""
 }
 
-function ta(e) {
-    return na("{\n", ia(ea(e, "\n")), "\n}")
+function la(e) {
+    return oa("{\n", sa(ra(e, "\n")), "\n}")
 }
 
-function na(e, t) {
+function oa(e, t) {
     var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "";
     return null != t && "" !== t ? e + t + n : ""
 }
 
-function ia(e) {
-    return na("  ", e.replace(/\n/g, "\n  "))
+function sa(e) {
+    return oa("  ", e.replace(/\n/g, "\n  "))
 }
 
-function aa(e) {
+function ca(e) {
     return -1 !== e.indexOf("\n")
 }
 
-function ra(e) {
-    return null != e && e.some(aa)
+function ua(e) {
+    return null != e && e.some(ca)
 }
-var la = Hi(Object.freeze({
+var da = ji(Object.freeze({
         __proto__: null,
         [Symbol.toStringTag]: "Module",
         print: function(e) {
             return function(e, t) {
-                var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : Zi,
+                var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : ea,
                     i = void 0,
                     a = Array.isArray(e),
                     r = [e],
                     l = -1,
                     o = [],
                     s = void 0,
                     c = void 0,
                     u = void 0,
-                    A = [],
                     d = [],
+                    A = [],
                     f = e;
                 do {
                     var h = ++l === r.length,
                         m = h && 0 !== o.length;
                     if (h) {
-                        if (c = 0 === d.length ? void 0 : A[A.length - 1], s = u, u = d.pop(), m) {
+                        if (c = 0 === A.length ? void 0 : d[d.length - 1], s = u, u = A.pop(), m) {
                             if (a) s = s.slice();
                             else {
                                 for (var p = {}, g = 0, v = Object.keys(s); g < v.length; g++) {
                                     var y = v[g];
                                     p[y] = s[y]
                                 }
                                 s = p
@@ -5873,66 +6006,66 @@
                                     w = o[b][1];
                                 a && (I -= E), a && null === w ? (s.splice(I, 1), E++) : s[I] = w
                             }
                         }
                         l = i.index, r = i.keys, o = i.edits, a = i.inArray, i = i.prev
                     } else {
                         if (c = u ? a ? l : r[l] : void 0, null == (s = u ? u[c] : f)) continue;
-                        u && A.push(c)
+                        u && d.push(c)
                     }
                     var C, B = void 0;
                     if (!Array.isArray(s)) {
-                        if (!Ki(s)) throw new Error("Invalid AST Node: ".concat(ji(s), "."));
-                        var S = Gi(t, s.kind, h);
+                        if (!_i(s)) throw new Error("Invalid AST Node: ".concat(Yi(s), "."));
+                        var S = na(t, s.kind, h);
                         if (S) {
-                            if ((B = S.call(t, s, c, u, A, d)) === Yi) break;
+                            if ((B = S.call(t, s, c, u, d, A)) === ta) break;
                             if (!1 === B) {
                                 if (!h) {
-                                    A.pop();
+                                    d.pop();
                                     continue
                                 }
                             } else if (void 0 !== B && (o.push([c, B]), !h)) {
-                                if (!Ki(B)) {
-                                    A.pop();
+                                if (!_i(B)) {
+                                    d.pop();
                                     continue
                                 }
                                 s = B
                             }
                         }
                     }
-                    void 0 === B && m && o.push([c, s]), h ? A.pop() : (i = {
+                    void 0 === B && m && o.push([c, s]), h ? d.pop() : (i = {
                         inArray: a,
                         index: l,
                         keys: r,
                         edits: o,
                         prev: i
-                    }, r = (a = Array.isArray(s)) ? s : null !== (C = n[s.kind]) && void 0 !== C ? C : [], l = -1, o = [], u && d.push(u), u = s)
+                    }, r = (a = Array.isArray(s)) ? s : null !== (C = n[s.kind]) && void 0 !== C ? C : [], l = -1, o = [], u && A.push(u), u = s)
                 } while (void 0 !== i);
                 return 0 !== o.length && (f = o[o.length - 1][1]), f
             }(e, {
-                leave: $i
+                leave: ia
             })
         }
     })),
-    oa = {},
-    sa = {},
-    ca = function(e) {
+    Aa = {},
+    fa = {},
+    ha = function(e) {
         var t = e.uri,
             n = e.name,
             i = e.type;
         this.uri = t, this.name = n, this.type = i
     },
-    ua = ca,
-    Aa = function(e) {
-        return "undefined" != typeof File && e instanceof File || "undefined" != typeof Blob && e instanceof Blob || e instanceof ua
+    ma = ha,
+    pa = function(e) {
+        return "undefined" != typeof File && e instanceof File || "undefined" != typeof Blob && e instanceof Blob || e instanceof ma
     },
-    da = Aa;
-sa.ReactNativeFile = ca, sa.extractFiles = function e(t, n, i) {
+    ga = pa;
+fa.ReactNativeFile = ha, fa.extractFiles = function e(t, n, i) {
     var a;
-    void 0 === n && (n = ""), void 0 === i && (i = da);
+    void 0 === n && (n = ""), void 0 === i && (i = ga);
     var r = new Map;
 
     function l(e, t) {
         var n = r.get(t);
         n ? n.push.apply(n, e) : r.set(t, e)
     }
     if (i(t)) a = null, l([n], t);
@@ -5951,118 +6084,118 @@
                 c.files.forEach(l), a[s] = c.clone
             } else a = t
     }
     return {
         clone: a,
         files: r
     }
-}, sa.isExtractableFile = Aa;
-var fa = "object" == typeof self ? self.FormData : window.FormData,
-    ha = Di && Di.__importDefault || function(e) {
+}, fa.isExtractableFile = pa;
+var va = "object" == typeof self ? self.FormData : window.FormData,
+    ya = Ji && Ji.__importDefault || function(e) {
         return e && e.__esModule ? e : {
             default: e
         }
     };
-Object.defineProperty(oa, "__esModule", {
+Object.defineProperty(Aa, "__esModule", {
     value: !0
 });
-var ma = sa,
-    pa = ha(fa),
-    ga = function(e) {
-        return ma.isExtractableFile(e) || null !== e && "object" == typeof e && "function" == typeof e.pipe
+var Ea = fa,
+    ba = ya(va),
+    Ia = function(e) {
+        return Ea.isExtractableFile(e) || null !== e && "object" == typeof e && "function" == typeof e.pipe
     };
-oa.default = function(e, t) {
-    var n = ma.extractFiles({
+Aa.default = function(e, t) {
+    var n = Ea.extractFiles({
             query: e,
             variables: t
-        }, "", ga),
+        }, "", Ia),
         i = n.clone,
         a = n.files;
     if (0 === a.size) return JSON.stringify(i);
-    var r = new("undefined" == typeof FormData ? pa.default : FormData);
+    var r = new("undefined" == typeof FormData ? ba.default : FormData);
     r.append("operations", JSON.stringify(i));
     var l = {},
         o = 0;
     return a.forEach((function(e) {
         l[++o] = e
     })), r.append("map", JSON.stringify(l)), o = 0, a.forEach((function(e, t) {
         r.append("" + ++o, t)
     })), r
 };
-var va, ya = {},
-    Ea = Di && Di.__extends || (va = function(e, t) {
-        return (va = Object.setPrototypeOf || {
+var wa, Ca = {},
+    Ba = Ji && Ji.__extends || (wa = function(e, t) {
+        return (wa = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
             })(e, t)
     }, function(e, t) {
         function n() {
             this.constructor = e
         }
-        va(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+        wa(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
     });
-Object.defineProperty(ya, "__esModule", {
+Object.defineProperty(Ca, "__esModule", {
     value: !0
-}), ya.ClientError = void 0;
-var ba = function(e) {
+}), Ca.ClientError = void 0;
+var Sa = function(e) {
     function t(n, i) {
         var a = this,
             r = t.extractMessage(n) + ": " + JSON.stringify({
                 response: n,
                 request: i
             });
         return a = e.call(this, r) || this, Object.setPrototypeOf(a, t.prototype), a.response = n, a.request = i, "function" == typeof Error.captureStackTrace && Error.captureStackTrace(a, t), a
     }
-    return Ea(t, e), t.extractMessage = function(e) {
+    return Ba(t, e), t.extractMessage = function(e) {
         try {
             return e.errors[0].message
         } catch (t) {
             return "GraphQL Error (Code: " + e.status + ")"
         }
     }, t
 }(Error);
-ya.ClientError = ba,
+Ca.ClientError = Sa,
     function(e) {
-        var t = Di && Di.__assign || function() {
+        var t = Ji && Ji.__assign || function() {
                 return (t = Object.assign || function(e) {
                     for (var t, n = 1, i = arguments.length; n < i; n++)
                         for (var a in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, a) && (e[a] = t[a]);
                     return e
                 }).apply(this, arguments)
             },
-            n = Di && Di.__createBinding || (Object.create ? function(e, t, n, i) {
+            n = Ji && Ji.__createBinding || (Object.create ? function(e, t, n, i) {
                 void 0 === i && (i = n), Object.defineProperty(e, i, {
                     enumerable: !0,
                     get: function() {
                         return t[n]
                     }
                 })
             } : function(e, t, n, i) {
                 void 0 === i && (i = n), e[i] = t[n]
             }),
-            i = Di && Di.__setModuleDefault || (Object.create ? function(e, t) {
+            i = Ji && Ji.__setModuleDefault || (Object.create ? function(e, t) {
                 Object.defineProperty(e, "default", {
                     enumerable: !0,
                     value: t
                 })
             } : function(e, t) {
                 e.default = t
             }),
-            a = Di && Di.__importStar || function(e) {
+            a = Ji && Ji.__importStar || function(e) {
                 if (e && e.__esModule) return e;
                 var t = {};
                 if (null != e)
                     for (var a in e) "default" !== a && Object.prototype.hasOwnProperty.call(e, a) && n(t, e, a);
                 return i(t, e), t
             },
-            r = Di && Di.__awaiter || function(e, t, n, i) {
+            r = Ji && Ji.__awaiter || function(e, t, n, i) {
                 return new(n || (n = Promise))((function(a, r) {
                     function l(e) {
                         try {
                             s(i.next(e))
                         } catch (t) {
                             r(t)
                         }
@@ -6081,15 +6214,15 @@
                         e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                             e(t)
                         }))).then(l, o)
                     }
                     s((i = i.apply(e, t || [])).next())
                 }))
             },
-            l = Di && Di.__generator || function(e, t) {
+            l = Ji && Ji.__generator || function(e, t) {
                 var n, i, a, r, l = {
                     label: 0,
                     sent: function() {
                         if (1 & a[0]) throw a[1];
                         return a[1]
                     },
                     trys: [],
@@ -6156,37 +6289,37 @@
                                 value: r[0] ? r[1] : void 0,
                                 done: !0
                             }
                         }([r, o])
                     }
                 }
             },
-            o = Di && Di.__rest || function(e, t) {
+            o = Ji && Ji.__rest || function(e, t) {
                 var n = {};
                 for (var i in e) Object.prototype.hasOwnProperty.call(e, i) && t.indexOf(i) < 0 && (n[i] = e[i]);
                 if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                     var a = 0;
                     for (i = Object.getOwnPropertySymbols(e); a < i.length; a++) t.indexOf(i[a]) < 0 && Object.prototype.propertyIsEnumerable.call(e, i[a]) && (n[i[a]] = e[i[a]])
                 }
                 return n
             },
-            s = Di && Di.__importDefault || function(e) {
+            s = Ji && Ji.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             };
         Object.defineProperty(e, "__esModule", {
             value: !0
         }), e.gql = e.request = e.rawRequest = e.GraphQLClient = e.ClientError = void 0;
-        var c = a(Qi.exports),
+        var c = a(Mi.exports),
             u = c,
-            A = la,
-            d = s(oa),
-            f = ya,
-            h = ya;
+            d = da,
+            A = s(Aa),
+            f = Ca,
+            h = Ca;
         Object.defineProperty(e, "ClientError", {
             enumerable: !0,
             get: function() {
                 return h.ClientError
             }
         });
         var m = function(e) {
@@ -6204,25 +6337,25 @@
             },
             p = function() {
                 function e(e, t) {
                     this.url = e, this.options = t || {}
                 }
                 return e.prototype.rawRequest = function(e, n, i) {
                     return r(this, void 0, void 0, (function() {
-                        var a, r, s, u, A, h, p, g, y, E, b;
+                        var a, r, s, u, d, h, p, g, y, E, b;
                         return l(this, (function(l) {
                             switch (l.label) {
                                 case 0:
-                                    return a = this.options, r = a.headers, s = a.fetch, u = void 0 === s ? c.default : s, A = o(a, ["headers", "fetch"]), h = d.default(e, n), [4, u(this.url, t({
+                                    return a = this.options, r = a.headers, s = a.fetch, u = void 0 === s ? c.default : s, d = o(a, ["headers", "fetch"]), h = A.default(e, n), [4, u(this.url, t({
                                         method: "POST",
                                         headers: t(t(t({}, "string" == typeof h ? {
                                             "Content-Type": "application/json"
                                         } : {}), m(r)), m(i)),
                                         body: h
-                                    }, A))];
+                                    }, d))];
                                 case 1:
                                     return [4, v(p = l.sent())];
                                 case 2:
                                     if (g = l.sent(), p.ok && !g.errors && g.data) return y = p.headers, E = p.status, [2, t(t({}, g), {
                                         headers: y,
                                         status: E
                                     })];
@@ -6241,16 +6374,16 @@
                 }, e.prototype.request = function(e, n, i) {
                     return r(this, void 0, void 0, (function() {
                         var a, r, s, u, h, p, g, y, E, b;
                         return l(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return a = this.options, r = a.headers, s = a.fetch, u = void 0 === s ? c.default : s, h = o(a, ["headers", "fetch"]), p = function(e) {
-                                        return "string" == typeof e ? e : A.print(e)
-                                    }(e), g = d.default(p, n), [4, u(this.url, t({
+                                        return "string" == typeof e ? e : d.print(e)
+                                    }(e), g = A.default(p, n), [4, u(this.url, t({
                                         method: "POST",
                                         headers: t(t(t({}, "string" == typeof g ? {
                                             "Content-Type": "application/json"
                                         } : {}), m(r)), m(i)),
                                         body: g
                                     }, h))];
                                 case 1:
@@ -6296,21 +6429,21 @@
             }))
         }, e.request = g, e.default = g, e.gql = function(e) {
             for (var t = [], n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
             return e.reduce((function(e, n, i) {
                 return "" + e + n + (i in t ? t[i] : "")
             }), "")
         }
-    }(Ni);
+    }(qi);
 
-function Ia(e) {
+function La(e) {
     let t;
 
     function n(e, t) {
-        return e[2] ? Sa : Ba
+        return e[2] ? Ra : ka
     }
     let i = n(e),
         a = i(e);
     return {
         c() {
             a.c(), t = j()
         },
@@ -6325,15 +6458,15 @@
         },
         d(e) {
             a.d(e), e && D(t)
         }
     }
 }
 
-function wa(e) {
+function Pa(e) {
     let t, n;
     return {
         c() {
             t = N("p"), n = W("Saving..."), this.h()
         },
         l(e) {
             t = _(e, "P", {
@@ -6351,15 +6484,15 @@
         p: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Ca(e) {
+function xa(e) {
     let t, n;
     return {
         c() {
             t = N("p"), n = W("Loading..."), this.h()
         },
         l(e) {
             t = _(e, "P", {
@@ -6377,15 +6510,15 @@
         p: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Ba(e) {
+function ka(e) {
     let t, n;
     return {
         c() {
             t = N("p"), n = W("Disconnected"), this.h()
         },
         l(e) {
             t = _(e, "P", {
@@ -6402,15 +6535,15 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function Sa(e) {
+function Ra(e) {
     let t, n;
     return {
         c() {
             t = N("p"), n = W("Connected"), this.h()
         },
         l(e) {
             t = _(e, "P", {
@@ -6427,19 +6560,19 @@
         },
         d(e) {
             e && D(t)
         }
     }
 }
 
-function La(e) {
+function Va(e) {
     let t;
 
     function n(e, t) {
-        return e[0] ? e[1] ? wa : null !== e[2] ? Ia : void 0 : Ca
+        return e[0] ? e[1] ? Pa : null !== e[2] ? La : void 0 : xa
     }
     let i = n(e),
         a = i && i(e);
     return {
         c() {
             a && a.c(), t = j()
         },
@@ -6456,36 +6589,36 @@
         o: c,
         d(e) {
             a && a.d(e), e && D(t)
         }
     }
 }
 
-function Pa(e, t, n) {
+function Xa(e, t, n) {
     let {
         loaded: i
     } = t, {
         saving: a = !1
     } = t, {
         listening: r = null
     } = t;
     return e.$$set = e => {
         "loaded" in e && n(0, i = e.loaded), "saving" in e && n(1, a = e.saving), "listening" in e && n(2, r = e.listening)
     }, [i, a, r]
 }
-class xa extends it {
+class Oa extends at {
     constructor(e) {
-        super(), nt(this, e, Pa, La, p, {
+        super(), it(this, e, Xa, Va, p, {
             loaded: 0,
             saving: 1,
             listening: 2
         })
     }
 }
-var ka = {
+var Fa = {
     kind: "Document",
     definitions: [{
         kind: "OperationDefinition",
         operation: "query",
         name: {
             kind: "Name",
             value: "Balancing"
@@ -6700,75 +6833,75 @@
     }],
     loc: {
         start: 0,
         end: 312
     }
 };
 
-function Ra(e, t) {
+function Ua(e, t) {
     if ("FragmentSpread" === e.kind) t.add(e.name.value);
     else if ("VariableDefinition" === e.kind) {
         var n = e.type;
         "NamedType" === n.kind && t.add(n.name.value)
     }
     e.selectionSet && e.selectionSet.selections.forEach((function(e) {
-        Ra(e, t)
+        Ua(e, t)
     })), e.variableDefinitions && e.variableDefinitions.forEach((function(e) {
-        Ra(e, t)
+        Ua(e, t)
     })), e.definitions && e.definitions.forEach((function(e) {
-        Ra(e, t)
+        Ua(e, t)
     }))
 }
-ka.loc.source = {
+Fa.loc.source = {
     body: "query Balancing($run: ID!) {\n  balancing(runId: $run) {\n    sessions {\n      id\n      name\n    }\n    players {\n      id\n      session\n      name\n      email\n      inactive\n      ready\n    }\n    teams {\n      id\n      session\n      name\n      ready\n      players\n    }\n    minimumPlayers\n    maximumPlayers\n  }\n}\n",
     name: "GraphQL request",
     locationOffset: {
         line: 1,
         column: 1
     }
 };
-var Va = {};
+var za = {};
 
-function Xa(e, t) {
+function Ta(e, t) {
     for (var n = 0; n < e.definitions.length; n++) {
         var i = e.definitions[n];
         if (i.name && i.name.value == t) return i
     }
 }
-ka.definitions.forEach((function(e) {
+Fa.definitions.forEach((function(e) {
         if (e.name) {
             var t = new Set;
-            Ra(e, t), Va[e.name.value] = t
+            Ua(e, t), za[e.name.value] = t
         }
     })),
     function(e, t) {
         var n = {
             kind: e.kind,
-            definitions: [Xa(e, t)]
+            definitions: [Ta(e, t)]
         };
         e.hasOwnProperty("loc") && (n.loc = e.loc);
-        var i = Va[t] || new Set,
+        var i = za[t] || new Set,
             a = new Set,
             r = new Set;
         for (i.forEach((function(e) {
                 r.add(e)
             })); r.size > 0;) {
             var l = r;
             r = new Set, l.forEach((function(e) {
-                a.has(e) || (a.add(e), (Va[e] || new Set).forEach((function(e) {
+                a.has(e) || (a.add(e), (za[e] || new Set).forEach((function(e) {
                     r.add(e)
                 })))
             }))
         }
         a.forEach((function(t) {
-            var i = Xa(e, t);
+            var i = Ta(e, t);
             i && n.definitions.push(i)
         }))
-    }(ka, "Balancing");
-var Oa = {
+    }(Fa, "Balancing");
+var Da = {
     kind: "Document",
     definitions: [{
         kind: "OperationDefinition",
         operation: "mutation",
         name: {
             kind: "Name",
             value: "AlterPlayer"
@@ -6900,75 +7033,75 @@
     }],
     loc: {
         start: 0,
         end: 169
     }
 };
 
-function Fa(e, t) {
+function Ha(e, t) {
     if ("FragmentSpread" === e.kind) t.add(e.name.value);
     else if ("VariableDefinition" === e.kind) {
         var n = e.type;
         "NamedType" === n.kind && t.add(n.name.value)
     }
     e.selectionSet && e.selectionSet.selections.forEach((function(e) {
-        Fa(e, t)
+        Ha(e, t)
     })), e.variableDefinitions && e.variableDefinitions.forEach((function(e) {
-        Fa(e, t)
+        Ha(e, t)
     })), e.definitions && e.definitions.forEach((function(e) {
-        Fa(e, t)
+        Ha(e, t)
     }))
 }
-Oa.loc.source = {
+Da.loc.source = {
     body: "mutation AlterPlayer($playerId: ID!, $active: Boolean!) {\n  alterPlayer(playerId: $playerId, active: $active) {\n    id\n    session\n    name\n    email\n    inactive\n  }\n}\n",
     name: "GraphQL request",
     locationOffset: {
         line: 1,
         column: 1
     }
 };
-var Ua = {};
+var Na = {};
 
-function za(e, t) {
+function Qa(e, t) {
     for (var n = 0; n < e.definitions.length; n++) {
         var i = e.definitions[n];
         if (i.name && i.name.value == t) return i
     }
 }
-Oa.definitions.forEach((function(e) {
+Da.definitions.forEach((function(e) {
         if (e.name) {
             var t = new Set;
-            Fa(e, t), Ua[e.name.value] = t
+            Ha(e, t), Na[e.name.value] = t
         }
     })),
     function(e, t) {
         var n = {
             kind: e.kind,
-            definitions: [za(e, t)]
+            definitions: [Qa(e, t)]
         };
         e.hasOwnProperty("loc") && (n.loc = e.loc);
-        var i = Ua[t] || new Set,
+        var i = Na[t] || new Set,
             a = new Set,
             r = new Set;
         for (i.forEach((function(e) {
                 r.add(e)
             })); r.size > 0;) {
             var l = r;
             r = new Set, l.forEach((function(e) {
-                a.has(e) || (a.add(e), (Ua[e] || new Set).forEach((function(e) {
+                a.has(e) || (a.add(e), (Na[e] || new Set).forEach((function(e) {
                     r.add(e)
                 })))
             }))
         }
         a.forEach((function(t) {
-            var i = za(e, t);
+            var i = Qa(e, t);
             i && n.definitions.push(i)
         }))
-    }(Oa, "AlterPlayer");
-var Ta = {
+    }(Da, "AlterPlayer");
+var Wa = {
     kind: "Document",
     definitions: [{
         kind: "OperationDefinition",
         operation: "mutation",
         name: {
             kind: "Name",
             value: "UpdateBalancing"
@@ -7255,101 +7388,101 @@
     }],
     loc: {
         start: 0,
         end: 409
     }
 };
 
-function Da(e, t) {
+function Ja(e, t) {
     if ("FragmentSpread" === e.kind) t.add(e.name.value);
     else if ("VariableDefinition" === e.kind) {
         var n = e.type;
         "NamedType" === n.kind && t.add(n.name.value)
     }
     e.selectionSet && e.selectionSet.selections.forEach((function(e) {
-        Da(e, t)
+        Ja(e, t)
     })), e.variableDefinitions && e.variableDefinitions.forEach((function(e) {
-        Da(e, t)
+        Ja(e, t)
     })), e.definitions && e.definitions.forEach((function(e) {
-        Da(e, t)
+        Ja(e, t)
     }))
 }
-Ta.loc.source = {
+Wa.loc.source = {
     body: "mutation UpdateBalancing($run: ID!, $teams: [TeamInput!], $deleteTeams: [ID!]) {\n  balanceTeams(runId: $run, teams: $teams, deleteTeams: $deleteTeams) {\n    sessions {\n      id\n      name\n    }\n    players {\n      id\n      session\n      name\n      email\n      inactive\n      ready\n    }\n    teams {\n      id\n      session\n      name\n      players\n      ready\n    }\n    minimumPlayers\n    maximumPlayers\n  }\n}\n",
     name: "GraphQL request",
     locationOffset: {
         line: 1,
         column: 1
     }
 };
-var Ha = {};
+var ja = {};
 
-function Na(e, t) {
+function qa(e, t) {
     for (var n = 0; n < e.definitions.length; n++) {
         var i = e.definitions[n];
         if (i.name && i.name.value == t) return i
     }
 }
 
-function Qa(e) {
+function Ma(e) {
     let t, n;
-    return t = new xa({
+    return t = new Oa({
         props: {
             loaded: e[1],
             saving: e[0]
         }
     }), {
         c() {
-            Ge(t.$$.fragment)
+            $e(t.$$.fragment)
         },
         l(e) {
-            $e(t.$$.fragment, e)
+            _e(t.$$.fragment, e)
         },
         m(e, i) {
-            _e(t, e, i), n = !0
+            et(t, e, i), n = !0
         },
         p(e, [n]) {
             const i = {};
             2 & n && (i.loaded = e[1]), 1 & n && (i.saving = e[0]), t.$set(i)
         },
         i(e) {
-            n || (De(t.$$.fragment, e), n = !0)
+            n || (He(t.$$.fragment, e), n = !0)
         },
         o(e) {
-            He(t.$$.fragment, e), n = !1
+            Ne(t.$$.fragment, e), n = !1
         },
         d(e) {
-            et(t, e)
+            tt(t, e)
         }
     }
 }
 
-function Wa(e, t, n) {
+function Ka(e, t, n) {
     let i, a;
-    y(e, lt, (e => n(4, i = e))), y(e, ot, (e => n(1, a = e)));
+    y(e, ot, (e => n(4, i = e))), y(e, st, (e => n(1, a = e)));
     let {
         endpoint: r = "/graphql/"
     } = t, {
         run: l
     } = t, c = !1;
-    const u = new Ni.GraphQLClient(r, {
+    const u = new qi.GraphQLClient(r, {
         credentials: "include"
     });
-    var A, d = {};
+    var d = {};
     return ge((() => {
-        B(ot, a = !1, a), u.request(ka, {
+        B(st, a = !1, a), u.request(Fa, {
             run: l
         }).then((e => {
-            (null == e ? void 0 : e.balancing) && (d = JSON.parse(JSON.stringify(e.balancing)), B(lt, i = e.balancing, i)), B(ot, a = !0, a)
+            (null == e ? void 0 : e.balancing) && (d = JSON.parse(JSON.stringify(e.balancing)), B(ot, i = e.balancing, i)), B(st, a = !0, a)
         }))
-    })), A = st.subscribe((async e => {
+    })), ve(ct.subscribe((async e => {
         if (!e) return;
-        let t = await u.request(Oa, e);
-        (null == t ? void 0 : t.alterPlayer) && B(lt, i.players = i.players.map((e => e.id == t.alterPlayer.id ? Object.assign(e, t.alterPlayer) : e)), i)
-    })), pe().$$.on_destroy.push(A), e.$$set = e => {
+        let t = await u.request(Da, e);
+        (null == t ? void 0 : t.alterPlayer) && B(ot, i.players = i.players.map((e => e.id == t.alterPlayer.id ? Object.assign(e, t.alterPlayer) : e)), i)
+    }))), e.$$set = e => {
         "endpoint" in e && n(2, r = e.endpoint), "run" in e && n(3, l = e.run)
     }, e.$$.update = () => {
         19 & e.$$.dirty && a && i && !c && (console.debug("checking for changes"), function() {
             if (!d.teams) return;
             const e = i.teams.map((e => e.id)),
                 t = {
                     run: l,
@@ -7358,75 +7491,75 @@
                         const t = d.teams.find((t => t.id === e.id));
                         return !t || t.name !== e.name || t.players.length !== e.players.length || !t.players.every((t => e.players.includes(t)))
                     })).map((e => s(o({}, e), {
                         ready: void 0,
                         internalId: void 0
                     })))
                 };
-            (t.deleteTeams.length || t.teams.length) && (console.debug("updating data"), n(0, c = !0), d = JSON.parse(JSON.stringify(i)), u.request(Ta, t).then((e => {
+            (t.deleteTeams.length || t.teams.length) && (console.debug("updating data"), n(0, c = !0), d = JSON.parse(JSON.stringify(i)), u.request(Wa, t).then((e => {
                 if (null == e ? void 0 : e.balanceTeams) {
                     const t = i.teams.filter((e => e.internalId));
-                    B(lt, i = s(o({}, e.balanceTeams), {
+                    B(ot, i = s(o({}, e.balanceTeams), {
                         teams: e.balanceTeams.teams.map((e => {
                             var n = t.find((t => t.id === e.id)) || t.find((t => t.name === e.name));
                             return n ? s(o({}, e), {
                                 internalId: n.internalId
                             }) : e
                         }))
                     }), i), d = JSON.parse(JSON.stringify(i))
                 }
                 n(0, c = !1)
             })))
         }())
     }, [c, a, r, l, i]
 }
-Ta.definitions.forEach((function(e) {
+Wa.definitions.forEach((function(e) {
         if (e.name) {
             var t = new Set;
-            Da(e, t), Ha[e.name.value] = t
+            Ja(e, t), ja[e.name.value] = t
         }
     })),
     function(e, t) {
         var n = {
             kind: e.kind,
-            definitions: [Na(e, t)]
+            definitions: [qa(e, t)]
         };
         e.hasOwnProperty("loc") && (n.loc = e.loc);
-        var i = Ha[t] || new Set,
+        var i = ja[t] || new Set,
             a = new Set,
             r = new Set;
         for (i.forEach((function(e) {
                 r.add(e)
             })); r.size > 0;) {
             var l = r;
             r = new Set, l.forEach((function(e) {
-                a.has(e) || (a.add(e), (Ha[e] || new Set).forEach((function(e) {
+                a.has(e) || (a.add(e), (ja[e] || new Set).forEach((function(e) {
                     r.add(e)
                 })))
             }))
         }
         a.forEach((function(t) {
-            var i = Na(e, t);
+            var i = qa(e, t);
             i && n.definitions.push(i)
         }))
-    }(Ta, "UpdateBalancing");
-class Ja extends it {
+    }(Wa, "UpdateBalancing");
+class Za extends at {
     constructor(e) {
-        super(), nt(this, e, Wa, Qa, p, {
+        super(), it(this, e, Ka, Ma, p, {
             endpoint: 2,
             run: 3
         })
     }
 }
 
-function ja(e) {
+function Ya(e) {
     let t;
 
     function n(e, t) {
-        return 1 == e[3] ? Ma : qa
+        return 1 == e[3] ? $a : Ga
     }
     let i = n(e),
         a = i(e);
     return {
         c() {
             t = N("span"), a.c(), this.h()
         },
@@ -7448,15 +7581,15 @@
         },
         d(e) {
             e && D(t), a.d()
         }
     }
 }
 
-function qa(e) {
+function Ga(e) {
     let t, n;
     return {
         c() {
             t = W(e[3]), n = W(" players need balancing")
         },
         l(i) {
             t = ee(i, e[3]), n = ee(i, " players need balancing")
@@ -7469,15 +7602,15 @@
         },
         d(e) {
             e && D(t), e && D(n)
         }
     }
 }
 
-function Ma(e) {
+function $a(e) {
     let t, n;
     return {
         c() {
             t = W(e[3]), n = W(" player needs balancing")
         },
         l(i) {
             t = ee(i, e[3]), n = ee(i, " player needs balancing")
@@ -7490,16 +7623,16 @@
         },
         d(e) {
             e && D(t), e && D(n)
         }
     }
 }
 
-function Ka(e) {
-    let t, n, i, a, r, l = e[3] && ja(e);
+function _a(e) {
+    let t, n, i, a, r, l = e[3] && Ya(e);
     return {
         c() {
             t = N("li"), n = N("a"), i = N("span"), a = W("Manage Teams"), r = J(), l && l.c(), this.h()
         },
         l(e) {
             t = _(e, "LI", {
                 class: !0
@@ -7519,51 +7652,51 @@
         h() {
             Z(i, "class", "todo-link-title"), Z(n, "class", "todo-link"), Z(n, "href", e[1]), re(n, "is-active", e[0]), re(n, "is-alert", e[3]), re(n, "is-complete", !e[3] && e[2].length), Z(t, "class", "todo-item")
         },
         m(e, o) {
             T(e, t, o), z(t, n), z(n, i), z(i, a), z(n, r), l && l.m(n, null)
         },
         p(e, [t]) {
-            e[3] ? l ? l.p(e, t) : (l = ja(e), l.c(), l.m(n, null)) : l && (l.d(1), l = null), 2 & t && Z(n, "href", e[1]), 1 & t && re(n, "is-active", e[0]), 8 & t && re(n, "is-alert", e[3]), 12 & t && re(n, "is-complete", !e[3] && e[2].length)
+            e[3] ? l ? l.p(e, t) : (l = Ya(e), l.c(), l.m(n, null)) : l && (l.d(1), l = null), 2 & t && Z(n, "href", e[1]), 1 & t && re(n, "is-active", e[0]), 8 & t && re(n, "is-alert", e[3]), 12 & t && re(n, "is-complete", !e[3] && e[2].length)
         },
         i: c,
         o: c,
         d(e) {
             e && D(t), l && l.d()
         }
     }
 }
 
-function Za(e, t, n) {
+function er(e, t, n) {
     let i;
-    y(e, lt, (e => n(4, i = e)));
+    y(e, ot, (e => n(4, i = e)));
     let a, {
             active: r = !1
         } = t,
         {
             href: l
         } = t,
         o = [];
     return e.$$set = e => {
         "active" in e && n(0, r = e.active), "href" in e && n(1, l = e.href)
     }, e.$$.update = () => {
         var t;
         20 & e.$$.dirty && (n(2, o = i.teams.flatMap((e => e.players))), n(3, a = null == (t = i.players) ? void 0 : t.filter((e => !o.includes(e.id) && !e.inactive)).length))
     }, [r, l, o, a, i]
 }
-class Ya extends it {
+class tr extends at {
     constructor(e) {
-        super(), nt(this, e, Za, Ka, p, {
+        super(), it(this, e, er, _a, p, {
             active: 0,
             href: 1
         })
     }
 }
 
-function Ga(e) {
+function nr(e) {
     let t, n, i, a;
     return {
         c() {
             t = N("li"), n = N("a"), i = N("span"), a = W("Start Game"), this.h()
         },
         l(e) {
             t = _(e, "LI", {
@@ -7594,73 +7727,73 @@
         o: c,
         d(e) {
             e && D(t)
         }
     }
 }
 
-function $a(e, t, n) {
+function ir(e, t, n) {
     let i;
-    y(e, lt, (e => n(3, i = e)));
+    y(e, ot, (e => n(3, i = e)));
     let a, {
             href: r = null
         } = t,
         l = [];
     return e.$$set = e => {
         "href" in e && n(0, r = e.href)
     }, e.$$.update = () => {
         var t;
         10 & e.$$.dirty && (n(1, l = i.teams.flatMap((e => e.players))), n(2, a = null == (t = i.players) ? void 0 : t.filter((e => !l.includes(e.id))).length))
     }, [r, l, a, i]
 }
-class _a extends it {
+class ar extends at {
     constructor(e) {
-        super(), nt(this, e, $a, Ga, p, {
+        super(), it(this, e, ir, nr, p, {
             href: 0
         })
     }
 }
 
-function er(e) {
-    e || (e = document.getElementById("app")), new Ti({
+function rr(e) {
+    e || (e = document.getElementById("app")), new Wi({
         target: e,
         props: e.dataset
     });
     const t = document.getElementById("loader");
-    t && new Ja({
+    t && new Za({
         target: t,
         props: t.dataset
-    }), lt.subscribe((e => {
+    }), ot.subscribe((e => {
         if (!e.players) return;
         const t = document.getElementById("simpl-team-nav");
         if (t) {
             const e = t.getElementsByTagName("A")[0];
-            new Ya({
+            new tr({
                 target: t,
                 hydrate: !0,
                 props: {
                     href: e.href,
                     active: e.classList.contains("is-active")
                 }
             })
         }
         const n = document.getElementById("simpl-start-nav");
         if (n) {
             const e = n.getElementsByTagName("A")[0].href;
-            new _a({
+            new ar({
                 target: n,
                 hydrate: !0,
                 props: {
                     href: e
                 }
             })
         }
     }))
 }
-class tr {
+class lr {
     constructor() {
         this.buttonAttr = "data-toggle-elements", document.querySelectorAll(`[${this.buttonAttr}]`).forEach(this.initComponent, this)
     }
     toggleEl(e) {
         document.querySelectorAll(e).forEach((e => {
             e.classList.contains("hide") ? e.classList.remove("hide") : e.classList.add("hide")
         }))
@@ -7668,15 +7801,15 @@
     initComponent(e) {
         const t = e.getAttribute(this.buttonAttr);
         e.addEventListener("click", (e => {
             e.preventDefault(), this.toggleEl(t)
         }))
     }
 }
-class nr {
+class or {
     constructor() {
         this.collapsibleAttr = "data-is-accordion", this.toggleButtonAttr = "data-toggle-collapsible", this.expandAllAttr = "data-expand-all", this.collapseAllAttr = "data-collapse-all", this.allCollapsibles = document.querySelectorAll(`[${this.collapsibleAttr}]`), this.toggleButtons = document.querySelectorAll(`[${this.toggleButtonAttr}]`), this.expandAllButtons = document.querySelectorAll(`[${this.expandAllAttr}]`), this.collapseAllButtons = document.querySelectorAll(`[${this.collapseAllAttr}]`), this.toggleButtons.forEach((e => e.addEventListener("click", (t => this.toggleCollapsible(e))))), this.expandAllButtons.forEach((e => e.addEventListener("click", (e => this.expandAll())))), this.collapseAllButtons.forEach((e => e.addEventListener("click", (e => this.collapseAll()))))
     }
     hide(e) {
         e.classList.add("hide")
     }
     show(e) {
@@ -7698,26 +7831,26 @@
     expandAll() {
         this.expandAllButtons.forEach((e => this.hide(e))), this.collapseAllButtons.forEach((e => this.show(e))), this.allCollapsibles.forEach((e => this.show(e))), this.toggleButtons.forEach((e => this.setExpanded(e)))
     }
     collapseAll() {
         this.collapseAllButtons.forEach((e => this.hide(e))), this.expandAllButtons.forEach((e => this.show(e))), this.allCollapsibles.forEach((e => this.hide(e))), this.toggleButtons.forEach((e => this.removeExpanded(e)))
     }
 }
-class ir {
+class sr {
     constructor() {
         this.selector = "[data-toast]", document.querySelectorAll(this.selector).forEach(this.initComponent, this)
     }
     initComponent(e) {
         const t = parseInt(e.getAttribute("data-timeout")) || 5e3;
         setTimeout((() => {
             e.classList.contains("collapse") ? e.classList.remove("in") : e.classList.add("hide")
         }), t)
     }
 }
-class ar {
+class cr {
     constructor() {
         this.selector = ".field-pair", document.querySelectorAll(this.selector).forEach(this.initComponent, this)
     }
     toggleCheckboxes(e) {
         this.checkbox = e.querySelector("[type=checkbox]"), this.willDisable = e.querySelector("[data-disabled-when-unchecked]"), this.willDisableFields = this.willDisable.querySelectorAll("input");
         let t = !!e.querySelector("[data-disable-fields]:checked");
         t ? this.willDisableFields.forEach((e => e.removeAttribute("disabled"))) : this.willDisableFields.forEach((e => e.setAttribute("disabled", "disabled"))), this.willDisable.classList.toggle("is-disabled", !t), e.classList.toggle("has-checked", t)
@@ -7725,13 +7858,13 @@
     initComponent(e) {
         this.toggleCheckboxes(e), this.checkbox.addEventListener("change", (() => {
             this.toggleCheckboxes(e)
         }))
     }
 }
 
-function rr() {
-    new tr, new ir, new ar, new nr
+function ur() {
+    new lr, new sr, new cr, new or
 }
 export {
-    tr as ToggleElement, er as initBalancing, rr as initComponents
+    lr as ToggleElement, rr as initBalancing, ur as initComponents
 };
```

### Comparing `simpl-cloud-1.2.4/simpl/static/simpl/simpl.umd.js` & `simpl-cloud-1.3.0/simpl/static/simpl/simpl.umd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -142,27 +142,27 @@
         for (; e < t;) {
             const a = e + (t - e >> 1);
             n(a) <= i ? e = a + 1 : t = a
         }
         return e
     }
 
-    function P(e) {
+    function L(e) {
         if (!e) return document;
         const t = e.getRootNode ? e.getRootNode() : e.ownerDocument;
         return t.host ? t : document
     }
 
-    function L(e) {
+    function P(e) {
         const t = O("style");
         return function(e, t) {
             ! function(e, t) {
                 e.appendChild(t)
             }(e.head || e, t)
-        }(P(e), t), t
+        }(L(e), t), t
     }
 
     function x(e, t) {
         if (B) {
             for (! function(e) {
                     if (e.hydrate_init) return;
                     e.hydrate_init = !0;
@@ -225,23 +225,23 @@
         return document.createElementNS("http://www.w3.org/2000/svg", e)
     }
 
     function F(e) {
         return document.createTextNode(e)
     }
 
-    function U() {
+    function T() {
         return F(" ")
     }
 
-    function z() {
+    function U() {
         return F("")
     }
 
-    function T(e, t, n, i) {
+    function z(e, t, n, i) {
         return e.addEventListener(t, n, i), () => e.removeEventListener(t, n, i)
     }
 
     function D(e) {
         return function(t) {
             return t.preventDefault(), e.call(this, t)
         }
@@ -344,17 +344,17 @@
         let c = "{\n";
         for (let p = 0; p <= 1; p += s) {
             const e = t + (n - t) * r(p);
             c += 100 * p + `%{${l(e,1-e)}}\n`
         }
         const u = c + `100% {${l(n,1-n)}}\n}`,
             d = `__svelte_${function(e){let t=5381,n=e.length;for(;n--;)t=(t<<5)-t^e.charCodeAt(n);return t>>>0}(u)}_${o}`,
-            A = P(e);
+            A = L(e);
         _.add(A);
-        const f = A.__svelte_stylesheet || (A.__svelte_stylesheet = L(e).sheet),
+        const f = A.__svelte_stylesheet || (A.__svelte_stylesheet = P(e).sheet),
             h = A.__svelte_rules || (A.__svelte_rules = {});
         h[d] || (h[d] = !0, f.insertRule(`@keyframes ${d} ${u}`, f.cssRules.length));
         const m = e.style.animation || "";
         return e.style.animation = `${m?`${m}, `:""}${d} ${i}ms linear ${a}ms 1 both`, te += 1, d
     }
 
     function ie(e, t) {
@@ -432,118 +432,122 @@
         return ee
     }
 
     function ce(e) {
         se().$$.on_mount.push(e)
     }
 
-    function ue() {
+    function ue(e) {
+        se().$$.on_destroy.push(e)
+    }
+
+    function de() {
         const e = se();
         return (t, n) => {
             const i = e.$$.callbacks[t];
             if (i) {
                 const a = $(t, n);
                 i.slice().forEach((t => {
                     t.call(e, a)
                 }))
             }
         }
     }
 
-    function de(e, t) {
+    function Ae(e, t) {
         const n = e.$$.callbacks[t.type];
         n && n.slice().forEach((e => e.call(this, t)))
     }
-    const Ae = [],
-        fe = [],
+    const fe = [],
         he = [],
         me = [],
-        pe = Promise.resolve();
-    let ge = !1;
-
-    function ve(e) {
-        he.push(e)
-    }
+        pe = [],
+        ge = Promise.resolve();
+    let ve = !1;
 
     function ye(e) {
         me.push(e)
     }
-    let Ee = !1;
-    const be = new Set;
 
-    function Ie() {
-        if (!Ee) {
-            Ee = !0;
+    function Ee(e) {
+        pe.push(e)
+    }
+    let be = !1;
+    const Ie = new Set;
+
+    function we() {
+        if (!be) {
+            be = !0;
             do {
-                for (let e = 0; e < Ae.length; e += 1) {
-                    const t = Ae[e];
-                    oe(t), we(t.$$)
+                for (let e = 0; e < fe.length; e += 1) {
+                    const t = fe[e];
+                    oe(t), Ce(t.$$)
                 }
-                for (oe(null), Ae.length = 0; fe.length;) fe.pop()();
-                for (let e = 0; e < he.length; e += 1) {
-                    const t = he[e];
-                    be.has(t) || (be.add(t), t())
+                for (oe(null), fe.length = 0; he.length;) he.pop()();
+                for (let e = 0; e < me.length; e += 1) {
+                    const t = me[e];
+                    Ie.has(t) || (Ie.add(t), t())
                 }
-                he.length = 0
-            } while (Ae.length);
-            for (; me.length;) me.pop()();
-            ge = !1, Ee = !1, be.clear()
+                me.length = 0
+            } while (fe.length);
+            for (; pe.length;) pe.pop()();
+            ve = !1, be = !1, Ie.clear()
         }
     }
 
-    function we(e) {
+    function Ce(e) {
         if (null !== e.fragment) {
             e.update(), l(e.before_update);
             const t = e.dirty;
-            e.dirty = [-1], e.fragment && e.fragment.p(e.ctx, t), e.after_update.forEach(ve)
+            e.dirty = [-1], e.fragment && e.fragment.p(e.ctx, t), e.after_update.forEach(ye)
         }
     }
-    let Ce;
+    let Be;
 
-    function Be() {
-        return Ce || (Ce = Promise.resolve(), Ce.then((() => {
-            Ce = null
-        }))), Ce
+    function Se() {
+        return Be || (Be = Promise.resolve(), Be.then((() => {
+            Be = null
+        }))), Be
     }
 
-    function Se(e, t, n) {
+    function Le(e, t, n) {
         e.dispatchEvent($(`${t?"intro":"outro"}${n}`))
     }
     const Pe = new Set;
-    let Le;
+    let xe;
 
-    function xe() {
-        Le = {
+    function ke() {
+        xe = {
             r: 0,
             c: [],
-            p: Le
+            p: xe
         }
     }
 
-    function ke() {
-        Le.r || l(Le.c), Le = Le.p
+    function Re() {
+        xe.r || l(xe.c), xe = xe.p
     }
 
-    function Re(e, t) {
+    function Ve(e, t) {
         e && e.i && (Pe.delete(e), e.i(t))
     }
 
-    function Ve(e, t, n, i) {
+    function Oe(e, t, n, i) {
         if (e && e.o) {
             if (Pe.has(e)) return;
-            Pe.add(e), Le.c.push((() => {
+            Pe.add(e), xe.c.push((() => {
                 Pe.delete(e), i && (n && e.d(1), i())
             })), e.o(t)
         }
     }
-    const Oe = {
+    const Xe = {
         duration: 0
     };
 
-    function Xe(e, i, a) {
+    function Fe(e, i, a) {
         let r, l, s = i(e, a),
             c = !1,
             u = 0;
 
         function d() {
             r && ie(e, r)
         }
@@ -551,71 +555,71 @@
         function A() {
             const {
                 delay: i = 0,
                 duration: a = 300,
                 easing: o = n,
                 tick: A = t,
                 css: f
-            } = s || Oe;
+            } = s || Xe;
             f && (r = ne(e, 0, 1, a, i, o, f, u++)), A(0, 1);
             const h = E() + i,
                 m = h + a;
-            l && l.abort(), c = !0, ve((() => Se(e, !0, "start"))), l = C((t => {
+            l && l.abort(), c = !0, ye((() => Le(e, !0, "start"))), l = C((t => {
                 if (c) {
-                    if (t >= m) return A(1, 0), Se(e, !0, "end"), d(), c = !1;
+                    if (t >= m) return A(1, 0), Le(e, !0, "end"), d(), c = !1;
                     if (t >= h) {
                         const e = o((t - h) / a);
                         A(e, 1 - e)
                     }
                 }
                 return c
             }))
         }
         let f = !1;
         return {
             start() {
-                f || (f = !0, ie(e), o(s) ? (s = s(), Be().then(A)) : A())
+                f || (f = !0, ie(e), o(s) ? (s = s(), Se().then(A)) : A())
             },
             invalidate() {
                 f = !1
             },
             end() {
                 c && (d(), c = !1)
             }
         }
     }
 
-    function Fe(e, i, a) {
+    function Te(e, i, a) {
         let r, s = i(e, a),
             c = !0;
-        const u = Le;
+        const u = xe;
 
         function d() {
             const {
                 delay: i = 0,
                 duration: a = 300,
                 easing: o = n,
                 tick: d = t,
                 css: A
-            } = s || Oe;
+            } = s || Xe;
             A && (r = ne(e, 1, 0, a, i, o, A));
             const f = E() + i,
                 h = f + a;
-            ve((() => Se(e, !1, "start"))), C((t => {
+            ye((() => Le(e, !1, "start"))), C((t => {
                 if (c) {
-                    if (t >= h) return d(0, 1), Se(e, !1, "end"), --u.r || l(u.c), !1;
+                    if (t >= h) return d(0, 1), Le(e, !1, "end"), --u.r || l(u.c), !1;
                     if (t >= f) {
                         const e = o((t - f) / a);
                         d(1 - e, e)
                     }
                 }
                 return c
             }))
         }
-        return u.r += 1, o(s) ? Be().then((() => {
+        return u.r += 1, o(s) ? Se().then((() => {
             s = s(), d()
         })) : d(), {
             end(t) {
                 t && s.tick && s.tick(1, 0), c && (r && ie(e, r), c = !1)
             }
         }
     }
@@ -647,56 +651,56 @@
         function m(i) {
             const {
                 delay: a = 0,
                 duration: r = 300,
                 easing: o = n,
                 tick: m = t,
                 css: p
-            } = s || Oe, g = {
+            } = s || Xe, g = {
                 start: E() + a,
                 b: i
             };
-            i || (g.group = Le, Le.r += 1), u || d ? d = g : (p && (f(), A = ne(e, c, i, r, a, o, p)), i && m(0, 1), u = h(g, r), ve((() => Se(e, i, "start"))), C((t => {
-                if (d && t > d.start && (u = h(d, r), d = null, Se(e, u.b, "start"), p && (f(), A = ne(e, c, u.b, u.duration, 0, o, s.css))), u)
-                    if (t >= u.end) m(c = u.b, 1 - c), Se(e, u.b, "end"), d || (u.b ? f() : --u.group.r || l(u.group.c)), u = null;
+            i || (g.group = xe, xe.r += 1), u || d ? d = g : (p && (f(), A = ne(e, c, i, r, a, o, p)), i && m(0, 1), u = h(g, r), ye((() => Le(e, i, "start"))), C((t => {
+                if (d && t > d.start && (u = h(d, r), d = null, Le(e, u.b, "start"), p && (f(), A = ne(e, c, u.b, u.duration, 0, o, s.css))), u)
+                    if (t >= u.end) m(c = u.b, 1 - c), Le(e, u.b, "end"), d || (u.b ? f() : --u.group.r || l(u.group.c)), u = null;
                     else if (t >= u.start) {
                     const e = t - u.start;
                     c = u.a + u.d * o(e / u.duration), m(c, 1 - c)
                 }
                 return !(!u && !d)
             })))
         }
         return {
             run(e) {
-                o(s) ? Be().then((() => {
+                o(s) ? Se().then((() => {
                     s = s(), m(e)
                 })) : m(e)
             },
             end() {
                 f(), u = d = null
             }
         }
     }
     const ze = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : global;
 
-    function Te(e, t) {
+    function De(e, t) {
         e.d(1), t.delete(e.key)
     }
 
-    function De(e, t) {
-        Ve(e, 1, 1, (() => {
+    function He(e, t) {
+        Oe(e, 1, 1, (() => {
             t.delete(e.key)
         }))
     }
 
-    function He(e, t) {
-        e.f(), De(e, t)
+    function Ne(e, t) {
+        e.f(), He(e, t)
     }
 
-    function Ne(e, t, n, i, a, r, l, o, s, c, u, d) {
+    function Qe(e, t, n, i, a, r, l, o, s, c, u, d) {
         let A = e.length,
             f = r.length,
             h = A;
         const m = {};
         for (; h--;) m[e[h].key] = h;
         const p = [],
             g = new Map,
@@ -707,15 +711,15 @@
             let s = l.get(o);
             s ? i && s.p(e, t) : (s = c(o, e), s.c()), g.set(o, p[h] = s), o in m && v.set(o, Math.abs(h - m[o]))
         }
         const y = new Set,
             E = new Set;
 
         function b(e) {
-            Re(e, 1), e.m(o, u), l.set(e.key, e), u = e.first, f--
+            Ve(e, 1), e.m(o, u), l.set(e.key, e), u = e.first, f--
         }
         for (; A && f;) {
             const t = p[f - 1],
                 n = e[A - 1],
                 i = t.key,
                 a = n.key;
             t === n ? (u = t.first, A--, f--) : g.has(a) ? !l.has(i) || y.has(i) ? b(t) : E.has(a) ? A-- : v.get(i) > v.get(a) ? (E.add(i), b(t)) : (y.add(a), A--) : (s(n, l), A--)
@@ -724,50 +728,50 @@
             const t = e[A];
             g.has(t.key) || s(t, l)
         }
         for (; f;) b(p[f - 1]);
         return p
     }
 
-    function Qe(e, t, n) {
+    function We(e, t, n) {
         const i = e.$$.props[t];
         void 0 !== i && (e.$$.bound[i] = n, n(e.$$.ctx[i]))
     }
 
-    function We(e) {
+    function Je(e) {
         e && e.c()
     }
 
-    function Je(e, t) {
+    function je(e, t) {
         e && e.l(t)
     }
 
-    function je(e, t, n, i) {
+    function qe(e, t, n, i) {
         const {
             fragment: r,
             on_mount: s,
             on_destroy: c,
             after_update: u
         } = e.$$;
-        r && r.m(t, n), i || ve((() => {
+        r && r.m(t, n), i || ye((() => {
             const t = s.map(a).filter(o);
             c ? c.push(...t) : l(t), e.$$.on_mount = []
-        })), u.forEach(ve)
+        })), u.forEach(ye)
     }
 
-    function qe(e, t) {
+    function Me(e, t) {
         const n = e.$$;
         null !== n.fragment && (l(n.on_destroy), n.fragment && n.fragment.d(t), n.on_destroy = n.fragment = null, n.ctx = [])
     }
 
-    function Me(e, t) {
-        -1 === e.$$.dirty[0] && (Ae.push(e), ge || (ge = !0, pe.then(Ie)), e.$$.dirty.fill(0)), e.$$.dirty[t / 31 | 0] |= 1 << t % 31
+    function Ke(e, t) {
+        -1 === e.$$.dirty[0] && (fe.push(e), ve || (ve = !0, ge.then(we)), e.$$.dirty.fill(0)), e.$$.dirty[t / 31 | 0] |= 1 << t % 31
     }
 
-    function Ke(e, n, i, a, o, s, c, u = [-1]) {
+    function Ze(e, n, i, a, o, s, c, u = [-1]) {
         const d = ee;
         oe(e);
         const A = e.$$ = {
             fragment: null,
             ctx: null,
             props: s,
             update: t,
@@ -784,53 +788,53 @@
             skip_bound: !1,
             root: n.target || d.$$.root
         };
         c && c(A.root);
         let f = !1;
         if (A.ctx = i ? i(e, n.props || {}, ((t, n, ...i) => {
                 const a = i.length ? i[0] : n;
-                return A.ctx && o(A.ctx[t], A.ctx[t] = a) && (!A.skip_bound && A.bound[t] && A.bound[t](a), f && Me(e, t)), n
+                return A.ctx && o(A.ctx[t], A.ctx[t] = a) && (!A.skip_bound && A.bound[t] && A.bound[t](a), f && Ke(e, t)), n
             })) : [], A.update(), f = !0, l(A.before_update), A.fragment = !!a && a(A.ctx), n.target) {
             if (n.hydrate) {
                 B = !0;
                 const e = W(n.target);
                 A.fragment && A.fragment.l(e), e.forEach(R)
             } else A.fragment && A.fragment.c();
-            n.intro && Re(e.$$.fragment), je(e, n.target, n.anchor, n.customElement), B = !1, Ie()
+            n.intro && Ve(e.$$.fragment), qe(e, n.target, n.anchor, n.customElement), B = !1, we()
         }
         oe(d)
     }
-    class Ze {
+    class Ye {
         $destroy() {
-            qe(this, 1), this.$destroy = t
+            Me(this, 1), this.$destroy = t
         }
         $on(e, t) {
             const n = this.$$.callbacks[e] || (this.$$.callbacks[e] = []);
             return n.push(t), () => {
                 const e = n.indexOf(t); - 1 !== e && n.splice(e, 1)
             }
         }
         $set(e) {
             var t;
             this.$$set && (t = e, 0 !== Object.keys(t).length) && (this.$$.skip_bound = !0, this.$$set(e), this.$$.skip_bound = !1)
         }
     }
-    const Ye = [];
+    const Ge = [];
 
-    function Ge(e, n = t) {
+    function $e(e, n = t) {
         let i;
         const a = new Set;
 
         function r(t) {
             if (s(e, t) && (e = t, i)) {
-                const t = !Ye.length;
-                for (const n of a) n[1](), Ye.push(n, e);
+                const t = !Ge.length;
+                for (const n of a) n[1](), Ge.push(n, e);
                 if (t) {
-                    for (let e = 0; e < Ye.length; e += 2) Ye[e][0](Ye[e + 1]);
-                    Ye.length = 0
+                    for (let e = 0; e < Ge.length; e += 2) Ge[e][0](Ge[e + 1]);
+                    Ge.length = 0
                 }
             }
         }
         return {
             set: r,
             update: function(t) {
                 r(t(e))
@@ -839,103 +843,103 @@
                 const s = [l, o];
                 return a.add(s), 1 === a.size && (i = n(r) || t), l(e), () => {
                     a.delete(s), 0 === a.size && (i(), i = null)
                 }
             }
         }
     }
-    const $e = Ge({
+    const _e = $e({
             sessions: [],
             teams: [],
             players: null,
             minimumPlayers: null,
             maximumPlayers: null
         }),
-        _e = Ge(!1);
-    const et = function() {
+        et = $e(!1);
+    const tt = function() {
         const e = new Set;
         return {
             subscribe: t => (e.add(t), () => {
                 e.delete(t)
             }),
             notify: t => {
                 e.forEach((e => e(t)))
             }
         }
     }();
-    var tt = window.CustomEvent;
+    var nt = window.CustomEvent;
 
-    function nt(e, t) {
+    function it(e, t) {
         var n = "on" + t.type.toLowerCase();
         return "function" == typeof e[n] && e[n](t), e.dispatchEvent(t)
     }
 
-    function it(e) {
+    function at(e) {
         for (; e;) {
             if ("dialog" === e.localName) return e;
             e = e.parentElement ? e.parentElement : e.parentNode ? e.parentNode.host : null
         }
         return null
     }
 
-    function at(e) {
+    function rt(e) {
         for (; e && e.shadowRoot && e.shadowRoot.activeElement;) e = e.shadowRoot.activeElement;
         e && e.blur && e !== document.body && e.blur()
     }
 
-    function rt(e, t) {
+    function lt(e, t) {
         for (var n = 0; n < e.length; ++n)
             if (e[n] === t) return !0;
         return !1
     }
 
-    function lt(e) {
+    function ot(e) {
         return !(!e || !e.hasAttribute("method")) && "dialog" === e.getAttribute("method").toLowerCase()
     }
 
-    function ot(e) {
+    function st(e) {
         var t = ["button", "input", "keygen", "select", "textarea"].map((function(e) {
             return e + ":not([disabled])"
         }));
         t.push('[tabindex]:not([disabled]):not([tabindex=""])');
         var n = e.querySelector(t.join(", "));
         if (!n && "attachShadow" in Element.prototype)
-            for (var i = e.querySelectorAll("*"), a = 0; a < i.length && !(i[a].tagName && i[a].shadowRoot && (n = ot(i[a].shadowRoot))); a++);
+            for (var i = e.querySelectorAll("*"), a = 0; a < i.length && !(i[a].tagName && i[a].shadowRoot && (n = st(i[a].shadowRoot))); a++);
         return n
     }
 
-    function st(e) {
+    function ct(e) {
         return e.isConnected || document.body.contains(e)
     }
 
-    function ct(e) {
+    function ut(e) {
         if (e.submitter) return e.submitter;
         var t = e.target;
         if (!(t instanceof HTMLFormElement)) return null;
-        var n = At.formSubmitter;
+        var n = ft.formSubmitter;
         if (!n) {
             var i = e.target;
             n = ("getRootNode" in i && i.getRootNode() || document).activeElement
         }
         return n && n.form === t ? n : null
     }
 
-    function ut(e) {
+    function dt(e) {
         if (!e.defaultPrevented) {
             var t = e.target,
-                n = At.imagemapUseValue,
-                i = ct(e);
+                n = ft.imagemapUseValue,
+                i = ut(e);
             null === n && i && (n = i.value);
-            var a = it(t);
+            var a = at(t);
             if (a) "dialog" === (i && i.getAttribute("formmethod") || t.getAttribute("method")) && (e.preventDefault(), null != n ? a.close(n) : a.close())
         }
     }
 
-    function dt(e) {
-        if (this.dialog_ = e, this.replacedStyleTop_ = !1, this.openAsModal_ = !1, e.hasAttribute("role") || e.setAttribute("role", "dialog"), e.show = this.show.bind(this), e.showModal = this.showModal.bind(this), e.close = this.close.bind(this), e.addEventListener("submit", ut, !1), "returnValue" in e || (e.returnValue = ""), "MutationObserver" in window) {
+    function At(e) {
+        if (this.dialog_ = e, this.replacedStyleTop_ = !1, this.openAsModal_ = !1, e.hasAttribute("role") || e.setAttribute("role", "dialog"), e.show = this.show.bind(this), e.showModal = this.showModal.bind(this), e.close = this.close.bind(this), e.addEventListener("submit", dt, !1), "returnValue" in e || (e.returnValue = ""), "MutationObserver" in window) {
             new MutationObserver(this.maybeHideModal.bind(this)).observe(e, {
                 attributes: !0,
                 attributeFilter: ["open"]
             })
         } else {
             var t, n = !1,
                 i = function() {
@@ -952,27 +956,27 @@
             }))
         }
         Object.defineProperty(e, "open", {
             set: this.setOpen.bind(this),
             get: e.hasAttribute.bind(e, "open")
         }), this.backdrop_ = document.createElement("div"), this.backdrop_.className = "backdrop", this.backdrop_.addEventListener("mouseup", this.backdropMouseEvent_.bind(this)), this.backdrop_.addEventListener("mousedown", this.backdropMouseEvent_.bind(this)), this.backdrop_.addEventListener("click", this.backdropMouseEvent_.bind(this))
     }
-    tt && "object" != typeof tt || ((tt = function(e, t) {
+    nt && "object" != typeof nt || ((nt = function(e, t) {
         t = t || {};
         var n = document.createEvent("CustomEvent");
         return n.initCustomEvent(e, !!t.bubbles, !!t.cancelable, t.detail || null), n
-    }).prototype = window.Event.prototype), dt.prototype = {
+    }).prototype = window.Event.prototype), At.prototype = {
         get dialog() {
             return this.dialog_
         },
         maybeHideModal: function() {
-            this.dialog_.hasAttribute("open") && st(this.dialog_) || this.downgradeModal()
+            this.dialog_.hasAttribute("open") && ct(this.dialog_) || this.downgradeModal()
         },
         downgradeModal: function() {
-            this.openAsModal_ && (this.openAsModal_ = !1, this.dialog_.style.zIndex = "", this.replacedStyleTop_ && (this.dialog_.style.top = "", this.replacedStyleTop_ = !1), this.backdrop_.parentNode && this.backdrop_.parentNode.removeChild(this.backdrop_), At.dm.removeDialog(this))
+            this.openAsModal_ && (this.openAsModal_ = !1, this.dialog_.style.zIndex = "", this.replacedStyleTop_ && (this.dialog_.style.top = "", this.replacedStyleTop_ = !1), this.backdrop_.parentNode && this.backdrop_.parentNode.removeChild(this.backdrop_), ft.dm.removeDialog(this))
         },
         setOpen: function(e) {
             e ? this.dialog_.hasAttribute("open") || this.dialog_.setAttribute("open", "") : (this.dialog_.removeAttribute("open"), this.maybeHideModal())
         },
         backdropMouseEvent_: function(e) {
             if (this.dialog_.hasAttribute("tabindex")) this.dialog_.focus();
             else {
@@ -980,50 +984,50 @@
                 this.dialog_.insertBefore(t, this.dialog_.firstChild), t.tabIndex = -1, t.focus(), this.dialog_.removeChild(t)
             }
             var n = document.createEvent("MouseEvents");
             n.initMouseEvent(e.type, e.bubbles, e.cancelable, window, e.detail, e.screenX, e.screenY, e.clientX, e.clientY, e.ctrlKey, e.altKey, e.shiftKey, e.metaKey, e.button, e.relatedTarget), this.dialog_.dispatchEvent(n), e.stopPropagation()
         },
         focus_: function() {
             var e = this.dialog_.querySelector("[autofocus]:not([disabled])");
-            !e && this.dialog_.tabIndex >= 0 && (e = this.dialog_), e || (e = ot(this.dialog_)), at(document.activeElement), e && e.focus()
+            !e && this.dialog_.tabIndex >= 0 && (e = this.dialog_), e || (e = st(this.dialog_)), rt(document.activeElement), e && e.focus()
         },
         updateZIndex: function(e, t) {
             if (e < t) throw new Error("dialogZ should never be < backdropZ");
             this.dialog_.style.zIndex = e, this.backdrop_.style.zIndex = t
         },
         show: function() {
             this.dialog_.open || (this.setOpen(!0), this.focus_())
         },
         showModal: function() {
             if (this.dialog_.hasAttribute("open")) throw new Error("Failed to execute 'showModal' on dialog: The element is already open, and therefore cannot be opened modally.");
-            if (!st(this.dialog_)) throw new Error("Failed to execute 'showModal' on dialog: The element is not in a Document.");
-            if (!At.dm.pushDialog(this)) throw new Error("Failed to execute 'showModal' on dialog: There are too many open modal dialogs.");
+            if (!ct(this.dialog_)) throw new Error("Failed to execute 'showModal' on dialog: The element is not in a Document.");
+            if (!ft.dm.pushDialog(this)) throw new Error("Failed to execute 'showModal' on dialog: There are too many open modal dialogs.");
             (function(e) {
                 for (; e && e !== document.body;) {
                     var t = window.getComputedStyle(e),
                         n = function(e, n) {
                             return !(void 0 === t[e] || t[e] === n)
                         };
                     if (t.opacity < 1 || n("zIndex", "auto") || n("transform", "none") || n("mixBlendMode", "normal") || n("filter", "none") || n("perspective", "none") || "isolate" === t.isolation || "fixed" === t.position || "touch" === t.webkitOverflowScrolling) return !0;
                     e = e.parentElement
                 }
                 return !1
-            })(this.dialog_.parentElement) && console.warn("A dialog is being shown inside a stacking context. This may cause it to be unusable. For more information, see this link: https://github.com/GoogleChrome/dialog-polyfill/#stacking-context"), this.setOpen(!0), this.openAsModal_ = !0, At.needsCentering(this.dialog_) ? (At.reposition(this.dialog_), this.replacedStyleTop_ = !0) : this.replacedStyleTop_ = !1, this.dialog_.parentNode.insertBefore(this.backdrop_, this.dialog_.nextSibling), this.focus_()
+            })(this.dialog_.parentElement) && console.warn("A dialog is being shown inside a stacking context. This may cause it to be unusable. For more information, see this link: https://github.com/GoogleChrome/dialog-polyfill/#stacking-context"), this.setOpen(!0), this.openAsModal_ = !0, ft.needsCentering(this.dialog_) ? (ft.reposition(this.dialog_), this.replacedStyleTop_ = !0) : this.replacedStyleTop_ = !1, this.dialog_.parentNode.insertBefore(this.backdrop_, this.dialog_.nextSibling), this.focus_()
         },
         close: function(e) {
             if (!this.dialog_.hasAttribute("open")) throw new Error("Failed to execute 'close' on dialog: The element does not have an 'open' attribute, and therefore cannot be closed.");
             this.setOpen(!1), void 0 !== e && (this.dialog_.returnValue = e);
-            var t = new tt("close", {
+            var t = new nt("close", {
                 bubbles: !1,
                 cancelable: !1
             });
-            nt(this.dialog_, t)
+            it(this.dialog_, t)
         }
     };
-    var At = {
+    var ft = {
         reposition: function(e) {
             var t = document.body.scrollTop || document.documentElement.scrollTop,
                 n = t + (window.innerHeight - e.offsetHeight) / 2;
             e.style.top = Math.max(t, n) + "px"
         },
         isInlinePositionSetByStylesheet: function(e) {
             for (var t = 0; t < document.styleSheets.length; ++t) {
@@ -1035,138 +1039,138 @@
                 if (i)
                     for (var a = 0; a < i.length; ++a) {
                         var r = i[a],
                             l = null;
                         try {
                             l = document.querySelectorAll(r.selectorText)
                         } catch (c) {}
-                        if (l && rt(l, e)) {
+                        if (l && lt(l, e)) {
                             var o = r.style.getPropertyValue("top"),
                                 s = r.style.getPropertyValue("bottom");
                             if (o && "auto" !== o || s && "auto" !== s) return !0
                         }
                     }
             }
             return !1
         },
         needsCentering: function(e) {
-            return "absolute" === window.getComputedStyle(e).position && (!("auto" !== e.style.top && "" !== e.style.top || "auto" !== e.style.bottom && "" !== e.style.bottom) && !At.isInlinePositionSetByStylesheet(e))
+            return "absolute" === window.getComputedStyle(e).position && (!("auto" !== e.style.top && "" !== e.style.top || "auto" !== e.style.bottom && "" !== e.style.bottom) && !ft.isInlinePositionSetByStylesheet(e))
         },
         forceRegisterDialog: function(e) {
             if ((window.HTMLDialogElement || e.showModal) && console.warn("This browser already supports <dialog>, the polyfill may not work correctly", e), "dialog" !== e.localName) throw new Error("Failed to register dialog: The element is not a dialog.");
-            new dt(e)
+            new At(e)
         },
         registerDialog: function(e) {
-            e.showModal || At.forceRegisterDialog(e)
+            e.showModal || ft.forceRegisterDialog(e)
         },
         DialogManager: function() {
             this.pendingDialogStack = [];
             var e = this.checkDOM_.bind(this);
             this.overlay = document.createElement("div"), this.overlay.className = "_dialog_overlay", this.overlay.addEventListener("click", function(t) {
                 this.forwardTab_ = void 0, t.stopPropagation(), e([])
             }.bind(this)), this.handleKey_ = this.handleKey_.bind(this), this.handleFocus_ = this.handleFocus_.bind(this), this.zIndexLow_ = 1e5, this.zIndexHigh_ = 100150, this.forwardTab_ = void 0, "MutationObserver" in window && (this.mo_ = new MutationObserver((function(t) {
                 var n = [];
                 t.forEach((function(e) {
                     for (var t, i = 0; t = e.removedNodes[i]; ++i) t instanceof Element && ("dialog" === t.localName && n.push(t), n = n.concat(t.querySelectorAll("dialog")))
                 })), n.length && e(n)
             })))
         }
     };
-    if (At.DialogManager.prototype.blockDocument = function() {
+    if (ft.DialogManager.prototype.blockDocument = function() {
             document.documentElement.addEventListener("focus", this.handleFocus_, !0), document.addEventListener("keydown", this.handleKey_), this.mo_ && this.mo_.observe(document, {
                 childList: !0,
                 subtree: !0
             })
-        }, At.DialogManager.prototype.unblockDocument = function() {
+        }, ft.DialogManager.prototype.unblockDocument = function() {
             document.documentElement.removeEventListener("focus", this.handleFocus_, !0), document.removeEventListener("keydown", this.handleKey_), this.mo_ && this.mo_.disconnect()
-        }, At.DialogManager.prototype.updateStacking = function() {
+        }, ft.DialogManager.prototype.updateStacking = function() {
             for (var e, t = this.zIndexHigh_, n = 0; e = this.pendingDialogStack[n]; ++n) e.updateZIndex(--t, --t), 0 === n && (this.overlay.style.zIndex = --t);
             var i = this.pendingDialogStack[0];
             i ? (i.dialog.parentNode || document.body).appendChild(this.overlay) : this.overlay.parentNode && this.overlay.parentNode.removeChild(this.overlay)
-        }, At.DialogManager.prototype.containedByTopDialog_ = function(e) {
-            for (; e = it(e);) {
+        }, ft.DialogManager.prototype.containedByTopDialog_ = function(e) {
+            for (; e = at(e);) {
                 for (var t, n = 0; t = this.pendingDialogStack[n]; ++n)
                     if (t.dialog === e) return 0 === n;
                 e = e.parentElement
             }
             return !1
-        }, At.DialogManager.prototype.handleFocus_ = function(e) {
+        }, ft.DialogManager.prototype.handleFocus_ = function(e) {
             var t = e.composedPath ? e.composedPath()[0] : e.target;
-            if (!this.containedByTopDialog_(t) && document.activeElement !== document.documentElement && (e.preventDefault(), e.stopPropagation(), at(t), void 0 !== this.forwardTab_)) {
+            if (!this.containedByTopDialog_(t) && document.activeElement !== document.documentElement && (e.preventDefault(), e.stopPropagation(), rt(t), void 0 !== this.forwardTab_)) {
                 var n = this.pendingDialogStack[0];
                 return n.dialog.compareDocumentPosition(t) & Node.DOCUMENT_POSITION_PRECEDING && (this.forwardTab_ ? n.focus_() : t !== document.documentElement && document.documentElement.focus()), !1
             }
-        }, At.DialogManager.prototype.handleKey_ = function(e) {
+        }, ft.DialogManager.prototype.handleKey_ = function(e) {
             if (this.forwardTab_ = void 0, 27 === e.keyCode) {
                 e.preventDefault(), e.stopPropagation();
-                var t = new tt("cancel", {
+                var t = new nt("cancel", {
                         bubbles: !1,
                         cancelable: !0
                     }),
                     n = this.pendingDialogStack[0];
-                n && nt(n.dialog, t) && n.dialog.close()
+                n && it(n.dialog, t) && n.dialog.close()
             } else 9 === e.keyCode && (this.forwardTab_ = !e.shiftKey)
-        }, At.DialogManager.prototype.checkDOM_ = function(e) {
+        }, ft.DialogManager.prototype.checkDOM_ = function(e) {
             this.pendingDialogStack.slice().forEach((function(t) {
                 -1 !== e.indexOf(t.dialog) ? t.downgradeModal() : t.maybeHideModal()
             }))
-        }, At.DialogManager.prototype.pushDialog = function(e) {
+        }, ft.DialogManager.prototype.pushDialog = function(e) {
             var t = (this.zIndexHigh_ - this.zIndexLow_) / 2 - 1;
             return !(this.pendingDialogStack.length >= t) && (1 === this.pendingDialogStack.unshift(e) && this.blockDocument(), this.updateStacking(), !0)
-        }, At.DialogManager.prototype.removeDialog = function(e) {
+        }, ft.DialogManager.prototype.removeDialog = function(e) {
             var t = this.pendingDialogStack.indexOf(e); - 1 !== t && (this.pendingDialogStack.splice(t, 1), 0 === this.pendingDialogStack.length && this.unblockDocument(), this.updateStacking())
-        }, At.dm = new At.DialogManager, At.formSubmitter = null, At.imagemapUseValue = null, void 0 === window.HTMLDialogElement) {
-        var ft = document.createElement("form");
-        if (ft.setAttribute("method", "dialog"), "dialog" !== ft.method) {
-            var ht = Object.getOwnPropertyDescriptor(HTMLFormElement.prototype, "method");
-            if (ht) {
-                var mt = ht.get;
-                ht.get = function() {
-                    return lt(this) ? "dialog" : mt.call(this)
+        }, ft.dm = new ft.DialogManager, ft.formSubmitter = null, ft.imagemapUseValue = null, void 0 === window.HTMLDialogElement) {
+        var ht = document.createElement("form");
+        if (ht.setAttribute("method", "dialog"), "dialog" !== ht.method) {
+            var mt = Object.getOwnPropertyDescriptor(HTMLFormElement.prototype, "method");
+            if (mt) {
+                var pt = mt.get;
+                mt.get = function() {
+                    return ot(this) ? "dialog" : pt.call(this)
                 };
-                var pt = ht.set;
-                ht.set = function(e) {
-                    return "string" == typeof e && "dialog" === e.toLowerCase() ? this.setAttribute("method", e) : pt.call(this, e)
-                }, Object.defineProperty(HTMLFormElement.prototype, "method", ht)
+                var gt = mt.set;
+                mt.set = function(e) {
+                    return "string" == typeof e && "dialog" === e.toLowerCase() ? this.setAttribute("method", e) : gt.call(this, e)
+                }, Object.defineProperty(HTMLFormElement.prototype, "method", mt)
             }
         }
         document.addEventListener("click", (function(e) {
-            if (At.formSubmitter = null, At.imagemapUseValue = null, !e.defaultPrevented) {
+            if (ft.formSubmitter = null, ft.imagemapUseValue = null, !e.defaultPrevented) {
                 var t = e.target;
                 if ("composedPath" in e) t = e.composedPath().shift() || t;
-                if (t && lt(t.form)) {
+                if (t && ot(t.form)) {
                     if (!("submit" === t.type && ["button", "input"].indexOf(t.localName) > -1)) {
                         if ("input" !== t.localName || "image" !== t.type) return;
-                        At.imagemapUseValue = e.offsetX + "," + e.offsetY
+                        ft.imagemapUseValue = e.offsetX + "," + e.offsetY
                     }
-                    it(t) && (At.formSubmitter = t)
+                    at(t) && (ft.formSubmitter = t)
                 }
             }
         }), !1), document.addEventListener("submit", (function(e) {
             var t = e.target;
-            if (!it(t)) {
-                var n = ct(e);
+            if (!at(t)) {
+                var n = ut(e);
                 "dialog" === (n && n.getAttribute("formmethod") || t.getAttribute("method")) && e.preventDefault()
             }
         }));
-        var gt = HTMLFormElement.prototype.submit;
+        var vt = HTMLFormElement.prototype.submit;
         HTMLFormElement.prototype.submit = function() {
-            if (!lt(this)) return gt.call(this);
-            var e = it(this);
+            if (!ot(this)) return vt.call(this);
+            var e = at(this);
             e && e.close()
         }
     }
 
-    function vt(e) {
+    function yt(e) {
         let t, n, i, a, r, l, o, s, c;
         const u = e[3].default,
             d = A(u, e, e[2], null);
         return {
             c() {
-                t = O("dialog"), n = O("button"), i = X("svg"), a = X("path"), r = U(), l = O("div"), d && d.c(), this.h()
+                t = O("dialog"), n = O("button"), i = X("svg"), a = X("path"), r = T(), l = O("div"), d && d.c(), this.h()
             },
             l(e) {
                 t = j(e, "DIALOG", {
                     class: !0
                 });
                 var o = W(t);
                 n = j(o, "BUTTON", {
@@ -1188,63 +1192,63 @@
                 var u = W(l);
                 d && d.l(u), u.forEach(R), o.forEach(R), this.h()
             },
             h() {
                 N(a, "fill", "currentColor"), N(a, "d", "M11.38 7.75L16 3.14a1.86 1.86 0 00.25-2.38 1.79 1.79 0 00-2.74-.23L8.83 5.2a.76.76 0 01-1.08 0L3.14.6A1.86 1.86 0 00.76.33a1.79 1.79 0 00-.23 2.74L5.2 7.75a.76.76 0 010 1.08L.6 13.44a1.88 1.88 0 00-.27 2.39 1.81 1.81 0 002.74.23l4.68-4.68a.76.76 0 011.08 0L13.44 16a1.87 1.87 0 002.39.26 1.81 1.81 0 00.23-2.74l-4.68-4.69a.76.76 0 010-1.08z"), N(i, "class", "icon"), N(i, "viewBox", "0 0 16.59 16.59"), N(i, "xmlns", "http://www.w3.org/2000/svg"), N(n, "class", "close-button"), N(l, "class", "scroll-wrap"), N(t, "class", "modal")
             },
             m(u, A) {
-                k(u, t, A), x(t, n), x(n, i), x(i, a), x(t, r), x(t, l), d && d.m(l, null), e[5](t), o = !0, s || (c = T(n, "click", e[4]), s = !0)
+                k(u, t, A), x(t, n), x(n, i), x(i, a), x(t, r), x(t, l), d && d.m(l, null), e[5](t), o = !0, s || (c = z(n, "click", e[4]), s = !0)
             },
             p(e, [t]) {
                 d && d.p && (!o || 4 & t) && m(d, u, e, e[2], o ? h(u, e[2], t, null) : p(e[2]), null)
             },
             i(e) {
-                o || (Re(d, e), o = !0)
+                o || (Ve(d, e), o = !0)
             },
             o(e) {
-                Ve(d, e), o = !1
+                Oe(d, e), o = !1
             },
             d(n) {
                 n && R(t), d && d.d(n), e[5](null), s = !1, c()
             }
         }
     }
 
-    function yt(e, t, n) {
+    function Et(e, t, n) {
         let i, {
                 $$slots: a = {},
                 $$scope: r
             } = t,
             {
                 open: l = !1
             } = t;
         ce((() => {
-            At.registerDialog(i)
+            ft.registerDialog(i)
         }));
         return e.$$set = e => {
             "open" in e && n(0, l = e.open), "$$scope" in e && n(2, r = e.$$scope)
         }, e.$$.update = () => {
             3 & e.$$.dirty && (l ? null == i || i.showModal() : i && i.open && i.close())
         }, [l, i, r, a, () => {
             n(0, l = !1)
         }, function(e) {
-            fe[e ? "unshift" : "push"]((() => {
+            he[e ? "unshift" : "push"]((() => {
                 i = e, n(1, i)
             }))
         }]
     }
-    class Et extends Ze {
+    class bt extends Ye {
         constructor(e) {
-            super(), Ke(this, e, yt, vt, s, {
+            super(), Ze(this, e, Et, yt, s, {
                 open: 0
             })
         }
     }
 
-    function bt(e) {
+    function It(e) {
         let t, n, i, a, r;
         return {
             c() {
                 t = O("input"), this.h()
             },
             l(e) {
                 t = j(e, "INPUT", {
@@ -1255,26 +1259,26 @@
                     step: !0
                 }), this.h()
             },
             h() {
                 N(t, "class", "auto-assign-input"), N(t, "type", "number"), N(t, "min", n = e[2].minimumPlayers || 1), N(t, "max", i = e[2].maximumPlayers), N(t, "step", "1")
             },
             m(n, i) {
-                k(n, t, i), Z(t, e[3]), a || (r = T(t, "input", e[5]), a = !0)
+                k(n, t, i), Z(t, e[3]), a || (r = z(t, "input", e[5]), a = !0)
             },
             p(e, a) {
                 4 & a && n !== (n = e[2].minimumPlayers || 1) && N(t, "min", n), 4 & a && i !== (i = e[2].maximumPlayers) && N(t, "max", i), 8 & a && Q(t.value) !== e[3] && Z(t, e[3])
             },
             d(e) {
                 e && R(t), a = !1, r()
             }
         }
     }
 
-    function It(e) {
+    function wt(e) {
         let t;
         return {
             c() {
                 t = F(e[3])
             },
             l(n) {
                 t = q(n, e[3])
@@ -1287,42 +1291,42 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function wt(e) {
+    function Ct(e) {
         let t;
 
         function n(e, t) {
-            return e[2].minimumPlayers > 1 && e[2].maximumPlayers ? St : e[2].minimumPlayers > 1 ? Bt : e[2].maximumPlayers ? Ct : void 0
+            return e[2].minimumPlayers > 1 && e[2].maximumPlayers ? Lt : e[2].minimumPlayers > 1 ? St : e[2].maximumPlayers ? Bt : void 0
         }
         let i = n(e),
             a = i && i(e);
         return {
             c() {
-                a && a.c(), t = z()
+                a && a.c(), t = U()
             },
             l(e) {
-                a && a.l(e), t = z()
+                a && a.l(e), t = U()
             },
             m(e, n) {
                 a && a.m(e, n), k(e, t, n)
             },
             p(e, r) {
                 i === (i = n(e)) && a ? a.p(e, r) : (a && a.d(1), a = i && i(e), a && (a.c(), a.m(t.parentNode, t)))
             },
             d(e) {
                 a && a.d(e), e && R(t)
             }
         }
     }
 
-    function Ct(e) {
+    function Bt(e) {
         let t, n, i, a, r = e[2].maximumPlayers + "";
         return {
             c() {
                 t = O("em"), n = F("(at most "), i = F(r), a = F(")")
             },
             l(e) {
                 t = j(e, "EM", {});
@@ -1337,15 +1341,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function Bt(e) {
+    function St(e) {
         let t, n, i, a, r = e[2].minimumPlayers + "";
         return {
             c() {
                 t = O("em"), n = F("(at least "), i = F(r), a = F(")")
             },
             l(e) {
                 t = j(e, "EM", {});
@@ -1360,15 +1364,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function St(e) {
+    function Lt(e) {
         let t, n, i, a, r, l, o = e[2].minimumPlayers + "",
             s = e[2].maximumPlayers + "";
         return {
             c() {
                 t = O("em"), n = F("(between "), i = F(o), a = F(" and\n              "), r = F(s), l = F(")")
             },
             l(e) {
@@ -1389,22 +1393,22 @@
     }
 
     function Pt(e) {
         let t, n, i, a, r, l, o, s, c, u, d, A, f, h, m, p, g, v, y = 1 == e[3] ? "player" : "players",
             E = e[1].length + "";
 
         function b(e, t) {
-            return e[2].minimumPlayers && e[2].maximumPlayers && e[2].minimumPlayers === e[2].maximumPlayers ? It : bt
+            return e[2].minimumPlayers && e[2].maximumPlayers && e[2].minimumPlayers === e[2].maximumPlayers ? wt : It
         }
         let I = b(e),
             w = I(e),
-            C = e[2].minimumPlayers !== e[2].maximumPlayers && wt(e);
+            C = e[2].minimumPlayers !== e[2].maximumPlayers && Ct(e);
         return {
             c() {
-                t = O("div"), n = O("form"), i = O("h2"), a = F("Auto Assign"), r = U(), l = O("p"), o = F("Fill or create teams of up to "), w.c(), s = U(), c = F(y), u = U(), C && C.c(), d = U(), A = O("div"), f = O("button"), h = F("Assign "), m = F(E), p = F(" Players"), this.h()
+                t = O("div"), n = O("form"), i = O("h2"), a = F("Auto Assign"), r = T(), l = O("p"), o = F("Fill or create teams of up to "), w.c(), s = T(), c = F(y), u = T(), C && C.c(), d = T(), A = O("div"), f = O("button"), h = F("Assign "), m = F(E), p = F(" Players"), this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
                     class: !0
                 });
                 var g = W(t);
                 n = j(g, "FORM", {});
@@ -1425,79 +1429,79 @@
                 var S = W(f);
                 h = q(S, "Assign "), m = q(S, E), p = q(S, " Players"), S.forEach(R), B.forEach(R), v.forEach(R), g.forEach(R), this.h()
             },
             h() {
                 N(i, "class", "modal-heading"), N(f, "class", "button"), N(A, "class", "button-wrap align-center"), N(t, "class", "text-center")
             },
             m(y, E) {
-                k(y, t, E), x(t, n), x(n, i), x(i, a), x(n, r), x(n, l), x(l, o), w.m(l, null), x(l, s), x(l, c), x(l, u), C && C.m(l, null), x(n, d), x(n, A), x(A, f), x(f, h), x(f, m), x(f, p), g || (v = T(n, "submit", D(e[6])), g = !0)
+                k(y, t, E), x(t, n), x(n, i), x(i, a), x(n, r), x(n, l), x(l, o), w.m(l, null), x(l, s), x(l, c), x(l, u), C && C.m(l, null), x(n, d), x(n, A), x(A, f), x(f, h), x(f, m), x(f, p), g || (v = z(n, "submit", D(e[6])), g = !0)
             },
             p(e, t) {
-                I === (I = b(e)) && w ? w.p(e, t) : (w.d(1), w = I(e), w && (w.c(), w.m(l, s))), 8 & t && y !== (y = 1 == e[3] ? "player" : "players") && K(c, y), e[2].minimumPlayers !== e[2].maximumPlayers ? C ? C.p(e, t) : (C = wt(e), C.c(), C.m(l, null)) : C && (C.d(1), C = null), 2 & t && E !== (E = e[1].length + "") && K(m, E)
+                I === (I = b(e)) && w ? w.p(e, t) : (w.d(1), w = I(e), w && (w.c(), w.m(l, s))), 8 & t && y !== (y = 1 == e[3] ? "player" : "players") && K(c, y), e[2].minimumPlayers !== e[2].maximumPlayers ? C ? C.p(e, t) : (C = Ct(e), C.c(), C.m(l, null)) : C && (C.d(1), C = null), 2 & t && E !== (E = e[1].length + "") && K(m, E)
             },
             d(e) {
                 e && R(t), w.d(), C && C.d(), g = !1, v()
             }
         }
     }
 
-    function Lt(e) {
+    function xt(e) {
         let t, n, i;
 
         function a(t) {
             e[7](t)
         }
         let r = {
             $$slots: {
                 default: [Pt]
             },
             $$scope: {
                 ctx: e
             }
         };
-        return void 0 !== e[0] && (r.open = e[0]), t = new Et({
+        return void 0 !== e[0] && (r.open = e[0]), t = new bt({
             props: r
-        }), fe.push((() => Qe(t, "open", a))), {
+        }), he.push((() => We(t, "open", a))), {
             c() {
-                We(t.$$.fragment)
+                Je(t.$$.fragment)
             },
             l(e) {
-                Je(t.$$.fragment, e)
+                je(t.$$.fragment, e)
             },
             m(e, n) {
-                je(t, e, n), i = !0
+                qe(t, e, n), i = !0
             },
             p(e, [i]) {
                 const a = {};
                 527 & i && (a.$$scope = {
                     dirty: i,
                     ctx: e
-                }), !n && 1 & i && (n = !0, a.open = e[0], ye((() => n = !1))), t.$set(a)
+                }), !n && 1 & i && (n = !0, a.open = e[0], Ee((() => n = !1))), t.$set(a)
             },
             i(e) {
-                i || (Re(t.$$.fragment, e), i = !0)
+                i || (Ve(t.$$.fragment, e), i = !0)
             },
             o(e) {
-                Ve(t.$$.fragment, e), i = !1
+                Oe(t.$$.fragment, e), i = !1
             },
             d(e) {
-                qe(t, e)
+                Me(t, e)
             }
         }
     }
 
-    function xt(e, t, n) {
+    function kt(e, t, n) {
         let i, a;
-        d(e, $e, (e => n(2, i = e)));
+        d(e, _e, (e => n(2, i = e)));
         let {
             open: r
         } = t, {
             unassigned: l
         } = t;
-        const o = ue();
+        const o = de();
         return e.$$set = e => {
             "open" in e && n(0, r = e.open), "unassigned" in e && n(1, l = e.unassigned)
         }, e.$$.update = () => {
             var t, r;
             4 & e.$$.dirty && (t = i.minimumPlayers, r = i.maximumPlayers, n(3, a = t && r ? Math.floor((r + t) / 2) : t ? Math.max(t, 3) : r ? Math.min(r, 3) : 3))
         }, [r, l, i, a, o, function() {
             a = Q(this.value), n(3, a)
@@ -1505,24 +1509,24 @@
             o("submit", {
                 fillCount: a
             }), n(0, r = !1)
         }, function(e) {
             r = e, n(0, r)
         }]
     }
-    class kt extends Ze {
+    class Rt extends Ye {
         constructor(e) {
-            super(), Ke(this, e, xt, Lt, s, {
+            super(), Ze(this, e, kt, xt, s, {
                 open: 0,
                 unassigned: 1
             })
         }
     }
 
-    function Rt(e) {
+    function Vt(e) {
         let t, n, i;
         const a = e[1].default,
             r = A(a, e, e[0], null);
         return {
             c() {
                 t = O("div"), n = O("ul"), r && r.c(), this.h()
             },
@@ -1544,41 +1548,41 @@
             m(e, a) {
                 k(e, t, a), x(t, n), r && r.m(n, null), i = !0
             },
             p(e, [t]) {
                 r && r.p && (!i || 1 & t) && m(r, a, e, e[0], i ? h(a, e[0], t, null) : p(e[0]), null)
             },
             i(e) {
-                i || (Re(r, e), i = !0)
+                i || (Ve(r, e), i = !0)
             },
             o(e) {
-                Ve(r, e), i = !1
+                Oe(r, e), i = !1
             },
             d(e) {
                 e && R(t), r && r.d(e)
             }
         }
     }
 
-    function Vt(e, t, n) {
+    function Ot(e, t, n) {
         let {
             $$slots: i = {},
             $$scope: a
         } = t;
         return e.$$set = e => {
             "$$scope" in e && n(0, a = e.$$scope)
         }, [a, i]
     }
-    class Ot extends Ze {
+    class Xt extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Vt, Rt, s, {})
+            super(), Ze(this, e, Ot, Vt, s, {})
         }
     }
 
-    function Xt(e) {
+    function Ft(e) {
         let t, n, i, a, r, o;
         const s = e[6].default,
             c = A(s, e, e[5], null);
         return {
             c() {
                 t = O("li"), n = O("button"), c && c.c(), this.h()
             },
@@ -1595,32 +1599,32 @@
                 var a = W(n);
                 c && c.l(a), a.forEach(R), i.forEach(R), this.h()
             },
             h() {
                 N(n, "class", "tab-link svelte-1jc2hdr"), N(n, "aria-selected", i = e[0] === e[1]), N(n, "data-notification-badge", e[2]), G(n, "outline", e[3] || e[2]), N(t, "class", "tab-item")
             },
             m(i, l) {
-                k(i, t, l), x(t, n), c && c.m(n, null), a = !0, r || (o = [v(e[4].call(null, n)), T(n, "click", e[7])], r = !0)
+                k(i, t, l), x(t, n), c && c.m(n, null), a = !0, r || (o = [v(e[4].call(null, n)), z(n, "click", e[7])], r = !0)
             },
             p(e, [t]) {
                 c && c.p && (!a || 32 & t) && m(c, s, e, e[5], a ? h(s, e[5], t, null) : p(e[5]), null), (!a || 3 & t && i !== (i = e[0] === e[1])) && N(n, "aria-selected", i), (!a || 4 & t) && N(n, "data-notification-badge", e[2]), 12 & t && G(n, "outline", e[3] || e[2])
             },
             i(e) {
-                a || (Re(c, e), a = !0)
+                a || (Ve(c, e), a = !0)
             },
             o(e) {
-                Ve(c, e), a = !1
+                Oe(c, e), a = !1
             },
             d(e) {
                 e && R(t), c && c.d(e), r = !1, l(o)
             }
         }
     }
 
-    function Ft(e, t, n) {
+    function Tt(e, t, n) {
         let {
             $$slots: i = {},
             $$scope: a
         } = t, {
             state: r
         } = t, {
             value: l = null
@@ -1631,31 +1635,31 @@
         } = t;
         return e.$$set = e => {
             "state" in e && n(0, r = e.state), "value" in e && n(1, l = e.value), "badge" in e && n(2, o = e.badge), "outline" in e && n(3, s = e.outline), "$$scope" in e && n(5, a = e.$$scope)
         }, [r, l, o, s, e => {
             l || n(1, l = e.innerText)
         }, a, i, () => n(0, r = l)]
     }
-    class Ut extends Ze {
+    class Ut extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Ft, Xt, s, {
+            super(), Ze(this, e, Tt, Ft, s, {
                 state: 0,
                 value: 1,
                 badge: 2,
                 outline: 3
             })
         }
     }
 
     function zt(e) {
         const t = e - 1;
         return t * t * t + 1
     }
 
-    function Tt(e, t, n = {}) {
+    function Dt(e, t, n = {}) {
         const i = getComputedStyle(e),
             a = "none" === i.transform ? "" : i.transform,
             r = t.from.width / e.clientWidth,
             l = t.from.height / e.clientHeight,
             s = (t.from.left - t.to.left) / r,
             c = (t.from.top - t.to.top) / l,
             u = Math.sqrt(s * s + c * c),
@@ -1668,15 +1672,15 @@
             delay: d,
             duration: o(A) ? A(u) : A,
             easing: f,
             css: (e, t) => `transform: ${a} translate(${t*s}px, ${t*c}px);`
         }
     }
 
-    function Dt(e, t = 41, n = 24) {
+    function Ht(e, t = 41, n = 24) {
         const i = function(e, t) {
             var n, i, a, r, l, o, s, c;
             for (n = 3 & e.length, i = e.length - n, a = t, l = 3432918353, o = 461845907, c = 0; c < i;) s = 255 & e.charCodeAt(c) | (255 & e.charCodeAt(++c)) << 8 | (255 & e.charCodeAt(++c)) << 16 | (255 & e.charCodeAt(++c)) << 24, ++c, a = 27492 + (65535 & (r = 5 * (65535 & (a = (a ^= s = (65535 & (s = (s = (65535 & s) * l + (((s >>> 16) * l & 65535) << 16) & 4294967295) << 15 | s >>> 17)) * o + (((s >>> 16) * o & 65535) << 16) & 4294967295) << 13 | a >>> 19)) + ((5 * (a >>> 16) & 65535) << 16) & 4294967295)) + ((58964 + (r >>> 16) & 65535) << 16);
             switch (s = 0, n) {
                 case 3:
                     s ^= (255 & e.charCodeAt(c + 2)) << 16;
                     break;
@@ -1691,55 +1695,157 @@
         let a = i % 360,
             r = (i >>> 11) % 100,
             l = (i >>> 17) % 100;
         r = Math.floor(r / 100 * t + (100 - t) / 2), l = Math.floor(l / 100 * n + (100 - n) / 2.5);
         return `hsl(${a},${r}%,${l}%)`
     }
 
-    function Ht(e, t, n) {
+    function Nt(e) {
+        let t, n, i, a, r, o, s, c;
+        const u = e[6].default,
+            d = A(u, e, e[5], null);
+        return {
+            c() {
+                t = O("div"), n = O("a"), i = F(e[1]), a = T(), r = O("div"), d && d.c(), this.h()
+            },
+            l(l) {
+                t = j(l, "DIV", {
+                    class: !0
+                });
+                var o = W(t);
+                n = j(o, "A", {
+                    href: !0,
+                    class: !0,
+                    "aria-expanded": !0
+                });
+                var s = W(n);
+                i = q(s, e[1]), s.forEach(R), a = M(o), r = j(o, "DIV", {
+                    class: !0
+                });
+                var c = W(r);
+                d && d.l(c), c.forEach(R), o.forEach(R), this.h()
+            },
+            h() {
+                N(n, "href", "#"), N(n, "class", "button dropdown-button hollow small"), N(n, "aria-expanded", e[0]), N(r, "class", "dropdown"), N(t, "class", "has-dropdown narrow-dropdown"), G(t, "is-expanded", e[0])
+            },
+            m(l, u) {
+                k(l, t, u), x(t, n), x(n, i), x(t, a), x(t, r), d && d.m(r, null), e[8](r), e[9](t), o = !0, s || (c = [z(n, "click", D(e[7])), z(n, "click", e[4])], s = !0)
+            },
+            p(e, [a]) {
+                (!o || 2 & a) && K(i, e[1]), (!o || 1 & a) && N(n, "aria-expanded", e[0]), d && d.p && (!o || 32 & a) && m(d, u, e, e[5], o ? h(u, e[5], a, null) : p(e[5]), null), 1 & a && G(t, "is-expanded", e[0])
+            },
+            i(e) {
+                o || (Ve(d, e), o = !0)
+            },
+            o(e) {
+                Oe(d, e), o = !1
+            },
+            d(n) {
+                n && R(t), d && d.d(n), e[8](null), e[9](null), s = !1, l(c)
+            }
+        }
+    }
+
+    function Qt(e, t, n) {
+        let i, a, {
+                $$slots: r = {},
+                $$scope: l
+            } = t,
+            {
+                placeholderText: o = "Select"
+            } = t,
+            {
+                expanded: s = !1
+            } = t;
+        const c = () => {
+                const e = e => {
+                    i.contains(null == e ? void 0 : e.target) || d()
+                };
+                return document.addEventListener("click", e), {
+                    destroy() {
+                        document.removeEventListener("click", e)
+                    }
+                }
+            },
+            u = e => {
+                i.contains(e.relatedTarget) || d()
+            },
+            d = () => {
+                n(0, s = !1)
+            };
+        return ce((() => {
+            document.addEventListener("click", c), i.addEventListener("focusout", u)
+        })), ue((() => {
+            document.removeEventListener("click", c), i.removeEventListener("focusout", u)
+        })), e.$$set = e => {
+            "placeholderText" in e && n(1, o = e.placeholderText), "expanded" in e && n(0, s = e.expanded), "$$scope" in e && n(5, l = e.$$scope)
+        }, [s, o, i, a, () => {
+            n(0, s = !s)
+        }, l, r, function(t) {
+            Ae.call(this, e, t)
+        }, function(e) {
+            he[e ? "unshift" : "push"]((() => {
+                a = e, n(3, a)
+            }))
+        }, function(e) {
+            he[e ? "unshift" : "push"]((() => {
+                i = e, n(2, i)
+            }))
+        }]
+    }
+    class Wt extends Ye {
+        constructor(e) {
+            super(), Ze(this, e, Qt, Nt, s, {
+                placeholderText: 1,
+                expanded: 0
+            })
+        }
+    }
+
+    function Jt(e, t, n) {
         const i = e.slice();
-        return i[18] = t[n], i
+        return i[17] = t[n], i
     }
 
-    function Nt(e) {
+    function jt(e) {
         var t;
-        let n, i, a = (null == (t = e[8](e[18].session)) ? void 0 : t.name) + "";
+        let n, i, a = (null == (t = e[8](e[17].session)) ? void 0 : t.name) + "";
         return {
             c() {
                 n = O("small"), i = F(a)
             },
             l(e) {
                 n = j(e, "SMALL", {});
                 var t = W(n);
                 i = q(t, a), t.forEach(R)
             },
             m(e, t) {
                 k(e, n, t), x(n, i)
             },
             p(e, t) {
                 var n;
-                16 & t && a !== (a = (null == (n = e[8](e[18].session)) ? void 0 : n.name) + "") && K(i, a)
+                16 & t && a !== (a = (null == (n = e[8](e[17].session)) ? void 0 : n.name) + "") && K(i, a)
             },
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function Qt(e) {
-        let t, n, i, a, r, l, o = e[18].name + "",
-            s = e[8](e[18].session),
-            c = s && Nt(e);
+    function qt(e) {
+        let t, n, i, a, r, l, o = e[17].name + "",
+            s = e[8](e[17].session),
+            c = s && jt(e);
 
         function u() {
-            return e[11](e[18])
+            return e[10](e[17])
         }
         return {
             c() {
-                t = O("li"), n = O("a"), i = F(o), a = U(), c && c.c(), this.h()
+                t = O("li"), n = O("a"), i = F(o), a = T(), c && c.c(), this.h()
             },
             l(e) {
                 t = j(e, "LI", {
                     class: !0
                 });
                 var r = W(t);
                 n = j(r, "A", {
@@ -1749,26 +1855,26 @@
                 var l = W(n);
                 i = q(l, o), a = M(l), c && c.l(l), l.forEach(R), r.forEach(R), this.h()
             },
             h() {
                 N(n, "class", "dropdown-link"), N(n, "href", "."), N(t, "class", "dropdown-item")
             },
             m(e, o) {
-                k(e, t, o), x(t, n), x(n, i), x(n, a), c && c.m(n, null), r || (l = T(n, "click", H(D(u))), r = !0)
+                k(e, t, o), x(t, n), x(n, i), x(n, a), c && c.m(n, null), r || (l = z(n, "click", H(D(u))), r = !0)
             },
             p(t, a) {
-                e = t, 16 & a && o !== (o = e[18].name + "") && K(i, o), 16 & a && (s = e[8](e[18].session)), s ? c ? c.p(e, a) : (c = Nt(e), c.c(), c.m(n, null)) : c && (c.d(1), c = null)
+                e = t, 16 & a && o !== (o = e[17].name + "") && K(i, o), 16 & a && (s = e[8](e[17].session)), s ? c ? c.p(e, a) : (c = jt(e), c.c(), c.m(n, null)) : c && (c.d(1), c = null)
             },
             d(e) {
                 e && R(t), c && c.d(), r = !1, l()
             }
         }
     }
 
-    function Wt(e) {
+    function Mt(e) {
         let n, i, a, r, l, o, s;
         return {
             c() {
                 n = O("li"), i = O("a"), a = X("svg"), r = X("path"), l = F("\n              Mark inactive"), this.h()
             },
             l(e) {
                 n = j(e, "LI", {
@@ -1792,24 +1898,24 @@
                     stroke: !0
                 }, 1), W(r).forEach(R), s.forEach(R), l = q(o, "\n              Mark inactive"), o.forEach(R), t.forEach(R), this.h()
             },
             h() {
                 N(r, "d", "M4.91 9.541h3.272c1.164 0 2.283.48 3.111 1.337a4.68 4.68 0 0 1 1.298 3.25v1.13c0 .023-.01.042-.02.052a.037.037 0 0 1-.025.012h-12a.037.037 0 0 1-.027-.012.076.076 0 0 1-.019-.053v-1.13a4.68 4.68 0 0 1 1.298-3.249 4.324 4.324 0 0 1 3.111-1.337ZM3.226 3.956c0-.922.354-1.804.978-2.45A3.253 3.253 0 0 1 6.545.5c.875 0 1.717.36 2.34 1.006a3.53 3.53 0 0 1 .979 2.45 3.53 3.53 0 0 1-.978 2.45 3.253 3.253 0 0 1-2.34 1.005c-.875 0-1.717-.36-2.34-1.005a3.53 3.53 0 0 1-.979-2.45Z"), N(r, "stroke", "currentColor"), N(a, "class", "icon theme-alert-color"), N(a, "viewBox", "0 0 14 16"), N(a, "fill", "none"), N(a, "xmlns", "http://www.w3.org/2000/svg"), N(i, "class", "dropdown-link"), N(i, "href", "."), N(n, "class", "dropdown-item")
             },
             m(t, c) {
-                k(t, n, c), x(n, i), x(i, a), x(a, r), x(i, l), o || (s = T(i, "click", H(D(e[14]))), o = !0)
+                k(t, n, c), x(n, i), x(i, a), x(a, r), x(i, l), o || (s = z(i, "click", H(D(e[13]))), o = !0)
             },
             p: t,
             d(e) {
                 e && R(n), o = !1, s()
             }
         }
     }
 
-    function Jt(e) {
+    function Kt(e) {
         let n, i, a, r, l;
         return {
             c() {
                 n = O("li"), i = O("a"), a = F("Mark active"), this.h()
             },
             l(e) {
                 n = j(e, "LI", {
@@ -1823,24 +1929,24 @@
                 var r = W(i);
                 a = q(r, "Mark active"), r.forEach(R), t.forEach(R), this.h()
             },
             h() {
                 N(i, "class", "dropdown-link"), N(i, "href", "."), N(n, "class", "dropdown-item")
             },
             m(t, o) {
-                k(t, n, o), x(n, i), x(i, a), r || (l = T(i, "click", H(D(e[13]))), r = !0)
+                k(t, n, o), x(n, i), x(i, a), r || (l = z(i, "click", H(D(e[12]))), r = !0)
             },
             p: t,
             d(e) {
                 e && R(n), r = !1, l()
             }
         }
     }
 
-    function jt(e) {
+    function Zt(e) {
         let n, i, a, r, l, o, s;
         return {
             c() {
                 n = O("li"), i = O("a"), a = X("svg"), r = X("path"), l = F("\n              Unassign"), this.h()
             },
             l(e) {
                 n = j(e, "LI", {
@@ -1864,203 +1970,230 @@
                     fill: !0
                 }, 1), W(r).forEach(R), s.forEach(R), l = q(o, "\n              Unassign"), o.forEach(R), t.forEach(R), this.h()
             },
             h() {
                 N(r, "d", "M4.91 9.541h3.272c1.164 0 2.283.48 3.111 1.337a4.68 4.68 0 0 1 1.298 3.25v1.13c0 .023-.01.042-.02.052a.037.037 0 0 1-.025.012h-12a.037.037 0 0 1-.027-.012.076.076 0 0 1-.019-.053v-1.13a4.68 4.68 0 0 1 1.298-3.249 4.324 4.324 0 0 1 3.111-1.337ZM3.226 3.956c0-.922.354-1.804.978-2.45A3.253 3.253 0 0 1 6.545.5c.875 0 1.717.36 2.34 1.006a3.53 3.53 0 0 1 .979 2.45 3.53 3.53 0 0 1-.978 2.45 3.253 3.253 0 0 1-2.34 1.005c-.875 0-1.717-.36-2.34-1.005a3.53 3.53 0 0 1-.979-2.45Z"), N(r, "fill", "currentColor"), N(a, "class", "icon theme-info-color"), N(a, "viewBox", "0 0 14 16"), N(a, "fill", "none"), N(a, "xmlns", "http://www.w3.org/2000/svg"), N(i, "class", "dropdown-link"), N(i, "href", "."), N(n, "class", "dropdown-item")
             },
             m(t, c) {
-                k(t, n, c), x(n, i), x(i, a), x(a, r), x(i, l), o || (s = T(i, "click", H(D(e[15]))), o = !0)
+                k(t, n, c), x(n, i), x(i, a), x(a, r), x(i, l), o || (s = z(i, "click", H(D(e[14]))), o = !0)
             },
             p: t,
             d(e) {
                 e && R(n), o = !1, s()
             }
         }
     }
 
-    function qt(e) {
-        let n, i, a, r, o, s, c, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, P, L, z, Q, J, Z, $ = e[0].name + "",
-            _ = e[4],
-            ee = [];
-        for (let t = 0; t < _.length; t += 1) ee[t] = Qt(Ht(e, _, t));
-
-        function te(e, t) {
-            return e[0].inactive ? Jt : Wt
-        }
-        let ne = te(e),
-            ie = ne(e),
-            ae = e[3] && jt(e);
-        return {
-            c() {
-                n = O("div"), i = O("div"), a = O("div"), r = O("div"), o = F(e[7]), s = U(), c = O("p"), u = F($), d = U(), A = O("div"), f = O("a"), h = F("Assign to…"), m = U(), p = O("div"), g = O("ul");
-                for (let e = 0; e < ee.length; e += 1) ee[e].c();
-                v = U(), y = O("li"), E = O("a"), b = X("svg"), I = X("g"), w = X("path"), C = X("path"), B = X("path"), S = F("\n            New Team"), P = U(), ie.c(), L = U(), ae && ae.c(), z = U(), Q = O("input"), this.h()
+    function Yt(e) {
+        let t, n, i, a, r, l, o, s, c, u, d, A, f, h, m = e[4],
+            p = [];
+        for (let b = 0; b < m.length; b += 1) p[b] = qt(Jt(e, m, b));
+
+        function g(e, t) {
+            return e[0].inactive ? Kt : Mt
+        }
+        let v = g(e),
+            y = v(e),
+            E = e[3] && Zt(e);
+        return {
+            c() {
+                t = O("ul");
+                for (let e = 0; e < p.length; e += 1) p[e].c();
+                n = T(), i = O("li"), a = O("a"), r = X("svg"), l = X("g"), o = X("path"), s = X("path"), c = X("path"), u = F("\n            New Team"), d = T(), y.c(), A = T(), E && E.c(), this.h()
             },
-            l(t) {
-                n = j(t, "DIV", {
-                    class: !0,
-                    "aria-readonly": !0
-                });
-                var l = W(n);
-                i = j(l, "DIV", {
-                    class: !0
-                });
-                var x = W(i);
-                a = j(x, "DIV", {
-                    class: !0,
-                    style: !0
-                });
-                var k = W(a);
-                r = j(k, "DIV", {
-                    class: !0
-                });
-                var V = W(r);
-                o = q(V, e[7]), V.forEach(R), k.forEach(R), s = M(x), c = j(x, "P", {
-                    class: !0
-                });
-                var O = W(c);
-                u = q(O, $), O.forEach(R), x.forEach(R), d = M(l), A = j(l, "DIV", {
-                    class: !0
-                });
-                var X = W(A);
-                f = j(X, "A", {
-                    href: !0,
-                    class: !0
-                });
-                var F = W(f);
-                h = q(F, "Assign to…"), F.forEach(R), m = M(X), p = j(X, "DIV", {
-                    class: !0
-                });
-                var U = W(p);
-                g = j(U, "UL", {
+            l(e) {
+                t = j(e, "UL", {
                     class: !0
                 });
-                var T = W(g);
-                for (let e = 0; e < ee.length; e += 1) ee[e].l(T);
-                v = M(T), y = j(T, "LI", {
+                var f = W(t);
+                for (let t = 0; t < p.length; t += 1) p[t].l(f);
+                n = M(f), i = j(f, "LI", {
                     class: !0
                 });
-                var D = W(y);
-                E = j(D, "A", {
+                var h = W(i);
+                a = j(h, "A", {
                     class: !0,
                     href: !0
                 });
-                var H = W(E);
-                b = j(H, "svg", {
+                var m = W(a);
+                r = j(m, "svg", {
                     class: !0,
                     viewBox: !0,
                     id: !0,
                     xmlns: !0
                 }, 1);
-                var N = W(b);
-                I = j(N, "g", {
+                var g = W(r);
+                l = j(g, "g", {
                     fill: !0
                 }, 1);
-                var J = W(I);
-                w = j(J, "path", {
+                var v = W(l);
+                o = j(v, "path", {
                     d: !0
-                }, 1), W(w).forEach(R), C = j(J, "path", {
+                }, 1), W(o).forEach(R), s = j(v, "path", {
                     d: !0
-                }, 1), W(C).forEach(R), B = j(J, "path", {
+                }, 1), W(s).forEach(R), c = j(v, "path", {
                     d: !0
-                }, 1), W(B).forEach(R), J.forEach(R), N.forEach(R), S = q(H, "\n            New Team"), H.forEach(R), D.forEach(R), P = M(T), ie.l(T), L = M(T), ae && ae.l(T), T.forEach(R), U.forEach(R), X.forEach(R), z = M(l), Q = j(l, "INPUT", {
-                    class: !0,
-                    type: !0
-                }), l.forEach(R), this.h()
+                }, 1), W(c).forEach(R), v.forEach(R), g.forEach(R), u = q(m, "\n            New Team"), m.forEach(R), h.forEach(R), d = M(f), y.l(f), A = M(f), E && E.l(f), f.forEach(R), this.h()
             },
             h() {
-                N(r, "class", "avatar-inner"), N(a, "class", "avatar"), Y(a, "background", Dt(e[0].name)), N(c, "class", "avatar-detail-meta"), N(i, "class", "avatar-detail"), N(f, "href", "."), N(f, "class", "button dropdown-button hollow small"), N(w, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), N(C, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), N(B, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), N(I, "fill", "currentColor"), N(b, "class", "icon theme-info-color"), N(b, "viewBox", "0 0 17.928 22.481"), N(b, "id", "people"), N(b, "xmlns", "http://www.w3.org/2000/svg"), N(E, "class", "dropdown-link is-new"), N(E, "href", "."), N(y, "class", "dropdown-item"), N(g, "class", "dropdown-list"), N(p, "class", "dropdown"), N(A, "class", "has-dropdown narrow-dropdown"), N(Q, "class", "show-for-sr-only svelte-hxuor6"), N(Q, "type", "checkbox"), Q.checked = e[1], N(n, "class", "player-item svelte-hxuor6"), N(n, "aria-readonly", e[2]), G(n, "is-selected", e[1])
+                N(o, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), N(s, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), N(c, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), N(l, "fill", "currentColor"), N(r, "class", "icon theme-info-color"), N(r, "viewBox", "0 0 17.928 22.481"), N(r, "id", "people"), N(r, "xmlns", "http://www.w3.org/2000/svg"), N(a, "class", "dropdown-link is-new"), N(a, "href", "."), N(i, "class", "dropdown-item"), N(t, "class", "dropdown-list")
             },
-            m(t, l) {
-                k(t, n, l), x(n, i), x(i, a), x(a, r), x(r, o), x(i, s), x(i, c), x(c, u), x(n, d), x(n, A), x(A, f), x(f, h), x(A, m), x(A, p), x(p, g);
-                for (let e = 0; e < ee.length; e += 1) ee[e].m(g, null);
-                x(g, v), x(g, y), x(y, E), x(E, b), x(b, I), x(I, w), x(I, C), x(I, B), x(E, S), x(g, P), ie.m(g, null), x(g, L), ae && ae.m(g, null), x(n, z), x(n, Q), J || (Z = [T(f, "click", H(D(e[10]))), T(E, "click", H(D(e[12]))), T(n, "click", e[16])], J = !0)
+            m(m, g) {
+                k(m, t, g);
+                for (let e = 0; e < p.length; e += 1) p[e].m(t, null);
+                x(t, n), x(t, i), x(i, a), x(a, r), x(r, l), x(l, o), x(l, s), x(l, c), x(a, u), x(t, d), y.m(t, null), x(t, A), E && E.m(t, null), f || (h = z(a, "click", H(D(e[11]))), f = !0)
             },
-            p(e, [t]) {
-                if (1 & t && Y(a, "background", Dt(e[0].name)), 1 & t && $ !== ($ = e[0].name + "") && K(u, $), 337 & t) {
-                    let n;
-                    for (_ = e[4], n = 0; n < _.length; n += 1) {
-                        const i = Ht(e, _, n);
-                        ee[n] ? ee[n].p(i, t) : (ee[n] = Qt(i), ee[n].c(), ee[n].m(g, v))
+            p(e, i) {
+                if (337 & i) {
+                    let a;
+                    for (m = e[4], a = 0; a < m.length; a += 1) {
+                        const r = Jt(e, m, a);
+                        p[a] ? p[a].p(r, i) : (p[a] = qt(r), p[a].c(), p[a].m(t, n))
                     }
-                    for (; n < ee.length; n += 1) ee[n].d(1);
-                    ee.length = _.length
+                    for (; a < p.length; a += 1) p[a].d(1);
+                    p.length = m.length
                 }
-                ne === (ne = te(e)) && ie ? ie.p(e, t) : (ie.d(1), ie = ne(e), ie && (ie.c(), ie.m(g, L))), e[3] ? ae ? ae.p(e, t) : (ae = jt(e), ae.c(), ae.m(g, null)) : ae && (ae.d(1), ae = null), 2 & t && (Q.checked = e[1]), 4 & t && N(n, "aria-readonly", e[2]), 2 & t && G(n, "is-selected", e[1])
+                v === (v = g(e)) && y ? y.p(e, i) : (y.d(1), y = v(e), y && (y.c(), y.m(t, A))), e[3] ? E ? E.p(e, i) : (E = Zt(e), E.c(), E.m(t, null)) : E && (E.d(1), E = null)
             },
-            i: t,
-            o: t,
             d(e) {
-                e && R(n), V(ee, e), ie.d(), ae && ae.d(), J = !1, l(Z)
+                e && R(t), V(p, e), y.d(), E && E.d(), f = !1, h()
             }
         }
     }
 
-    function Mt(e, t, n) {
+    function Gt(e) {
+        let t, n, i, a, r, l, o, s, c, u, d, A, f, h, m, p = e[0].name + "";
+        return u = new Wt({
+            props: {
+                placeholderText: "Assign to…",
+                $$slots: {
+                    default: [Yt]
+                },
+                $$scope: {
+                    ctx: e
+                }
+            }
+        }), {
+            c() {
+                t = O("div"), n = O("div"), i = O("div"), a = O("div"), r = F(e[7]), l = T(), o = O("p"), s = F(p), c = T(), Je(u.$$.fragment), d = T(), A = O("input"), this.h()
+            },
+            l(f) {
+                t = j(f, "DIV", {
+                    class: !0,
+                    "aria-readonly": !0
+                });
+                var h = W(t);
+                n = j(h, "DIV", {
+                    class: !0
+                });
+                var m = W(n);
+                i = j(m, "DIV", {
+                    class: !0,
+                    style: !0
+                });
+                var g = W(i);
+                a = j(g, "DIV", {
+                    class: !0
+                });
+                var v = W(a);
+                r = q(v, e[7]), v.forEach(R), g.forEach(R), l = M(m), o = j(m, "P", {
+                    class: !0
+                });
+                var y = W(o);
+                s = q(y, p), y.forEach(R), m.forEach(R), c = M(h), je(u.$$.fragment, h), d = M(h), A = j(h, "INPUT", {
+                    class: !0,
+                    type: !0
+                }), h.forEach(R), this.h()
+            },
+            h() {
+                N(a, "class", "avatar-inner"), N(i, "class", "avatar"), Y(i, "background", Ht(e[0].name)), N(o, "class", "avatar-detail-meta"), N(n, "class", "avatar-detail"), N(A, "class", "show-for-sr-only svelte-hxuor6"), N(A, "type", "checkbox"), A.checked = e[1], N(t, "class", "player-item svelte-hxuor6"), N(t, "aria-readonly", e[2]), G(t, "is-selected", e[1])
+            },
+            m(p, g) {
+                k(p, t, g), x(t, n), x(n, i), x(i, a), x(a, r), x(n, l), x(n, o), x(o, s), x(t, c), qe(u, t, null), x(t, d), x(t, A), f = !0, h || (m = z(t, "click", e[15]), h = !0)
+            },
+            p(e, [n]) {
+                (!f || 1 & n) && Y(i, "background", Ht(e[0].name)), (!f || 1 & n) && p !== (p = e[0].name + "") && K(s, p);
+                const a = {};
+                1048635 & n && (a.$$scope = {
+                    dirty: n,
+                    ctx: e
+                }), u.$set(a), (!f || 2 & n) && (A.checked = e[1]), (!f || 4 & n) && N(t, "aria-readonly", e[2]), 2 & n && G(t, "is-selected", e[1])
+            },
+            i(e) {
+                f || (Ve(u.$$.fragment, e), f = !0)
+            },
+            o(e) {
+                Oe(u.$$.fragment, e), f = !1
+            },
+            d(e) {
+                e && R(t), Me(u), h = !1, m()
+            }
+        }
+    }
+
+    function $t(e, t, n) {
         let i;
-        d(e, $e, (e => n(5, i = e)));
+        d(e, _e, (e => n(5, i = e)));
         let {
             isSelected: a = !1
         } = t, {
             player: r
         } = t, {
             currentTeam: l = null
         } = t, {
             readOnly: o = !1
         } = t, {
             assigned: s = !1
         } = t;
-        const c = ue(),
+        const c = de(),
             u = r.name.replace(/(\w)[^ ]+/g, "$1").replace(/[^\w]/g, "");
         var A = u[0] + u[u.length - 1];
         let f;
         return e.$$set = e => {
             "isSelected" in e && n(1, a = e.isSelected), "player" in e && n(0, r = e.player), "currentTeam" in e && n(9, l = e.currentTeam), "readOnly" in e && n(2, o = e.readOnly), "assigned" in e && n(3, s = e.assigned)
         }, e.$$.update = () => {
             561 & e.$$.dirty && (n(4, f = i.teams), r.session && i.sessions.find((e => e.id === r.session)) && n(4, f = f.filter((e => e.session === r.session))), l && n(4, f = f.filter((e => e !== l))))
-        }, [r, a, o, s, f, i, c, A, e => e ? i.sessions.length <= 1 ? null : i.sessions.find((t => t.id === e)) : null, l, function(t) {
-            de.call(this, e, t)
-        }, e => {
+        }, [r, a, o, s, f, i, c, A, e => e ? i.sessions.length <= 1 ? null : i.sessions.find((t => t.id === e)) : null, l, e => {
             c("addPlayers", {
                 team: e,
                 adding: [r.id]
             })
         }, () => {
             c("addPlayers", {
                 team: null,
                 adding: [r.id],
                 session: r.session
             })
         }, () => {
-            et.notify({
+            tt.notify({
                 playerId: r.id,
                 active: !0
-            }), n(0, r.inactive = !1, r), $e.set(i)
+            }), n(0, r.inactive = !1, r), _e.set(i)
         }, () => {
-            et.notify({
+            tt.notify({
                 playerId: r.id,
                 active: !1
             }), a && c("selectPlayer", {
                 id: r.id
             }), s && c("unassignPlayer", {
                 id: r.id
-            }), n(0, r.inactive = !0, r), $e.set(i)
+            }), n(0, r.inactive = !0, r), _e.set(i)
         }, () => {
             c("unassignPlayer", {
                 id: r.id
             })
         }, () => {
             o || c("selectPlayer", {
                 id: r.id
             })
         }]
     }
-    class Kt extends Ze {
+    class _t extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Mt, qt, s, {
+            super(), Ze(this, e, $t, Gt, s, {
                 isSelected: 1,
                 player: 0,
                 currentTeam: 9,
                 readOnly: 2,
                 assigned: 3
             })
         }
@@ -2075,29 +2208,29 @@
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
         AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
         INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
         LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
         OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
         PERFORMANCE OF THIS SOFTWARE.
         ***************************************************************************** */
-    function Zt(e, {
+    function en(e, {
         delay: t = 0,
         duration: i = 400,
         easing: a = n
     } = {}) {
         const r = +getComputedStyle(e).opacity;
         return {
             delay: t,
             duration: i,
             easing: a,
             css: e => "opacity: " + e * r
         }
     }
 
-    function Yt(e, {
+    function tn(e, {
         delay: t = 0,
         duration: n = 400,
         easing: i = zt
     } = {}) {
         const a = getComputedStyle(e),
             r = +a.opacity,
             l = parseFloat(a.height),
@@ -2110,15 +2243,15 @@
         return {
             delay: t,
             duration: n,
             easing: i,
             css: e => `overflow: hidden;opacity: ${Math.min(20*e,1)*r};height: ${e*l}px;padding-top: ${e*o}px;padding-bottom: ${e*s}px;margin-top: ${e*c}px;margin-bottom: ${e*u}px;border-top-width: ${e*d}px;border-bottom-width: ${e*A}px;`
         }
     }
-    const [Gt, $t] = function(e) {
+    const [nn, an] = function(e) {
         var {
             fallback: t
         } = e, n = function(e, t) {
             var n = {};
             for (var i in e) Object.prototype.hasOwnProperty.call(e, i) && t.indexOf(i) < 0 && (n[i] = e[i]);
             if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                 var a = 0;
@@ -2164,20 +2297,20 @@
             return {
                 duration: 600,
                 css: e => `\n        transform: ${n} scale(${e});\n        opacity: ${e}\n      `
             }
         }
     });
 
-    function _t(e, t, n) {
+    function rn(e, t, n) {
         const i = e.slice();
         return i[6] = t[n], i
     }
 
-    function en(e) {
+    function ln(e) {
         let t;
         return {
             c() {
                 t = F("Inactive Players")
             },
             l(e) {
                 t = q(e, "Inactive Players")
@@ -2187,15 +2320,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function tn(e) {
+    function on(e) {
         let t;
         return {
             c() {
                 t = F("Unassigned Players")
             },
             l(e) {
                 t = q(e, "Unassigned Players")
@@ -2205,19 +2338,19 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function nn(e) {
+    function sn(e) {
         let t, n, i, a, r, l;
         return {
             c() {
-                t = O("span"), n = X("svg"), i = X("path"), a = U(), r = O("div"), l = F("Inactive players will not be able to participate or follow along once the game is set to play."), this.h()
+                t = O("span"), n = X("svg"), i = X("path"), a = T(), r = O("div"), l = F("Inactive players will not be able to participate or follow along once the game is set to play."), this.h()
             },
             l(e) {
                 t = j(e, "SPAN", {
                     class: !0
                 });
                 var o = W(t);
                 n = j(o, "svg", {
@@ -2246,91 +2379,91 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function an(e, n) {
+    function cn(e, n) {
         let i, a, r, l, o, s, c, u = t;
-        return a = new Kt({
+        return a = new _t({
             props: {
                 isSelected: n[0].includes(n[6].id),
                 player: n[6]
             }
         }), a.$on("selectPlayer", n[4]), a.$on("addPlayers", n[5]), {
             key: e,
             first: null,
             c() {
-                i = O("div"), We(a.$$.fragment), r = U(), this.h()
+                i = O("div"), Je(a.$$.fragment), r = T(), this.h()
             },
             l(e) {
                 i = j(e, "DIV", {});
                 var t = W(i);
-                Je(a.$$.fragment, t), r = M(t), t.forEach(R), this.h()
+                je(a.$$.fragment, t), r = M(t), t.forEach(R), this.h()
             },
             h() {
                 this.first = i
             },
             m(e, t) {
-                k(e, i, t), je(a, i, null), x(i, r), c = !0
+                k(e, i, t), qe(a, i, null), x(i, r), c = !0
             },
             p(e, t) {
                 n = e;
                 const i = {};
                 3 & t && (i.isSelected = n[0].includes(n[6].id)), 2 & t && (i.player = n[6]), a.$set(i)
             },
             r() {
                 s = i.getBoundingClientRect()
             },
             f() {
                 re(i), u(), le(i, s)
             },
             a() {
-                u(), u = ae(i, s, Tt, {})
+                u(), u = ae(i, s, Dt, {})
             },
             i(e) {
-                c || (Re(a.$$.fragment, e), e && ve((() => {
-                    o && o.end(1), l = Xe(i, $t, {
+                c || (Ve(a.$$.fragment, e), e && ye((() => {
+                    o && o.end(1), l = Fe(i, an, {
                         key: n[6].id
                     }), l.start()
                 })), c = !0)
             },
             o(e) {
-                Ve(a.$$.fragment, e), l && l.invalidate(), e && (o = Fe(i, Gt, {
+                Oe(a.$$.fragment, e), l && l.invalidate(), e && (o = Te(i, nn, {
                     key: n[6].id
                 })), c = !1
             },
             d(e) {
-                e && R(i), qe(a), e && o && o.end()
+                e && R(i), Me(a), e && o && o.end()
             }
         }
     }
 
-    function rn(e) {
+    function un(e) {
         let t, n, i, a, r, l, o, s, c, u = e[1].length + "",
             d = [],
             A = new Map;
 
         function f(e, t) {
-            return e[3] ? en : tn
+            return e[3] ? ln : on
         }
         let h = f(e),
             m = h(e),
-            p = e[3] && nn(),
+            p = e[3] && sn(),
             g = e[1];
         const v = e => e[6].id;
         for (let y = 0; y < g.length; y += 1) {
-            let t = _t(e, g, y),
+            let t = rn(e, g, y),
                 n = v(t);
-            A.set(n, d[y] = an(n, t))
+            A.set(n, d[y] = cn(n, t))
         }
         return {
             c() {
-                t = O("div"), n = O("p"), m.c(), i = F("\n    ("), a = F(u), r = F(")\n    "), p && p.c(), o = U(), s = O("div");
+                t = O("div"), n = O("p"), m.c(), i = F("\n    ("), a = F(u), r = F(")\n    "), p && p.c(), o = T(), s = O("div");
                 for (let e = 0; e < d.length; e += 1) d[e].c();
                 this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
                     class: !0
                 });
@@ -2354,75 +2487,75 @@
             },
             m(e, l) {
                 k(e, t, l), x(t, n), m.m(n, null), x(n, i), x(n, a), x(n, r), p && p.m(n, null), k(e, o, l), k(e, s, l);
                 for (let t = 0; t < d.length; t += 1) d[t].m(s, null);
                 c = !0
             },
             p(e, [r]) {
-                if (h !== (h = f(e)) && (m.d(1), m = h(e), m && (m.c(), m.m(n, i))), (!c || 2 & r) && u !== (u = e[1].length + "") && K(a, u), e[3] ? p || (p = nn(), p.c(), p.m(n, null)) : p && (p.d(1), p = null), (!c || 8 & r && l !== (l = e[3] ? "inactive-players" : "unassigned-players")) && N(n, "id", l), 14 & r && G(n, "note", !e[3] && e[1].length && e[2]), 14 & r && G(n, "theme-alert-color", !e[3] && e[1].length && e[2]), 8 & r && G(t, "pad-top", e[3]), 3 & r) {
-                    g = e[1], xe();
+                if (h !== (h = f(e)) && (m.d(1), m = h(e), m && (m.c(), m.m(n, i))), (!c || 2 & r) && u !== (u = e[1].length + "") && K(a, u), e[3] ? p || (p = sn(), p.c(), p.m(n, null)) : p && (p.d(1), p = null), (!c || 8 & r && l !== (l = e[3] ? "inactive-players" : "unassigned-players")) && N(n, "id", l), 14 & r && G(n, "note", !e[3] && e[1].length && e[2]), 14 & r && G(n, "theme-alert-color", !e[3] && e[1].length && e[2]), 8 & r && G(t, "pad-top", e[3]), 3 & r) {
+                    g = e[1], ke();
                     for (let e = 0; e < d.length; e += 1) d[e].r();
-                    d = Ne(d, r, v, 1, e, g, A, s, He, an, null, _t);
+                    d = Qe(d, r, v, 1, e, g, A, s, Ne, cn, null, rn);
                     for (let e = 0; e < d.length; e += 1) d[e].a();
-                    ke()
+                    Re()
                 }
                 8 & r && G(s, "glow-shadow", !e[3]), 8 & r && G(s, "is-inactive-player", e[3])
             },
             i(e) {
                 if (!c) {
-                    for (let e = 0; e < g.length; e += 1) Re(d[e]);
+                    for (let e = 0; e < g.length; e += 1) Ve(d[e]);
                     c = !0
                 }
             },
             o(e) {
-                for (let t = 0; t < d.length; t += 1) Ve(d[t]);
+                for (let t = 0; t < d.length; t += 1) Oe(d[t]);
                 c = !1
             },
             d(e) {
                 e && R(t), m.d(), p && p.d(), e && R(o), e && R(s);
                 for (let t = 0; t < d.length; t += 1) d[t].d()
             }
         }
     }
 
-    function ln(e, t, n) {
+    function dn(e, t, n) {
         let {
             selected: i
         } = t, {
             players: a
         } = t, {
             unassignedIsError: r = !1
         } = t, {
             inactive: l = !1
         } = t;
         return e.$$set = e => {
             "selected" in e && n(0, i = e.selected), "players" in e && n(1, a = e.players), "unassignedIsError" in e && n(2, r = e.unassignedIsError), "inactive" in e && n(3, l = e.inactive)
         }, [i, a, r, l, function(t) {
-            de.call(this, e, t)
+            Ae.call(this, e, t)
         }, function(t) {
-            de.call(this, e, t)
+            Ae.call(this, e, t)
         }]
     }
-    class on extends Ze {
+    class An extends Ye {
         constructor(e) {
-            super(), Ke(this, e, ln, rn, s, {
+            super(), Ze(this, e, dn, un, s, {
                 selected: 0,
                 players: 1,
                 unassignedIsError: 2,
                 inactive: 3
             })
         }
     }
 
-    function sn(e, t, n) {
+    function fn(e, t, n) {
         const i = e.slice();
         return i[14] = t[n], i
     }
 
-    function cn(e) {
+    function hn(e) {
         let n;
         return {
             c() {
                 n = F("Inactive Players")
             },
             l(e) {
                 n = q(e, "Inactive Players")
@@ -2433,15 +2566,15 @@
             p: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function un(e) {
+    function mn(e) {
         let t, n, i, a = 1 != e[4] ? "s" : "";
         return {
             c() {
                 t = O("a"), n = F("Inactive Player"), i = F(a), this.h()
             },
             l(e) {
                 t = j(e, "A", {
@@ -2461,19 +2594,19 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function dn(e) {
+    function pn(e) {
         let n, i, a, r, l;
         return {
             c() {
-                n = O("h3"), i = F("Create your first team"), a = U(), r = O("p"), l = F("Teams may be created manually now. Alternatively once players arrive, you\n      may randomly distribute players into teams."), this.h()
+                n = O("h3"), i = F("Create your first team"), a = T(), r = O("p"), l = F("Teams may be created manually now. Alternatively once players arrive, you\n      may randomly distribute players into teams."), this.h()
             },
             l(e) {
                 n = j(e, "H3", {
                     class: !0
                 });
                 var t = W(n);
                 i = q(t, "Create your first team"), t.forEach(R), a = M(e), r = j(e, "P", {
@@ -2491,28 +2624,28 @@
             p: t,
             d(e) {
                 e && R(n), e && R(a), e && R(r)
             }
         }
     }
 
-    function An(e) {
+    function gn(e) {
         let t, n, i = [],
             a = new Map,
-            r = e[6] && fn(e),
+            r = e[6] && vn(e),
             l = e[7];
         const o = e => e[14].internalId || e[14].id;
         for (let s = 0; s < l.length; s += 1) {
-            let t = sn(e, l, s),
+            let t = fn(e, l, s),
                 n = o(t);
-            a.set(n, i[s] = mn(n, t))
+            a.set(n, i[s] = En(n, t))
         }
         return {
             c() {
-                r && r.c(), t = U(), n = O("ul");
+                r && r.c(), t = T(), n = O("ul");
                 for (let e = 0; e < i.length; e += 1) i[e].c();
                 this.h()
             },
             l(e) {
                 r && r.l(e), t = M(e), n = j(e, "UL", {
                     class: !0
                 });
@@ -2524,24 +2657,24 @@
                 N(n, "class", "pill-list is-large")
             },
             m(e, a) {
                 r && r.m(e, a), k(e, t, a), k(e, n, a);
                 for (let t = 0; t < i.length; t += 1) i[t].m(n, null)
             },
             p(e, s) {
-                e[6] ? r ? r.p(e, s) : (r = fn(e), r.c(), r.m(t.parentNode, t)) : r && (r.d(1), r = null), 641 & s && (l = e[7], i = Ne(i, s, o, 1, e, l, a, n, Te, mn, null, sn))
+                e[6] ? r ? r.p(e, s) : (r = vn(e), r.c(), r.m(t.parentNode, t)) : r && (r.d(1), r = null), 641 & s && (l = e[7], i = Qe(i, s, o, 1, e, l, a, n, De, En, null, fn))
             },
             d(e) {
                 r && r.d(e), e && R(t), e && R(n);
                 for (let t = 0; t < i.length; t += 1) i[t].d()
             }
         }
     }
 
-    function fn(e) {
+    function vn(e) {
         let t, n;
         return {
             c() {
                 t = O("a"), n = F("Download CSV"), this.h()
             },
             l(e) {
                 t = j(e, "A", {
@@ -2562,15 +2695,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function hn(e) {
+    function yn(e) {
         let t, n, i, a, r = e[9](e[14].session).name + "";
         return {
             c() {
                 t = O("small"), n = F("("), i = F(r), a = F(")")
             },
             l(e) {
                 t = j(e, "SMALL", {});
@@ -2585,28 +2718,28 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function mn(e, t) {
+    function En(e, t) {
         let n, i, a, r, l, o, s, c, u, d, A, f, h = t[14].players.length + "",
             m = t[14].name + "",
             p = t[9](t[14].session);
 
         function g() {
             return t[11](t[14])
         }
-        let v = p && hn(t);
+        let v = p && yn(t);
         return {
             key: e,
             first: null,
             c() {
-                n = O("li"), i = O("span"), a = F(h), r = U(), l = O("span"), o = O("a"), s = F(m), u = U(), v && v.c(), d = U(), this.h()
+                n = O("li"), i = O("span"), a = F(h), r = T(), l = O("span"), o = O("a"), s = F(m), u = T(), v && v.c(), d = T(), this.h()
             },
             l(e) {
                 n = j(e, "LI", {
                     class: !0
                 });
                 var t = W(n);
                 i = j(t, "SPAN", {
@@ -2623,30 +2756,30 @@
                 var f = W(o);
                 s = q(f, m), f.forEach(R), u = M(A), v && v.l(A), A.forEach(R), d = M(t), t.forEach(R), this.h()
             },
             h() {
                 N(i, "class", "pill-var"), N(o, "href", c = "#" + (t[14].internalId || t[14].id)), N(l, "class", "pill-label"), N(n, "class", "pill-item"), this.first = n
             },
             m(e, t) {
-                k(e, n, t), x(n, i), x(i, a), x(n, r), x(n, l), x(l, o), x(o, s), x(l, u), v && v.m(l, null), x(n, d), A || (f = T(o, "click", g), A = !0)
+                k(e, n, t), x(n, i), x(i, a), x(n, r), x(n, l), x(l, o), x(o, s), x(l, u), v && v.m(l, null), x(n, d), A || (f = z(o, "click", g), A = !0)
             },
             p(e, n) {
-                t = e, 128 & n && h !== (h = t[14].players.length + "") && K(a, h), 128 & n && m !== (m = t[14].name + "") && K(s, m), 128 & n && c !== (c = "#" + (t[14].internalId || t[14].id)) && N(o, "href", c), 128 & n && (p = t[9](t[14].session)), p ? v ? v.p(t, n) : (v = hn(t), v.c(), v.m(l, null)) : v && (v.d(1), v = null)
+                t = e, 128 & n && h !== (h = t[14].players.length + "") && K(a, h), 128 & n && m !== (m = t[14].name + "") && K(s, m), 128 & n && c !== (c = "#" + (t[14].internalId || t[14].id)) && N(o, "href", c), 128 & n && (p = t[9](t[14].session)), p ? v ? v.p(t, n) : (v = yn(t), v.c(), v.m(l, null)) : v && (v.d(1), v = null)
             },
             d(e) {
                 e && R(n), v && v.d(), A = !1, f()
             }
         }
     }
 
-    function pn(e) {
-        let t, n, i, a, r, l, o, s, c, u, d, A = e[1] && gn(e);
+    function bn(e) {
+        let t, n, i, a, r, l, o, s, c, u, d, A = e[1] && In(e);
         return {
             c() {
-                t = O("button"), n = X("svg"), i = X("g"), a = X("path"), r = X("path"), l = X("path"), o = F("\n        Create New Team"), s = U(), A && A.c(), c = z(), this.h()
+                t = O("button"), n = X("svg"), i = X("g"), a = X("path"), r = X("path"), l = X("path"), o = F("\n        Create New Team"), s = T(), A && A.c(), c = U(), this.h()
             },
             l(e) {
                 t = j(e, "BUTTON", {
                     class: !0
                 });
                 var u = W(t);
                 n = j(u, "svg", {
@@ -2663,32 +2796,32 @@
                 var f = W(i);
                 a = j(f, "path", {
                     d: !0
                 }, 1), W(a).forEach(R), r = j(f, "path", {
                     d: !0
                 }, 1), W(r).forEach(R), l = j(f, "path", {
                     d: !0
-                }, 1), W(l).forEach(R), f.forEach(R), d.forEach(R), o = q(u, "\n        Create New Team"), u.forEach(R), s = M(e), A && A.l(e), c = z(), this.h()
+                }, 1), W(l).forEach(R), f.forEach(R), d.forEach(R), o = q(u, "\n        Create New Team"), u.forEach(R), s = M(e), A && A.l(e), c = U(), this.h()
             },
             h() {
                 N(a, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), N(r, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), N(l, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), N(i, "fill", "currentColor"), N(n, "class", "icon"), Y(n, "margin-left", "-8px"), N(n, "viewBox", "0 0 17.928 22.481"), N(n, "id", "people"), N(n, "xmlns", "http://www.w3.org/2000/svg"), N(t, "class", "button")
             },
             m(f, h) {
-                k(f, t, h), x(t, n), x(n, i), x(i, a), x(i, r), x(i, l), x(t, o), k(f, s, h), A && A.m(f, h), k(f, c, h), u || (d = T(t, "click", e[12]), u = !0)
+                k(f, t, h), x(t, n), x(n, i), x(i, a), x(i, r), x(i, l), x(t, o), k(f, s, h), A && A.m(f, h), k(f, c, h), u || (d = z(t, "click", e[12]), u = !0)
             },
             p(e, t) {
-                e[1] ? A ? A.p(e, t) : (A = gn(e), A.c(), A.m(c.parentNode, c)) : A && (A.d(1), A = null)
+                e[1] ? A ? A.p(e, t) : (A = In(e), A.c(), A.m(c.parentNode, c)) : A && (A.d(1), A = null)
             },
             d(e) {
                 e && R(t), e && R(s), A && A.d(e), e && R(c), u = !1, d()
             }
         }
     }
 
-    function gn(e) {
+    function In(e) {
         let t, n, i, a, r, l, o, s, c, u, d, A, f, h = 1 !== e[1] ? "s" : "";
         return {
             c() {
                 t = O("button"), n = X("svg"), i = X("g"), a = X("path"), r = X("path"), l = X("path"), o = F("\n          Auto-assign "), s = F(e[1]), c = F(" player"), u = F(h), d = F("\n          to teams"), this.h()
             },
             l(A) {
                 t = j(A, "BUTTON", {
@@ -2715,45 +2848,45 @@
                     d: !0
                 }, 1), W(l).forEach(R), p.forEach(R), m.forEach(R), o = q(f, "\n          Auto-assign "), s = q(f, e[1]), c = q(f, " player"), u = q(f, h), d = q(f, "\n          to teams"), f.forEach(R), this.h()
             },
             h() {
                 N(a, "d", "M16.731 7.152h-1.274a.59.59 0 00-.581.689.939.939 0 01.028.104v.003a2.487 2.487 0 01.068.707l-.514 5.696-.008.087a.331.331 0 01-.004.033l-.008.062a2.055 2.055 0 01-1.402 1.64l-.032.01a.589.589 0 00-.389.468c-.002 0-.002 0 0 0l-.008.088v.001l-.254 3.178-.004.036v.029c0 .326.264.59.59.59h1.791a.774.774 0 00.762-.637l.012-.15.416-5.191a.515.515 0 01.483-.502l.033-.001.033.001h.231v-.001a.776.776 0 00.766-.657v-.009l.008-.077.451-5a1.192 1.192 0 00-1.194-1.197zm-3.802-1.13a2.62 2.62 0 00.78.118A2.647 2.647 0 1013.42.862a.589.589 0 00-.454.811 4.179 4.179 0 01-.349 3.45l-.002.005-.033.056a.59.59 0 00.347.838z"), N(r, "d", "M12.402 15.095a.884.884 0 00.873-.749v-.01l.008-.087.514-5.699c0-.753-.609-1.363-1.362-1.363H5.547c-.753 0-1.363.61-1.363 1.363l.51 5.656.016.17a.884.884 0 00.867.719v.001h.268l.037-.001.039.001a.591.591 0 01.551.581l.474 5.928.011.133a.883.883 0 00.871.744h2.331a.883.883 0 00.868-.727l.014-.17.473-5.918c0-.02.002-.038.004-.057a.594.594 0 01.548-.515l.038-.001.037.001h.261zM8.99 6.032a3.013 3.013 0 003.018-3.016A3.016 3.016 0 108.99 6.032z"), N(l, "d", "M5.625 19.913l-.252-3.173v-.001l-.008-.088v-.001a.59.59 0 00-.435-.482h-.003a2.066 2.066 0 01-1.393-1.686l-.016-.171-.508-5.656a.924.924 0 01-.006-.105c0-.207.025-.406.072-.599.008-.039.02-.077.03-.115a.59.59 0 00-.582-.684H1.25c-.66 0-1.195.535-1.195 1.196l.447 4.964.013.149c.067.358.383.63.762.63v.001h.233l.034-.001.033.001a.519.519 0 01.485.509l.415 5.201.01.117a.776.776 0 00.765.652h1.79a.59.59 0 00.59-.59l-.001-.02-.006-.048zM4.272 6.14a2.652 2.652 0 00.78-.117l.006-.002a.59.59 0 00.342-.835l-.033-.057-.003-.005a4.173 4.173 0 01-.348-3.45v-.003l.022-.063a.589.589 0 00-.477-.746C4.556.86 4.55.86 4.543.859a2.296 2.296 0 00-.271-.014 2.648 2.648 0 000 5.295z"), N(i, "fill", "currentColor"), N(n, "class", "icon"), Y(n, "margin-left", "-8px"), N(n, "viewBox", "0 0 17.928 22.481"), N(n, "id", "people"), N(n, "xmlns", "http://www.w3.org/2000/svg"), N(t, "class", "button")
             },
             m(h, m) {
-                k(h, t, m), x(t, n), x(n, i), x(i, a), x(i, r), x(i, l), x(t, o), x(t, s), x(t, c), x(t, u), x(t, d), A || (f = T(t, "click", e[13]), A = !0)
+                k(h, t, m), x(t, n), x(n, i), x(i, a), x(i, r), x(i, l), x(t, o), x(t, s), x(t, c), x(t, u), x(t, d), A || (f = z(t, "click", e[13]), A = !0)
             },
             p(e, t) {
                 2 & t && K(s, e[1]), 2 & t && h !== (h = 1 !== e[1] ? "s" : "") && K(u, h)
             },
             d(e) {
                 e && R(t), A = !1, f()
             }
         }
     }
 
-    function vn(e) {
-        let n, i, a, r, l, o, s, c, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, P, L, V, X = 1 != e[2] ? "s" : "",
-            z = e[7].length + "",
-            T = 1 != e[7].length ? "s" : "";
+    function wn(e) {
+        let n, i, a, r, l, o, s, c, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, L, P, V, X = 1 != e[2] ? "s" : "",
+            U = e[7].length + "",
+            z = 1 != e[7].length ? "s" : "";
 
         function D(e, t) {
-            return e[4] ? un : cn
+            return e[4] ? mn : hn
         }
         let H = D(e),
             Q = H(e);
 
         function J(e, t) {
-            return e[7].length ? An : dn
+            return e[7].length ? gn : pn
         }
         let Z = J(e),
             G = Z(e),
-            $ = e[5] && pn(e);
+            $ = e[5] && bn(e);
         return {
             c() {
-                n = O("ul"), i = O("li"), a = O("span"), r = F(e[2]), l = U(), o = O("span"), s = F("Unassigned Player"), c = F(X), u = U(), d = O("li"), A = O("span"), f = F(z), h = U(), m = O("span"), p = O("a"), g = F("Team"), v = F(T), y = U(), E = O("li"), b = O("span"), I = F(e[4]), w = U(), C = O("span"), Q.c(), B = U(), S = O("div"), G.c(), P = U(), L = O("div"), $ && $.c(), this.h()
+                n = O("ul"), i = O("li"), a = O("span"), r = F(e[2]), l = T(), o = O("span"), s = F("Unassigned Player"), c = F(X), u = T(), d = O("li"), A = O("span"), f = F(U), h = T(), m = O("span"), p = O("a"), g = F("Team"), v = F(z), y = T(), E = O("li"), b = O("span"), I = F(e[4]), w = T(), C = O("span"), Q.c(), B = T(), S = O("div"), G.c(), L = T(), P = O("div"), $ && $.c(), this.h()
             },
             l(t) {
                 n = j(t, "UL", {
                     class: !0
                 });
                 var x = W(n);
                 i = j(x, "LI", {
@@ -2771,24 +2904,24 @@
                 s = q(O, "Unassigned Player"), c = q(O, X), O.forEach(R), k.forEach(R), u = M(x), d = j(x, "LI", {
                     class: !0
                 });
                 var F = W(d);
                 A = j(F, "SPAN", {
                     class: !0
                 });
-                var U = W(A);
-                f = q(U, z), U.forEach(R), h = M(F), m = j(F, "SPAN", {
+                var T = W(A);
+                f = q(T, U), T.forEach(R), h = M(F), m = j(F, "SPAN", {
                     class: !0
                 });
                 var D = W(m);
                 p = j(D, "A", {
                     href: !0
                 });
                 var H = W(p);
-                g = q(H, "Team"), v = q(H, T), H.forEach(R), D.forEach(R), F.forEach(R), y = M(x), E = j(x, "LI", {
+                g = q(H, "Team"), v = q(H, z), H.forEach(R), D.forEach(R), F.forEach(R), y = M(x), E = j(x, "LI", {
                     class: !0
                 });
                 var N = W(E);
                 b = j(N, "SPAN", {
                     class: !0
                 });
                 var J = W(b);
@@ -2796,39 +2929,39 @@
                     class: !0
                 });
                 var K = W(C);
                 Q.l(K), K.forEach(R), N.forEach(R), x.forEach(R), B = M(t), S = j(t, "DIV", {
                     class: !0
                 });
                 var Z = W(S);
-                G.l(Z), P = M(Z), L = j(Z, "DIV", {
+                G.l(Z), L = M(Z), P = j(Z, "DIV", {
                     class: !0,
                     style: !0
                 });
-                var Y = W(L);
+                var Y = W(P);
                 $ && $.l(Y), Y.forEach(R), Z.forEach(R), this.h()
             },
             h() {
-                N(a, "class", "pill-var"), N(o, "class", "pill-label"), N(i, "class", "pill-item"), N(A, "class", "pill-var"), N(p, "href", "#teams"), N(m, "class", "pill-label"), N(d, "class", "pill-item"), N(b, "class", "pill-var"), N(C, "class", "pill-label"), N(E, "class", "pill-item"), N(n, "class", "pill-list is-horizontal"), N(L, "class", V = e[7].length ? "button-wrap" : "button-wrap align-center"), Y(L, "padding-bottom", "0"), N(S, "class", "team-status-box well")
+                N(a, "class", "pill-var"), N(o, "class", "pill-label"), N(i, "class", "pill-item"), N(A, "class", "pill-var"), N(p, "href", "#teams"), N(m, "class", "pill-label"), N(d, "class", "pill-item"), N(b, "class", "pill-var"), N(C, "class", "pill-label"), N(E, "class", "pill-item"), N(n, "class", "pill-list is-horizontal"), N(P, "class", V = e[7].length ? "button-wrap" : "button-wrap align-center"), Y(P, "padding-bottom", "0"), N(S, "class", "team-status-box well")
             },
             m(e, t) {
-                k(e, n, t), x(n, i), x(i, a), x(a, r), x(i, l), x(i, o), x(o, s), x(o, c), x(n, u), x(n, d), x(d, A), x(A, f), x(d, h), x(d, m), x(m, p), x(p, g), x(p, v), x(n, y), x(n, E), x(E, b), x(b, I), x(E, w), x(E, C), Q.m(C, null), k(e, B, t), k(e, S, t), G.m(S, null), x(S, P), x(S, L), $ && $.m(L, null)
+                k(e, n, t), x(n, i), x(i, a), x(a, r), x(i, l), x(i, o), x(o, s), x(o, c), x(n, u), x(n, d), x(d, A), x(A, f), x(d, h), x(d, m), x(m, p), x(p, g), x(p, v), x(n, y), x(n, E), x(E, b), x(b, I), x(E, w), x(E, C), Q.m(C, null), k(e, B, t), k(e, S, t), G.m(S, null), x(S, L), x(S, P), $ && $.m(P, null)
             },
             p(e, [t]) {
-                4 & t && K(r, e[2]), 4 & t && X !== (X = 1 != e[2] ? "s" : "") && K(c, X), 128 & t && z !== (z = e[7].length + "") && K(f, z), 128 & t && T !== (T = 1 != e[7].length ? "s" : "") && K(v, T), 16 & t && K(I, e[4]), H === (H = D(e)) && Q ? Q.p(e, t) : (Q.d(1), Q = H(e), Q && (Q.c(), Q.m(C, null))), Z === (Z = J(e)) && G ? G.p(e, t) : (G.d(1), G = Z(e), G && (G.c(), G.m(S, P))), e[5] ? $ ? $.p(e, t) : ($ = pn(e), $.c(), $.m(L, null)) : $ && ($.d(1), $ = null), 128 & t && V !== (V = e[7].length ? "button-wrap" : "button-wrap align-center") && N(L, "class", V)
+                4 & t && K(r, e[2]), 4 & t && X !== (X = 1 != e[2] ? "s" : "") && K(c, X), 128 & t && U !== (U = e[7].length + "") && K(f, U), 128 & t && z !== (z = 1 != e[7].length ? "s" : "") && K(v, z), 16 & t && K(I, e[4]), H === (H = D(e)) && Q ? Q.p(e, t) : (Q.d(1), Q = H(e), Q && (Q.c(), Q.m(C, null))), Z === (Z = J(e)) && G ? G.p(e, t) : (G.d(1), G = Z(e), G && (G.c(), G.m(S, L))), e[5] ? $ ? $.p(e, t) : ($ = bn(e), $.c(), $.m(P, null)) : $ && ($.d(1), $ = null), 128 & t && V !== (V = e[7].length ? "button-wrap" : "button-wrap align-center") && N(P, "class", V)
             },
             i: t,
             o: t,
             d(e) {
                 e && R(n), Q.d(), e && R(B), e && R(S), G.d(), $ && $.d()
             }
         }
     }
 
-    function yn(e, n, i) {
+    function Cn(e, n, i) {
         let a, r, l = t,
             o = () => (l(), l = u(d, (e => i(10, r = e))), d);
         e.$$.on_destroy.push((() => l()));
         let {
             showAutoBalance: s
         } = n, {
             unassigned: c
@@ -2841,38 +2974,38 @@
         } = n, {
             currentSession: f
         } = n, {
             allowCreate: h = !0
         } = n, {
             downloadPlayersUrl: m
         } = n;
-        const p = ue();
+        const p = de();
         return e.$$set = e => {
             "showAutoBalance" in e && i(1, s = e.showAutoBalance), "unassigned" in e && i(2, c = e.unassigned), "data" in e && o(i(3, d = e.data)), "inactive" in e && i(4, A = e.inactive), "currentSession" in e && i(0, f = e.currentSession), "allowCreate" in e && i(5, h = e.allowCreate), "downloadPlayersUrl" in e && i(6, m = e.downloadPlayersUrl)
         }, e.$$.update = () => {
             1024 & e.$$.dirty && i(7, a = r.teams)
         }, [f, s, c, d, A, h, m, a, p, e => r.sessions.length <= 1 ? null : r.sessions.find((t => t.id === e)), r, e => {
             e.session && f && i(0, f = e.session)
         }, () => p("clickCreateTeam"), () => p("openAutoBalance")]
     }
-    class En extends Ze {
+    class Bn extends Ye {
         constructor(e) {
-            super(), Ke(this, e, yn, vn, s, {
+            super(), Ze(this, e, Cn, wn, s, {
                 showAutoBalance: 1,
                 unassigned: 2,
                 data: 3,
                 inactive: 4,
                 currentSession: 0,
                 allowCreate: 5,
                 downloadPlayersUrl: 6
             })
         }
     }
 
-    function bn(e) {
+    function Sn(e) {
         let n, i, a, r, l, o, s, c, u;
         return {
             c() {
                 n = O("p"), i = F("Choose\n    "), a = O("button"), r = X("svg"), l = X("path"), o = F("\n      Auto Balance"), s = F("\n    to randomly distribute players into teams."), this.h()
             },
             l(e) {
                 n = j(e, "P", {});
@@ -2893,24 +3026,24 @@
                     fill: !0
                 }, 1), W(l).forEach(R), u.forEach(R), o = q(c, "\n      Auto Balance"), c.forEach(R), s = q(t, "\n    to randomly distribute players into teams."), t.forEach(R), this.h()
             },
             h() {
                 N(l, "d", "M18.857 0H3.143A3.143 3.143 0 000 3.143v15.714A3.143 3.143 0 003.143 22h15.714A3.143 3.143 0 0022 18.857V3.143A3.143 3.143 0 0018.857 0zm0 9.429h-6.286V3.143h6.286v6.286zM3.143 3.143h6.286v6.286H3.143V3.143zm0 15.714v-6.286h6.286v6.286H3.143zm9.428 0v-6.286h6.286v6.286h-6.286z"), N(l, "fill", "#0C66B8"), N(r, "fill", "none"), N(r, "class", "icon"), N(r, "xmlns", "http://www.w3.org/2000/svg"), N(r, "viewBox", "0 0 22 22"), N(a, "class", "button no-border strong theme-info-color inline-help-button")
             },
             m(t, d) {
-                k(t, n, d), x(n, i), x(n, a), x(a, r), x(r, l), x(a, o), x(n, s), c || (u = T(a, "click", e[2]), c = !0)
+                k(t, n, d), x(n, i), x(n, a), x(a, r), x(r, l), x(a, o), x(n, s), c || (u = z(a, "click", e[2]), c = !0)
             },
             p: t,
             d(e) {
                 e && R(n), c = !1, u()
             }
         }
     }
 
-    function In(e) {
+    function Ln(e) {
         let t;
         return {
             c() {
                 t = F("Option 2: ")
             },
             l(e) {
                 t = q(e, "Option 2: ")
@@ -2920,20 +3053,20 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function wn(e) {
-        let n, i, a, r, l, o, s, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, P, L, V, z, D, H, Q, J, K, Z, Y, G, $, _, ee, te, ne, ie, ae, re, le, oe, se = e[0] && bn(e),
-            ce = e[0] && In();
+    function Pn(e) {
+        let n, i, a, r, l, o, s, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, L, P, V, U, D, H, Q, J, K, Z, Y, G, $, _, ee, te, ne, ie, ae, re, le, oe, se = e[0] && Sn(e),
+            ce = e[0] && Ln();
         return {
             c() {
-                n = O("div"), se && se.c(), i = U(), a = O("h3"), ce && ce.c(), r = F("Build teams manually"), l = U(), o = O("img"), u = U(), d = O("ol"), A = O("li"), f = F("Select one or more players from the ’Unassigned Players’ list by hovering over their name and clicking the check box."), h = U(), m = O("li"), p = F("Click\n      "), g = O("button"), v = X("svg"), y = X("circle"), E = X("g"), b = X("path"), I = X("defs"), w = X("clipPath"), C = X("rect"), B = F("\n\n        Add Team"), S = F("\n      to start a new team with the selected players, and repeat until all players are assigned."), P = U(), L = O("div"), V = X("svg"), z = X("path"), D = U(), H = O("div"), Q = O("p"), J = F("You may "), K = O("strong"), Z = F("rearrange teams"), Y = F(" as much as you’d like before the game is in play."), G = U(), $ = O("p"), _ = F("All players must be "), ee = O("em"), te = F("assigned"), ne = F(" or marked "), ie = O("em"), ae = F("inactive"), re = F(" before the game can start."), this.h()
+                n = O("div"), se && se.c(), i = T(), a = O("h3"), ce && ce.c(), r = F("Build teams manually"), l = T(), o = O("img"), u = T(), d = O("ol"), A = O("li"), f = F("Select one or more players from the ’Unassigned Players’ list by hovering over their name and clicking the check box."), h = T(), m = O("li"), p = F("Click\n      "), g = O("button"), v = X("svg"), y = X("circle"), E = X("g"), b = X("path"), I = X("defs"), w = X("clipPath"), C = X("rect"), B = F("\n\n        Add Team"), S = F("\n      to start a new team with the selected players, and repeat until all players are assigned."), L = T(), P = O("div"), V = X("svg"), U = X("path"), D = T(), H = O("div"), Q = O("p"), J = F("You may "), K = O("strong"), Z = F("rearrange teams"), Y = F(" as much as you’d like before the game is in play."), G = T(), $ = O("p"), _ = F("All players must be "), ee = O("em"), te = F("assigned"), ne = F(" or marked "), ie = O("em"), ae = F("inactive"), re = F(" before the game can start."), this.h()
             },
             l(e) {
                 n = j(e, "DIV", {});
                 var t = W(n);
                 se && se.l(t), i = M(t), a = j(t, "H3", {
                     class: !0
                 });
@@ -2971,39 +3104,39 @@
                     "clip-path": !0
                 }, 1);
                 var F = W(E);
                 b = j(F, "path", {
                     d: !0,
                     fill: !0
                 }, 1), W(b).forEach(R), F.forEach(R), I = j(X, "defs", {}, 1);
-                var U = W(I);
-                w = j(U, "clipPath", {
+                var T = W(I);
+                w = j(T, "clipPath", {
                     id: !0
                 }, 1);
-                var T = W(w);
-                C = j(T, "rect", {
+                var z = W(w);
+                C = j(z, "rect", {
                     width: !0,
                     height: !0,
                     fill: !0,
                     transform: !0
-                }, 1), W(C).forEach(R), T.forEach(R), U.forEach(R), X.forEach(R), B = q(O, "\n\n        Add Team"), O.forEach(R), S = q(k, "\n      to start a new team with the selected players, and repeat until all players are assigned."), k.forEach(R), c.forEach(R), P = M(t), L = j(t, "DIV", {
+                }, 1), W(C).forEach(R), z.forEach(R), T.forEach(R), X.forEach(R), B = q(O, "\n\n        Add Team"), O.forEach(R), S = q(k, "\n      to start a new team with the selected players, and repeat until all players are assigned."), k.forEach(R), c.forEach(R), L = M(t), P = j(t, "DIV", {
                     class: !0
                 });
-                var N = W(L);
+                var N = W(P);
                 V = j(N, "svg", {
                     class: !0,
                     fill: !0,
                     xmlns: !0,
                     viewBox: !0
                 }, 1);
                 var le = W(V);
-                z = j(le, "path", {
+                U = j(le, "path", {
                     d: !0,
                     fill: !0
-                }, 1), W(z).forEach(R), le.forEach(R), D = M(N), H = j(N, "DIV", {
+                }, 1), W(U).forEach(R), le.forEach(R), D = M(N), H = j(N, "DIV", {
                     class: !0
                 });
                 var oe = W(H);
                 Q = j(oe, "P", {});
                 var ue = W(Q);
                 J = q(ue, "You may "), K = j(ue, "STRONG", {});
                 var de = W(K);
@@ -3013,52 +3146,52 @@
                 var fe = W(ee);
                 te = q(fe, "assigned"), fe.forEach(R), ne = q(Ae, " or marked "), ie = j(Ae, "EM", {});
                 var he = W(ie);
                 ae = q(he, "inactive"), he.forEach(R), re = q(Ae, " before the game can start."), Ae.forEach(R), oe.forEach(R), N.forEach(R), t.forEach(R), this.h()
             },
             h() {
                 var e, t;
-                N(a, "class", "player-help-header"), N(o, "class", "player-help-img"), e = o.src, t = s = "data:image/png;base64,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", c || (c = document.createElement("a")), c.href = t, e !== c.href && N(o, "src", "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAdwAAAFACAYAAAAWB83NAAAK3WlDQ1BJQ0MgUHJvZmlsZQAASImVlwdQU+kWgM+96SGhBRCQEnoTpBNAamgBFKSDqIQkQCgxhICKXVlUcC2oiGBZ0VURBctSxIZYsLAo9r4gi4DyXCzYUPMu8Ai7++a9N+/M/Pd8c+75T/nn/jPnAtBDuWJxJqoMkCWSSiICfZlx8QlMUg8oAA5ogAcql5cj9gkPDwVMxvVf5cM9QEb0beuRWP/+/r+KKl+QwwNAEjFO5ufwsjBuxtYgTyyRAuCOYnaj+VLxCN/BWE2CFYhx3winjvHXEU4eZbzyqE9UBBtjYwAyjcuVpALQbDE7M4+XisWhhWNsK+ILRRgvx9iTl8blY4zlhSlZWfNGeABjc8xfDEBXw5iV/KeYqX+JnyyPz+Wmynmsr1Eh+wlzxJnchf/n0fxvycrMHc9hii1amiQoAtOa2Pk9yJgXImdR8oywcRbyR/1HOS03KHqceTnshHHmc/1C5HszZ4SOc4owgCOPI+VEjbMgxz9ynCXzIuS5UiRsn3HmSiby5mZEy+1pAo48fn5aVOw45wljZoxzTkZkyIQPW26X5EbI6xeIAn0n8gbIe8/K+VO/Qo58rzQtKkjeO3eifoHIZyJmTpy8Nr7Az3/CJ1ruL5b6ynOJM8Pl/oLMQLk9Jy9SvleKfZwTe8PlZ5jODQ4fZwiFQGBCNGSCFCTAhQAQgggEUsEC6Ugz7HnihRJhapqU6YPdOAGTI+LZTGHa29rbAYzc37FP4p3G6L1ENK5N2FZVAXiclMlkpyZswTcBjiUBUOsmbOazAZR7Aa6c5uVK8sZs+JEHAaigBGqgBXpgBOZgDfbgDO7gDf4QDGEQBfEwB3iQBllY5fNhMayAQiiGjbAVymE37IWDcASOQwOchvNwGa7DTbgLj6ETeuAVDMIHGEYQhITQEQaihegjJogVYo+wEE/EHwlFIpB4JAlJRURILrIYWYUUIyVIObIHqUKOISeR88hVpAN5iHQh/chb5AuKQ2moGqqLmqJTURbqg4agUehsNBXNRvPRAnQ9WoZWoofRevQ8eh29i3air9AhHOAUcBo4A5w1joVj48JwCbgUnAS3FFeEK8VV4mpwTbhW3G1cJ24A9xlPxDPwTLw13h0fhI/G8/DZ+KX4dfhy/EF8Pf4i/ja+Cz+I/06gE3QIVgQ3AocQR0glzCcUEkoJ+wl1hEuEu4QewgcikahBNCO6EIOI8cR04iLiOuJOYi2xmdhB7CYOkUgkLZIVyYMURuKSpKRC0nbSYdI50i1SD+kTWYGsT7YnB5ATyCLySnIp+RD5LPkWuZc8TFGmmFDcKGEUPmUhZQNlH6WJcoPSQxmmqlDNqB7UKGo6dQW1jFpDvUR9Qn2noKBgqOCqMFNBqLBcoUzhqMIVhS6FzzRVmiWNTUuk5dLW0w7QmmkPae/odLop3ZueQJfS19Or6Bfoz+ifFBmKNoocRb7iMsUKxXrFW4qvlShKJko+SnOU8pVKlU4o3VAaUKYomyqzlbnKS5UrlE8q31ceUmGo2KmEqWSprFM5pHJVpU+VpGqq6q/KVy1Q3at6QbWbgWMYMdgMHmMVYx/jEqNHjahmpsZRS1crVjui1q42qK6q7qgeo75AvUL9jHqnBk7DVIOjkamxQeO4xj2NL5N0J/lMEkxaO6lm0q1JHzUna3prCjSLNGs172p+0WJq+WtlaG3SatB6qo3XttSeqT1fe5f2Je2ByWqT3SfzJhdNPj75kQ6qY6kTobNIZ69Om86Qrp5uoK5Yd7vuBd0BPQ09b710vS16Z/X69Rn6nvpC/S365/RfMtWZPsxMZhnzInPQQMcgyCDXYI9Bu8GwoZlhtOFKw1rDp0ZUI5ZRitEWoxajQWN94+nGi42rjR+ZUExYJmkm20xaTT6ampnGmq42bTDtM9M045jlm1WbPTGnm3uZZ5tXmt+xIFqwLDIsdlrctEQtnSzTLCssb1ihVs5WQqudVh1TCFNcp4imVE65b02z9rHOs6627rLRsAm1WWnTYPN6qvHUhKmbprZO/W7rZJtpu8/2sZ2qXbDdSrsmu7f2lvY8+wr7Ow50hwCHZQ6NDm8crRwFjrscHzgxnKY7rXZqcfrm7OIsca5x7ncxdkly2eFyn6XGCmetY11xJbj6ui5zPe362c3ZTep23O0Pd2v3DPdD7n3TzKYJpu2b1u1h6MH12OPR6cn0TPL8ybPTy8CL61Xp9dzbyJvvvd+718fCJ93nsM9rX1tfiW+d70e2G3sJu9kP5xfoV+TX7q/qH+1f7v8swDAgNaA6YDDQKXBRYHMQISgkaFPQfY4uh8ep4gwGuwQvCb4YQguJDCkPeR5qGSoJbZqOTg+evnn6kxkmM0QzGsIgjBO2OexpuFl4dvipmcSZ4TMrZr6IsItYHNEayYicG3ko8kOUb9SGqMfR5tG50S0xSjGJMVUxH2P9YktiO+Omxi2Jux6vHS+Mb0wgJcQk7E8YmuU/a+usnkSnxMLEe7PNZi+YfXWO9pzMOWfmKs3lzj2RREiKTTqU9JUbxq3kDiVzknckD/LYvG28V3xv/hZ+v8BDUCLoTfFIKUnpS/VI3Zzan+aVVpo2IGQLy4Vv0oPSd6d/zAjLOJAhy4zNrM0iZyVlnRSpijJEF+fpzVswr0NsJS4Ud2a7ZW/NHpSESPbnIDmzcxqlatig1JZrnvtDbleeZ15F3qf5MfNPLFBZIFrQttBy4dqFvfkB+T8vwi/iLWpZbLB4xeKuJT5L9ixFliYvbVlmtKxgWc/ywOUHV1BXZKz4daXtypKV71fFrmoq0C1YXtD9Q+AP1YWKhZLC+6vdV+9eg18jXNO+1mHt9rXfi/hF14pti0uLv67jrbv2o92PZT/K1qesb9/gvGHXRuJG0cZ7m7w2HSxRKckv6d48fXP9FuaWoi3vt87derXUsXT3Nuq23G2dZaFljduNt2/c/rU8rfxuhW9F7Q6dHWt3fNzJ33lrl/eumt26u4t3f/lJ+NODPYF76itNK0v3Evfm7X2xL2Zf68+sn6v2a+8v3v/tgOhA58GIgxerXKqqDukc2lCNVudW9x9OPHzziN+Rxhrrmj21GrXFR+Fo7tGXx5KO3TsecrzlBOtEzS8mv+yoY9QV1SP1C+sHG9IaOhvjGztOBp9saXJvqjtlc+rAaYPTFWfUz2w4Sz1bcFZ2Lv/cULO4eeB86vnulrktjy/EXbhzcebF9kshl65cDrh8odWn9dwVjyunr7pdPXmNda3huvP1+jantrpfnX6ta3dur7/hcqPxpuvNpo5pHWdved06f9vv9uU7nDvX786423Ev+t6D+4n3Ox/wH/Q9zHz45lHeo+HHy58QnhQ9VX5a+kznWeVvFr/Vdjp3nuny62p7Hvn8cTev+9XvOb9/7Sl4QX9R2qvfW9Vn33e6P6D/5stZL3teiV8NDxT+Q+UfO16bv/7lD+8/2gbjBnveSN7I3q57p/XuwHvH9y1D4UPPPmR9GP5Y9Enr08HPrM+tX2K/9A7P/0r6WvbN4lvT95DvT2RZMpmYK+GOjgI4bKEpKQBvD2DzcTwAA5shqLPG5utRQcb+CUYJ/hOPzeCj4gxQg6mR0YjdDHAUW6bLAZS8AUbGoihvQB0c5OtfkpPiYD8Wi4ZNl4RPMtk7XQBSE8A3iUw2vFMm+7YPK/YhQHP22Fw/InrYP8YsKdAoax65tcHfZWzm/1OPf9cwUoEj/F3/E9T/HtBz9KX+AAAAimVYSWZNTQAqAAAACAAEARoABQAAAAEAAAA+ARsABQAAAAEAAABGASgAAwAAAAEAAgAAh2kABAAAAAEAAABOAAAAAAAAAJAAAAABAAAAkAAAAAEAA5KGAAcAAAASAAAAeKACAAQAAAABAAAB3KADAAQAAAABAAABQAAAAABBU0NJSQAAAFNjcmVlbnNob3Q3DfkqAAAACXBIWXMAABYlAAAWJQFJUiTwAAAB1mlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPHg6eG1wbWV0YSB4bWxuczp4PSJhZG9iZTpuczptZXRhLyIgeDp4bXB0az0iWE1QIENvcmUgNi4wLjAiPgogICA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPgogICAgICA8cmRmOkRlc2NyaXB0aW9uIHJkZjphYm91dD0iIgogICAgICAgICAgICB4bWxuczpleGlmPSJodHRwOi8vbnMuYWRvYmUuY29tL2V4aWYvMS4wLyI+CiAgICAgICAgIDxleGlmOlBpeGVsWURpbWVuc2lvbj4zMjA8L2V4aWY6UGl4ZWxZRGltZW5zaW9uPgogICAgICAgICA8ZXhpZjpQaXhlbFhEaW1lbnNpb24+NDc2PC9leGlmOlBpeGVsWERpbWVuc2lvbj4KICAgICAgICAgPGV4aWY6VXNlckNvbW1lbnQ+U2NyZWVuc2hvdDwvZXhpZjpVc2VyQ29tbWVudD4KICAgICAgPC9yZGY6RGVzY3JpcHRpb24+CiAgIDwvcmRmOlJERj4KPC94OnhtcG1ldGE+CnRq2CEAAAAcaURPVAAAAAIAAAAAAAAAoAAAACgAAACgAAAAoAAAMevKJG8/AAAxt0lEQVR4AeydB3wURRvG3xB6DV2KSC/SpIaigH70pnSQGhAIIF2KAtKlFykSmqH3KkV6FRABaaJU6b0kdEgIfPMu7mZ3c3e5snu5C8/4w92ZnZ3yv80+OzPvzPiEPn76hqw6H6tXbF3w9fUh3zhxlCjhryLojY1clIgGnSB/8Mfzh78/+XWC9w/ev+7UnziK/r0VvVcq/fORBTeury/FjetLcXycE1n54ebbfXRpcGXfuKnGyB/88fxp/4bx94f3D96/7mnxWdafNxTx+g2x8Po8fPLsTcL48ShOHO0fqSygjh59iBU36l1u+8GRP/jj+YvyB4i/Pze9cPH+wfvHxvvH52VY+Js4qu7fKH+pDgZYayG/IfGfG5555G/h1xa/Ifjj+cPfn4MvMyei4/2D94+lx0Z+//qI8Q1DZJAx67vy9BnLmerDjfAjf/DH82f5ZSf/feHvz7yPLrx/8P6x5/3jI/qVjRHct0+c/Ldt9Sh1bRmSozYLadhYN3asjfHWh/wFfPC39Gi4FIbnT+DD31+0zxDePya8f4T2SJ+aMfX8OZC/z6sI1wXX2rittafP6PEk5C//4taIa8PB39gvDjx/eP4s2a1o/+oiffj7e3f//lwSXHu/KiIfNdWZGFByFTvyFzzt+KpTUY88BX88f5FPg1Nn+PsT2PD359SzwwY9rrz/pWePc44h/s7m7xPxWtgrO1FzZ+up/3WkrJG/Hku0fvCPFpFdEfD8CUz4+7PrWVFHwt+fmobz5+/a35/Paxbc/1y0lReyrii7fJOBR+QvYCq/hgWw4I/nz8JjYVQQ/v7w9+ex75//hCfG9Meg/DWCa9QfLtIBARAAARAAARDQEhCC647ZedpM4QMBEAABEACBd42Aj7CYUzox0aUkfn6FhoVHAV266NK18FgYFYS/P/z94f1j468pFrx/NYJro6q4BAIgAAIgAAIg4AIBCK4L8HArCIAACIAACNhLAIJrLynEAwEQAAEQAAEXCEBwXYCHW0EABEAABEDAXgJeJbg3Tp+i2+fP0r0rlyj0+jV6cv8uPQ0NobBnzygiPFyqs2+8eBQ/cWJK4peSkqZOS36ZMlOaLFkpfc7clDFvfnu5IB4IgAAIgAAIGErAowU39OZ1OndgH106cpCunjxGEWFhLlXeN358er/gR5S1mD/lKl2W/DJkcik93AwCIAACIAAC9hLwSME9sXkDndqxma4dP2pvPZyKl7lwEcr/WRUqVKWGU/fjJhAAARAAARCwl4DHCC53Cx9atZSOrl9Fz0ND7S2/IfES+flRkZp1qUTdRlJ3tCGJIhEQAAEQAAEQUBHwCMH9fekCOrhsAYU9faoqmvtP4ydJQv4Nm1GpRs3cnzlyBAEQAAEQiNUEYlRwzx/cT3uDg+jepYseBTlN1mz0SUAg5fQv41HlQmFAAARAAAS8l0CMCe7WnybQsV9WeTS5j2rXpUodu3t0GVE4EAABEAAB7yDgdsG9feEcbZo4ku6cO+sVhNLlyk1Vu/Wl9DlyeUV5UUgQAAEQAAHPJOBWwT3z2y7aMHqoy9N73I2SpxPV6D2A8nxcwd1ZIz8QAAEQAIFYQsBtgnt0/WraNmW8V2Or+HUPYc1cx6vrgMKDAAiAAAjEDAG3CO6hVcto14zJMVNDg3Ot0K6zmD7U0OBUkRwIgAAIgEBsJ2C64MaGlq3+IUBLV08EfhAAARAAgegImCq4PGb7y7AB0ZXBK6/X7j8UY7pe+cuh0CAAAiAQMwRME1y2Rl7YPdDrDKTs/RnYkKrphCBYL9sLDPFAAARA4B0nYJrgzu3cxmum/jj7DPCUoZaTZzt7O+4DARAAARB4hwiYIrjesKiFUb8xFscwiiTSAQEQAIHYTcBwweXlGlcP7BO7qelqV2fwKCwDqWMCLwiAAAiAgJaA4YIbHNjC49ZG1lbZeB+vvRwQNM/4hJEiCIAACIBArCFgqODyrj97g6fHGjiOVOSTgPbYZcgRYIgLAiAAAu8YAcMEl/eznda8boxvsRdTvx9v7ddh/irspxtTPwDyBQEQAAEPJ2CY4O5bEEz7F/zs4dU1t3hlmrWmss0CzM0EqYMACIAACHglAcMEd0rjWvQ8NNQrIRhV6ER+fvT1knVGJYd0QAAEQAAEYhEBQwT3xOYNtHnCyFiExfmqVOnelwpVqeF8ArgTBEAABEAgVhIwRHAX9+lC144fjZWAHK1U5sJFqMmoSY7ehvggAAIgAAKxnIDLght68zrNDGgcyzE5Vr22wUvIL0Mmx25CbBAAARAAgVhNwGXBNWPrvaRp01Jusdl7tmL+QrgyUuLkfpRAWAGHv3xJzx+G0qO7t+nfw7/Tmd076eGtG1F+oOL1G1Ou0p9ECZcD3rx+TS+fPqUH167Q/auX6cLBfYaOP3vLFn6hDx/R4ydPZCyUPl1aih8vnuK39+TR48eUPFkye6Mjnh0Enj1/TgnEet2+vr52xEYUEAABbyDgsuAu79eTLh35w7C6lm3RhvwbNiXfuNG/+F+FhdH+xfPo4OK5mvwrd+lFhavX1oTZ8kSEh9Ff27fQ/oU/05O7d21Fteta1mIlqcHwcXbFNSLSmzdv6MrVa3Tm7Hk69c9p+vv0GQoNfUi5c+agD/PlpXx5c1O+PLkpUaKEmuwG/zCa1vyyQQkLnjmVPipYQPFHd3L12nVqHdiZ7t27L9JORFMmjKaiHxWK7jaXru/d9ztt37XbYhrx4sallClTUq4c2Sn/h3kpY4b3LMbz5MCw8HAK7NyDjh47IRWzV/fO9GWj+p5cZJQNBEDATgIuC+742v8zZEeg9LnzUPUe31GarNntLHpktFvnz9Cv40bQvYsXpEBHBVdOKeJVOC3t242u//X2ZSeHO3rknYR6/LLd0ducin/+34vUs+8AunLlqs3744syDRv4HVX636dKPFcFt8s3fWnvbweU9N57Lz39umaZ4jfjZNLU6RQ8f5FdSfuXKEbdOnegvLlz2RXfEyItWb6aRo2bqCnKjk1rKaWwgIcDARDwbgIuCe6N06doYbdAlwnkr1ydqnbtTXFc6D5Tr+HsrOByRR7fu0uz2zWl8GfPXapX04lBlDFvfpfSsHXzq1evKGjWHJo9Z76taFGulS3tTyOGfE/JkiUlVwW3QdMAOn/hXyUPFvWDe7YqfjNOHBFcOf/RwweLD40KstejjxMmT6N5C5doyrhq6XzK9kEWTRg8IAAC3kfAJcE9un41bZsy3qVa89zVtrMXizHapFHS4S7jm2f+ptv/nqcHVy5TvMSJKFWmLJS7bDlKlCy5Ej/sxXOa16kNhVx/28qzJLiHVi2lf3Ztlbqqk6ZOS6nez0KFqtaiFOnSK+nIJ4fXrqCd036UvU4dK37dg4rUrOPUvfbc1Kl7L9p/wHJXPgtfqlQp6cGDEAoTDNWOr/26dhmlEl2vrgruLCH2U4NmKclXFq3nUcMHKX4zTvSCy13ZhQsVIB6Xvy/qy13r+jrzOOja5QspU8YMZhTJ0DSPnzxFrdp2VNLkLvKt61diLFchghMQ8F4CLgmuEdvw1R06hnKUKBWFIHcTrx8xWBFRfYTSTVtRyfpfUvyECWmjmAN8astGJYolwV0/Zhj9s32zEkc+qTdsLGUv7i97pePVv47Tkm++1oQ56jFz276t23dS736DohSpa6dAqlmtMqVJk1q5dk60QKfN/Jl27torhU0Y/QNVKFdWOndVcHnseM26jXT4yFHKmycXNWlYj+KKcVQznV5wq1WpSD8MHqBk+VoI72oxLj1s5FgljE/atm5JHdu11oR5qufwn8do/cZNlCJFCmrRtDGlFh9PcCAAAt5PwCXBddVgKt//qlDNXv2jUDwpxHPT+BFRwi0FcKtX3/3riOBaWh3qhbC6ndyguqXs7A4zy3Dq4aNHVLlmPU0rjgV2xtSJNrsdz567QE/FetdFChdU6uCq4CoJufEkOsGVizJ6/CRavGyl7KUypUvS1AljFD9OQAAEQMDdBFwSXFe34ms9Yz6lzpJVU+dHd+/Q9Ob1NGGOehwRXE6784qNlDBp5LSW1xERNK5GBUez1cQ3a8u+UUJIlqiEhDOdO2saFSrwoSZ/ezyWBDc8LJzWbdhEx06cpBCxVGf2bFnp4zKlqHULYTmuG2M/fPQ4Bc2YrWTF1rSfVSgn+XlaS5ceb/dFTp48GQ3s14eSiqldy1f9QvsPHlSscIsULkT16tSm8h+XUdKxdWKv4O7as4+69/5OSSpLlvdp7bIFil8+YWvuFWt+kSy72cr79u07lDZtGsovrLu/Cmhu0eBq6IgxdFkYqSVNmpR69+hCiRMnpumz59CuPb/REzHNqox/SapVsxp9LMbL2V29foPmzFso6n2IHoqpWJx+PtEj0KFta/pAlEvtHj9+oil30Y8KU8f2bZQoy1auoS3bdpBPnDhUrXJFqvt5Tbp0+SqtFHXYsGkrvX4dQVUr/Y/6ftNNuYdP2JJ89boNdPLU3/TP6bPStaxiXLhQgfzUqlkTaUxffQM/G1dF97w9rl0b0dtUvKg9UREHBKIQ4Gf+zLnzlEHMKsgUzcwCs+JGKZRJAS4JrivrJ/NcW95dR+/WDv+ezu7dqQ92yO+I4HILueuKTdILTM4k5MZ1mtW6sex16mip5exUQrqbGrf4Skz/OaeEVq74GY0aNlDxO3KiF9zcuXIQt4QtOX45L/g5iJII0ZQdv+D7Dxome6lzh7bUumUzyc9zc8tXqqlcY9HYtmOX1fQDvwqg9l+1UuJbO7FXcFeuWafpVrbUwuU43BLWj/mq8+7ZtRM1a9JQHUTVvmhIt27dlsLez5yJ7t1/QM/FB4be/Th2pDAEjEPdvvmWIsRHnCU35ochVPGz8solTqtSjcix/2JFCtOsaZErl6l/Mx7fnSVsDRoK4zV1+nprcR6C6D/4B6v15HH9UcMGKUMNXJgqtevTnTv2TZEb8v13VKt6FaUOOAEBewksXLKcxk6cokSvUO5jmjB6uOJXn7gad8iAb6N8WKrTd8e5S4LrypSgDytVoxo9I1sgXFkjunI5HUcE97OO3ahYbW2L+vwf+2n1929bZ5yeM86sqUHFy36meblOmTiGypYq6UwRoxhNRZcICw8LkOwcEVz5HlvHn34cS6X9S9iKQvYILltw1xLj+7IocoId2gYQt8RkN3naTPp5btQWr3xdfVy+aA7lzJ5NCVILrhJo4YSFjIVQLYb6aBxn5+ZfKLEw/mLniOBy/BQpkkutZj6X3acVPqHxI99+CK1Y/QsNHzVOvmTzuEb0AMgtbkcEd9zIoUrPhs0McBEEVAR27t5LPfpEHVJs36YVBYq/V7U7JOxE2nXS9trwdUficg8cz2uPSeeS4I6pJroPheGMM65k42ZUvlV7za3XxTSjRQZMM7JHcLll+2nbztJGA9w9p3bLvutBl/88pA5y/NzHh3r9usfx+2zccefuPapSS/txsHndSkonuiidcerWknx/yRLFqP4XtSmeWHFq8fKV9MehI/Il6Xhk/06K8x8vRwWXu6TbtGouFscoLLW2howYLXV1yhnwAh2L5syUvRaPtgSXW9Wn/j4ttVovXb6i3M/57t6yTtM65y7hLxq+bY2z6LVp2ZRKia7gmzdv0c/zFmha4jyVihf1kJ1ecPn+7p07UrasH9D6XzcJg6eoxnmNG9aTuoB/23eA5oppP+pW9Xe9e1KDurWl5B0VXLlMfORu8wcPHkhl4a5m7i6vKFrLasH//rvekmGdj3g+t+3YLVq+w5Xrav5HxHDB06fP1MlL5zt276G1wlBOdtyaXr9ycZThBvk6jiBgjcCYCZNp0dIVUS7nzpWTls6PHKriCEbE5S7rjauXRsnPnQExJrjlv+oorIybaOr617ZN9OtYy90JmojReCwJ7tMH9+nB9WsUJ15cSpE2PSVNJSx5xUtH7y4c+p1WDeilD3bcb4Lg7vv9D/q6m7ZsR3/f7XjZ/rtDL7jcAuSWoOzYCrlU+coacVi/aokyvcYRwWVRmiNWsuIVr2SnFxcO/3XtcnovfTo5SpSjXnA5gjy2rBYW9Y3jRw2nT8t/rA6Szs+ev0CXLl2hsmX8KYkYh5Udj3dWqllX9kqrV+34dY3i1wuumglH4ns5DdmVEq32aaL1Ljt9HRo3qEt9enaVLuuZ2OpSltPj7vrmovchobDYVzv9eD+L8IBvtc/PgsXLaNyPU5Xbdm9db3WZzpuiG71WvSaKQDP31WKOMHerw4GAowSsiWiunDlomW5vdSPi6odaHC2vEfFdElxXupQLVatNVbpq//iPbVxLWydFvpicraAlwbUnLcPEVmRmRpfyqX/OULOAdpqqHNi1OcqLVhPBhkcvuJaWduzTbxBtEWOAsps2eTyVEq1gdo4IboH8+Wj+7CA5GeXYXixjqG5Fs7V1iWJFlOv6E71Y6a+r/fwHNlSMLxYv+pE62K5zvaj+eWCX+D57+4Gmv6b/6GGjqlVr1yv5sJiyqMrur7//oeatIxeMUQuyo4Kr7j6W05eP+vF+HlPOnEk7F/m6aNHLxm183+ygyRaX5+Ru+npfttKsaDZ6+CDNymVyvjiCgD0E0KVsDyVVHFeMpizNU7107AgtF0sruuocFVzeEGHvvFl0fMNaV7NW7jfDaOrFixdUuoLWOGXR3JmaVqNSADtO7BFc/cpHk8aPok+E1TI7IwRX3wrjLs86tWtYLb29gsst6q0bVlltrekzuCWsk68Ja2JeH/r6jZu0YvVazdjo4X07lJZ0dII7M3ge/TQ9skts2KD+VKNqJSXLu/fuSVO75IDi4gNjpvjQYOeo4AbPEOtfi4U/LDn/cpU0vROW4ujD+vXpSfWF1bje6T8i6n1Ri/r3/UYfDX4QcIiA3hCqvFgjYKJYK8CSczXu0AHfebfRlCvTgjIVKERfjo3symLAD+/cphkt6lti7VCYJcF9Lb7Q34j/LG2K8ECsULWoZ0dDdwwya1pQhSq1NEKgHv9zCJKI7AmCO2P2HLEwR7BSdL1xk3LhvxO94HJXMTPgMdnOYhqS2lo4Z47s0liQPOasT4unGPB46tr1GzVdwPp47PdYwbWy4QR3r7OBnaNuUP++9LmY0qR2W7btpD79BylBbLG+fGGw6YucKBniJFYT4L/D02LmRUaxEpw904LMiOsuwC51Kbuy8AUbLXVbtUVTT16eb3bbZlZXl9JEtuGxJLjySlMZPyxA9YaM1sy75aSMWF1KXSSzFr5o1a4THT/xl5IVW6luWb/KqW31PEFwR46dSEtXrFbqw/N1v6hlfdERveCqV5o6IOa5duyqbXV1CvyKvhKGWnrHBmjc5RoSEqK/ZNHvbYLLlfikYnUxL/ipUp+gyROUc0snvmIKE7eW1auFcYu/TqPmmnHbdcJIKoPorocDARBwjIBLguvq0o4dF62hJGy8pHIXxVZ/K8SWf644W4LL6fJmCdV7fBslix0zp9CRlcZYsVnqMo+SoRMBGzdvo34Dh2ru5LmvPAfWlnv+/IWwPI6reZl6guC2Fab+vDSk7CyNI8vX+GhLcPl63wGDafPWHXyquBWL5lKO7FkVP5/op73wPN06tWpSEbG9YKqUfhTYpadmbNkbBVf/cfbb9o0aS20NEAse3iqQxfaG6GKXHY8Dl/u4tOzFEQRAwAECLgmuq5sXVBWiV1CIn96tGvQtXfj9N32w3f7oBJcTqi/2q80m9q1Vu/CXL2hux9Yut7A5TTM3L9Abw3B+3A34be8e0qbl7Fc7Xvjg2++HipWRkogu1p+ljeb5ekwL7m2xsEJVscCC2tmykuV40Qnu06dPhZVwPU3XMlvRsjWtbM2snhLEaVavUomGD9bOB9Qbc3mj4OrHx/XzqLnusgsX4spTwdSu38BhtHHzViXI1v1KJJyAAAhYJeCS4Lq6PR93KwfOXUkJkyXTFJB3CdozZzodWbVME672FBY78ZRr2VZsp3eHtkweSzf+juxmtUdweaWr1tPnU4LESdTJ0g2xO9HCrtr5wZoIdnrM3J6P98BtICxG9Y67l8uIRTB4ub5kginvnMPLAKrnpPK6y7xzDi+04E7B5bLyXNUWTRtJxWbjoLYdu2rKxisu8cpLtlx0gsv36pd15DCe//u16F5mx5sDcN6y43FgnjokO0u9CN4ouDyNp7pYFUvteAqRvEwnT/viqWaTf5ouzTtmPsyJ3Toxl/j7IZHGK3nEnsKL5sxQ5mCr08Q5CICAfQRcElzOwpWpQXx/0ToN6H/tu/BpFHf5+J90dt9uuikWxHhw7Yq0hV+WwsWocLValDl/ISU+r1DFRk/3r1ySwuwRXI7Iol1ZbKOnd3vmzqKDi+fqg+32mzElSJ85r6k7YoztMTn9Pez/XIyPDhDWpdzac7fgcv6cb/LkyS2OnW5YvZQyisnptpw9gsv39+jTj3bu1vaSLBaW6LwZPW8AUaFyLU02vMUfGwPx+Lj6A0WO5I2Cy2Xn/ZKnqLZQlOvDH2c8vqufu7xUzH/MkD49fVq1dpRr8r3648ol8yi7WPQDDgRAwDYBlwXXFcMpuWgtfwqmdNlzyl6njuo9bO0VXM6o8ZjJ9H5B7TzNiPAwmtelHd27eMGpsphlMKUvzL8XL1Hnnn01Y2z6OLKfhY7XvK0utrOTXUwIrpy3+shlGzFkgF1zOu0V3FCxSQCvyqVe0SldurTSqkjcdWpJkNVlYotJ9diltwoub1fISzuq5wWr66k+b1jvC2nTA96TN0AY59nr5os1tgt8mM/e6IgHAu8sAZcF95Do9t01Y7JLALlruUavAZSr9CdOpXPp6GFa/m135V5HBDfFexmpVdAcsa9uIuV+Prl94ZzY1L61JsxeT4V2nalEXW1Xnr33OhqPFyRYtHQlHTx8WOwCcy5Ky5Hno/7v03KSpW72bFk1yY8a9yMtWb5KCVsQPEPskpNH8fMJzyfleaWyY0tX/xJFJe/W7bvEvrwD5UtineWvxUL/DSS/fvMCnqJTuGB+af9cuVXFQsvLCfLqR7nF6jL2uOmz5lDQrMhpRGorZf39v4tlKXv07qcZz+U9cXlvXN6qkC2k9csw8mIZ3b/uIK1MVbtBU2U9ZvWSlrXFOs1svcuO68BirHZz5i+mH6cGKUGjhw8WHxMVFL+tebj61rd6UQxOwJ7fTMlIdfLnsRPSkpfnxf7IMn++zOVnQzHeuaioOLKztMCKdMHK/yC4VsAgGAR0BFwW3NCb12lmQGNdss55C1SpIXUvx1cts2crpYhX4XR49XLaM3uaJpojgss3FhPi+JkQSb3bL6xb94luSEdd2+Al5JchZpa7423xuOWbSHxA8Mbl3HUor5DkaD1cia8XXPVKUzfE6kYvXr6U9u+NibKp68WWuDzW/fJlmGRMliZ1KvXlWHnOY7sPQkLJTzwbPL3H2jzlWFl5VAoEYpCAy4LLZV/cpwtdOx45tcOV+rAxU8n6TSl7cX9KmSmzxaQeXL1MvAwjrwwVIhat0LuyLdpQGZ1RkTwPVx9X9lfu2ps+/KwSxUsQuR7ty2dPaVLdqnIUu46ZCxehJqMm2RU3NkeyJbixud6oGwiAAAhYI2CI4J7YvIE2TxhpLQ+nw7mrOXma9JQkdRp6HfGKnt6/T09C7lH4s+dOp2n2jVW695V2IDI7H09PH4Lr6b8QygcCIOBuAoYILhfalXWV3V1ps/IzY/1ks8pqdroQXLMJI30QAAFvI2CY4O5bEEz7xZSCd9mVadaayjYLeJcRKHXnsVFe2zhCGHWxK1a0iGbrPyUiTkAABEDgHSFgmOCGCavPac3rUphY6edddPGTJKEO88WaxnYafL2LjFBnEAABEHiXCRgmuAzx96ULaG/w9HeS5ycB7alUo2bvZN1RaRAAARAAgegJGCq4nJ0rW/ZFX1zPjGHWVnyeWVuUCgRAAARAwBkChgvu+YP7afXAPs6UxWvvqTN4FOX0L+O15UfBQQAEQAAEzCdguOBykV3dts/8ahuXg1nb8BlXQqQEAiAAAiDgCQRMEVyu2NzObejOubOeUEfTypAuV25qOXm2aekjYRAAARAAgdhDwDTB5bWIF3YPpAix1V5sdLwjUNMJQZQ+R67YWD3UCQRAAARAwGACpgkul/PMb7vol2EDDC6yZyRXu/9QyvNxBc8oDEoBAiAAAiDg8QRMFVyu/dH1q2nblPEeD8KRAlYUe+gWEXvpwoEACIAACICAvQRMF1wuiBFb+NlbIbPjuXPrPbPrgvRBAARAAATcR8AtgsvViQ0tXbRs3fdgIicQAAEQiG0E3Ca4DI7HdDeMHup1hlRsIFWj9wCM2ca2px/1AQEQAAE3EnCr4HK92Hp508SRXjNliKf+VO3WF9bIbnwokRUIgAAIxEYCbhdcGaI3LI6BRS3kXwtHEAABEAABVwnEmOBywXkZyL3BQXTv0kVX62Ho/bw28icBgViu0VCqSAwEQAAE3m0CMSq4MnreZejgsgUxvrUfb7Hn37AZdv2RfxgcQQAEQAAEDCPgEYLLteH9dA+tWiqsmVfR89BQwypoT0KJ/PzEvNq6VKJuI+xnaw8wxAEBEAABEHCYgMcIrrrkJzZvoFM7NtO140fVwYafZy5chPJ/VoUKValheNpIEARAAARAAATUBDxScOUCht68TucO7KNLRw7S1ZPHXJ5OxNN73i/4EWUt5k+5SpclvwyZ5KxwBAEQAAEQAAFTCXi04OprfuP0Kbp9/izdu3KJQq9foyf379LT0BCpOzoiPFyK7hsvntQtnMQvJSVNnZb8MmWmNFmyUvqcuSlj3vz6JOEHARAAARAAAbcQ8CrBdQsRZAICIAACIAACJhCA4JoAFUmCAAiAAAiAgJ4ABFdPBH4QAAEQAAEQMIEABNcEqEgSBEAABEAABPQEILh6IvCDAAiAAAiAgAkEILgmQEWSIAACIAACIKAnAMHVE4EfBEAABEAABEwgAME1ASqSBAEQAAEQAAE9AQiungj8IAACIAACIGACAQiuCVCRJAiAAAiAAAjoCUBw9UTgBwEQAAEQAAETCEBwTYCKJEEABEAABEBATwCCqycCPwiAAAiAAAiYQACCawJUJAkCIAACIAACegIQXD0R+EEABEAABEDABAIQXBOgIkkQAAEQAAEQ0BPwuXUv5I0+EH4QAAEQAAEQAAFjCUBwjeWJ1EAABEAABEDAIgGfu6HP0MK1iAaBIAACIAACIGAcAQiucSyREgiAAAiAAAhYJQDBtYoGF0AABEAABEDAOAIQXONYIiUQAAEQAAEQsEoAgmsVDS6AAAiAAAiAgHEEILjGsURKIAACIAACIGCVAATXKhpcAAEQAAEQAAHjCEBwjWOJlEAABEAABEDAKgEIrlU0uAACIAACIAACxhGA4BrHEimBAAiAAAiAgFUCEFyraHABBEAABEAABIwjAME1jiVSAgEQAAEQAAGrBCC4VtHgAgiAAAiAAAgYRwCCaxxLpAQCIAACIAACVgl4jeBGvHlDD5+8oqcvX9GzsAh6Lv69DI+gVxFvKCziNYW/ervpUby4PhTfNw7F9fWhhPF8KVF8X0rM/xLEJb+kcSmOj49VGLgAAiAAAiAAAmYR8GjBffQ8gu49ekn3H7+kkKfhhjBIlTQepU6agNKmSEBJE/oakiYSAQEQAAEQAIHoCHic4L4If003HrygW6HP6cmLiOjK79L1ZEJwM6RMJP1LEA8tX5dg4mYQAAEQAAGbBDxGcEOehNOlu0/p7qMwmwU24yJLbTrR4s2aLgmlSBzXjCyQJgiAAAiAwDtOIMYF974Q2LM3H9Njk1uz9v7OLLh5MiYnvyQQXnuZIR4IgAAIgED0BGJMcMOEkdOZ64/pZuiL6EsZAzEyp05EuTMmpbhx0NUcA/iRJQiAAAjEOgIxIri3Q1/SqasP6dVrz+YZX1g8F8riR6mSxfPsgqJ0IAACIAACHk/ArYIrZvbQP9ef0LX7zzwejLqA2dMnoZzvJVEH4RwEQAAEQAAEHCLgNsF9KZqzR/8NIZ7q442OpxMVzupH8cT8XjgQAAEQAAEQcJSAWwSXF6k4eO4B8bitNzuet1s8RyrirmY4EAABEAABEHCEgOmC+/jFKzp0PkRaEcqRgnlq3ITx4lDJXKnEKlZxPLWIKBcIgAAIgIAHEjBVcEOfvqLDF0LoNQ/exiLHLdySOVOJ5SKxUlUs+llRFRAAARAwlYBpgstjtX+IbuTYJrbyr8GiWyp3arR0ZSA4ggAIgAAI2CRgiuByN/If50Io4nXsatnqSXK3sn/uVJQgLrqX9WzgBwEQAAEQ0BIwXHBZZH/75z6xVfK74HhlKn8xpgsHAiAAAiAAArYIGC64xy6G0p0YWA/ZViXNvpY9XWLKmSGp2dkgfRAAARAAAS8mYKjgXr3/nP659tiLcThf9BI5UlJKMVcXDgRAAARAAAQsETBMcMPFRvB7/r4X68dtLUHkMN7o/uN8qQkzdK0RQjgIgAAIvNsEDBPcv648ohshnrkRgbt+4jxis4MP0iZ2V3bIBwRAAARAwIsIGCK4T4RV8v4zD7yo2uYU1VfsLFTuwzRY/tEcvEgVBEAABLyagCGCyytJhTwN92oQRhX+gzSJKE+mZEYlh3RAAARAAARiCQGXBffhs1fSOsmxhIfL1Yjj40Pl86OV6zJIJAACIAACsYyAy4LLSzc+eILWrfq5yCrGcXnzejgQAAEQAAEQkAm4JLi8otQBjN3KLJUjj+V+Klq5ccQRDgRAAARAAASYgEuCe1psJn/lnvGbyRf6IAWlTp7ALb/Q/Ucv6cTlh4bnVTBLcsqQMqHh6SJBEAABEAAB7yTgkuDuPHWXwk3Y4/bTgumEWCVyC9GbIc9p58k7hueVOll8Kpbdz/B0kSAIgAAIgIB3EnBacO8+fElHLxnfMmSMZghu0MxgOnz0GA0e8C1lyvCe8muZJbicQYX8abFZvUIaJyAAAiDwbhNwWnD/Fks4XhNLOZrhjBbc02fPU5MWbZSiBn4VQO2/aiX5zRTcAu8np4ypPLtb+fnz5xQSGqqw8UuRghInxuIdChDdycuXL+n+g8g552nTCIv0eFjSU4dJ8ep5JUuWjJIldb9B4eMnT2IkXwUETkBAEHBacPeKHYGeh0WYAtFowW3YrDWdO39BU9bcuXJKrd0UaTOZ0qXMmWXwS0gFP0iuydcsz/UbN2jxkqWa5FsHtKJUKVNqwvSebdt30KjRo5Xg1gEB1KRxI8WPEy2Bffv306DBQ5TAFi2aU/OmTRV/TJ6wuAXNmEHh4a+sFiNdurSUM0cOypUzJ6VNm9ZqPKMu/HHoEPXrP0BJrn69etS+XVvFb/YJ/1306PkNPRAfSYkSJaLhw4ZSwQIFzM4W6YOARQJOCS5vvbf71D2LCRoRaKTgclfy9NlzLBYrSZIkFDxnLh26aLzhF2fIm9Rzt7I73I+TJ9P69Rs0WTUTQtBSCIItB8G1RSfqNb3gftmkCQW0ahk1YgyE3L5zh5o1b2F3zr6+vlSxYkXq1CFQEiO7b3QgYkwLbv/vB9LBgweVEqdLl44Wzp+n+HECAu4k4JTg3hRrJp8Uayeb5YwSXH1Xsr6833T7mj6rUtO0Fi7nx0s98kb1ZrpXr17R53XqUlhYmCab5MmT04plS8lHLMZhzUFwrZGxHB6bBFeuIX949undi0qXKiUHGXaMacFtF9iBLl68qNQnfvz4tGHdL4ofJyDgTgJOCe65m0/o4h1zWoVceaME11JXsgy3aJHCNHvaJDJzDJfzKpbNT0xxii9na8pxx86dNGLkKItpjxo5gooWKWLxGgdCcK2isXjB2wQ3e/bsSj0iIiLo5s2bUT7M5AhNm35JrVrY30KW77N1jGnBXbh4Mc0RvViyK1euHA3o953sxREE3ErAKcE9JqyT7wgrZbOcEYK7cMlyGjtxisUi8hf90gU/S9bKZgtu3kxJKUsac42QOnXuQmfPnrVYV39/fxo2ZLDFaxwIwbWKxuIFbxPcrZs3RanH/fv3aeeu3TRdjPfqXdBPUymHGOM1ysW04L5584Y2bd5Cx44fp5w5c1Cdzz+nuHHjGlU9pAMCDhFwSnD3n7lPT16YYzDFpXdVcK/fvEWNm7ehJ8Iy0ZLjruSmjRtIl8wW3MypE9OHmc2zyrx16xY1b9lKqSa3aB49ekT37kWOsa9cvoy4e9mSg+BaomI9LDYIrly7a9euU89evSSDIjksY8aMFDx7llglzZhhkJgWXLleOIKAJxBwSnB3/HWXXokN581yrgpumw5d6M+jxy0WL5f4yl0mWreyM1tw04ru5CKiW9ksN33GTFqxcqWSfGBge0lwFy1arIR91aYNNWr49gNDCfzvxF7B5XHiDRt/pVN//01nzpyRPmbee+890WrISfXqfEFZsmSRUnz27BkNGjKEuPuSHRvmsOVz3jx5JL/8P05v4qTJoovzhhTk4xNHdPX1oxQpIj8MHj58ROs3bqBz587RhQv/0t27dyl16tSUO3duaiqMlbjFoncTJv5I165fI+7F6NihA/G0nXXr19PmLVtEXrekKTxc5sqVKtKnFSrob1f8vwtDG24FnjhxgkJCQqT6FStaVGr9qa26rRlNsVXsr5s20z+nT0vl54Tff/99ypcvLzVq0ICS6qbG8PSs/t9/L+WfKFFi6tPrG6kO27ZvF70Q2+nUqb+JP6YC27ej/B9+qJRTfWLJaMpSC1d9z4mTJ6nnN73UQdSpU0f6onZtKWzFylV04PcDyvXeQqDTC8MjtVu/YaNgtVMK4t+Ryy5bQFsS3ObNmtLqtWvp5Mm/6LTgk0JMRStYsCDVr1eXsn7wgTppzfmly5dpy9atdP78ebp8+Yp07QMRP3euXFS1ShXKnDmTJj57Tpw4SXNVRlJ1vviCPi5bVhPvgfh9Fy1eIj3XV69epQQJEki/c968eYjjx8Q0Jk0BY7mHG0YX/v2X0qdPT++Jf7acWXFt5WnkNacEd/vJuxTx2jMF11ZXMoNbPG825c2dU2FotuCmSByX/HOlUvIz8uT169f0Rd16xC9r2XFr9pnwN2/RUg6iNEJ0Fi9coPjVJ/YI7r/C6GSAsPa8I6xgrTn1+N+kKVNp3bp1SlQ/Pz9atGC+Zr4qW4cvEuNrsitZsiQNHzpE9gpx30g/TQuyOt7IEdu3aye9pJWbxElTYaUrlzOXeBE/fCiGP6yUu1KlStT7m57q24m7IH8KCqI1a9Zqwq15LAnu7j17aPSYsVbLzoY7/b77lsqULq0ky/NE69arr/h7C9H6UyzUsm3bNiWMTwZ+PyCKYMgRnBFcvrfvd/3oyJEjcjJUtmwZGvSf+A/7YQTt3r1buTY9aBplz5ZN8fOJ3kJ+3NgxVEgIKDu94BYQU3KuXLkifRRKEVT/44+zwYMGkr94FtSOP97mzp9Pi4Uo2nIBAa2oSaNGGiPB6J7vXaJuI0eNVj4Q9enzb9VLPCMVypfXX4LfAAIrV6+ioKDIoY3SpcvQkEFvPzz1ybsat/c3PaJ86OrzMNvvlOBuPXFHvJjMK5qlFu7jx2LiejLbXbPRdSW3b9OKAtsGaAputuCyhTJbKpvh9h84QAMHRY7PFinyEY0eOVLKqn2HjvSv+GqU3cQJ4y22jKJ7IXGrom279nIyNo89e3SXWhpsLc3d3NzKk11D0cJuK1ra7PiF26ZtO/mSNCVloRBkuSUxOziYlujmFCuRdSczpwdR1qxZlVC14CqBNk5+GD6MShQvrsSY8tM0WitaX/Y6veBya+/HSZPsuj149mylVaYXXJ4zqv6QkhOcOyeYMmbIIHs1R2cFl1uNY8aOU9JST50xWnCVTGycLF+6hPgjTXZDh/9Ae8RHjD2uRo3q1K1LFyWqref7hjAga93mK6tiKycCQyuZhLHHffv3iTntQ6Mkyj0gLZprpzPyGHyv3n1ciltH9MR1DAyMkoY7A5wS3C3Hrbd0jCi8XnB5ek/bjl2Jx14/r1nNahaOdCXLiZgtuLw/bsVCaeXsDD3y+Bt3mcmuv+iSLV/uE8m7bsMGmiS6bGVn7aVh64XE93bo1El04V2Qk6HatWtRQMuWUnfnGWGoxYIvCyu3BpYsWig+jJLRadHt3LlLV+U+Ppk9c4bUrcofA+qpGiN+GE7FixVT4vLYYsB/4sxpNhYLcRQvWoxu3b5FS5Yu03xIlChRgn4QixnIzpLg1qpVS7QmS9Ht27el+3ncW3b58uWjSRMnSN579+5TE90iFtwK5u547mbk8dugoOnyrdJRLbjcBd5IdHXL3ekcoXu3blL3NZ/v2fubaPmOUa5zC/ynKW9/I73gcnzZsfjIhj7cU2Btmpezgmvpt9okuvK5xWmG4LI9wZdNGktDA2w1PX7CRIUJ17lunTrUQQyNsLP0ouXelI/LlKXXryOkbn/1kArfM23qVGW4wdbzrbdgriK6pXneekrB+8+jR6WhmgcPQmic+M3UQx2cB5zrBLgnafXqNVESyp49B02fNlUTbkRc7rJeMG+uJl13e5wSXHe2cLllW71OI8UA6stG9alX985ROK1d/ysNGva2dRflogjQdyXLccwWXJ4CW6mQdsxLztuVI1uaNv4ycoUjfjmu/2Wt8mLmsVSemys7vr5q5QpKLFpOamfrhXTwjz+o/4DI7h11y0dOg8deAoWAym5A/35U7pO3oq8fX+YxyGpVq9BU0YqUXdWqValn926yVzlyNza3hLmrWV1mFvdGTb5U4rEYcYtIdnrBVXdvchx9i53HetesWindPlG0TDeIFqrs1F2rctimzZtp3Pi3As1hasHVt46rV6smBFf70cFjomrrYP5NuGVvSXBTpUpFo0eNpA/+Gx+Xy2Dt6KzgWsp7/tw5xGP0RgsuP0NTJv1IKVUroB3845B4zgYo1eKPLHmubIBogV67dk259rX4APxcfPSp3fyFC2nevPlKUP78+Wni+LctdlvPN9sa7Nu3X7nPVu+BEgknhhGwJqLZsmWnGUE/afIxIq6l95cmEzd4/g8AAP//JUJyMgAAMvxJREFU7Z0HfBRV18ZPGgmEkgQIRaUGBBUsCBZe5RULSO+9CkpHpClVpEkR6UWkSq+CUv0UBQV9KYIgRaoFCJAGJCEJad89E2cyM9md3ezOpPFcfjAzt89/l33mnnvuHY+w2/dSKZNh3++3KCk5k4Uykf2VasFUKjA/RUfHUM++79L5Cxc1pRs3rE/DBg2gQoUKSvGcr0HzthQTE6PJJ1/06tGNer/dXb7UHEOj4uj7U7c0cWZeeHt5UN0niptZpVTXii++oDVr1ir1vv766zR86BDlmk9Gjh5DR44cUeL69etLzZo0Ua755Nvv9tHUadOUuLe6d6f27dpK10uXL6f16zcoaa1atqT69esp1/JJr959KDk57QvRoUN76t61q5SUlJREXbu/Rbdu2eYbFBREq1auoHz58slVOXXs2LmLps5v9uwmDw8Pqaw+7f/27slQZ8vWbeju3btK/N7du8jT05PeEfdx5coVJX7RwgVUsUIF5ZpPDh46ROM+Gq/EdWgv7rdb2v326dePLl68pKRNGP8RlSpVSrnmkxs3btLoMWOUuE9nfELVnniCosV3t0XLVko8nyxetIjKly8nzpwLNwXnToKNOti6f3U6n18PDaWu3bT/P7Zs2kiFCxemiZM/pv379ytFPlu0kCqUL69c88nsuXNpx46dStyMT6ZT9WrVpOvD4vs3SnwP5cDfoV7vvC1fSsfU1FRqLu49NjZWid/x1Xby8fGhem82UOL4e7L9y63k7e2txPHJvbg4atqsuRLH+XZ+/ZV0bfT9nr9wIW3btl0px9/HPr170X9q187QhpIJJ6YROHjooPi/NCFDfZ07daQunTtr4k/89hsNG/6+Jo4vMpO3efNm1Ld37wx1ZGWEhyuCe+BMOMUnpljWT1lwx4yfTDt27bXZTuVKIbRkwWxJdAcNH0n7Dxy0ma9kyRK0cdUyRZz1mawWXD8fT3r5sWL6Zt265h+oVm3aakRj9qyZ9FjVqpp6f/7lFxr74TglrnTp0rRy+TLlmk+MfpBGjBpNR48e1eR3dFG79os0buxYJdulS5eod99+yrX6ZP7cOVS5cmV1lM3zsLAwSRSuXw+l0BuhtHPnLs2979m1k7y8vKSyzgiuXlh379wh/cA2bNyE7t+/r/RBLeRypJHg6svLZYyO7w4cSI0aNsgguFWqVKG5s2cZFc2Q5qrg/vK//9GYsR8q9eXPn5++2valdJ0VgssN6R9Wlny+WHoIeqtHT6Vf/F3h74ytoP/ct27eJP7PFzL8fh8/foKGf/BBhur4u/T8889RCyHi1aunPThkyIQIUwhsEQ9QixYtVup64YUXaPy49O+ikiBO3M3LA5KCBdMGaep6s/LcJcE9eC6CYhOSLesnC+7hgz/QuIlTDNtgeJ3ataZFS5bbzbd4/iyqWeNpu+lWC25BX296sUqQ3fZdSTh67BiNGDnKlaK0aMF8qlixolLWSHD1wqQUMjipU6cOjR45QpNj4KD36OzZs5o4Hk2sX7tGGZlqEsUFWys2bt5Me/d+Q5GRkfpkzbUZgssj9EZNmir1qkVHiRQn9gSXy9dv0FCd1anzIUMGU/033shWwV2+ciWtXbtO6e/jjz9Osz6dIV1nleAO/2AEHT9+XOnDtClTKD4hXvPA+OKLL9JHH6Y/zCmZxcmAdwfRuXPnlKi5c2ZTlUcfNRRczrzws8W0detWpZz+pGbNmpIA6EfV+ny4dp0A/1+/KB7MS5YsSSVLlDCsyKq8ho2amOiS4B69FEWRMYkmdkNblTzCnT5zLq3dsFmbmImrDm1b0bD3BhiWsFpwixbKRzUqBBj2IbOJo8aMpcOHD2e2mJS/Xr16NHTwe0pZI8EdP3ES/fjjj0reYeIJsXgxY/N4BWGCLVKksFLmt5Mnaeiw4cq1+qTXO+9Qq5Yt1FHSeXh4hDTiuX37doY0WxFmCC6Pat6o/6ZSPV9zvfpgT3A5X7MWLTVmURYNo+Dp5UmPP/aYNLrWm5SzaoTL7bZr30Ezsm/WrCn169NH6npWCW6vPn3p8uXLCq6lYoSbIKwNffv1V+J4tDlj+nTlWn3yVs+36Z9//lGi1q5eRcWLF3couFyAzZWrxfTMb+JoKzRt2pT6903jYSsdcSDgLAGXBPfM1Wi6GhHnbBuZzicLLhfcvmO3w5GurQYcmZLlMlYLbpmiBajKw+aZMe7cuSvMyW3k7mf6yELC5kJ53tRIcNeIUc8KMfqRwzgxuqgtRhnOhoSEBOrQqbPG/Ksuy31ZIUzc+qfa9h07UXh4uJL12WefpTfF3DHPdQYEBND7I3g0dEJJN0NweQSjn9tlTjzSVQcjwR00eAidPn1ayc7zjQUKFFCujU6yS3A/mfEp7f3mG03XVq5YTqX/nXue9PEU+uGHH5R0HvnyCFgdzJjDbdq8BcWJuVg5sJlfb3Vgq8iGdel+C3JenmJh64Q8HaB+WDL6fsvl5SOPng6IB0z+3qv9Dvg7t2nDejkbjiDgMgGXBPevsHv0x3XbDkou90RVUC24HH3u/EXq2WegZvSgym7z1JEpWS5kteBWfaggPVLMuR9duU9Gx/UbN9LSpenzsOWFA8vC+fOMikiipzbLymZMLmT0g6Sf2+O2PhOORLKDkrpRdpDSm91mzp5Du3btUrK1aNGC4sWP6q7du5U4/Uju6tVr1L1HDyW9bt26NOJ97QiZ592sENy+/QfQhQsXlLYHvTuQGjZId9rhBL0jmdppat6ChbR9e7oTTksxeu8tRvG2gp5XVgsuO41NnjKVjonpCXVQO81x/OIlS2jTpnQrUzvhUNdDONapw4RJk+nAgQNKlJHTlC0mh37+mT4c95FSXi1w+ocg2clMySxOfjp4kD4aP0GJevjhh2n50iXStdH3WymgO2Gh7yKcyGTRVQu4LisuQSBTBFwS3Ii79+nYFefMfZnqzb+Z9YLL0Sy6Y4UT1QWVF6i9up0xJctlrRbcmhUDKbCgj9yc28e2wvynFs8B/ftTk8aNDOv9YvVqWrVqtZKHzb4snByMfpBSUlKoc9duyg8P52enqMGDBkkerHx95cqftHLVF3Tw4CHJweQT4fHMgnzq999p8JChnEUK/CPKZr5EIcxswlSPZtTCpjdB6+ftvtu3j6ZMnSZXKx3NGuHqH2bYCjB92lTJGY0dkjZt3qIRVG5cLbi2nJa6CY/tdm3bSE5dPBI7IpzQli5bLplPu3fvRh3atZPuwSrBHaWaT+fP88+//qLz5y/QqVOnlBGh1AHxDwvVsiWfax6o9uzdSzM+nSlnkT73sWNG05PVq1NkVBQtEnOg33//vZLOJ0aCy+L1kXCKea5WLanMRfH/efDQoZrvQ2/hKdyyeXMpfeu2bbRw4SLpnP/x9/eXPpNKISFSHFsUeP5XHt1y5AfiAe1V8aDGwej7HRERQfyQVLZsGWrburVizeCHIf7ey1aWsmXL0pLFn0n14R8QcIeAS4KbLH44vjsZ5k67hmVtCS4X4OU/PcRI10h0+T/k7m0b7Xol6xu2UnA9RGOvVQ8WP2D6Vl275h8XNluqgzNmyzBhnu0gzLTqsEyMAB4RP7BGP0ic/+zZczRQCKw+MOfExETNDx3n4R/LRmJU2KlLV1LPwfLcm+zxqRdN/hFmMWaTYXR0NLVo1VrTHJswWQzOnDmjmaeTM5kluPHx8ZJZWf3jLbdh76gWXM6zdv16Wr58RYbsvMSGl73w6Ekd5GU2Vgmuui2jc7Y0jB09Spr3VOfjkXCbdu0z9Js/M/29yOWMBFfOww8zfn5+GaYb+Hu1eeMGxVrCDyk8P3v16lW5qHSUp0T0n5Xek9no+z1k2DA6efKUVB/fT40aNSQv1l9//VXz3e3apQt16thB0z4uQMAVAi4JLjf0y/lIuhuX5EqbDsvYE1y5oNFyoU+nTqRX6rwkZ3V4tFJwA/19qGZIoMM+OJtBb7pjD8rJE9NNaUb16M2lTcV63P5iXa7RD5Jc305hFp47b77dH1g5X0hIRZo+dSotW7GSvv76azmaXnvtNXp/WPpolxP6DRgoRlrnlTxPP/0UyU5GH4p1rofEeld7gb0Zb9y4oSSbJbhcof5hQGnk3xN+aJB/pDlKL7g8ipw9Z67GbK6vQ75u3LgxDRCfAVsEsktwWWgGDhhADd6sL3crw3HDxk20ZOnSDPFyBFsvNA9XButw5TK2jiy2bCHh75E68DphXt72lxidG4VKlSoJj+JxVKxYUSWbve83CzWPYtXWIqWQ6oT7smDePM2oX5WMUxDIFAGXBfdCaAxduXUvU405m9mR4HI9a9Zvok9maecuGzWoRxPGjnS2GSmflYIbUsKfKpT0z1R/7GXmH/IGjRorosfOPDPFpgnqJT72ynI8m2pHinW18oiAf9y2bd0i1i//SBMnTVKK9u71DrUUc636wGthZwkhYVOk2hzM+djk1qZ1K3rt1Vfpb+Ep+vY7vZTiLI48iiugcz7iH9HewjNVXdck8fBQSzxE8EYGLPDffvutUg+fBAcH09s9e0gbE6g31JA3ruA8HH/9+nU+lcy4LMb6oBd7tWBzXhbUqWJELs/hcRyPUDt37iRtHKJ2NNILLuflwCb1BWJjBTa5q0eCLHBPCOevrl06S05gablJ4tBEtXmDkUeuXEZ/tGXS1ufhkWG5cuXoUbFkJkQsD3vxheclRzR9Pv01P4jwg4T685KZvCEeqPoPfFexPtgb4fK983dh+YoV0hSE3AZ/l5966kka8t57wsO9iBytOfJId6OYS96xc6fmYYsz8fry5sKzupnwJtYHo+83O/V9KUzW27/6WjEfy+X5/0enjh2lernfCCBgBgGXBfd2bBIdvmi8PtLVDjojuFz3kWPHpTW4bGquK0a19naTMuqHlYL7wqNBVMjP26j5XJnGZkYeYeYXHrjBYumFr6+vJffBJutr165JDwnFRDtBgeZZC5zpMIsLLzUJCiqqGTU5U1adh4WbR4AsUPzQwLta5dbA9xEaeoOCigZRCXEvrgZ+qAoVD128lj6z9fDDJ38veK7m4YceMmX0yd7//FApqpQEXO+d7up9ohwIqAm4LLhcyf7T4ZSQlKKuz5RzZwXXjMasElx/Xy+qXSXdtGVGX1EHCIAACIBA7iXgluBevBFLl2/Gmn73eUFwK5cqSOWCzVsOZDpkVAgCIAACIJClBNwS3Htie8efxDaPZoe8ILh1HhOmVh+T3JPNBoz6QAAEQAAEspyAW4LLvT1+OYrCos3d5rFEgB/55csaR4X4+8l083a8qeBLB/rRE2XStzc0tXJUBgIgAAIgkCsJuC24d+OSxRIh80e5uZLmv51+qWpRyp9FDwy5mRP6DgIgAAIPEgG3BZdhHbt8myKi7z9I3Ozeaykxuq2G0a1dPkgAARAAgQeVgCmCGx2fRD//Yc0Sodz0wfCSgpeqFiN+By4CCIAACIAACKgJmCK4XOGZf8QbhCLT3/ahbuRBOa8gNroIMWmjiweFGe4TBEAABB4UAqYJbmJyKh04E07JKakPCjvNfebz9iD2TOZRLgIIgAAIgAAI6AmYJrhcMb8jl9+V+yCGZ8oHULHC+R7EW8c9gwAIgAAIOEHAVMHl9k78eYdu3Ulwoum8k6WMeN9tFfHeWwQQAAEQAAEQsEfAdMFlk/JBsRlGfKL5Wz7au4nsjC/k50XPVS5KnjAlZ+fHgLZBAARAIMcTMF1w+Y7v3EuiIxejKEW84SMvBx8xb/t8JV5zC6/kvPw5495AAARAwAwClggudyyvi26a2AZhgwszvoWoAwRAAAQeAAKWCS6zi4pJlDbFyGsjXRbbWiFBxG8EQgABEAABEAABZwhYKrjcAR7pHr0UlWeWC/GmFrUqBWFzC2e+XcgDAiAAAiCgELBccLmlGLET1REhuolJuXtOl0e0z1YMwluAlK8PTkAABEAABJwlkCWCy52Ju59Cx69ECfFNdrZvOSpfUEEferJcAPl4wR05R30w6AwIgAAI5BICWSa4zIOdln//+y6Fmvw6PKtZVxTbNVYU2zYigAAIgAAIgICrBLJUcOVO8o5U567F5PhlQ77enuLNP0UoqJCP3HUcQQAEQAAEQMAlAtkiuNzThMRUOn31DoXfzZmv9XtE7B5VubQ/eWFzZJe+WCgEAiAAAiCgJZBtgit34+btBLpwI4buJeSMud1Afx8htIWoSAFvuYs4ggAIgAAIgIDbBLJdcOU7iBAj3SthsRQp1u5mdWA3qJIBflQ22J8K58fa2qzmj/ZAAARA4EEgkGMEV4Z9734yXY+Mp9CoOMmzWY634sjiWiowv/SXX6+HAAIgAAIgAAJWEchxgqu+0duxSRQRnUDh4i9voOFu4BcMBAiTcbFCvhRcxJcKYKcod5GiPAiAAAiAgJMEcrTgqu8hSbyF6I4wN8ckJImRbzLFieN98dJ7fvF9YnKKsqkGj1R9vDzJW6yXzZ/PS/nr7+tNgWItLQIIgAAIgAAIZAeBXCO42QEHbYIACIAACICAWQQguGaRRD0gAAIgAAIgYEAAgmsAB0kgAAIgAAIgYBYBCK5ZJFEPCIAACIAACBgQgOAawEESCIAACIAACJhFAIJrFknUAwIgAAIgAAIGBCC4BnCQBAIgAAIgAAJmEYDgmkUS9YAACIAACICAAQEIrgEcJIEACIAACICAWQQguGaRRD0gAAIgAAIgYEAAgmsAB0kgAAIgAAIgYBYBCK5ZJFEPCIAACIAACBgQgOAawEESCIAACIAACJhFAIJrFknUAwIgAAIgAAIGBDxuhEelGqQjCQRAAARAAARAwAQCEFwTIKIKEAABEAABEHBEACZlR4SQDgIgAAIgAAImEIDgmgARVYAACIAACICAIwIQXEeEkA4CIAACIAACJhCA4JoAEVWAAAiAAAiAgCMCEFxHhJAOAiAAAiAAAiYQgOCaABFVgAAIgAAIgIAjAhBcR4SQDgIgAAIgAAImEIDgmgARVYAACIAACICAIwIQXEeEkA4CIAACIAACJhCA4JoAEVWAAAiAAAiAgCMCEFxHhJAOAiAAAiAAAiYQgOCaABFVgAAIgAAIgIAjAhBcR4SQDgIgAAIgAAImEIDgmgARVYAACIAACICAIwK5RnCTU1PpTkwSxSYk0b37yRQn/iYkJlNScirdT06hxKS01/r6eHtQPi9P8vbyID8fL8qfz4sK8F9fbwoo6E2eHh6OmCAdBEAABEAABEwnkKMF925cMoXfTaCI6ASKik005eaDCvpQ0YK+VLyILxX08zKlTlQCAiAAAiAAAo4I5DjBjU9MoeuR8XTjdhzFxCc76r9b6YWE4JYKzC/99fXByNctmCgMAiAAAiBgSCDHCG5UTCL9GRZLYXfvG3bYikSW2mAx4i0X7E9FCnhb0QTqBAEQAAEQeMAJZLvgRgiBPR8aTdEWj2ad/ZxZcB8tXZgC/CG8zjJDPhAAARAAAccEsk1w7wsnpz+uRVPo7XjHvcyGHA8XzU+VSxckb0+YmrMBP5oEARAAgTxHIFsE9+btBDr9zx1KSsnZPPMJj+fqZQIoqJBPzu4oegcCIAACIJDjCWSp4IqVPXT2WgxdjbiX48GoO1ihhD+FlPRXR+EcBEAABEAABDJFIMsEN0EMZ49fjiJe6pMbAy8nerJcAPmI9b0IIAACIAACIJBZAlkiuLxJxf8uRBLP2+bmwOt2n60YRGxqRgABEAABEACBzBCwXHCj45PoyMUoaUeozHQsp+b18/GkWpWCxC5Wnjm1i+gXCIAACIBADiRgqeDejk2io5eiKIUnb/NQ4BFurZAgsV0kdqrKQx8rbgUEQAAELCVgmeDyXO1hYUbOa2Irfxosus9XLoqRrgwERxAAARAAAUMClggum5EPX4ii5JS8NbLVk2Sz8nOVg8jXG+ZlPRtcgwAIgAAIaAmYLrgssj+djSD2Sn4QAu9M9ZyY00UAARAAARAAASMCpgvuiSu36VY27IdsdJNWp1UILkAhpQpa3QzqBwEQAAEQyMUETBXcfyLi6OzV6FyMw/Wu16wYSIFirS4CCIAACIAACNgiYJrgJooXwR84E57n521tQeQ4ftH9f6oWJazQtUcI8SAAAiDwYBMwTXB///suXY/KmS8iyKqP+FHxsoOyxQtkVXNoBwRAAARAIBcRMEVwY4RX8qE/InPRbVvTVS/xZqGXHyuG7R+twYtaQQAEQCBXEzBFcHknqajYxFwNwqzOly2Wnx59qJBZ1aEeEAABEACBPELAbcG9cy9J2ic5j/Bw+zY8PTyozuMY5boNEhWAAAiAQB4j4Lbg8taNkTEY3aq/F+XEPC6/vB4BBEAABEAABGQCbgku7yj1M+ZuZZbKkedyXxGjXE9xRAABEAABEAABJuCW4J4TL5P/O9z8l8lXL1uEihb2zZJPKOJuAp38647pbVUrU5hKBfqZXi8qBAEQAAEQyJ0E3BLc70+HUaIF77h9pVqwEKv8WUI0NCqOvj91y/S2ihbKRzUqBJheLyoEARAAARDInQRcFtywOwl0/E/zR4aM0QrBXfT5cjp6/AR9NGYEPVSqpPJpWSW43MB/Hy+Ol9UrpHECAiAAAg82AZcF94zYwvGq2MrRimC24J47f5Had+mhdLV3z+7Uq2c36dpKwX3ikcJUOghmZQU8TtwmcPfuXYqJjZXq8fT0pJIlSih1pqSk0I2bN5Xr/H5+FBgYqFzjBARAIHsJuCy4P4o3AsXdT7ak92YLbptOb9GFi5c0fa1cKUQa7RYp/pAlJmVurFSAH1UrW1jTrrsXCQkJtGjxYkpMTJKq8i9QgDp36kgFC2bOKzouLo5WrlpFMTFpP95c2Vvdu1EQfqDd/Yjo2vXrtG79Bk09ZrGdPXcu7dixU6l79qyZ9FjVqtJ1ZFQUtW3XXkmrXr0azZg+XbnGCQiAQPYScElw+dV7+0+HW9ZzMwWXTcmfLV1hs6/+/v60fMVKOnLFfMcvbpBfUs9mZTPDzVu3qFPnLpoq673xBg0dMlgT5+hi4WeLaevWrZpsSz5fTGXLlNHE4SLzBPSiyDV06tiRunbpnPnKdCX0dc/4ZDpVr1ZNygXB1cHCJQjkMAIuCW6o2DP5lNg72apgluDqTcn6/g4d1J/q1mtk2QiX2+OtHvlF9WYFW4LLda9csZxKlyrlVDORkZHUtn2HDHkhuBmQZDoiKSmJmjZvQffv39eULVy4MG3euIE8xMYo7gQIrjv0UBYEspeAS4J7ITSGrtyyZlTIOMwSXFumZBn3M08/SUsXziEr53C5rRrlA8QSp3xys24f7QlurVq1aNKE8U7VP3XadPr2u+8y5IXgZkCS6Yh9339PH0+ZarPc1Ckf0zNPP20zzdlICK6zpJAPBHIeAZcE94TwTr4lvJStCmYI7pr1m+iTWfNsdpFNyRtWL5O8la0W3CoPFaQyxcx7g5A9weUbnT93DlWuXNnmPcuRV69eo+490h3I5Hg+QnDVNFw77zdgIJ0/f95m4eeee44mjv/IZpqzkRBcZ0khHwjkPAIuCe6hPyIoJt4ahylG5K7gXgu9Qe069xAOQTE2ibMpuWO71lKa1YL7cNEC9NjDmXNostnpfyONBJfFlkXXKIwcPYaOHDliMwsE1yYWpyNv3LhBnbt2U/JXqFCB2Ks4PDzd32HLpo3E5mVXAwTXVXIoBwLZT8Alwd33exgliRfOWxXcFdwefQbSr8d/s9m9SiEVaaMY3crBasEtLszJTwuzslnBSHC5jY8nT6Jna9Sw2RyPvHgEZi/YEtzk5GTas3cv/X76DF26dImuXbtGfmK5SaVKlah+vTfov3XqZKjuq6930P4D+8V8pSfVfeW/1ODNN+mfq1dp565d9N13+4iXr/z3v3VoQL9+mrJhQpi++eb/6Oy5c3ThwgXi+dDy5cuLUXslerNePXrkkUek/PeEh/XYD8dRamqKdP3UU09RZ+GUpA48hzpi1Cgl6plnnqGO7dM9eDmBnYzWrltPf/zxB/3zzz/k6+tLFStWpCpVHqXmzZpRoUx6fn+2+HPavGWL0mbv3r0kwV27dp0S11NYF9q2SXvYUyJ1J6mpqbT9q6/oyNFjdPr0aYlXuXLl6PXXX5M+g507dyklXHGaYq47d+2m02fOSPfOD6YlS5akkJAQatm8GZWx4Tg3c9ZsunrtKnl5eVF38VBRtWoVOvHbb7Rr9x765ZdfpOVHbdu0EZ91faVvOAEBZwjw9+/S5ctUQixxUy9zs1XWqry22rIiziXB/e5UGCWn5EzBNTIlM8B1XyylKpVDFJZWC26RAt70XKUgpT13T/SCy6NatQmzdOnStGLZUpvOOXpzJ4smC5sc9IJ76vffafLHUzQjNDmvfHzxxRdp3NgxmvZmzJxFe/bskbIEBASIpSnT6J3efYjFWw7BwcG0ZtUX8iXt+/4HmiaWsKjzKIn/nrBYtWndisIjIqhDx05K8tNiXnSamB9VB1721KRZcyWK73XBvLnK9Q/799OUqdPstpcvXz4aNnSIzQcKpRLVCT9ENGvRkrhdOfBolh8OOnfpKkdRsWLFaN2a1cq1/iRa/PiMHDWazomHDmdCZgX38pUrNGbsh3RLeLvbCx07dqBuXbSe8B2FZ7xcpm7dulTz2Wdp6rRpmioaNGhA771r/4FOkxkXICAIbPlyKy1atFhh8cILL9L4cWOVa/WJu3mHDx2c6eWT6vbNOHdJcP/v5C0xujCjedt12BrhRkfHUKFCxqZZR6bkXj26Ue+3u2satVpw2UOZPZXNCnrBbdasKfG87NGjR5UmPnh/OL0qfhTV4eixYzRiZPqIr0qVKvT000/ROjHCk4NacI+fOEHD3/9ATjI89uvXl5o1aaLkUQsuR7IJlU2r6lC7Ngt12n+sbWI0N3/+AnWy3fNlSz4nv/z53RLc66Gh9FaPnnbFVm785ZdfpjGjRsqXhsdDP/9MH45Ln59lttOmTJHK9OrTly6LJ3g5zJr5KT3+2GPypeb4Vs+3pdG2JtLgIjOC++dff9Hb7/QyqC09acjg94QFo54SoRZcfhjRe2FzxncHDqRGDRsoZXACAkYEDh46SOM+mpAhC+8r0KVzZ008W1OGDX9fE8cXmcnbXFhv+vbunaGOrIxwSXC/+c3+07EZndcLLi/vebvvu8Rzr00bvWm3icyYkuVKrBZcfj/ua9XNW4trS3CbNm6icYRigduwbi15e3vLt0ldu79F18WGDHLgud6fDh2yK7hsduQfWV5CxIHX+r722qviQSuVdgiT5oEDB+SqiH+Ad379lXKtF1wlQZw8/PDDFCVMue+83VMyNfOIrp1YoqT+AX/yySfFutUO0jKni8KMvWLlF3RFjMw6d+5EXTp1IjY9uzPCXbNuHa0Q66/lUE8IC6+RDRSj8V+PH5fMwpGRUdKmEUWKFJazGR6HDBtGJ0+eUvKMFubsOi+/JF1/vXMnzZmTPrq2J+T7D/xIEydNUurgk9693qGX/vMfunfvnhgNbFMsB3KmzAhuH2HCv6jaAKZJk8bCPNyV2InwDzHdwA8M8ufNn+n6tWvEQ24hqSm14Mpt85Hz8aidP9M5s2dRubJl1ck4BwG7BBYsWkRfiu+0PlSoUJE+WzhfE21GXjZZr/4i/f+9poEsunBJcLNyhMsj2wbN2yoOUB3atqJh7w3IgGf7jt00bmLaiCJDoojQm5LlPFYLLi+7fL16sNyc20dbgtuvTx+aOv0T+vbbb5X6+Ye6ZYsW0vX3P/wgmYblxJo1a9LkiRNo2YoVdgWX8/KP769i/+knxY5FxYtrHxpat21Ht2/flqukDevXKbtU2RLcbuKHvVXLFtI8qVJInPCuWVu2bFWieHekT4SpUr9eledu5N203BXccePH08GDh5Q2M7OGWSmkOokQJu52HdLnkHmec8dX25UHHhZLXpsrB07fumUzFRAjdXVghyt2vJLDIGGebSjMtOowYdJkzcOOs4L7v8OHafSYdFOd3qTPbfA8Wm8xGpfDmNGj6OWX0h4abAnuxAkTqFbNZzN8VnJ5HEHAiIA9ES1fvgItXqS1eJmR19Z33qh/VqS5JLj7fr8lnKas6E5anfIIl8W2pxjZnr9wUdNY44b1adigAYqJWS/KmsziwpYpWc5jteB6e3lQ3Se0YiW37crRnuDqdxnikQdvtMBHFgO1OC5fulSMNB9yKLhG/Zs5ew7tEk5QcuAtBFksOegFV20+lvPLR/288pxZsySHHDnd1tFdwZ2/cCFt27ZdqTooKIj6CAen/9SurYikkujEyYovvqA1a9YqOV9//XUaLuZ/1UHvHa43w7NF4c2GjZQi/LltF/NbaisFJ7rqpbx0+XJar9puslXLllS/frrJWG64l2quvUOH9tIImNP0ggvzsUwMR1cJwKTsJLkDZ8IpPjHFydyZzyYL7pjxk2nHrr02K+C9kJcsmC2J7qDhI4VX7EGb+UqWLEEbVy1TxFmfyWrBzYo5XB7hctB7ybLzS7GixWj2nDnKbbPDywgxx8vB0QhXKSROeA722rXrFHojlELFsqufDv6kMU9OnjRRcqThMnrBnfXpDHr88cfV1Snn7GgU++9m/Bz5zZ7dDkdM7grucTFqH/5BxvlpHnk+//xz1EI4W8kPD0pH7Zywib1Vm7aaOWr1/sZysZ+FJy97VsuBndtWLl8mX9Jff/9NPd9+R7nWO3nJCa4K7gjhiKWe55frMzqqH5T0gvt/e9Oc4ozKIw0EHBHI6Aj1gnCa+tBmMXfz8kOwbCWz2UAWRLo0wj14LoJiE6wb4rLgHj74g6GJmNkwvE5iPe2iJcvtolo8fxbVrGF/dx+rBbegrze9WCXIbv8ym2BvhMv1sEdsa/HjL8+H8iiJl/CoHZZ4Xq5o0aJSs44Elz1vdwtvY17mo3b6sdVnQ8G14yTEHsn1GzRUqssvTKxfbftSubZ34q7gcr229pJWt8dmd/6Prx9hqvPwud4ZTZ9udL1owXxpGRLn0QvyCy88L9ofl6G4q4LLXuI8D56ZUEcs+Ro9coRUBIKbGXLImxkCPF3Evhq8NM2ZZUFW5M1Mf93J65LgHr0URZExie60a1hWHuFOnzmX1m7YbJjXKNHefK+6jNWCa/aL6I0El+9rw8ZNtESYjG0F9miWR8OcbiS4bOIcOXo08WjQmeCK4HK9DYXDl/yAwNfOjJzMEFxuiz0fVwtT8G/iaCs0bdqU+vdNsx7YSue4UWJe9LCYH3UlsLPWUOENzIGXYA0eMlSpRu3lrESKE1cFd/zESfTjjz8qVfGSp+LFjKc6eOMO2WkMgqugwwkIuEzAJcG18l24fCey4PK5I2cozmMrODIly2WsFtwyYqepKhbuNKUXURZKNnGqzbR8r2wu3STmdNWbORgJ7iefzqS9YsMLObAJtFWrlsJaUENyoNosHJ3Uwu6q4OqXzKwSXoSOnnLDwyOovWqjC17iNFd4yKqDo3W46rz8hH1AiNEasUGFvNaU03kN8aYN69VZNed37twVrNto4jJzwZ8Jj+jZEqF/iNCbnOV6XRVcvrcVK9M9NMd9OJZqizXUzgYIrrOkkA8E7BNwSXD/CrtHf1y3vW2i/aacT1ELLpfiZUE9xe5RehExqtGRKVkua7XgVhV7KT9i4V7KesHl+9rzzTc0Y8an8i1Kx65iIwNeaqMORoLLm0bImzjwso9VK1dozKv6kbSrgqt/kULjxo1pYH/tDlTcZ36QkM27egcjTudlSSxccggLC6MOnTrLl9LOWOqNL5QE1QmbuLt0666ILgvinl07VTm0p+s3bqSlS9PnYXlXrIXz52kz6a64T/LSG04aIl6rWP+NN6TlVm/U1y5503tPc/8GDR6i2RTDWS/lX/73P2nDC7k73NfPFi6wOV+uZi3nh+DKJHAEAdcJuCS4EXfv07Er6UtCXG/edkm94HIuFt2x4ydneJG8rRqcMSXL5awW3JoVAymwoI/cnNtHRyZlboAdeVg45CUmvM5yo1i2oxYkzmdPcHnutt6b6ctRuPyXYhmLvFSHt3gcMmy45gHIVcG1td1kP2HGbSo20uD2eJ3uZ+LdvXvFQ0SjRg3p3QFpS8Jatm6jmZvmBw/e3pH7ekRsAsI7ZMkPDHyvaickXsYzb8FCKlu2DLVt3Zp47pgDCw0vzZH3Pi4r1pQuWfyZlGbrH37FoVo8B/TvT00ap3sa2yrzxerVtGrVaiWJzbYsfByGioX9avM2t887aAUGBhLvEDVLeIbrd6ByVnD5M+V7U4/g2Slq8KBByt7OV678SSvF7l+8ZEq/PAuCq3xkOAEBlwm4JLjJ4gf9u5NhLjfqqKAtweUyvPyHN7e4oFq8r6+Lf3B3b9to1ytZn99KwRVLcMWmF8FCOPStun7tjOBy7Wx23bZ9u1i+lSSt5XxEbDihD/YEl/O1F1snysLD17xhRdWqVenmzRuaDR44jYOrgstl9aNcjuPRZZEiRTSCxvETxNt2nhdv3Vn8+RLatNn5+X214Ko3qeB2aggzOTvg/frrr5rlU7asAtwHDrzHMY821YGX8RQoUEAdleFcbzrmDMuWLiH+fM6cPUvvDkqb081Q0E6Es4LLxc+ePUcDhcDqA/+fSUxM1Mylcx7eC7pl8+ZSdgiunhquQSDzBFwSXG7ml/ORdDcuKfMtOlHCnuDKRY2WC306dSK9UuclOavDo5WCG+jvQzVDAh32ITMZnBVcZ+o0Elz97kj6+tijUB5Bc5o7gsuj2FHiLUZnheAYBRbGCR+NIx8fH8kjm3ebsjfNwELKf2WHLFlw+ZpHeuqRqa02Q8RLLhbMm6eM6vV59BtQyJuJ6PPZuu7bf4BmD2sezfcX22Ny4JcE7Nq921YxKY5HnuodrTIjuFwBv0Bi7rz5Dre15PufPnWqsowCgmv3I0ECCDhNwGXBtfIl9I4El+/O1ksKGjWoRxPGOrf3rUzISsENKeFPFUr6y02ZcrRScPVzhjxHyVsg8tyhHNj8ys5THdq1o+linnjfvn1SEu8bzJ61HOaJfZH5bTdycOY9vZx3y9attHHT5gxiyG8J6iTMxa+INwzJZm3Oz05Lkz6enMGTmoV50MABdOLkSWUuWxZcLpeQkEBfbtsm+vi1ZhTPaTza47aaCxM1C7atwObZBo0aK1yYycwZnyhLfGyVUcf9JvrFLyiQHwa4zW1btyhZmAO/xUi9nIvNyyzKj4qXVfBmIfx2Iw5qwY2OjqYWrVor9TCHKeLtUfrA89uzxFaTp06d0pjdOR+3wy+IeO3VV8nT01Mpqt4alLkYzW0rhXACAiCgIeCy4N6OTaLDF9P22dXUaMKFM4LLzRw5dlxag8um5rpiVKt/MYEzXbFScF94NIgK+Xk7040cm4fng0PFdoN3bt+hIgFFqJQY2apFz4qOx8fHS6/z8xVOULylpDzHaq8tfiDgjSM4cP8c5VfXw6LNAsRmf/YMzkxZdT1WnPMonPd0Dg4ursyzmt0OizpbKvILU3iwYM2vKEQAARCwhoDLgsvd2X86nBKSzN9xylnBNQOJVYLr7+tFtaukbTBhRj9RBwiAAAiAQO4m4JbgXrwRS5dvxppOIC8IbuVSBalcsLEDjengUCEIgAAIgECOJeCW4N5LSKafxDaPZoe8ILh1HhPmOR8T3ZPNhoz6QAAEQAAEspSAW4LLPT1+OYrCos3d5rFEgB/55bPtsGI2nfj7yXTzdryp1ZYO9KMnyjj3HlVTG0ZlIAACIAACOZaA24J7Ny5ZLBEyf5SbY4k50bGXqhal/Fn0wOBEd5AFBEAABEAgBxBwW3D5Ho5dvk0R0fdzwO1kfxdKidFtNYxus/+DQA9AAARAIIcRMEVwo+OT6Oc/rFkilMN4GXaHl5a8VLUY8TtwEUAABEAABEBATcAUweUKz/wTTVcj49R1P3DnFcRGFyEmb3TxwEHEDYMACIBAHiVgmuAmJqfSgTPhlJySmkdRGd9WPm8PYs9kM/dNNm4RqSAAAiAAArmJgGmCyzd9NSKO+F25D2J4pnwAFSuc/nq4B5EB7hkEQAAEQMA+AVMFl5s58ecdunUnwX6LeTCljHjfbRXx3lsEEAABEAABELBHwHTBZZPyQbEZRnyi+Vs+2ruJ7Iwv5OdFz1UuSp7Y4yI7Pwa0DQIgAAI5noDpgst3fOdeEh25GEUpYuP7vBx8xLzt85V4zS28kvPy54x7AwEQAAEzCFgiuNyxvC66aWIbhA0uzPgWog4QAAEQeAAIWCa4zC4qJlHaFCOvjXRZbGuFBBG/EQgBBEAABEAABJwhYKngcgd4pHv0UlSeWS7Em1rUqhSEzS2c+XYhDwiAAAiAgELAcsHllmLETlRHhOgmJuXuOV0e0T5bMQhvAVK+PjgBARAAARBwlkCWCC53Ju5+Ch2/EiXEN9nZvuWofEEFfejJcgHk4wV35Bz1waAzIAACIJBLCGSZ4DIPdlr+/e+7FGry6/CsZl1RbNdYUWzbiAACIAACIAACrhLIUsGVO8k7Up27FpPjlw35enuKN/8UoaBCPnLXcQQBEAABEAABlwhki+ByTxMSU+n01TsUfjdnvtbvEbF7VOXS/uSFzZFd+mKhEAiAAAiAgJZAtgmu3I2btxPowo0YupeQM+Z2A/19hNAWoiIFvOUu4ggCIAACIAACbhPIdsGV7yBCjHSvhMVSpFi7m9WB3aBKBvhR2WB/Kpwfa2uzmj/aAwEQAIEHgUCOEVwZ9r37yXQ9Mp5Co+Ikz2Y53ooji2upwPzSX369HgIIgAAIgAAIWEUgxwmu+kZvxyZRRHQChYu/vIGGu4FfMBAgTMbFCvlScBFfKoCdotxFivIgAAIgAAJOEsjRgqu+hyTxFqI7wtwck5AkRr7JFCeO98VL7/nF94nJKcqmGjxS9fHyJG+xXjZ/Pi/lr7+vNwWKtbQIIAACIAACIJAdBHKN4GYHHLQJAiAAAiAAAmYRgOCaRRL1gAAIgAAIgIABAQiuARwkgQAIgAAIgIBZBCC4ZpFEPSAAAiAAAiBgQACCawAHSSAAAiAAAiBgFgEIrlkkUQ8IgAAIgAAIGBCA4BrAQRIIgAAIgAAImEUAgmsWSdQDAiAAAiAAAgYEILgGcJAEAiAAAiAAAmYRgOCaRRL1gAAIgAAIgIABAQiuARwkgQAIgAAIgIBZBCC4ZpFEPSAAAiAAAiBgQACCawAHSSAAAiAAAiBgFgEIrlkkUQ8IgAAIgAAIGBDwuBEelWqQjiQQAAEQAAEQAAETCEBwTYCIKkAABEAABEDAEQGPa1FhqR4eHpQq/qSIl7zzH/IQ/0rj3rRrPpfi+V8+F+kc4+HhKcWnikipDk704CROT6uTO8DpUrwU+28yJ3Def4NURL7QHUX3EEAABEAABEDAIQGntYRlSgTWl39PpRPWMik+TcyUDLLG8ZH/pKamcGkhl+KvVCQtns/5TPqXD5wu/nh6etD/AywQeinkZWCrAAAAAElFTkSuQmCC"), N(o, "alt", "Player Management Examples"), N(y, "cx", "13"), N(y, "cy", "13"), N(y, "r", "12"), N(y, "stroke", "currentColor"), N(y, "stroke-width", "2"), N(b, "d", "M17.9653 11.6049H15.1504C14.9504 11.6049 14.7585 11.5254 14.6171 11.384C14.4757 11.2426 14.3962 11.0507 14.3962 10.8507H14.3952V8.00958C14.3885 7.81386 14.3061 7.62837 14.1652 7.49226C14.0244 7.35615 13.8363 7.28005 13.6404 7.28003H12.3612C12.262 7.27989 12.1637 7.29931 12.072 7.33717C11.9803 7.37503 11.8969 7.43059 11.8267 7.50068C11.7564 7.57077 11.7007 7.65402 11.6626 7.74565C11.6246 7.83729 11.605 7.93553 11.6049 8.03476V10.8497C11.6049 11.2666 11.2666 11.6039 10.8507 11.6039H8.0227C7.82453 11.6076 7.63572 11.6889 7.49685 11.8303C7.35798 11.9717 7.28013 12.162 7.28003 12.3602V13.6394C7.28003 14.0516 7.61098 14.3878 8.0227 14.3936H10.8507V14.3946C11.2677 14.3946 11.6049 14.7329 11.6049 15.1488V17.9774C11.6083 18.1753 11.6894 18.364 11.8305 18.5028C11.9717 18.6416 12.1617 18.7194 12.3596 18.7195H13.6394C14.0521 18.7195 14.3873 18.3886 14.3936 17.9774V15.1488H14.3946C14.3946 14.7319 14.7329 14.3946 15.1488 14.3946V14.3936H17.9894C18.1852 14.3872 18.3708 14.3049 18.5071 14.1642C18.6433 14.0234 18.7195 13.8353 18.7195 13.6394V12.3602C18.7196 12.261 18.7002 12.1628 18.6624 12.0712C18.6246 11.9796 18.569 11.8963 18.499 11.8262C18.4289 11.756 18.3457 11.7004 18.2542 11.6624C18.1626 11.6245 18.0644 11.6049 17.9653 11.6049Z"), N(b, "fill", "currentColor"), N(E, "clip-path", "url(#clip0)"), N(C, "width", "11.44"), N(C, "height", "11.44"), N(C, "fill", "white"), N(C, "transform", "translate(7.28003 7.28003)"), N(w, "id", "clip0"), N(v, "width", "26"), N(v, "height", "26"), N(v, "viewBox", "0 0 26 26"), N(v, "fill", "none"), N(v, "xmlns", "http://www.w3.org/2000/svg"), N(v, "class", "icon"), N(g, "class", "button no-border strong theme-info-color inline-help-button"), N(z, "d", "M26.115 11.345 15.639.86a3.094 3.094 0 0 0-4.278 0L.885 11.345a3.029 3.029 0 0 0 0 4.28l10.476 10.487a3.02 3.02 0 0 0 4.278 0l10.476-10.489a3.029 3.029 0 0 0 0-4.28v.002ZM12.054 6.73A1.449 1.449 0 0 1 13.5 5.282a1.446 1.446 0 0 1 1.446 1.447v5.792A1.449 1.449 0 0 1 13.5 13.97a1.446 1.446 0 0 1-1.446-1.448V6.73ZM13.5 20.243a1.928 1.928 0 0 1-1.892-2.307 1.931 1.931 0 0 1 2.63-1.407 1.93 1.93 0 0 1 .626 3.149 1.928 1.928 0 0 1-1.364.565Z"), N(z, "fill", "#FFBE15"), N(V, "class", "icon"), N(V, "fill", "none"), N(V, "xmlns", "http://www.w3.org/2000/svg"), N(V, "viewBox", "0 0 27 27"), N(H, "class", "note-content"), N(L, "class", "note border-theme theme-caution-color")
+                N(a, "class", "player-help-header"), N(o, "class", "player-help-img"), e = o.src, t = s = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAdwAAAFACAYAAAAWB83NAAAK3WlDQ1BJQ0MgUHJvZmlsZQAASImVlwdQU+kWgM+96SGhBRCQEnoTpBNAamgBFKSDqIQkQCgxhICKXVlUcC2oiGBZ0VURBctSxIZYsLAo9r4gi4DyXCzYUPMu8Ai7++a9N+/M/Pd8c+75T/nn/jPnAtBDuWJxJqoMkCWSSiICfZlx8QlMUg8oAA5ogAcql5cj9gkPDwVMxvVf5cM9QEb0beuRWP/+/r+KKl+QwwNAEjFO5ufwsjBuxtYgTyyRAuCOYnaj+VLxCN/BWE2CFYhx3winjvHXEU4eZbzyqE9UBBtjYwAyjcuVpALQbDE7M4+XisWhhWNsK+ILRRgvx9iTl8blY4zlhSlZWfNGeABjc8xfDEBXw5iV/KeYqX+JnyyPz+Wmynmsr1Eh+wlzxJnchf/n0fxvycrMHc9hii1amiQoAtOa2Pk9yJgXImdR8oywcRbyR/1HOS03KHqceTnshHHmc/1C5HszZ4SOc4owgCOPI+VEjbMgxz9ynCXzIuS5UiRsn3HmSiby5mZEy+1pAo48fn5aVOw45wljZoxzTkZkyIQPW26X5EbI6xeIAn0n8gbIe8/K+VO/Qo58rzQtKkjeO3eifoHIZyJmTpy8Nr7Az3/CJ1ruL5b6ynOJM8Pl/oLMQLk9Jy9SvleKfZwTe8PlZ5jODQ4fZwiFQGBCNGSCFCTAhQAQgggEUsEC6Ugz7HnihRJhapqU6YPdOAGTI+LZTGHa29rbAYzc37FP4p3G6L1ENK5N2FZVAXiclMlkpyZswTcBjiUBUOsmbOazAZR7Aa6c5uVK8sZs+JEHAaigBGqgBXpgBOZgDfbgDO7gDf4QDGEQBfEwB3iQBllY5fNhMayAQiiGjbAVymE37IWDcASOQwOchvNwGa7DTbgLj6ETeuAVDMIHGEYQhITQEQaihegjJogVYo+wEE/EHwlFIpB4JAlJRURILrIYWYUUIyVIObIHqUKOISeR88hVpAN5iHQh/chb5AuKQ2moGqqLmqJTURbqg4agUehsNBXNRvPRAnQ9WoZWoofRevQ8eh29i3air9AhHOAUcBo4A5w1joVj48JwCbgUnAS3FFeEK8VV4mpwTbhW3G1cJ24A9xlPxDPwTLw13h0fhI/G8/DZ+KX4dfhy/EF8Pf4i/ja+Cz+I/06gE3QIVgQ3AocQR0glzCcUEkoJ+wl1hEuEu4QewgcikahBNCO6EIOI8cR04iLiOuJOYi2xmdhB7CYOkUgkLZIVyYMURuKSpKRC0nbSYdI50i1SD+kTWYGsT7YnB5ATyCLySnIp+RD5LPkWuZc8TFGmmFDcKGEUPmUhZQNlH6WJcoPSQxmmqlDNqB7UKGo6dQW1jFpDvUR9Qn2noKBgqOCqMFNBqLBcoUzhqMIVhS6FzzRVmiWNTUuk5dLW0w7QmmkPae/odLop3ZueQJfS19Or6Bfoz+ifFBmKNoocRb7iMsUKxXrFW4qvlShKJko+SnOU8pVKlU4o3VAaUKYomyqzlbnKS5UrlE8q31ceUmGo2KmEqWSprFM5pHJVpU+VpGqq6q/KVy1Q3at6QbWbgWMYMdgMHmMVYx/jEqNHjahmpsZRS1crVjui1q42qK6q7qgeo75AvUL9jHqnBk7DVIOjkamxQeO4xj2NL5N0J/lMEkxaO6lm0q1JHzUna3prCjSLNGs172p+0WJq+WtlaG3SatB6qo3XttSeqT1fe5f2Je2ByWqT3SfzJhdNPj75kQ6qY6kTobNIZ69Om86Qrp5uoK5Yd7vuBd0BPQ09b710vS16Z/X69Rn6nvpC/S365/RfMtWZPsxMZhnzInPQQMcgyCDXYI9Bu8GwoZlhtOFKw1rDp0ZUI5ZRitEWoxajQWN94+nGi42rjR+ZUExYJmkm20xaTT6ampnGmq42bTDtM9M045jlm1WbPTGnm3uZZ5tXmt+xIFqwLDIsdlrctEQtnSzTLCssb1ihVs5WQqudVh1TCFNcp4imVE65b02z9rHOs6627rLRsAm1WWnTYPN6qvHUhKmbprZO/W7rZJtpu8/2sZ2qXbDdSrsmu7f2lvY8+wr7Ow50hwCHZQ6NDm8crRwFjrscHzgxnKY7rXZqcfrm7OIsca5x7ncxdkly2eFyn6XGCmetY11xJbj6ui5zPe362c3ZTep23O0Pd2v3DPdD7n3TzKYJpu2b1u1h6MH12OPR6cn0TPL8ybPTy8CL61Xp9dzbyJvvvd+718fCJ93nsM9rX1tfiW+d70e2G3sJu9kP5xfoV+TX7q/qH+1f7v8swDAgNaA6YDDQKXBRYHMQISgkaFPQfY4uh8ep4gwGuwQvCb4YQguJDCkPeR5qGSoJbZqOTg+evnn6kxkmM0QzGsIgjBO2OexpuFl4dvipmcSZ4TMrZr6IsItYHNEayYicG3ko8kOUb9SGqMfR5tG50S0xSjGJMVUxH2P9YktiO+Omxi2Jux6vHS+Mb0wgJcQk7E8YmuU/a+usnkSnxMLEe7PNZi+YfXWO9pzMOWfmKs3lzj2RREiKTTqU9JUbxq3kDiVzknckD/LYvG28V3xv/hZ+v8BDUCLoTfFIKUnpS/VI3Zzan+aVVpo2IGQLy4Vv0oPSd6d/zAjLOJAhy4zNrM0iZyVlnRSpijJEF+fpzVswr0NsJS4Ud2a7ZW/NHpSESPbnIDmzcxqlatig1JZrnvtDbleeZ15F3qf5MfNPLFBZIFrQttBy4dqFvfkB+T8vwi/iLWpZbLB4xeKuJT5L9ixFliYvbVlmtKxgWc/ywOUHV1BXZKz4daXtypKV71fFrmoq0C1YXtD9Q+AP1YWKhZLC+6vdV+9eg18jXNO+1mHt9rXfi/hF14pti0uLv67jrbv2o92PZT/K1qesb9/gvGHXRuJG0cZ7m7w2HSxRKckv6d48fXP9FuaWoi3vt87derXUsXT3Nuq23G2dZaFljduNt2/c/rU8rfxuhW9F7Q6dHWt3fNzJ33lrl/eumt26u4t3f/lJ+NODPYF76itNK0v3Evfm7X2xL2Zf68+sn6v2a+8v3v/tgOhA58GIgxerXKqqDukc2lCNVudW9x9OPHzziN+Rxhrrmj21GrXFR+Fo7tGXx5KO3TsecrzlBOtEzS8mv+yoY9QV1SP1C+sHG9IaOhvjGztOBp9saXJvqjtlc+rAaYPTFWfUz2w4Sz1bcFZ2Lv/cULO4eeB86vnulrktjy/EXbhzcebF9kshl65cDrh8odWn9dwVjyunr7pdPXmNda3huvP1+jantrpfnX6ta3dur7/hcqPxpuvNpo5pHWdved06f9vv9uU7nDvX786423Ev+t6D+4n3Ox/wH/Q9zHz45lHeo+HHy58QnhQ9VX5a+kznWeVvFr/Vdjp3nuny62p7Hvn8cTev+9XvOb9/7Sl4QX9R2qvfW9Vn33e6P6D/5stZL3teiV8NDxT+Q+UfO16bv/7lD+8/2gbjBnveSN7I3q57p/XuwHvH9y1D4UPPPmR9GP5Y9Enr08HPrM+tX2K/9A7P/0r6WvbN4lvT95DvT2RZMpmYK+GOjgI4bKEpKQBvD2DzcTwAA5shqLPG5utRQcb+CUYJ/hOPzeCj4gxQg6mR0YjdDHAUW6bLAZS8AUbGoihvQB0c5OtfkpPiYD8Wi4ZNl4RPMtk7XQBSE8A3iUw2vFMm+7YPK/YhQHP22Fw/InrYP8YsKdAoax65tcHfZWzm/1OPf9cwUoEj/F3/E9T/HtBz9KX+AAAAimVYSWZNTQAqAAAACAAEARoABQAAAAEAAAA+ARsABQAAAAEAAABGASgAAwAAAAEAAgAAh2kABAAAAAEAAABOAAAAAAAAAJAAAAABAAAAkAAAAAEAA5KGAAcAAAASAAAAeKACAAQAAAABAAAB3KADAAQAAAABAAABQAAAAABBU0NJSQAAAFNjcmVlbnNob3Q3DfkqAAAACXBIWXMAABYlAAAWJQFJUiTwAAAB1mlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPHg6eG1wbWV0YSB4bWxuczp4PSJhZG9iZTpuczptZXRhLyIgeDp4bXB0az0iWE1QIENvcmUgNi4wLjAiPgogICA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPgogICAgICA8cmRmOkRlc2NyaXB0aW9uIHJkZjphYm91dD0iIgogICAgICAgICAgICB4bWxuczpleGlmPSJodHRwOi8vbnMuYWRvYmUuY29tL2V4aWYvMS4wLyI+CiAgICAgICAgIDxleGlmOlBpeGVsWURpbWVuc2lvbj4zMjA8L2V4aWY6UGl4ZWxZRGltZW5zaW9uPgogICAgICAgICA8ZXhpZjpQaXhlbFhEaW1lbnNpb24+NDc2PC9leGlmOlBpeGVsWERpbWVuc2lvbj4KICAgICAgICAgPGV4aWY6VXNlckNvbW1lbnQ+U2NyZWVuc2hvdDwvZXhpZjpVc2VyQ29tbWVudD4KICAgICAgPC9yZGY6RGVzY3JpcHRpb24+CiAgIDwvcmRmOlJERj4KPC94OnhtcG1ldGE+CnRq2CEAAAAcaURPVAAAAAIAAAAAAAAAoAAAACgAAACgAAAAoAAAMevKJG8/AAAxt0lEQVR4AeydB3wURRvG3xB6DV2KSC/SpIaigH70pnSQGhAIIF2KAtKlFykSmqH3KkV6FRABaaJU6b0kdEgIfPMu7mZ3c3e5snu5C8/4w92ZnZ3yv80+OzPvzPiEPn76hqw6H6tXbF3w9fUh3zhxlCjhryLojY1clIgGnSB/8Mfzh78/+XWC9w/ev+7UnziK/r0VvVcq/fORBTeury/FjetLcXycE1n54ebbfXRpcGXfuKnGyB/88fxp/4bx94f3D96/7mnxWdafNxTx+g2x8Po8fPLsTcL48ShOHO0fqSygjh59iBU36l1u+8GRP/jj+YvyB4i/Pze9cPH+wfvHxvvH52VY+Js4qu7fKH+pDgZYayG/IfGfG5555G/h1xa/Ifjj+cPfn4MvMyei4/2D94+lx0Z+//qI8Q1DZJAx67vy9BnLmerDjfAjf/DH82f5ZSf/feHvz7yPLrx/8P6x5/3jI/qVjRHct0+c/Ldt9Sh1bRmSozYLadhYN3asjfHWh/wFfPC39Gi4FIbnT+DD31+0zxDePya8f4T2SJ+aMfX8OZC/z6sI1wXX2rittafP6PEk5C//4taIa8PB39gvDjx/eP4s2a1o/+oiffj7e3f//lwSXHu/KiIfNdWZGFByFTvyFzzt+KpTUY88BX88f5FPg1Nn+PsT2PD359SzwwY9rrz/pWePc44h/s7m7xPxWtgrO1FzZ+up/3WkrJG/Hku0fvCPFpFdEfD8CUz4+7PrWVFHwt+fmobz5+/a35/Paxbc/1y0lReyrii7fJOBR+QvYCq/hgWw4I/nz8JjYVQQ/v7w9+ex75//hCfG9Meg/DWCa9QfLtIBARAAARAAARDQEhCC647ZedpM4QMBEAABEACBd42Aj7CYUzox0aUkfn6FhoVHAV266NK18FgYFYS/P/z94f1j468pFrx/NYJro6q4BAIgAAIgAAIg4AIBCK4L8HArCIAACIAACNhLAIJrLynEAwEQAAEQAAEXCEBwXYCHW0EABEAABEDAXgJeJbg3Tp+i2+fP0r0rlyj0+jV6cv8uPQ0NobBnzygiPFyqs2+8eBQ/cWJK4peSkqZOS36ZMlOaLFkpfc7clDFvfnu5IB4IgAAIgAAIGErAowU39OZ1OndgH106cpCunjxGEWFhLlXeN358er/gR5S1mD/lKl2W/DJkcik93AwCIAACIAAC9hLwSME9sXkDndqxma4dP2pvPZyKl7lwEcr/WRUqVKWGU/fjJhAAARAAARCwl4DHCC53Cx9atZSOrl9Fz0ND7S2/IfES+flRkZp1qUTdRlJ3tCGJIhEQAAEQAAEQUBHwCMH9fekCOrhsAYU9faoqmvtP4ydJQv4Nm1GpRs3cnzlyBAEQAAEQiNUEYlRwzx/cT3uDg+jepYseBTlN1mz0SUAg5fQv41HlQmFAAARAAAS8l0CMCe7WnybQsV9WeTS5j2rXpUodu3t0GVE4EAABEAAB7yDgdsG9feEcbZo4ku6cO+sVhNLlyk1Vu/Wl9DlyeUV5UUgQAAEQAAHPJOBWwT3z2y7aMHqoy9N73I2SpxPV6D2A8nxcwd1ZIz8QAAEQAIFYQsBtgnt0/WraNmW8V2Or+HUPYc1cx6vrgMKDAAiAAAjEDAG3CO6hVcto14zJMVNDg3Ot0K6zmD7U0OBUkRwIgAAIgEBsJ2C64MaGlq3+IUBLV08EfhAAARAAgegImCq4PGb7y7AB0ZXBK6/X7j8UY7pe+cuh0CAAAiAQMwRME1y2Rl7YPdDrDKTs/RnYkKrphCBYL9sLDPFAAARA4B0nYJrgzu3cxmum/jj7DPCUoZaTZzt7O+4DARAAARB4hwiYIrjesKiFUb8xFscwiiTSAQEQAIHYTcBwweXlGlcP7BO7qelqV2fwKCwDqWMCLwiAAAiAgJaA4YIbHNjC49ZG1lbZeB+vvRwQNM/4hJEiCIAACIBArCFgqODyrj97g6fHGjiOVOSTgPbYZcgRYIgLAiAAAu8YAcMEl/eznda8boxvsRdTvx9v7ddh/irspxtTPwDyBQEQAAEPJ2CY4O5bEEz7F/zs4dU1t3hlmrWmss0CzM0EqYMACIAACHglAcMEd0rjWvQ8NNQrIRhV6ER+fvT1knVGJYd0QAAEQAAEYhEBQwT3xOYNtHnCyFiExfmqVOnelwpVqeF8ArgTBEAABEAgVhIwRHAX9+lC144fjZWAHK1U5sJFqMmoSY7ehvggAAIgAAKxnIDLght68zrNDGgcyzE5Vr22wUvIL0Mmx25CbBAAARAAgVhNwGXBNWPrvaRp01Jusdl7tmL+QrgyUuLkfpRAWAGHv3xJzx+G0qO7t+nfw7/Tmd076eGtG1F+oOL1G1Ou0p9ECZcD3rx+TS+fPqUH167Q/auX6cLBfYaOP3vLFn6hDx/R4ydPZCyUPl1aih8vnuK39+TR48eUPFkye6Mjnh0Enj1/TgnEet2+vr52xEYUEAABbyDgsuAu79eTLh35w7C6lm3RhvwbNiXfuNG/+F+FhdH+xfPo4OK5mvwrd+lFhavX1oTZ8kSEh9Ff27fQ/oU/05O7d21Fteta1mIlqcHwcXbFNSLSmzdv6MrVa3Tm7Hk69c9p+vv0GQoNfUi5c+agD/PlpXx5c1O+PLkpUaKEmuwG/zCa1vyyQQkLnjmVPipYQPFHd3L12nVqHdiZ7t27L9JORFMmjKaiHxWK7jaXru/d9ztt37XbYhrx4sallClTUq4c2Sn/h3kpY4b3LMbz5MCw8HAK7NyDjh47IRWzV/fO9GWj+p5cZJQNBEDATgIuC+742v8zZEeg9LnzUPUe31GarNntLHpktFvnz9Cv40bQvYsXpEBHBVdOKeJVOC3t242u//X2ZSeHO3rknYR6/LLd0ducin/+34vUs+8AunLlqs3744syDRv4HVX636dKPFcFt8s3fWnvbweU9N57Lz39umaZ4jfjZNLU6RQ8f5FdSfuXKEbdOnegvLlz2RXfEyItWb6aRo2bqCnKjk1rKaWwgIcDARDwbgIuCe6N06doYbdAlwnkr1ydqnbtTXFc6D5Tr+HsrOByRR7fu0uz2zWl8GfPXapX04lBlDFvfpfSsHXzq1evKGjWHJo9Z76taFGulS3tTyOGfE/JkiUlVwW3QdMAOn/hXyUPFvWDe7YqfjNOHBFcOf/RwweLD40KstejjxMmT6N5C5doyrhq6XzK9kEWTRg8IAAC3kfAJcE9un41bZsy3qVa89zVtrMXizHapFHS4S7jm2f+ptv/nqcHVy5TvMSJKFWmLJS7bDlKlCy5Ej/sxXOa16kNhVx/28qzJLiHVi2lf3Ztlbqqk6ZOS6nez0KFqtaiFOnSK+nIJ4fXrqCd036UvU4dK37dg4rUrOPUvfbc1Kl7L9p/wHJXPgtfqlQp6cGDEAoTDNWOr/26dhmlEl2vrgruLCH2U4NmKclXFq3nUcMHKX4zTvSCy13ZhQsVIB6Xvy/qy13r+jrzOOja5QspU8YMZhTJ0DSPnzxFrdp2VNLkLvKt61diLFchghMQ8F4CLgmuEdvw1R06hnKUKBWFIHcTrx8xWBFRfYTSTVtRyfpfUvyECWmjmAN8astGJYolwV0/Zhj9s32zEkc+qTdsLGUv7i97pePVv47Tkm++1oQ56jFz276t23dS736DohSpa6dAqlmtMqVJk1q5dk60QKfN/Jl27torhU0Y/QNVKFdWOndVcHnseM26jXT4yFHKmycXNWlYj+KKcVQznV5wq1WpSD8MHqBk+VoI72oxLj1s5FgljE/atm5JHdu11oR5qufwn8do/cZNlCJFCmrRtDGlFh9PcCAAAt5PwCXBddVgKt//qlDNXv2jUDwpxHPT+BFRwi0FcKtX3/3riOBaWh3qhbC6ndyguqXs7A4zy3Dq4aNHVLlmPU0rjgV2xtSJNrsdz567QE/FetdFChdU6uCq4CoJufEkOsGVizJ6/CRavGyl7KUypUvS1AljFD9OQAAEQMDdBFwSXFe34ms9Yz6lzpJVU+dHd+/Q9Ob1NGGOehwRXE6784qNlDBp5LSW1xERNK5GBUez1cQ3a8u+UUJIlqiEhDOdO2saFSrwoSZ/ezyWBDc8LJzWbdhEx06cpBCxVGf2bFnp4zKlqHULYTmuG2M/fPQ4Bc2YrWTF1rSfVSgn+XlaS5ceb/dFTp48GQ3s14eSiqldy1f9QvsPHlSscIsULkT16tSm8h+XUdKxdWKv4O7as4+69/5OSSpLlvdp7bIFil8+YWvuFWt+kSy72cr79u07lDZtGsovrLu/Cmhu0eBq6IgxdFkYqSVNmpR69+hCiRMnpumz59CuPb/REzHNqox/SapVsxp9LMbL2V29foPmzFso6n2IHoqpWJx+PtEj0KFta/pAlEvtHj9+oil30Y8KU8f2bZQoy1auoS3bdpBPnDhUrXJFqvt5Tbp0+SqtFHXYsGkrvX4dQVUr/Y/6ftNNuYdP2JJ89boNdPLU3/TP6bPStaxiXLhQgfzUqlkTaUxffQM/G1dF97w9rl0b0dtUvKg9UREHBKIQ4Gf+zLnzlEHMKsgUzcwCs+JGKZRJAS4JrivrJ/NcW95dR+/WDv+ezu7dqQ92yO+I4HILueuKTdILTM4k5MZ1mtW6sex16mip5exUQrqbGrf4Skz/OaeEVq74GY0aNlDxO3KiF9zcuXIQt4QtOX45L/g5iJII0ZQdv+D7Dxome6lzh7bUumUzyc9zc8tXqqlcY9HYtmOX1fQDvwqg9l+1UuJbO7FXcFeuWafpVrbUwuU43BLWj/mq8+7ZtRM1a9JQHUTVvmhIt27dlsLez5yJ7t1/QM/FB4be/Th2pDAEjEPdvvmWIsRHnCU35ochVPGz8solTqtSjcix/2JFCtOsaZErl6l/Mx7fnSVsDRoK4zV1+nprcR6C6D/4B6v15HH9UcMGKUMNXJgqtevTnTv2TZEb8v13VKt6FaUOOAEBewksXLKcxk6cokSvUO5jmjB6uOJXn7gad8iAb6N8WKrTd8e5S4LrypSgDytVoxo9I1sgXFkjunI5HUcE97OO3ahYbW2L+vwf+2n1929bZ5yeM86sqUHFy36meblOmTiGypYq6UwRoxhNRZcICw8LkOwcEVz5HlvHn34cS6X9S9iKQvYILltw1xLj+7IocoId2gYQt8RkN3naTPp5btQWr3xdfVy+aA7lzJ5NCVILrhJo4YSFjIVQLYb6aBxn5+ZfKLEw/mLniOBy/BQpkkutZj6X3acVPqHxI99+CK1Y/QsNHzVOvmTzuEb0AMgtbkcEd9zIoUrPhs0McBEEVAR27t5LPfpEHVJs36YVBYq/V7U7JOxE2nXS9trwdUficg8cz2uPSeeS4I6pJroPheGMM65k42ZUvlV7za3XxTSjRQZMM7JHcLll+2nbztJGA9w9p3bLvutBl/88pA5y/NzHh3r9usfx+2zccefuPapSS/txsHndSkonuiidcerWknx/yRLFqP4XtSmeWHFq8fKV9MehI/Il6Xhk/06K8x8vRwWXu6TbtGouFscoLLW2howYLXV1yhnwAh2L5syUvRaPtgSXW9Wn/j4ttVovXb6i3M/57t6yTtM65y7hLxq+bY2z6LVp2ZRKia7gmzdv0c/zFmha4jyVihf1kJ1ecPn+7p07UrasH9D6XzcJg6eoxnmNG9aTuoB/23eA5oppP+pW9Xe9e1KDurWl5B0VXLlMfORu8wcPHkhl4a5m7i6vKFrLasH//rvekmGdj3g+t+3YLVq+w5Xrav5HxHDB06fP1MlL5zt276G1wlBOdtyaXr9ycZThBvk6jiBgjcCYCZNp0dIVUS7nzpWTls6PHKriCEbE5S7rjauXRsnPnQExJrjlv+oorIybaOr617ZN9OtYy90JmojReCwJ7tMH9+nB9WsUJ15cSpE2PSVNJSx5xUtH7y4c+p1WDeilD3bcb4Lg7vv9D/q6m7ZsR3/f7XjZ/rtDL7jcAuSWoOzYCrlU+coacVi/aokyvcYRwWVRmiNWsuIVr2SnFxcO/3XtcnovfTo5SpSjXnA5gjy2rBYW9Y3jRw2nT8t/rA6Szs+ev0CXLl2hsmX8KYkYh5Udj3dWqllX9kqrV+34dY3i1wuumglH4ns5DdmVEq32aaL1Ljt9HRo3qEt9enaVLuuZ2OpSltPj7vrmovchobDYVzv9eD+L8IBvtc/PgsXLaNyPU5Xbdm9db3WZzpuiG71WvSaKQDP31WKOMHerw4GAowSsiWiunDlomW5vdSPi6odaHC2vEfFdElxXupQLVatNVbpq//iPbVxLWydFvpicraAlwbUnLcPEVmRmRpfyqX/OULOAdpqqHNi1OcqLVhPBhkcvuJaWduzTbxBtEWOAsps2eTyVEq1gdo4IboH8+Wj+7CA5GeXYXixjqG5Fs7V1iWJFlOv6E71Y6a+r/fwHNlSMLxYv+pE62K5zvaj+eWCX+D57+4Gmv6b/6GGjqlVr1yv5sJiyqMrur7//oeatIxeMUQuyo4Kr7j6W05eP+vF+HlPOnEk7F/m6aNHLxm183+ygyRaX5+Ru+npfttKsaDZ6+CDNymVyvjiCgD0E0KVsDyVVHFeMpizNU7107AgtF0sruuocFVzeEGHvvFl0fMNaV7NW7jfDaOrFixdUuoLWOGXR3JmaVqNSADtO7BFc/cpHk8aPok+E1TI7IwRX3wrjLs86tWtYLb29gsst6q0bVlltrekzuCWsk68Ja2JeH/r6jZu0YvVazdjo4X07lJZ0dII7M3ge/TQ9skts2KD+VKNqJSXLu/fuSVO75IDi4gNjpvjQYOeo4AbPEOtfi4U/LDn/cpU0vROW4ujD+vXpSfWF1bje6T8i6n1Ri/r3/UYfDX4QcIiA3hCqvFgjYKJYK8CSczXu0AHfebfRlCvTgjIVKERfjo3symLAD+/cphkt6lti7VCYJcF9Lb7Q34j/LG2K8ECsULWoZ0dDdwwya1pQhSq1NEKgHv9zCJKI7AmCO2P2HLEwR7BSdL1xk3LhvxO94HJXMTPgMdnOYhqS2lo4Z47s0liQPOasT4unGPB46tr1GzVdwPp47PdYwbWy4QR3r7OBnaNuUP++9LmY0qR2W7btpD79BylBbLG+fGGw6YucKBniJFYT4L/D02LmRUaxEpw904LMiOsuwC51Kbuy8AUbLXVbtUVTT16eb3bbZlZXl9JEtuGxJLjySlMZPyxA9YaM1sy75aSMWF1KXSSzFr5o1a4THT/xl5IVW6luWb/KqW31PEFwR46dSEtXrFbqw/N1v6hlfdERveCqV5o6IOa5duyqbXV1CvyKvhKGWnrHBmjc5RoSEqK/ZNHvbYLLlfikYnUxL/ipUp+gyROUc0snvmIKE7eW1auFcYu/TqPmmnHbdcJIKoPorocDARBwjIBLguvq0o4dF62hJGy8pHIXxVZ/K8SWf644W4LL6fJmCdV7fBslix0zp9CRlcZYsVnqMo+SoRMBGzdvo34Dh2ru5LmvPAfWlnv+/IWwPI6reZl6guC2Fab+vDSk7CyNI8vX+GhLcPl63wGDafPWHXyquBWL5lKO7FkVP5/op73wPN06tWpSEbG9YKqUfhTYpadmbNkbBVf/cfbb9o0aS20NEAse3iqQxfaG6GKXHY8Dl/u4tOzFEQRAwAECLgmuq5sXVBWiV1CIn96tGvQtXfj9N32w3f7oBJcTqi/2q80m9q1Vu/CXL2hux9Yut7A5TTM3L9Abw3B+3A34be8e0qbl7Fc7Xvjg2++HipWRkogu1p+ljeb5ekwL7m2xsEJVscCC2tmykuV40Qnu06dPhZVwPU3XMlvRsjWtbM2snhLEaVavUomGD9bOB9Qbc3mj4OrHx/XzqLnusgsX4spTwdSu38BhtHHzViXI1v1KJJyAAAhYJeCS4Lq6PR93KwfOXUkJkyXTFJB3CdozZzodWbVME672FBY78ZRr2VZsp3eHtkweSzf+juxmtUdweaWr1tPnU4LESdTJ0g2xO9HCrtr5wZoIdnrM3J6P98BtICxG9Y67l8uIRTB4ub5kginvnMPLAKrnpPK6y7xzDi+04E7B5bLyXNUWTRtJxWbjoLYdu2rKxisu8cpLtlx0gsv36pd15DCe//u16F5mx5sDcN6y43FgnjokO0u9CN4ouDyNp7pYFUvteAqRvEwnT/viqWaTf5ouzTtmPsyJ3Toxl/j7IZHGK3nEnsKL5sxQ5mCr08Q5CICAfQRcElzOwpWpQXx/0ToN6H/tu/BpFHf5+J90dt9uuikWxHhw7Yq0hV+WwsWocLValDl/ISU+r1DFRk/3r1ySwuwRXI7Iol1ZbKOnd3vmzqKDi+fqg+32mzElSJ85r6k7YoztMTn9Pez/XIyPDhDWpdzac7fgcv6cb/LkyS2OnW5YvZQyisnptpw9gsv39+jTj3bu1vaSLBaW6LwZPW8AUaFyLU02vMUfGwPx+Lj6A0WO5I2Cy2Xn/ZKnqLZQlOvDH2c8vqufu7xUzH/MkD49fVq1dpRr8r3648ol8yi7WPQDDgRAwDYBlwXXFcMpuWgtfwqmdNlzyl6njuo9bO0VXM6o8ZjJ9H5B7TzNiPAwmtelHd27eMGpsphlMKUvzL8XL1Hnnn01Y2z6OLKfhY7XvK0utrOTXUwIrpy3+shlGzFkgF1zOu0V3FCxSQCvyqVe0SldurTSqkjcdWpJkNVlYotJ9diltwoub1fISzuq5wWr66k+b1jvC2nTA96TN0AY59nr5os1tgt8mM/e6IgHAu8sAZcF95Do9t01Y7JLALlruUavAZSr9CdOpXPp6GFa/m135V5HBDfFexmpVdAcsa9uIuV+Prl94ZzY1L61JsxeT4V2nalEXW1Xnr33OhqPFyRYtHQlHTx8WOwCcy5Ky5Hno/7v03KSpW72bFk1yY8a9yMtWb5KCVsQPEPskpNH8fMJzyfleaWyY0tX/xJFJe/W7bvEvrwD5UtineWvxUL/DSS/fvMCnqJTuGB+af9cuVXFQsvLCfLqR7nF6jL2uOmz5lDQrMhpRGorZf39v4tlKXv07qcZz+U9cXlvXN6qkC2k9csw8mIZ3b/uIK1MVbtBU2U9ZvWSlrXFOs1svcuO68BirHZz5i+mH6cGKUGjhw8WHxMVFL+tebj61rd6UQxOwJ7fTMlIdfLnsRPSkpfnxf7IMn++zOVnQzHeuaioOLKztMCKdMHK/yC4VsAgGAR0BFwW3NCb12lmQGNdss55C1SpIXUvx1cts2crpYhX4XR49XLaM3uaJpojgss3FhPi+JkQSb3bL6xb94luSEdd2+Al5JchZpa7423xuOWbSHxA8Mbl3HUor5DkaD1cia8XXPVKUzfE6kYvXr6U9u+NibKp68WWuDzW/fJlmGRMliZ1KvXlWHnOY7sPQkLJTzwbPL3H2jzlWFl5VAoEYpCAy4LLZV/cpwtdOx45tcOV+rAxU8n6TSl7cX9KmSmzxaQeXL1MvAwjrwwVIhat0LuyLdpQGZ1RkTwPVx9X9lfu2ps+/KwSxUsQuR7ty2dPaVLdqnIUu46ZCxehJqMm2RU3NkeyJbixud6oGwiAAAhYI2CI4J7YvIE2TxhpLQ+nw7mrOXma9JQkdRp6HfGKnt6/T09C7lH4s+dOp2n2jVW695V2IDI7H09PH4Lr6b8QygcCIOBuAoYILhfalXWV3V1ps/IzY/1ks8pqdroQXLMJI30QAAFvI2CY4O5bEEz7xZSCd9mVadaayjYLeJcRKHXnsVFe2zhCGHWxK1a0iGbrPyUiTkAABEDgHSFgmOCGCavPac3rUphY6edddPGTJKEO88WaxnYafL2LjFBnEAABEHiXCRgmuAzx96ULaG/w9HeS5ycB7alUo2bvZN1RaRAAARAAgegJGCq4nJ0rW/ZFX1zPjGHWVnyeWVuUCgRAAARAwBkChgvu+YP7afXAPs6UxWvvqTN4FOX0L+O15UfBQQAEQAAEzCdguOBykV3dts/8ahuXg1nb8BlXQqQEAiAAAiDgCQRMEVyu2NzObejOubOeUEfTypAuV25qOXm2aekjYRAAARAAgdhDwDTB5bWIF3YPpAix1V5sdLwjUNMJQZQ+R67YWD3UCQRAAARAwGACpgkul/PMb7vol2EDDC6yZyRXu/9QyvNxBc8oDEoBAiAAAiDg8QRMFVyu/dH1q2nblPEeD8KRAlYUe+gWEXvpwoEACIAACICAvQRMF1wuiBFb+NlbIbPjuXPrPbPrgvRBAARAAATcR8AtgsvViQ0tXbRs3fdgIicQAAEQiG0E3Ca4DI7HdDeMHup1hlRsIFWj9wCM2ca2px/1AQEQAAE3EnCr4HK92Hp508SRXjNliKf+VO3WF9bIbnwokRUIgAAIxEYCbhdcGaI3LI6BRS3kXwtHEAABEAABVwnEmOBywXkZyL3BQXTv0kVX62Ho/bw28icBgViu0VCqSAwEQAAE3m0CMSq4MnreZejgsgUxvrUfb7Hn37AZdv2RfxgcQQAEQAAEDCPgEYLLteH9dA+tWiqsmVfR89BQwypoT0KJ/PzEvNq6VKJuI+xnaw8wxAEBEAABEHCYgMcIrrrkJzZvoFM7NtO140fVwYafZy5chPJ/VoUKValheNpIEARAAARAAATUBDxScOUCht68TucO7KNLRw7S1ZPHXJ5OxNN73i/4EWUt5k+5SpclvwyZ5KxwBAEQAAEQAAFTCXi04OprfuP0Kbp9/izdu3KJQq9foyf379LT0BCpOzoiPFyK7hsvntQtnMQvJSVNnZb8MmWmNFmyUvqcuSlj3vz6JOEHARAAARAAAbcQ8CrBdQsRZAICIAACIAACJhCA4JoAFUmCAAiAAAiAgJ4ABFdPBH4QAAEQAAEQMIEABNcEqEgSBEAABEAABPQEILh6IvCDAAiAAAiAgAkEILgmQEWSIAACIAACIKAnAMHVE4EfBEAABEAABEwgAME1ASqSBAEQAAEQAAE9AQiungj8IAACIAACIGACAQiuCVCRJAiAAAiAAAjoCUBw9UTgBwEQAAEQAAETCEBwTYCKJEEABEAABEBATwCCqycCPwiAAAiAAAiYQACCawJUJAkCIAACIAACegIQXD0R+EEABEAABEDABAIQXBOgIkkQAAEQAAEQ0BPwuXUv5I0+EH4QAAEQAAEQAAFjCUBwjeWJ1EAABEAABEDAIgGfu6HP0MK1iAaBIAACIAACIGAcAQiucSyREgiAAAiAAAhYJQDBtYoGF0AABEAABEDAOAIQXONYIiUQAAEQAAEQsEoAgmsVDS6AAAiAAAiAgHEEILjGsURKIAACIAACIGCVAATXKhpcAAEQAAEQAAHjCEBwjWOJlEAABEAABEDAKgEIrlU0uAACIAACIAACxhGA4BrHEimBAAiAAAiAgFUCEFyraHABBEAABEAABIwjAME1jiVSAgEQAAEQAAGrBCC4VtHgAgiAAAiAAAgYRwCCaxxLpAQCIAACIAACVgl4jeBGvHlDD5+8oqcvX9GzsAh6Lv69DI+gVxFvKCziNYW/ervpUby4PhTfNw7F9fWhhPF8KVF8X0rM/xLEJb+kcSmOj49VGLgAAiAAAiAAAmYR8GjBffQ8gu49ekn3H7+kkKfhhjBIlTQepU6agNKmSEBJE/oakiYSAQEQAAEQAIHoCHic4L4If003HrygW6HP6cmLiOjK79L1ZEJwM6RMJP1LEA8tX5dg4mYQAAEQAAGbBDxGcEOehNOlu0/p7qMwmwU24yJLbTrR4s2aLgmlSBzXjCyQJgiAAAiAwDtOIMYF974Q2LM3H9Njk1uz9v7OLLh5MiYnvyQQXnuZIR4IgAAIgED0BGJMcMOEkdOZ64/pZuiL6EsZAzEyp05EuTMmpbhx0NUcA/iRJQiAAAjEOgIxIri3Q1/SqasP6dVrz+YZX1g8F8riR6mSxfPsgqJ0IAACIAACHk/ArYIrZvbQP9ef0LX7zzwejLqA2dMnoZzvJVEH4RwEQAAEQAAEHCLgNsF9KZqzR/8NIZ7q442OpxMVzupH8cT8XjgQAAEQAAEQcJSAWwSXF6k4eO4B8bitNzuet1s8RyrirmY4EAABEAABEHCEgOmC+/jFKzp0PkRaEcqRgnlq3ITx4lDJXKnEKlZxPLWIKBcIgAAIgIAHEjBVcEOfvqLDF0LoNQ/exiLHLdySOVOJ5SKxUlUs+llRFRAAARAwlYBpgstjtX+IbuTYJrbyr8GiWyp3arR0ZSA4ggAIgAAI2CRgiuByN/If50Io4nXsatnqSXK3sn/uVJQgLrqX9WzgBwEQAAEQ0BIwXHBZZH/75z6xVfK74HhlKn8xpgsHAiAAAiAAArYIGC64xy6G0p0YWA/ZViXNvpY9XWLKmSGp2dkgfRAAARAAAS8mYKjgXr3/nP659tiLcThf9BI5UlJKMVcXDgRAAARAAAQsETBMcMPFRvB7/r4X68dtLUHkMN7o/uN8qQkzdK0RQjgIgAAIvNsEDBPcv648ohshnrkRgbt+4jxis4MP0iZ2V3bIBwRAAARAwIsIGCK4T4RV8v4zD7yo2uYU1VfsLFTuwzRY/tEcvEgVBEAABLyagCGCyytJhTwN92oQRhX+gzSJKE+mZEYlh3RAAARAAARiCQGXBffhs1fSOsmxhIfL1Yjj40Pl86OV6zJIJAACIAACsYyAy4LLSzc+eILWrfq5yCrGcXnzejgQAAEQAAEQkAm4JLi8otQBjN3KLJUjj+V+Klq5ccQRDgRAAARAAASYgEuCe1psJn/lnvGbyRf6IAWlTp7ALb/Q/Ucv6cTlh4bnVTBLcsqQMqHh6SJBEAABEAAB7yTgkuDuPHWXwk3Y4/bTgumEWCVyC9GbIc9p58k7hueVOll8Kpbdz/B0kSAIgAAIgIB3EnBacO8+fElHLxnfMmSMZghu0MxgOnz0GA0e8C1lyvCe8muZJbicQYX8abFZvUIaJyAAAiDwbhNwWnD/Fks4XhNLOZrhjBbc02fPU5MWbZSiBn4VQO2/aiX5zRTcAu8np4ypPLtb+fnz5xQSGqqw8UuRghInxuIdChDdycuXL+n+g8g552nTCIv0eFjSU4dJ8ep5JUuWjJIldb9B4eMnT2IkXwUETkBAEHBacPeKHYGeh0WYAtFowW3YrDWdO39BU9bcuXJKrd0UaTOZ0qXMmWXwS0gFP0iuydcsz/UbN2jxkqWa5FsHtKJUKVNqwvSebdt30KjRo5Xg1gEB1KRxI8WPEy2Bffv306DBQ5TAFi2aU/OmTRV/TJ6wuAXNmEHh4a+sFiNdurSUM0cOypUzJ6VNm9ZqPKMu/HHoEPXrP0BJrn69etS+XVvFb/YJ/1306PkNPRAfSYkSJaLhw4ZSwQIFzM4W6YOARQJOCS5vvbf71D2LCRoRaKTgclfy9NlzLBYrSZIkFDxnLh26aLzhF2fIm9Rzt7I73I+TJ9P69Rs0WTUTQtBSCIItB8G1RSfqNb3gftmkCQW0ahk1YgyE3L5zh5o1b2F3zr6+vlSxYkXq1CFQEiO7b3QgYkwLbv/vB9LBgweVEqdLl44Wzp+n+HECAu4k4JTg3hRrJp8Uayeb5YwSXH1Xsr6833T7mj6rUtO0Fi7nx0s98kb1ZrpXr17R53XqUlhYmCab5MmT04plS8lHLMZhzUFwrZGxHB6bBFeuIX949undi0qXKiUHGXaMacFtF9iBLl68qNQnfvz4tGHdL4ofJyDgTgJOCe65m0/o4h1zWoVceaME11JXsgy3aJHCNHvaJDJzDJfzKpbNT0xxii9na8pxx86dNGLkKItpjxo5gooWKWLxGgdCcK2isXjB2wQ3e/bsSj0iIiLo5s2bUT7M5AhNm35JrVrY30KW77N1jGnBXbh4Mc0RvViyK1euHA3o953sxREE3ErAKcE9JqyT7wgrZbOcEYK7cMlyGjtxisUi8hf90gU/S9bKZgtu3kxJKUsac42QOnXuQmfPnrVYV39/fxo2ZLDFaxwIwbWKxuIFbxPcrZs3RanH/fv3aeeu3TRdjPfqXdBPUymHGOM1ysW04L5584Y2bd5Cx44fp5w5c1Cdzz+nuHHjGlU9pAMCDhFwSnD3n7lPT16YYzDFpXdVcK/fvEWNm7ehJ8Iy0ZLjruSmjRtIl8wW3MypE9OHmc2zyrx16xY1b9lKqSa3aB49ekT37kWOsa9cvoy4e9mSg+BaomI9LDYIrly7a9euU89evSSDIjksY8aMFDx7llglzZhhkJgWXLleOIKAJxBwSnB3/HWXXokN581yrgpumw5d6M+jxy0WL5f4yl0mWreyM1tw04ru5CKiW9ksN33GTFqxcqWSfGBge0lwFy1arIR91aYNNWr49gNDCfzvxF7B5XHiDRt/pVN//01nzpyRPmbee+890WrISfXqfEFZsmSRUnz27BkNGjKEuPuSHRvmsOVz3jx5JL/8P05v4qTJoovzhhTk4xNHdPX1oxQpIj8MHj58ROs3bqBz587RhQv/0t27dyl16tSUO3duaiqMlbjFoncTJv5I165fI+7F6NihA/G0nXXr19PmLVtEXrekKTxc5sqVKtKnFSrob1f8vwtDG24FnjhxgkJCQqT6FStaVGr9qa26rRlNsVXsr5s20z+nT0vl54Tff/99ypcvLzVq0ICS6qbG8PSs/t9/L+WfKFFi6tPrG6kO27ZvF70Q2+nUqb+JP6YC27ej/B9+qJRTfWLJaMpSC1d9z4mTJ6nnN73UQdSpU0f6onZtKWzFylV04PcDyvXeQqDTC8MjtVu/YaNgtVMK4t+Ryy5bQFsS3ObNmtLqtWvp5Mm/6LTgk0JMRStYsCDVr1eXsn7wgTppzfmly5dpy9atdP78ebp8+Yp07QMRP3euXFS1ShXKnDmTJj57Tpw4SXNVRlJ1vviCPi5bVhPvgfh9Fy1eIj3XV69epQQJEki/c968eYjjx8Q0Jk0BY7mHG0YX/v2X0qdPT++Jf7acWXFt5WnkNacEd/vJuxTx2jMF11ZXMoNbPG825c2dU2FotuCmSByX/HOlUvIz8uT169f0Rd16xC9r2XFr9pnwN2/RUg6iNEJ0Fi9coPjVJ/YI7r/C6GSAsPa8I6xgrTn1+N+kKVNp3bp1SlQ/Pz9atGC+Zr4qW4cvEuNrsitZsiQNHzpE9gpx30g/TQuyOt7IEdu3aye9pJWbxElTYaUrlzOXeBE/fCiGP6yUu1KlStT7m57q24m7IH8KCqI1a9Zqwq15LAnu7j17aPSYsVbLzoY7/b77lsqULq0ky/NE69arr/h7C9H6UyzUsm3bNiWMTwZ+PyCKYMgRnBFcvrfvd/3oyJEjcjJUtmwZGvSf+A/7YQTt3r1buTY9aBplz5ZN8fOJ3kJ+3NgxVEgIKDu94BYQU3KuXLkifRRKEVT/44+zwYMGkr94FtSOP97mzp9Pi4Uo2nIBAa2oSaNGGiPB6J7vXaJuI0eNVj4Q9enzb9VLPCMVypfXX4LfAAIrV6+ioKDIoY3SpcvQkEFvPzz1ybsat/c3PaJ86OrzMNvvlOBuPXFHvJjMK5qlFu7jx2LiejLbXbPRdSW3b9OKAtsGaAputuCyhTJbKpvh9h84QAMHRY7PFinyEY0eOVLKqn2HjvSv+GqU3cQJ4y22jKJ7IXGrom279nIyNo89e3SXWhpsLc3d3NzKk11D0cJuK1ra7PiF26ZtO/mSNCVloRBkuSUxOziYlujmFCuRdSczpwdR1qxZlVC14CqBNk5+GD6MShQvrsSY8tM0WitaX/Y6veBya+/HSZPsuj149mylVaYXXJ4zqv6QkhOcOyeYMmbIIHs1R2cFl1uNY8aOU9JST50xWnCVTGycLF+6hPgjTXZDh/9Ae8RHjD2uRo3q1K1LFyWqref7hjAga93mK6tiKycCQyuZhLHHffv3iTntQ6Mkyj0gLZprpzPyGHyv3n1ciltH9MR1DAyMkoY7A5wS3C3Hrbd0jCi8XnB5ek/bjl2Jx14/r1nNahaOdCXLiZgtuLw/bsVCaeXsDD3y+Bt3mcmuv+iSLV/uE8m7bsMGmiS6bGVn7aVh64XE93bo1El04V2Qk6HatWtRQMuWUnfnGWGoxYIvCyu3BpYsWig+jJLRadHt3LlLV+U+Ppk9c4bUrcofA+qpGiN+GE7FixVT4vLYYsB/4sxpNhYLcRQvWoxu3b5FS5Yu03xIlChRgn4QixnIzpLg1qpVS7QmS9Ht27el+3ncW3b58uWjSRMnSN579+5TE90iFtwK5u547mbk8dugoOnyrdJRLbjcBd5IdHXL3ekcoXu3blL3NZ/v2fubaPmOUa5zC/ynKW9/I73gcnzZsfjIhj7cU2Btmpezgmvpt9okuvK5xWmG4LI9wZdNGktDA2w1PX7CRIUJ17lunTrUQQyNsLP0ouXelI/LlKXXryOkbn/1kArfM23qVGW4wdbzrbdgriK6pXneekrB+8+jR6WhmgcPQmic+M3UQx2cB5zrBLgnafXqNVESyp49B02fNlUTbkRc7rJeMG+uJl13e5wSXHe2cLllW71OI8UA6stG9alX985ROK1d/ysNGva2dRflogjQdyXLccwWXJ4CW6mQdsxLztuVI1uaNv4ycoUjfjmu/2Wt8mLmsVSemys7vr5q5QpKLFpOamfrhXTwjz+o/4DI7h11y0dOg8deAoWAym5A/35U7pO3oq8fX+YxyGpVq9BU0YqUXdWqValn926yVzlyNza3hLmrWV1mFvdGTb5U4rEYcYtIdnrBVXdvchx9i53HetesWindPlG0TDeIFqrs1F2rctimzZtp3Pi3As1hasHVt46rV6smBFf70cFjomrrYP5NuGVvSXBTpUpFo0eNpA/+Gx+Xy2Dt6KzgWsp7/tw5xGP0RgsuP0NTJv1IKVUroB3845B4zgYo1eKPLHmubIBogV67dk259rX4APxcfPSp3fyFC2nevPlKUP78+Wni+LctdlvPN9sa7Nu3X7nPVu+BEgknhhGwJqLZsmWnGUE/afIxIq6l95cmEzd4/g8AAP//JUJyMgAAMvxJREFU7Z0HfBRV18ZPGgmEkgQIRaUGBBUsCBZe5RULSO+9CkpHpClVpEkR6UWkSq+CUv0UBQV9KYIgRaoFCJAGJCEJad89E2cyM9md3ezOpPFcfjAzt89/l33mnnvuHY+w2/dSKZNh3++3KCk5k4Uykf2VasFUKjA/RUfHUM++79L5Cxc1pRs3rE/DBg2gQoUKSvGcr0HzthQTE6PJJ1/06tGNer/dXb7UHEOj4uj7U7c0cWZeeHt5UN0niptZpVTXii++oDVr1ir1vv766zR86BDlmk9Gjh5DR44cUeL69etLzZo0Ua755Nvv9tHUadOUuLe6d6f27dpK10uXL6f16zcoaa1atqT69esp1/JJr959KDk57QvRoUN76t61q5SUlJREXbu/Rbdu2eYbFBREq1auoHz58slVOXXs2LmLps5v9uwmDw8Pqaw+7f/27slQZ8vWbeju3btK/N7du8jT05PeEfdx5coVJX7RwgVUsUIF5ZpPDh46ROM+Gq/EdWgv7rdb2v326dePLl68pKRNGP8RlSpVSrnmkxs3btLoMWOUuE9nfELVnniCosV3t0XLVko8nyxetIjKly8nzpwLNwXnToKNOti6f3U6n18PDaWu3bT/P7Zs2kiFCxemiZM/pv379ytFPlu0kCqUL69c88nsuXNpx46dStyMT6ZT9WrVpOvD4vs3SnwP5cDfoV7vvC1fSsfU1FRqLu49NjZWid/x1Xby8fGhem82UOL4e7L9y63k7e2txPHJvbg4atqsuRLH+XZ+/ZV0bfT9nr9wIW3btl0px9/HPr170X9q187QhpIJJ6YROHjooPi/NCFDfZ07daQunTtr4k/89hsNG/6+Jo4vMpO3efNm1Ld37wx1ZGWEhyuCe+BMOMUnpljWT1lwx4yfTDt27bXZTuVKIbRkwWxJdAcNH0n7Dxy0ma9kyRK0cdUyRZz1mawWXD8fT3r5sWL6Zt265h+oVm3aakRj9qyZ9FjVqpp6f/7lFxr74TglrnTp0rRy+TLlmk+MfpBGjBpNR48e1eR3dFG79os0buxYJdulS5eod99+yrX6ZP7cOVS5cmV1lM3zsLAwSRSuXw+l0BuhtHPnLs2979m1k7y8vKSyzgiuXlh379wh/cA2bNyE7t+/r/RBLeRypJHg6svLZYyO7w4cSI0aNsgguFWqVKG5s2cZFc2Q5qrg/vK//9GYsR8q9eXPn5++2valdJ0VgssN6R9Wlny+WHoIeqtHT6Vf/F3h74ytoP/ct27eJP7PFzL8fh8/foKGf/BBhur4u/T8889RCyHi1aunPThkyIQIUwhsEQ9QixYtVup64YUXaPy49O+ikiBO3M3LA5KCBdMGaep6s/LcJcE9eC6CYhOSLesnC+7hgz/QuIlTDNtgeJ3ataZFS5bbzbd4/iyqWeNpu+lWC25BX296sUqQ3fZdSTh67BiNGDnKlaK0aMF8qlixolLWSHD1wqQUMjipU6cOjR45QpNj4KD36OzZs5o4Hk2sX7tGGZlqEsUFWys2bt5Me/d+Q5GRkfpkzbUZgssj9EZNmir1qkVHiRQn9gSXy9dv0FCd1anzIUMGU/033shWwV2+ciWtXbtO6e/jjz9Osz6dIV1nleAO/2AEHT9+XOnDtClTKD4hXvPA+OKLL9JHH6Y/zCmZxcmAdwfRuXPnlKi5c2ZTlUcfNRRczrzws8W0detWpZz+pGbNmpIA6EfV+ny4dp0A/1+/KB7MS5YsSSVLlDCsyKq8ho2amOiS4B69FEWRMYkmdkNblTzCnT5zLq3dsFmbmImrDm1b0bD3BhiWsFpwixbKRzUqBBj2IbOJo8aMpcOHD2e2mJS/Xr16NHTwe0pZI8EdP3ES/fjjj0reYeIJsXgxY/N4BWGCLVKksFLmt5Mnaeiw4cq1+qTXO+9Qq5Yt1FHSeXh4hDTiuX37doY0WxFmCC6Pat6o/6ZSPV9zvfpgT3A5X7MWLTVmURYNo+Dp5UmPP/aYNLrWm5SzaoTL7bZr30Ezsm/WrCn169NH6npWCW6vPn3p8uXLCq6lYoSbIKwNffv1V+J4tDlj+nTlWn3yVs+36Z9//lGi1q5eRcWLF3couFyAzZWrxfTMb+JoKzRt2pT6903jYSsdcSDgLAGXBPfM1Wi6GhHnbBuZzicLLhfcvmO3w5GurQYcmZLlMlYLbpmiBajKw+aZMe7cuSvMyW3k7mf6yELC5kJ53tRIcNeIUc8KMfqRwzgxuqgtRhnOhoSEBOrQqbPG/Ksuy31ZIUzc+qfa9h07UXh4uJL12WefpTfF3DHPdQYEBND7I3g0dEJJN0NweQSjn9tlTjzSVQcjwR00eAidPn1ayc7zjQUKFFCujU6yS3A/mfEp7f3mG03XVq5YTqX/nXue9PEU+uGHH5R0HvnyCFgdzJjDbdq8BcWJuVg5sJlfb3Vgq8iGdel+C3JenmJh64Q8HaB+WDL6fsvl5SOPng6IB0z+3qv9Dvg7t2nDejkbjiDgMgGXBPevsHv0x3XbDkou90RVUC24HH3u/EXq2WegZvSgym7z1JEpWS5kteBWfaggPVLMuR9duU9Gx/UbN9LSpenzsOWFA8vC+fOMikiipzbLymZMLmT0g6Sf2+O2PhOORLKDkrpRdpDSm91mzp5Du3btUrK1aNGC4sWP6q7du5U4/Uju6tVr1L1HDyW9bt26NOJ97QiZ592sENy+/QfQhQsXlLYHvTuQGjZId9rhBL0jmdppat6ChbR9e7oTTksxeu8tRvG2gp5XVgsuO41NnjKVjonpCXVQO81x/OIlS2jTpnQrUzvhUNdDONapw4RJk+nAgQNKlJHTlC0mh37+mT4c95FSXi1w+ocg2clMySxOfjp4kD4aP0GJevjhh2n50iXStdH3WymgO2Gh7yKcyGTRVQu4LisuQSBTBFwS3Ii79+nYFefMfZnqzb+Z9YLL0Sy6Y4UT1QWVF6i9up0xJctlrRbcmhUDKbCgj9yc28e2wvynFs8B/ftTk8aNDOv9YvVqWrVqtZKHzb4snByMfpBSUlKoc9duyg8P52enqMGDBkkerHx95cqftHLVF3Tw4CHJweQT4fHMgnzq999p8JChnEUK/CPKZr5EIcxswlSPZtTCpjdB6+ftvtu3j6ZMnSZXKx3NGuHqH2bYCjB92lTJGY0dkjZt3qIRVG5cLbi2nJa6CY/tdm3bSE5dPBI7IpzQli5bLplPu3fvRh3atZPuwSrBHaWaT+fP88+//qLz5y/QqVOnlBGh1AHxDwvVsiWfax6o9uzdSzM+nSlnkT73sWNG05PVq1NkVBQtEnOg33//vZLOJ0aCy+L1kXCKea5WLanMRfH/efDQoZrvQ2/hKdyyeXMpfeu2bbRw4SLpnP/x9/eXPpNKISFSHFsUeP5XHt1y5AfiAe1V8aDGwej7HRERQfyQVLZsGWrburVizeCHIf7ey1aWsmXL0pLFn0n14R8QcIeAS4KbLH44vjsZ5k67hmVtCS4X4OU/PcRI10h0+T/k7m0b7Xol6xu2UnA9RGOvVQ8WP2D6Vl275h8XNluqgzNmyzBhnu0gzLTqsEyMAB4RP7BGP0ic/+zZczRQCKw+MOfExETNDx3n4R/LRmJU2KlLV1LPwfLcm+zxqRdN/hFmMWaTYXR0NLVo1VrTHJswWQzOnDmjmaeTM5kluPHx8ZJZWf3jLbdh76gWXM6zdv16Wr58RYbsvMSGl73w6Ekd5GU2Vgmuui2jc7Y0jB09Spr3VOfjkXCbdu0z9Js/M/29yOWMBFfOww8zfn5+GaYb+Hu1eeMGxVrCDyk8P3v16lW5qHSUp0T0n5Xek9no+z1k2DA6efKUVB/fT40aNSQv1l9//VXz3e3apQt16thB0z4uQMAVAi4JLjf0y/lIuhuX5EqbDsvYE1y5oNFyoU+nTqRX6rwkZ3V4tFJwA/19qGZIoMM+OJtBb7pjD8rJE9NNaUb16M2lTcV63P5iXa7RD5Jc305hFp47b77dH1g5X0hIRZo+dSotW7GSvv76azmaXnvtNXp/WPpolxP6DRgoRlrnlTxPP/0UyU5GH4p1rofEeld7gb0Zb9y4oSSbJbhcof5hQGnk3xN+aJB/pDlKL7g8ipw9Z67GbK6vQ75u3LgxDRCfAVsEsktwWWgGDhhADd6sL3crw3HDxk20ZOnSDPFyBFsvNA9XButw5TK2jiy2bCHh75E68DphXt72lxidG4VKlSoJj+JxVKxYUSWbve83CzWPYtXWIqWQ6oT7smDePM2oX5WMUxDIFAGXBfdCaAxduXUvU405m9mR4HI9a9Zvok9maecuGzWoRxPGjnS2GSmflYIbUsKfKpT0z1R/7GXmH/IGjRorosfOPDPFpgnqJT72ynI8m2pHinW18oiAf9y2bd0i1i//SBMnTVKK9u71DrUUc636wGthZwkhYVOk2hzM+djk1qZ1K3rt1Vfpb+Ep+vY7vZTiLI48iiugcz7iH9HewjNVXdck8fBQSzxE8EYGLPDffvutUg+fBAcH09s9e0gbE6g31JA3ruA8HH/9+nU+lcy4LMb6oBd7tWBzXhbUqWJELs/hcRyPUDt37iRtHKJ2NNILLuflwCb1BWJjBTa5q0eCLHBPCOevrl06S05gablJ4tBEtXmDkUeuXEZ/tGXS1ufhkWG5cuXoUbFkJkQsD3vxheclRzR9Pv01P4jwg4T685KZvCEeqPoPfFexPtgb4fK983dh+YoV0hSE3AZ/l5966kka8t57wsO9iBytOfJId6OYS96xc6fmYYsz8fry5sKzupnwJtYHo+83O/V9KUzW27/6WjEfy+X5/0enjh2lernfCCBgBgGXBfd2bBIdvmi8PtLVDjojuFz3kWPHpTW4bGquK0a19naTMuqHlYL7wqNBVMjP26j5XJnGZkYeYeYXHrjBYumFr6+vJffBJutr165JDwnFRDtBgeZZC5zpMIsLLzUJCiqqGTU5U1adh4WbR4AsUPzQwLta5dbA9xEaeoOCigZRCXEvrgZ+qAoVD128lj6z9fDDJ38veK7m4YceMmX0yd7//FApqpQEXO+d7up9ohwIqAm4LLhcyf7T4ZSQlKKuz5RzZwXXjMasElx/Xy+qXSXdtGVGX1EHCIAACIBA7iXgluBevBFLl2/Gmn73eUFwK5cqSOWCzVsOZDpkVAgCIAACIJClBNwS3Htie8efxDaPZoe8ILh1HhOmVh+T3JPNBoz6QAAEQAAEspyAW4LLvT1+OYrCos3d5rFEgB/55csaR4X4+8l083a8qeBLB/rRE2XStzc0tXJUBgIgAAIgkCsJuC24d+OSxRIh80e5uZLmv51+qWpRyp9FDwy5mRP6DgIgAAIPEgG3BZdhHbt8myKi7z9I3Ozeaykxuq2G0a1dPkgAARAAgQeVgCmCGx2fRD//Yc0Sodz0wfCSgpeqFiN+By4CCIAACIAACKgJmCK4XOGZf8QbhCLT3/ahbuRBOa8gNroIMWmjiweFGe4TBEAABB4UAqYJbmJyKh04E07JKakPCjvNfebz9iD2TOZRLgIIgAAIgAAI6AmYJrhcMb8jl9+V+yCGZ8oHULHC+R7EW8c9gwAIgAAIOEHAVMHl9k78eYdu3Ulwoum8k6WMeN9tFfHeWwQQAAEQAAEQsEfAdMFlk/JBsRlGfKL5Wz7au4nsjC/k50XPVS5KnjAlZ+fHgLZBAARAIMcTMF1w+Y7v3EuiIxejKEW84SMvBx8xb/t8JV5zC6/kvPw5495AAARAwAwClggudyyvi26a2AZhgwszvoWoAwRAAAQeAAKWCS6zi4pJlDbFyGsjXRbbWiFBxG8EQgABEAABEAABZwhYKrjcAR7pHr0UlWeWC/GmFrUqBWFzC2e+XcgDAiAAAiCgELBccLmlGLET1REhuolJuXtOl0e0z1YMwluAlK8PTkAABEAABJwlkCWCy52Ju59Cx69ECfFNdrZvOSpfUEEferJcAPl4wR05R30w6AwIgAAI5BICWSa4zIOdln//+y6Fmvw6PKtZVxTbNVYU2zYigAAIgAAIgICrBLJUcOVO8o5U567F5PhlQ77enuLNP0UoqJCP3HUcQQAEQAAEQMAlAtkiuNzThMRUOn31DoXfzZmv9XtE7B5VubQ/eWFzZJe+WCgEAiAAAiCgJZBtgit34+btBLpwI4buJeSMud1Afx8htIWoSAFvuYs4ggAIgAAIgIDbBLJdcOU7iBAj3SthsRQp1u5mdWA3qJIBflQ22J8K58fa2qzmj/ZAAARA4EEgkGMEV4Z9734yXY+Mp9CoOMmzWY634sjiWiowv/SXX6+HAAIgAAIgAAJWEchxgqu+0duxSRQRnUDh4i9voOFu4BcMBAiTcbFCvhRcxJcKYKcod5GiPAiAAAiAgJMEcrTgqu8hSbyF6I4wN8ckJImRbzLFieN98dJ7fvF9YnKKsqkGj1R9vDzJW6yXzZ/PS/nr7+tNgWItLQIIgAAIgAAIZAeBXCO42QEHbYIACIAACICAWQQguGaRRD0gAAIgAAIgYEAAgmsAB0kgAAIgAAIgYBYBCK5ZJFEPCIAACIAACBgQgOAawEESCIAACIAACJhFAIJrFknUAwIgAAIgAAIGBCC4BnCQBAIgAAIgAAJmEYDgmkUS9YAACIAACICAAQEIrgEcJIEACIAACICAWQQguGaRRD0gAAIgAAIgYEAAgmsAB0kgAAIgAAIgYBYBCK5ZJFEPCIAACIAACBgQgOAawEESCIAACIAACJhFAIJrFknUAwIgAAIgAAIGBDxuhEelGqQjCQRAAARAAARAwAQCEFwTIKIKEAABEAABEHBEACZlR4SQDgIgAAIgAAImEIDgmgARVYAACIAACICAIwIQXEeEkA4CIAACIAACJhCA4JoAEVWAAAiAAAiAgCMCEFxHhJAOAiAAAiAAAiYQgOCaABFVgAAIgAAIgIAjAhBcR4SQDgIgAAIgAAImEIDgmgARVYAACIAACICAIwIQXEeEkA4CIAACIAACJhCA4JoAEVWAAAiAAAiAgCMCEFxHhJAOAiAAAiAAAiYQgOCaABFVgAAIgAAIgIAjAhBcR4SQDgIgAAIgAAImEIDgmgARVYAACIAACICAIwK5RnCTU1PpTkwSxSYk0b37yRQn/iYkJlNScirdT06hxKS01/r6eHtQPi9P8vbyID8fL8qfz4sK8F9fbwoo6E2eHh6OmCAdBEAABEAABEwnkKMF925cMoXfTaCI6ASKik005eaDCvpQ0YK+VLyILxX08zKlTlQCAiAAAiAAAo4I5DjBjU9MoeuR8XTjdhzFxCc76r9b6YWE4JYKzC/99fXByNctmCgMAiAAAiBgSCDHCG5UTCL9GRZLYXfvG3bYikSW2mAx4i0X7E9FCnhb0QTqBAEQAAEQeMAJZLvgRgiBPR8aTdEWj2ad/ZxZcB8tXZgC/CG8zjJDPhAAARAAAccEsk1w7wsnpz+uRVPo7XjHvcyGHA8XzU+VSxckb0+YmrMBP5oEARAAgTxHIFsE9+btBDr9zx1KSsnZPPMJj+fqZQIoqJBPzu4oegcCIAACIJDjCWSp4IqVPXT2WgxdjbiX48GoO1ihhD+FlPRXR+EcBEAABEAABDJFIMsEN0EMZ49fjiJe6pMbAy8nerJcAPmI9b0IIAACIAACIJBZAlkiuLxJxf8uRBLP2+bmwOt2n60YRGxqRgABEAABEACBzBCwXHCj45PoyMUoaUeozHQsp+b18/GkWpWCxC5Wnjm1i+gXCIAACIBADiRgqeDejk2io5eiKIUnb/NQ4BFurZAgsV0kdqrKQx8rbgUEQAAELCVgmeDyXO1hYUbOa2Irfxosus9XLoqRrgwERxAAARAAAUMClggum5EPX4ii5JS8NbLVk2Sz8nOVg8jXG+ZlPRtcgwAIgAAIaAmYLrgssj+djSD2Sn4QAu9M9ZyY00UAARAAARAAASMCpgvuiSu36VY27IdsdJNWp1UILkAhpQpa3QzqBwEQAAEQyMUETBXcfyLi6OzV6FyMw/Wu16wYSIFirS4CCIAACIAACNgiYJrgJooXwR84E57n521tQeQ4ftH9f6oWJazQtUcI8SAAAiDwYBMwTXB///suXY/KmS8iyKqP+FHxsoOyxQtkVXNoBwRAAARAIBcRMEVwY4RX8qE/InPRbVvTVS/xZqGXHyuG7R+twYtaQQAEQCBXEzBFcHknqajYxFwNwqzOly2Wnx59qJBZ1aEeEAABEACBPELAbcG9cy9J2ic5j/Bw+zY8PTyozuMY5boNEhWAAAiAQB4j4Lbg8taNkTEY3aq/F+XEPC6/vB4BBEAABEAABGQCbgku7yj1M+ZuZZbKkedyXxGjXE9xRAABEAABEAABJuCW4J4TL5P/O9z8l8lXL1uEihb2zZJPKOJuAp38647pbVUrU5hKBfqZXi8qBAEQAAEQyJ0E3BLc70+HUaIF77h9pVqwEKv8WUI0NCqOvj91y/S2ihbKRzUqBJheLyoEARAAARDInQRcFtywOwl0/E/zR4aM0QrBXfT5cjp6/AR9NGYEPVSqpPJpWSW43MB/Hy+Ol9UrpHECAiAAAg82AZcF94zYwvGq2MrRimC24J47f5Had+mhdLV3z+7Uq2c36dpKwX3ikcJUOghmZQU8TtwmcPfuXYqJjZXq8fT0pJIlSih1pqSk0I2bN5Xr/H5+FBgYqFzjBARAIHsJuCy4P4o3AsXdT7ak92YLbptOb9GFi5c0fa1cKUQa7RYp/pAlJmVurFSAH1UrW1jTrrsXCQkJtGjxYkpMTJKq8i9QgDp36kgFC2bOKzouLo5WrlpFMTFpP95c2Vvdu1EQfqDd/Yjo2vXrtG79Bk09ZrGdPXcu7dixU6l79qyZ9FjVqtJ1ZFQUtW3XXkmrXr0azZg+XbnGCQiAQPYScElw+dV7+0+HW9ZzMwWXTcmfLV1hs6/+/v60fMVKOnLFfMcvbpBfUs9mZTPDzVu3qFPnLpoq673xBg0dMlgT5+hi4WeLaevWrZpsSz5fTGXLlNHE4SLzBPSiyDV06tiRunbpnPnKdCX0dc/4ZDpVr1ZNygXB1cHCJQjkMAIuCW6o2DP5lNg72apgluDqTcn6/g4d1J/q1mtk2QiX2+OtHvlF9WYFW4LLda9csZxKlyrlVDORkZHUtn2HDHkhuBmQZDoiKSmJmjZvQffv39eULVy4MG3euIE8xMYo7gQIrjv0UBYEspeAS4J7ITSGrtyyZlTIOMwSXFumZBn3M08/SUsXziEr53C5rRrlA8QSp3xys24f7QlurVq1aNKE8U7VP3XadPr2u+8y5IXgZkCS6Yh9339PH0+ZarPc1Ckf0zNPP20zzdlICK6zpJAPBHIeAZcE94TwTr4lvJStCmYI7pr1m+iTWfNsdpFNyRtWL5O8la0W3CoPFaQyxcx7g5A9weUbnT93DlWuXNnmPcuRV69eo+490h3I5Hg+QnDVNFw77zdgIJ0/f95m4eeee44mjv/IZpqzkRBcZ0khHwjkPAIuCe6hPyIoJt4ahylG5K7gXgu9Qe069xAOQTE2ibMpuWO71lKa1YL7cNEC9NjDmXNostnpfyONBJfFlkXXKIwcPYaOHDliMwsE1yYWpyNv3LhBnbt2U/JXqFCB2Ks4PDzd32HLpo3E5mVXAwTXVXIoBwLZT8Alwd33exgliRfOWxXcFdwefQbSr8d/s9m9SiEVaaMY3crBasEtLszJTwuzslnBSHC5jY8nT6Jna9Sw2RyPvHgEZi/YEtzk5GTas3cv/X76DF26dImuXbtGfmK5SaVKlah+vTfov3XqZKjuq6930P4D+8V8pSfVfeW/1ODNN+mfq1dp565d9N13+4iXr/z3v3VoQL9+mrJhQpi++eb/6Oy5c3ThwgXi+dDy5cuLUXslerNePXrkkUek/PeEh/XYD8dRamqKdP3UU09RZ+GUpA48hzpi1Cgl6plnnqGO7dM9eDmBnYzWrltPf/zxB/3zzz/k6+tLFStWpCpVHqXmzZpRoUx6fn+2+HPavGWL0mbv3r0kwV27dp0S11NYF9q2SXvYUyJ1J6mpqbT9q6/oyNFjdPr0aYlXuXLl6PXXX5M+g507dyklXHGaYq47d+2m02fOSPfOD6YlS5akkJAQatm8GZWx4Tg3c9ZsunrtKnl5eVF38VBRtWoVOvHbb7Rr9x765ZdfpOVHbdu0EZ91faVvOAEBZwjw9+/S5ctUQixxUy9zs1XWqry22rIiziXB/e5UGCWn5EzBNTIlM8B1XyylKpVDFJZWC26RAt70XKUgpT13T/SCy6NatQmzdOnStGLZUpvOOXpzJ4smC5sc9IJ76vffafLHUzQjNDmvfHzxxRdp3NgxmvZmzJxFe/bskbIEBASIpSnT6J3efYjFWw7BwcG0ZtUX8iXt+/4HmiaWsKjzKIn/nrBYtWndisIjIqhDx05K8tNiXnSamB9VB1721KRZcyWK73XBvLnK9Q/799OUqdPstpcvXz4aNnSIzQcKpRLVCT9ENGvRkrhdOfBolh8OOnfpKkdRsWLFaN2a1cq1/iRa/PiMHDWazomHDmdCZgX38pUrNGbsh3RLeLvbCx07dqBuXbSe8B2FZ7xcpm7dulTz2Wdp6rRpmioaNGhA771r/4FOkxkXICAIbPlyKy1atFhh8cILL9L4cWOVa/WJu3mHDx2c6eWT6vbNOHdJcP/v5C0xujCjedt12BrhRkfHUKFCxqZZR6bkXj26Ue+3u2satVpw2UOZPZXNCnrBbdasKfG87NGjR5UmPnh/OL0qfhTV4eixYzRiZPqIr0qVKvT000/ROjHCk4NacI+fOEHD3/9ATjI89uvXl5o1aaLkUQsuR7IJlU2r6lC7Ngt12n+sbWI0N3/+AnWy3fNlSz4nv/z53RLc66Gh9FaPnnbFVm785ZdfpjGjRsqXhsdDP/9MH45Ln59lttOmTJHK9OrTly6LJ3g5zJr5KT3+2GPypeb4Vs+3pdG2JtLgIjOC++dff9Hb7/QyqC09acjg94QFo54SoRZcfhjRe2FzxncHDqRGDRsoZXACAkYEDh46SOM+mpAhC+8r0KVzZ008W1OGDX9fE8cXmcnbXFhv+vbunaGOrIxwSXC/+c3+07EZndcLLi/vebvvu8Rzr00bvWm3icyYkuVKrBZcfj/ua9XNW4trS3CbNm6icYRigduwbi15e3vLt0ldu79F18WGDHLgud6fDh2yK7hsduQfWV5CxIHX+r722qviQSuVdgiT5oEDB+SqiH+Ad379lXKtF1wlQZw8/PDDFCVMue+83VMyNfOIrp1YoqT+AX/yySfFutUO0jKni8KMvWLlF3RFjMw6d+5EXTp1IjY9uzPCXbNuHa0Q66/lUE8IC6+RDRSj8V+PH5fMwpGRUdKmEUWKFJazGR6HDBtGJ0+eUvKMFubsOi+/JF1/vXMnzZmTPrq2J+T7D/xIEydNUurgk9693qGX/vMfunfvnhgNbFMsB3KmzAhuH2HCv6jaAKZJk8bCPNyV2InwDzHdwA8M8ufNn+n6tWvEQ24hqSm14Mpt85Hz8aidP9M5s2dRubJl1ck4BwG7BBYsWkRfiu+0PlSoUJE+WzhfE21GXjZZr/4i/f+9poEsunBJcLNyhMsj2wbN2yoOUB3atqJh7w3IgGf7jt00bmLaiCJDoojQm5LlPFYLLi+7fL16sNyc20dbgtuvTx+aOv0T+vbbb5X6+Ye6ZYsW0vX3P/wgmYblxJo1a9LkiRNo2YoVdgWX8/KP769i/+knxY5FxYtrHxpat21Ht2/flqukDevXKbtU2RLcbuKHvVXLFtI8qVJInPCuWVu2bFWieHekT4SpUr9eledu5N203BXccePH08GDh5Q2M7OGWSmkOokQJu52HdLnkHmec8dX25UHHhZLXpsrB07fumUzFRAjdXVghyt2vJLDIGGebSjMtOowYdJkzcOOs4L7v8OHafSYdFOd3qTPbfA8Wm8xGpfDmNGj6OWX0h4abAnuxAkTqFbNZzN8VnJ5HEHAiIA9ES1fvgItXqS1eJmR19Z33qh/VqS5JLj7fr8lnKas6E5anfIIl8W2pxjZnr9wUdNY44b1adigAYqJWS/KmsziwpYpWc5jteB6e3lQ3Se0YiW37crRnuDqdxnikQdvtMBHFgO1OC5fulSMNB9yKLhG/Zs5ew7tEk5QcuAtBFksOegFV20+lvPLR/288pxZsySHHDnd1tFdwZ2/cCFt27ZdqTooKIj6CAen/9SurYikkujEyYovvqA1a9YqOV9//XUaLuZ/1UHvHa43w7NF4c2GjZQi/LltF/NbaisFJ7rqpbx0+XJar9puslXLllS/frrJWG64l2quvUOH9tIImNP0ggvzsUwMR1cJwKTsJLkDZ8IpPjHFydyZzyYL7pjxk2nHrr02K+C9kJcsmC2J7qDhI4VX7EGb+UqWLEEbVy1TxFmfyWrBzYo5XB7hctB7ybLzS7GixWj2nDnKbbPDywgxx8vB0QhXKSROeA722rXrFHojlELFsqufDv6kMU9OnjRRcqThMnrBnfXpDHr88cfV1Snn7GgU++9m/Bz5zZ7dDkdM7grucTFqH/5BxvlpHnk+//xz1EI4W8kPD0pH7Zywib1Vm7aaOWr1/sZysZ+FJy97VsuBndtWLl8mX9Jff/9NPd9+R7nWO3nJCa4K7gjhiKWe55frMzqqH5T0gvt/e9Oc4ozKIw0EHBHI6Aj1gnCa+tBmMXfz8kOwbCWz2UAWRLo0wj14LoJiE6wb4rLgHj74g6GJmNkwvE5iPe2iJcvtolo8fxbVrGF/dx+rBbegrze9WCXIbv8ym2BvhMv1sEdsa/HjL8+H8iiJl/CoHZZ4Xq5o0aJSs44Elz1vdwtvY17mo3b6sdVnQ8G14yTEHsn1GzRUqssvTKxfbftSubZ34q7gcr229pJWt8dmd/6Prx9hqvPwud4ZTZ9udL1owXxpGRLn0QvyCy88L9ofl6G4q4LLXuI8D56ZUEcs+Ro9coRUBIKbGXLImxkCPF3Evhq8NM2ZZUFW5M1Mf93J65LgHr0URZExie60a1hWHuFOnzmX1m7YbJjXKNHefK+6jNWCa/aL6I0El+9rw8ZNtESYjG0F9miWR8OcbiS4bOIcOXo08WjQmeCK4HK9DYXDl/yAwNfOjJzMEFxuiz0fVwtT8G/iaCs0bdqU+vdNsx7YSue4UWJe9LCYH3UlsLPWUOENzIGXYA0eMlSpRu3lrESKE1cFd/zESfTjjz8qVfGSp+LFjKc6eOMO2WkMgqugwwkIuEzAJcG18l24fCey4PK5I2cozmMrODIly2WsFtwyYqepKhbuNKUXURZKNnGqzbR8r2wu3STmdNWbORgJ7iefzqS9YsMLObAJtFWrlsJaUENyoNosHJ3Uwu6q4OqXzKwSXoSOnnLDwyOovWqjC17iNFd4yKqDo3W46rz8hH1AiNEasUGFvNaU03kN8aYN69VZNed37twVrNto4jJzwZ8Jj+jZEqF/iNCbnOV6XRVcvrcVK9M9NMd9OJZqizXUzgYIrrOkkA8E7BNwSXD/CrtHf1y3vW2i/aacT1ELLpfiZUE9xe5RehExqtGRKVkua7XgVhV7KT9i4V7KesHl+9rzzTc0Y8an8i1Kx65iIwNeaqMORoLLm0bImzjwso9VK1dozKv6kbSrgqt/kULjxo1pYH/tDlTcZ36QkM27egcjTudlSSxccggLC6MOnTrLl9LOWOqNL5QE1QmbuLt0666ILgvinl07VTm0p+s3bqSlS9PnYXlXrIXz52kz6a64T/LSG04aIl6rWP+NN6TlVm/U1y5503tPc/8GDR6i2RTDWS/lX/73P2nDC7k73NfPFi6wOV+uZi3nh+DKJHAEAdcJuCS4EXfv07Er6UtCXG/edkm94HIuFt2x4ydneJG8rRqcMSXL5awW3JoVAymwoI/cnNtHRyZlboAdeVg45CUmvM5yo1i2oxYkzmdPcHnutt6b6ctRuPyXYhmLvFSHt3gcMmy45gHIVcG1td1kP2HGbSo20uD2eJ3uZ+LdvXvFQ0SjRg3p3QFpS8Jatm6jmZvmBw/e3pH7ekRsAsI7ZMkPDHyvaickXsYzb8FCKlu2DLVt3Zp47pgDCw0vzZH3Pi4r1pQuWfyZlGbrH37FoVo8B/TvT00ap3sa2yrzxerVtGrVaiWJzbYsfByGioX9avM2t887aAUGBhLvEDVLeIbrd6ByVnD5M+V7U4/g2Slq8KBByt7OV678SSvF7l+8ZEq/PAuCq3xkOAEBlwm4JLjJ4gf9u5NhLjfqqKAtweUyvPyHN7e4oFq8r6+Lf3B3b9to1ytZn99KwRVLcMWmF8FCOPStun7tjOBy7Wx23bZ9u1i+lSSt5XxEbDihD/YEl/O1F1snysLD17xhRdWqVenmzRuaDR44jYOrgstl9aNcjuPRZZEiRTSCxvETxNt2nhdv3Vn8+RLatNn5+X214Ko3qeB2aggzOTvg/frrr5rlU7asAtwHDrzHMY821YGX8RQoUEAdleFcbzrmDMuWLiH+fM6cPUvvDkqb081Q0E6Es4LLxc+ePUcDhcDqA/+fSUxM1Mylcx7eC7pl8+ZSdgiunhquQSDzBFwSXG7ml/ORdDcuKfMtOlHCnuDKRY2WC306dSK9UuclOavDo5WCG+jvQzVDAh32ITMZnBVcZ+o0Elz97kj6+tijUB5Bc5o7gsuj2FHiLUZnheAYBRbGCR+NIx8fH8kjm3ebsjfNwELKf2WHLFlw+ZpHeuqRqa02Q8RLLhbMm6eM6vV59BtQyJuJ6PPZuu7bf4BmD2sezfcX22Ny4JcE7Nq921YxKY5HnuodrTIjuFwBv0Bi7rz5Dre15PufPnWqsowCgmv3I0ECCDhNwGXBtfIl9I4El+/O1ksKGjWoRxPGOrf3rUzISsENKeFPFUr6y02ZcrRScPVzhjxHyVsg8tyhHNj8ys5THdq1o+linnjfvn1SEu8bzJ61HOaJfZH5bTdycOY9vZx3y9attHHT5gxiyG8J6iTMxa+INwzJZm3Oz05Lkz6enMGTmoV50MABdOLkSWUuWxZcLpeQkEBfbtsm+vi1ZhTPaTza47aaCxM1C7atwObZBo0aK1yYycwZnyhLfGyVUcf9JvrFLyiQHwa4zW1btyhZmAO/xUi9nIvNyyzKj4qXVfBmIfx2Iw5qwY2OjqYWrVor9TCHKeLtUfrA89uzxFaTp06d0pjdOR+3wy+IeO3VV8nT01Mpqt4alLkYzW0rhXACAiCgIeCy4N6OTaLDF9P22dXUaMKFM4LLzRw5dlxag8um5rpiVKt/MYEzXbFScF94NIgK+Xk7040cm4fng0PFdoN3bt+hIgFFqJQY2apFz4qOx8fHS6/z8xVOULylpDzHaq8tfiDgjSM4cP8c5VfXw6LNAsRmf/YMzkxZdT1WnPMonPd0Dg4ursyzmt0OizpbKvILU3iwYM2vKEQAARCwhoDLgsvd2X86nBKSzN9xylnBNQOJVYLr7+tFtaukbTBhRj9RBwiAAAiAQO4m4JbgXrwRS5dvxppOIC8IbuVSBalcsLEDjengUCEIgAAIgECOJeCW4N5LSKafxDaPZoe8ILh1HhPmOR8T3ZPNhoz6QAAEQAAEspSAW4LLPT1+OYrCos3d5rFEgB/55bPtsGI2nfj7yXTzdryp1ZYO9KMnyjj3HlVTG0ZlIAACIAACOZaA24J7Ny5ZLBEyf5SbY4k50bGXqhal/Fn0wOBEd5AFBEAABEAgBxBwW3D5Ho5dvk0R0fdzwO1kfxdKidFtNYxus/+DQA9AAARAIIcRMEVwo+OT6Oc/rFkilMN4GXaHl5a8VLUY8TtwEUAABEAABEBATcAUweUKz/wTTVcj49R1P3DnFcRGFyEmb3TxwEHEDYMACIBAHiVgmuAmJqfSgTPhlJySmkdRGd9WPm8PYs9kM/dNNm4RqSAAAiAAArmJgGmCyzd9NSKO+F25D2J4pnwAFSuc/nq4B5EB7hkEQAAEQMA+AVMFl5s58ecdunUnwX6LeTCljHjfbRXx3lsEEAABEAABELBHwHTBZZPyQbEZRnyi+Vs+2ruJ7Iwv5OdFz1UuSp7Y4yI7Pwa0DQIgAAI5noDpgst3fOdeEh25GEUpYuP7vBx8xLzt85V4zS28kvPy54x7AwEQAAEzCFgiuNyxvC66aWIbhA0uzPgWog4QAAEQeAAIWCa4zC4qJlHaFCOvjXRZbGuFBBG/EQgBBEAABEAABJwhYKngcgd4pHv0UlSeWS7Em1rUqhSEzS2c+XYhDwiAAAiAgELAcsHllmLETlRHhOgmJuXuOV0e0T5bMQhvAVK+PjgBARAAARBwlkCWCC53Ju5+Ch2/EiXEN9nZvuWofEEFfejJcgHk4wV35Bz1waAzIAACIJBLCGSZ4DIPdlr+/e+7FGry6/CsZl1RbNdYUWzbiAACIAACIAACrhLIUsGVO8k7Up27FpPjlw35enuKN/8UoaBCPnLXcQQBEAABEAABlwhki+ByTxMSU+n01TsUfjdnvtbvEbF7VOXS/uSFzZFd+mKhEAiAAAiAgJZAtgmu3I2btxPowo0YupeQM+Z2A/19hNAWoiIFvOUu4ggCIAACIAACbhPIdsGV7yBCjHSvhMVSpFi7m9WB3aBKBvhR2WB/Kpwfa2uzmj/aAwEQAIEHgUCOEVwZ9r37yXQ9Mp5Co+Ikz2Y53ooji2upwPzSX369HgIIgAAIgAAIWEUgxwmu+kZvxyZRRHQChYu/vIGGu4FfMBAgTMbFCvlScBFfKoCdotxFivIgAAIgAAJOEsjRgqu+hyTxFqI7wtwck5AkRr7JFCeO98VL7/nF94nJKcqmGjxS9fHyJG+xXjZ/Pi/lr7+vNwWKtbQIIAACIAACIJAdBHKN4GYHHLQJAiAAAiAAAmYRgOCaRRL1gAAIgAAIgIABAQiuARwkgQAIgAAIgIBZBCC4ZpFEPSAAAiAAAiBgQACCawAHSSAAAiAAAiBgFgEIrlkkUQ8IgAAIgAAIGBCA4BrAQRIIgAAIgAAImEUAgmsWSdQDAiAAAiAAAgYEILgGcJAEAiAAAiAAAmYRgOCaRRL1gAAIgAAIgIABAQiuARwkgQAIgAAIgIBZBCC4ZpFEPSAAAiAAAiBgQACCawAHSSAAAiAAAiBgFgEIrlkkUQ8IgAAIgAAIGBDwuBEelWqQjiQQAAEQAAEQAAETCEBwTYCIKkAABEAABEDAEQGPa1FhqR4eHpQq/qSIl7zzH/IQ/0rj3rRrPpfi+V8+F+kc4+HhKcWnikipDk704CROT6uTO8DpUrwU+28yJ3Def4NURL7QHUX3EEAABEAABEDAIQGntYRlSgTWl39PpRPWMik+TcyUDLLG8ZH/pKamcGkhl+KvVCQtns/5TPqXD5wu/nh6etD/AywQeinkZWCrAAAAAElFTkSuQmCC", c || (c = document.createElement("a")), c.href = t, e !== c.href && N(o, "src", "data:image/png;base64,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"), N(o, "alt", "Player Management Examples"), N(y, "cx", "13"), N(y, "cy", "13"), N(y, "r", "12"), N(y, "stroke", "currentColor"), N(y, "stroke-width", "2"), N(b, "d", "M17.9653 11.6049H15.1504C14.9504 11.6049 14.7585 11.5254 14.6171 11.384C14.4757 11.2426 14.3962 11.0507 14.3962 10.8507H14.3952V8.00958C14.3885 7.81386 14.3061 7.62837 14.1652 7.49226C14.0244 7.35615 13.8363 7.28005 13.6404 7.28003H12.3612C12.262 7.27989 12.1637 7.29931 12.072 7.33717C11.9803 7.37503 11.8969 7.43059 11.8267 7.50068C11.7564 7.57077 11.7007 7.65402 11.6626 7.74565C11.6246 7.83729 11.605 7.93553 11.6049 8.03476V10.8497C11.6049 11.2666 11.2666 11.6039 10.8507 11.6039H8.0227C7.82453 11.6076 7.63572 11.6889 7.49685 11.8303C7.35798 11.9717 7.28013 12.162 7.28003 12.3602V13.6394C7.28003 14.0516 7.61098 14.3878 8.0227 14.3936H10.8507V14.3946C11.2677 14.3946 11.6049 14.7329 11.6049 15.1488V17.9774C11.6083 18.1753 11.6894 18.364 11.8305 18.5028C11.9717 18.6416 12.1617 18.7194 12.3596 18.7195H13.6394C14.0521 18.7195 14.3873 18.3886 14.3936 17.9774V15.1488H14.3946C14.3946 14.7319 14.7329 14.3946 15.1488 14.3946V14.3936H17.9894C18.1852 14.3872 18.3708 14.3049 18.5071 14.1642C18.6433 14.0234 18.7195 13.8353 18.7195 13.6394V12.3602C18.7196 12.261 18.7002 12.1628 18.6624 12.0712C18.6246 11.9796 18.569 11.8963 18.499 11.8262C18.4289 11.756 18.3457 11.7004 18.2542 11.6624C18.1626 11.6245 18.0644 11.6049 17.9653 11.6049Z"), N(b, "fill", "currentColor"), N(E, "clip-path", "url(#clip0)"), N(C, "width", "11.44"), N(C, "height", "11.44"), N(C, "fill", "white"), N(C, "transform", "translate(7.28003 7.28003)"), N(w, "id", "clip0"), N(v, "width", "26"), N(v, "height", "26"), N(v, "viewBox", "0 0 26 26"), N(v, "fill", "none"), N(v, "xmlns", "http://www.w3.org/2000/svg"), N(v, "class", "icon"), N(g, "class", "button no-border strong theme-info-color inline-help-button"), N(U, "d", "M26.115 11.345 15.639.86a3.094 3.094 0 0 0-4.278 0L.885 11.345a3.029 3.029 0 0 0 0 4.28l10.476 10.487a3.02 3.02 0 0 0 4.278 0l10.476-10.489a3.029 3.029 0 0 0 0-4.28v.002ZM12.054 6.73A1.449 1.449 0 0 1 13.5 5.282a1.446 1.446 0 0 1 1.446 1.447v5.792A1.449 1.449 0 0 1 13.5 13.97a1.446 1.446 0 0 1-1.446-1.448V6.73ZM13.5 20.243a1.928 1.928 0 0 1-1.892-2.307 1.931 1.931 0 0 1 2.63-1.407 1.93 1.93 0 0 1 .626 3.149 1.928 1.928 0 0 1-1.364.565Z"), N(U, "fill", "#FFBE15"), N(V, "class", "icon"), N(V, "fill", "none"), N(V, "xmlns", "http://www.w3.org/2000/svg"), N(V, "viewBox", "0 0 27 27"), N(H, "class", "note-content"), N(P, "class", "note border-theme theme-caution-color")
             },
             m(t, s) {
-                k(t, n, s), se && se.m(n, null), x(n, i), x(n, a), ce && ce.m(a, null), x(a, r), x(n, l), x(n, o), x(n, u), x(n, d), x(d, A), x(A, f), x(d, h), x(d, m), x(m, p), x(m, g), x(g, v), x(v, y), x(v, E), x(E, b), x(v, I), x(I, w), x(w, C), x(g, B), x(m, S), x(n, P), x(n, L), x(L, V), x(V, z), x(L, D), x(L, H), x(H, Q), x(Q, J), x(Q, K), x(K, Z), x(Q, Y), x(H, G), x(H, $), x($, _), x($, ee), x(ee, te), x($, ne), x($, ie), x(ie, ae), x($, re), le || (oe = T(g, "click", e[3]), le = !0)
+                k(t, n, s), se && se.m(n, null), x(n, i), x(n, a), ce && ce.m(a, null), x(a, r), x(n, l), x(n, o), x(n, u), x(n, d), x(d, A), x(A, f), x(d, h), x(d, m), x(m, p), x(m, g), x(g, v), x(v, y), x(v, E), x(E, b), x(v, I), x(I, w), x(w, C), x(g, B), x(m, S), x(n, L), x(n, P), x(P, V), x(V, U), x(P, D), x(P, H), x(H, Q), x(Q, J), x(Q, K), x(K, Z), x(Q, Y), x(H, G), x(H, $), x($, _), x($, ee), x(ee, te), x($, ne), x($, ie), x(ie, ae), x($, re), le || (oe = z(g, "click", e[3]), le = !0)
             },
             p(e, [t]) {
-                e[0] ? se ? se.p(e, t) : (se = bn(e), se.c(), se.m(n, i)) : se && (se.d(1), se = null), e[0] ? ce || (ce = In(), ce.c(), ce.m(a, r)) : ce && (ce.d(1), ce = null)
+                e[0] ? se ? se.p(e, t) : (se = Sn(e), se.c(), se.m(n, i)) : se && (se.d(1), se = null), e[0] ? ce || (ce = Ln(), ce.c(), ce.m(a, r)) : ce && (ce.d(1), ce = null)
             },
             i: t,
             o: t,
             d(e) {
                 e && R(n), se && se.d(), ce && ce.d(), le = !1, oe()
             }
         }
     }
 
-    function Cn(e, t, n) {
+    function xn(e, t, n) {
         let {
             showAutoBalance: i
         } = t;
-        const a = ue();
+        const a = de();
         return e.$$set = e => {
             "showAutoBalance" in e && n(0, i = e.showAutoBalance)
         }, [i, a, () => a("openAutoBalance"), () => a("clickCreateTeam")]
     }
-    class Bn extends Ze {
+    class kn extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Cn, wn, s, {
+            super(), Ze(this, e, xn, Pn, s, {
                 showAutoBalance: 0
             })
         }
     }
 
-    function Sn(e) {
+    function Rn(e) {
         let n, i, a, r, o, s, c, u, d, A, f, h, m, p, g, y, E, b;
         return {
             c() {
-                n = O("dialog"), i = O("button"), a = X("svg"), r = X("path"), o = U(), s = O("div"), c = O("form"), u = O("h2"), d = F("Rename Team"), A = U(), f = O("p"), h = O("input"), m = U(), p = O("div"), g = O("button"), y = F("Rename Team"), this.h()
+                n = O("dialog"), i = O("button"), a = X("svg"), r = X("path"), o = T(), s = O("div"), c = O("form"), u = O("h2"), d = F("Rename Team"), A = T(), f = O("p"), h = O("input"), m = T(), p = O("div"), g = O("button"), y = F("Rename Team"), this.h()
             },
             l(e) {
                 n = j(e, "DIALOG", {
                     class: !0
                 });
                 var t = W(n);
                 i = j(t, "BUTTON", {
@@ -3096,41 +3229,41 @@
                 var B = W(g);
                 y = q(B, "Rename Team"), B.forEach(R), C.forEach(R), b.forEach(R), E.forEach(R), t.forEach(R), this.h()
             },
             h() {
                 N(r, "fill", "currentColor"), N(r, "d", "M11.38 7.75L16 3.14a1.86 1.86 0 00.25-2.38 1.79 1.79 0 00-2.74-.23L8.83 5.2a.76.76 0 01-1.08 0L3.14.6A1.86 1.86 0 00.76.33a1.79 1.79 0 00-.23 2.74L5.2 7.75a.76.76 0 010 1.08L.6 13.44a1.88 1.88 0 00-.27 2.39 1.81 1.81 0 002.74.23l4.68-4.68a.76.76 0 011.08 0L13.44 16a1.87 1.87 0 002.39.26 1.81 1.81 0 00.23-2.74l-4.68-4.69a.76.76 0 010-1.08z"), N(a, "class", "icon"), N(a, "viewBox", "0 0 16.59 16.59"), N(a, "xmlns", "http://www.w3.org/2000/svg"), N(i, "class", "close-button"), N(u, "class", "modal-heading"), N(g, "class", "button"), N(p, "class", "button-wrap align-center"), N(s, "class", "scroll-wrap text-center"), N(n, "class", "modal large-pad")
             },
             m(t, l) {
-                k(t, n, l), x(n, i), x(i, a), x(a, r), x(n, o), x(n, s), x(s, c), x(c, u), x(u, d), x(c, A), x(c, f), x(f, h), Z(h, e[2]), x(c, m), x(c, p), x(p, g), x(g, y), e[9](n), E || (b = [T(i, "click", e[5]), T(h, "input", e[6]), v(Pn.call(null, h)), T(h, "keyup", e[7]), T(c, "submit", D(e[8]))], E = !0)
+                k(t, n, l), x(n, i), x(i, a), x(a, r), x(n, o), x(n, s), x(s, c), x(c, u), x(u, d), x(c, A), x(c, f), x(f, h), Z(h, e[2]), x(c, m), x(c, p), x(p, g), x(g, y), e[9](n), E || (b = [z(i, "click", e[5]), z(h, "input", e[6]), v(Vn.call(null, h)), z(h, "keyup", e[7]), z(c, "submit", D(e[8]))], E = !0)
             },
             p(e, [t]) {
                 4 & t && h.value !== e[2] && Z(h, e[2])
             },
             i: t,
             o: t,
             d(t) {
                 t && R(n), e[9](null), E = !1, l(b)
             }
         }
     }
 
-    function Pn(e) {
+    function Vn(e) {
         e.focus()
     }
 
-    function Ln(e, t, n) {
+    function On(e, t, n) {
         let {
             team: i
         } = t, {
             open: a = !1
         } = t;
-        const r = ue();
+        const r = de();
         let l, o = i.name;
         ce((() => {
-            At.registerDialog(l)
+            ft.registerDialog(l)
         }));
         return e.$$set = e => {
             "team" in e && n(4, i = e.team), "open" in e && n(0, a = e.open)
         }, e.$$.update = () => {
             3 & e.$$.dirty && l && (a ? l.showModal() : (null == l ? void 0 : l.open) && l.close(), document.body.classList.toggle("modal-is-open", a))
         }, [a, l, o, r, i, () => {
             n(0, a = !1)
@@ -3139,38 +3272,38 @@
         }, e => {
             "Escape" === e.key && r("close")
         }, () => {
             r("rename", {
                 name: o
             }), n(0, a = !1)
         }, function(e) {
-            fe[e ? "unshift" : "push"]((() => {
+            he[e ? "unshift" : "push"]((() => {
                 l = e, n(1, l)
             }))
         }]
     }
-    class xn extends Ze {
+    class Xn extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Ln, Sn, s, {
+            super(), Ze(this, e, On, Rn, s, {
                 team: 4,
                 open: 0
             })
         }
     }
 
-    function kn(e, t, n) {
+    function Fn(e, t, n) {
         const i = e.slice();
         return i[19] = t[n], i
     }
 
-    function Rn(e) {
+    function Tn(e) {
         let t, n, i, a;
 
         function r(e, t) {
-            return e[7].length > 1 ? On : Vn
+            return e[7].length > 1 ? zn : Un
         }
         let l = r(e),
             o = l(e);
         return {
             c() {
                 t = O("button"), n = F("Add "), o.c(), this.h()
             },
@@ -3181,26 +3314,26 @@
                 var i = W(t);
                 n = q(i, "Add "), o.l(i), i.forEach(R), this.h()
             },
             h() {
                 N(t, "class", "button small hollow theme-tint animate-in")
             },
             m(r, l) {
-                k(r, t, l), x(t, n), o.m(t, null), i || (a = T(t, "click", e[10]), i = !0)
+                k(r, t, l), x(t, n), o.m(t, null), i || (a = z(t, "click", e[10]), i = !0)
             },
             p(e, n) {
                 l === (l = r(e)) && o ? o.p(e, n) : (o.d(1), o = l(e), o && (o.c(), o.m(t, null)))
             },
             d(e) {
                 e && R(t), o.d(), i = !1, a()
             }
         }
     }
 
-    function Vn(e) {
+    function Un(e) {
         let n;
         return {
             c() {
                 n = F("player")
             },
             l(e) {
                 n = q(e, "player")
@@ -3211,15 +3344,15 @@
             p: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function On(e) {
+    function zn(e) {
         let t, n, i = e[7].length + "";
         return {
             c() {
                 t = F(i), n = F(" players")
             },
             l(e) {
                 t = q(e, i), n = q(e, " players")
@@ -3232,42 +3365,42 @@
             },
             d(e) {
                 e && R(t), e && R(n)
             }
         }
     }
 
-    function Xn(e) {
+    function Dn(e) {
         let t;
 
         function n(e, t) {
-            return !e[4].minimumPlayers || e[4].maximumPlayers && e[4].minimumPlayers !== e[4].maximumPlayers ? e[4].minimumPlayers && e[4].maximumPlayers ? Un : e[4].maximumPlayers ? Fn : void 0 : zn
+            return !e[4].minimumPlayers || e[4].maximumPlayers && e[4].minimumPlayers !== e[4].maximumPlayers ? e[4].minimumPlayers && e[4].maximumPlayers ? Nn : e[4].maximumPlayers ? Hn : void 0 : Qn
         }
         let i = n(e),
             a = i && i(e);
         return {
             c() {
-                a && a.c(), t = z()
+                a && a.c(), t = U()
             },
             l(e) {
-                a && a.l(e), t = z()
+                a && a.l(e), t = U()
             },
             m(e, n) {
                 a && a.m(e, n), k(e, t, n)
             },
             p(e, r) {
                 i === (i = n(e)) && a ? a.p(e, r) : (a && a.d(1), a = i && i(e), a && (a.c(), a.m(t.parentNode, t)))
             },
             d(e) {
                 a && a.d(e), e && R(t)
             }
         }
     }
 
-    function Fn(e) {
+    function Hn(e) {
         let t, n, i, a, r = e[4].maximumPlayers + "";
         return {
             c() {
                 t = O("em"), n = F("("), i = F(r), a = F(" maximum)")
             },
             l(e) {
                 t = j(e, "EM", {});
@@ -3282,15 +3415,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function Un(e) {
+    function Nn(e) {
         let t, n, i, a, r, l, o = e[4].minimumPlayers + "",
             s = e[4].maximumPlayers + "";
         return {
             c() {
                 t = O("em"), n = F("("), i = F(o), a = F(" to "), r = F(s), l = F(" required)")
             },
             l(e) {
@@ -3306,15 +3439,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function zn(e) {
+    function Qn(e) {
         let t, n, i, a, r = e[4].minimumPlayers + "";
         return {
             c() {
                 t = O("em"), n = F("("), i = F(r), a = F(" required)")
             },
             l(e) {
                 t = j(e, "EM", {});
@@ -3329,15 +3462,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function Tn(e) {
+    function Wn(e) {
         let t, n, i;
         return {
             c() {
                 t = O("div"), n = O("p"), i = F("Assign players to this team to get started."), this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
@@ -3358,106 +3491,106 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function Dn(e, n) {
+    function Jn(e, n) {
         let i, a, r, l, o, s, c, u = t;
-        return a = new Kt({
+        return a = new _t({
             props: {
                 isSelected: n[2].includes(n[19].id),
                 player: n[19],
                 assigned: !0,
                 readOnly: n[3],
                 currentTeam: n[0]
             }
         }), a.$on("selectPlayer", n[13]), a.$on("unassignPlayer", n[14]), a.$on("addPlayers", n[15]), {
             key: e,
             first: null,
             c() {
-                i = O("div"), We(a.$$.fragment), r = U(), this.h()
+                i = O("div"), Je(a.$$.fragment), r = T(), this.h()
             },
             l(e) {
                 i = j(e, "DIV", {});
                 var t = W(i);
-                Je(a.$$.fragment, t), r = M(t), t.forEach(R), this.h()
+                je(a.$$.fragment, t), r = M(t), t.forEach(R), this.h()
             },
             h() {
                 this.first = i
             },
             m(e, t) {
-                k(e, i, t), je(a, i, null), x(i, r), c = !0
+                k(e, i, t), qe(a, i, null), x(i, r), c = !0
             },
             p(e, t) {
                 n = e;
                 const i = {};
                 6 & t && (i.isSelected = n[2].includes(n[19].id)), 2 & t && (i.player = n[19]), 8 & t && (i.readOnly = n[3]), 1 & t && (i.currentTeam = n[0]), a.$set(i)
             },
             r() {
                 s = i.getBoundingClientRect()
             },
             f() {
                 re(i), u(), le(i, s)
             },
             a() {
-                u(), u = ae(i, s, Tt, {})
+                u(), u = ae(i, s, Dt, {})
             },
             i(e) {
-                c || (Re(a.$$.fragment, e), e && ve((() => {
-                    o && o.end(1), l = Xe(i, $t, {
+                c || (Ve(a.$$.fragment, e), e && ye((() => {
+                    o && o.end(1), l = Fe(i, an, {
                         key: n[19].id
                     }), l.start()
                 })), c = !0)
             },
             o(e) {
-                Ve(a.$$.fragment, e), l && l.invalidate(), e && (o = Fe(i, Gt, {
+                Oe(a.$$.fragment, e), l && l.invalidate(), e && (o = Te(i, nn, {
                     key: n[19].id
                 })), c = !1
             },
             d(e) {
-                e && R(i), qe(a), e && o && o.end()
+                e && R(i), Me(a), e && o && o.end()
             }
         }
     }
 
-    function Hn(e) {
-        let t, n, i, a, r, o, s, c, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, P, L, V, z, H, Q = e[0].name + "",
+    function jn(e) {
+        let t, n, i, a, r, o, s, c, u, d, A, f, h, m, p, g, v, y, E, b, I, w, C, B, S, L, P, V, U, H, Q = e[0].name + "",
             J = (e[1].length || "No") + "",
             Z = 1 === e[1].length ? "player" : "players",
             Y = [],
             $ = new Map,
-            _ = e[7].length && Rn(e),
-            ee = e[6] && Xn(e),
-            te = 0 == e[1].length && Tn(),
+            _ = e[7].length && Tn(e),
+            ee = e[6] && Dn(e),
+            te = 0 == e[1].length && Wn(),
             ne = e[1];
         const ie = e => {
             var t;
             return null == (t = e[19]) ? void 0 : t.id
         };
         for (let l = 0; l < ne.length; l += 1) {
-            let t = kn(e, ne, l),
+            let t = Fn(e, ne, l),
                 n = ie(t);
-            $.set(n, Y[l] = Dn(n, t))
+            $.set(n, Y[l] = Jn(n, t))
         }
 
         function ae(t) {
             e[16](t)
         }
         let re = {
             team: e[0]
         };
-        return void 0 !== e[5] && (re.open = e[5]), P = new xn({
+        return void 0 !== e[5] && (re.open = e[5]), L = new Xn({
             props: re
-        }), fe.push((() => Qe(P, "open", ae))), P.$on("close", e[17]), P.$on("rename", e[18]), {
+        }), he.push((() => We(L, "open", ae))), L.$on("close", e[17]), L.$on("rename", e[18]), {
             c() {
-                t = O("div"), n = O("h2"), i = F(Q), a = U(), _ && _.c(), r = U(), o = O("p"), s = F(J), c = U(), u = F(Z), d = U(), ee && ee.c(), A = U(), f = O("div"), h = O("a"), m = X("svg"), p = X("path"), g = U(), v = O("a"), y = X("svg"), E = X("path"), I = U(), w = O("div"), te && te.c(), C = U();
+                t = O("div"), n = O("h2"), i = F(Q), a = T(), _ && _.c(), r = T(), o = O("p"), s = F(J), c = T(), u = F(Z), d = T(), ee && ee.c(), A = T(), f = O("div"), h = O("a"), m = X("svg"), p = X("path"), g = T(), v = O("a"), y = X("svg"), E = X("path"), I = T(), w = O("div"), te && te.c(), C = T();
                 for (let e = 0; e < Y.length; e += 1) Y[e].c();
-                S = U(), We(P.$$.fragment), this.h()
+                S = T(), Je(L.$$.fragment), this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
                     class: !0,
                     id: !0
                 });
                 var l = W(t);
@@ -3468,216 +3601,216 @@
                 i = q(b, Q), b.forEach(R), a = M(l), _ && _.l(l), r = M(l), o = j(l, "P", {
                     class: !0
                 });
                 var B = W(o);
                 s = q(B, J), c = M(B), u = q(B, Z), d = M(B), ee && ee.l(B), B.forEach(R), A = M(l), f = j(l, "DIV", {
                     class: !0
                 });
-                var L = W(f);
-                h = j(L, "A", {
+                var P = W(f);
+                h = j(P, "A", {
                     class: !0,
                     href: !0
                 });
                 var x = W(h);
                 m = j(x, "svg", {
                     class: !0,
                     viewBox: !0,
                     id: !0,
                     xmlns: !0
                 }, 1);
                 var k = W(m);
                 p = j(k, "path", {
                     d: !0,
                     fill: !0
-                }, 1), W(p).forEach(R), k.forEach(R), x.forEach(R), g = M(L), v = j(L, "A", {
+                }, 1), W(p).forEach(R), k.forEach(R), x.forEach(R), g = M(P), v = j(P, "A", {
                     class: !0,
                     href: !0
                 });
                 var V = W(v);
                 y = j(V, "svg", {
                     class: !0,
                     viewBox: !0,
                     id: !0,
                     xmlns: !0
                 }, 1);
                 var O = W(y);
                 E = j(O, "path", {
                     d: !0,
                     fill: !0
-                }, 1), W(E).forEach(R), O.forEach(R), V.forEach(R), L.forEach(R), l.forEach(R), I = M(e), w = j(e, "DIV", {});
+                }, 1), W(E).forEach(R), O.forEach(R), V.forEach(R), P.forEach(R), l.forEach(R), I = M(e), w = j(e, "DIV", {});
                 var X = W(w);
                 te && te.l(X), C = M(X);
                 for (let t = 0; t < Y.length; t += 1) Y[t].l(X);
-                X.forEach(R), S = M(e), Je(P.$$.fragment, e), this.h()
+                X.forEach(R), S = M(e), je(L.$$.fragment, e), this.h()
             },
             h() {
                 N(n, "class", "player-card-heading"), N(o, "class", "player-card-summary"), N(p, "d", "M23.323 2.883L20.861.422a1.44 1.44 0 00-2.036 0l-2.122 2.122a.64.64 0 000 .905l3.593 3.593c.25.25.655.25.905 0l2.122-2.122a1.441 1.441 0 000-2.037zm-7.39 1.336a.639.639 0 00-.905 0l-11.75 11.75a.639.639 0 000 .905l3.593 3.593c.25.25.655.25.905 0l11.75-11.75a.64.64 0 000-.905l-3.593-3.593zM2.597 17.732a.48.48 0 00-.775.138l-.032.095-1.746 5.099-.032.093a.48.48 0 00.576.576l.093-.033 5.099-1.746.095-.032a.48.48 0 00.138-.775l-3.416-3.415z"), N(p, "fill", "currentColor"), N(m, "class", "icon"), N(m, "viewBox", "0 0 23.744 23.745"), N(m, "id", "pencil"), N(m, "xmlns", "http://www.w3.org/2000/svg"), N(h, "class", "button icon-button circle "), N(h, "href", "."), N(E, "d", "M15.67 4.446l-.057-.215-.409-1.545a.876.876 0 00-.692-.588l-.034-.005a51.6 51.6 0 00-3.453-.33l-.04.002a.638.638 0 01-.614-.46C10.234.993 9.978.311 9.663.184A1.438 1.438 0 009.448.12C9.39.11 9.331.103 9.272.095a10.745 10.745 0 00-2.867 0C6.348.103 6.288.11 6.23.12a1.225 1.225 0 00-.213.065C5.709.308 5.459.98 5.32 1.28a.634.634 0 01-.62.485c-.011 0-.021 0-.032-.002-1.146.071-2.28.18-3.404.325l-.142.018a.876.876 0 00-.648.581L.065 4.231l-.057.215a.904.904 0 00.874 1.027h13.915a.905.905 0 00.873-1.027zm-1.695 2.69H1.704a.906.906 0 00-.812.859l.02.232 1.005 12.18a.88.88 0 00.869.762h10.107c.44 0 .812-.326.869-.762l1.007-12.18.019-.232a.908.908 0 00-.813-.859z"), N(E, "fill", "currentColor"), N(y, "class", "icon"), N(y, "viewBox", "0 0 15.679 21.169"), N(y, "id", "trash"), N(y, "xmlns", "http://www.w3.org/2000/svg"), N(v, "class", "button icon-button circle "), N(v, "href", "."), N(f, "class", "player-card-actions"), N(t, "class", "player-item is-header theme-caution-color"), N(t, "id", b = e[0].internalId || e[0].id), G(t, "theme-caution-color", e[6])
             },
             m(l, b) {
                 k(l, t, b), x(t, n), x(n, i), x(t, a), _ && _.m(t, null), x(t, r), x(t, o), x(o, s), x(o, c), x(o, u), x(o, d), ee && ee.m(o, null), x(t, A), x(t, f), x(f, h), x(h, m), x(m, p), x(f, g), x(f, v), x(v, y), x(y, E), k(l, I, b), k(l, w, b), te && te.m(w, null), x(w, C);
                 for (let e = 0; e < Y.length; e += 1) Y[e].m(w, null);
-                k(l, S, b), je(P, l, b), V = !0, z || (H = [T(n, "dblclick", e[9]), T(h, "click", D(e[11])), T(v, "click", D(e[12]))], z = !0)
+                k(l, S, b), qe(L, l, b), V = !0, U || (H = [z(n, "dblclick", e[9]), z(h, "click", D(e[11])), z(v, "click", D(e[12]))], U = !0)
             },
             p(e, [n]) {
-                if ((!V || 1 & n) && Q !== (Q = e[0].name + "") && K(i, Q), e[7].length ? _ ? _.p(e, n) : (_ = Rn(e), _.c(), _.m(t, r)) : _ && (_.d(1), _ = null), (!V || 2 & n) && J !== (J = (e[1].length || "No") + "") && K(s, J), (!V || 2 & n) && Z !== (Z = 1 === e[1].length ? "player" : "players") && K(u, Z), e[6] ? ee ? ee.p(e, n) : (ee = Xn(e), ee.c(), ee.m(o, null)) : ee && (ee.d(1), ee = null), (!V || 1 & n && b !== (b = e[0].internalId || e[0].id)) && N(t, "id", b), 64 & n && G(t, "theme-caution-color", e[6]), 0 == e[1].length ? te || (te = Tn(), te.c(), te.m(w, C)) : te && (te.d(1), te = null), 15 & n) {
-                    ne = e[1], xe();
+                if ((!V || 1 & n) && Q !== (Q = e[0].name + "") && K(i, Q), e[7].length ? _ ? _.p(e, n) : (_ = Tn(e), _.c(), _.m(t, r)) : _ && (_.d(1), _ = null), (!V || 2 & n) && J !== (J = (e[1].length || "No") + "") && K(s, J), (!V || 2 & n) && Z !== (Z = 1 === e[1].length ? "player" : "players") && K(u, Z), e[6] ? ee ? ee.p(e, n) : (ee = Dn(e), ee.c(), ee.m(o, null)) : ee && (ee.d(1), ee = null), (!V || 1 & n && b !== (b = e[0].internalId || e[0].id)) && N(t, "id", b), 64 & n && G(t, "theme-caution-color", e[6]), 0 == e[1].length ? te || (te = Wn(), te.c(), te.m(w, C)) : te && (te.d(1), te = null), 15 & n) {
+                    ne = e[1], ke();
                     for (let e = 0; e < Y.length; e += 1) Y[e].r();
-                    Y = Ne(Y, n, ie, 1, e, ne, $, w, He, Dn, null, kn);
+                    Y = Qe(Y, n, ie, 1, e, ne, $, w, Ne, Jn, null, Fn);
                     for (let e = 0; e < Y.length; e += 1) Y[e].a();
-                    ke()
+                    Re()
                 }
                 const a = {};
-                1 & n && (a.team = e[0]), !L && 32 & n && (L = !0, a.open = e[5], ye((() => L = !1))), P.$set(a)
+                1 & n && (a.team = e[0]), !P && 32 & n && (P = !0, a.open = e[5], Ee((() => P = !1))), L.$set(a)
             },
             i(e) {
                 if (!V) {
-                    for (let e = 0; e < ne.length; e += 1) Re(Y[e]);
-                    e && ve((() => {
-                        B || (B = Ue(w, Yt, {}, !0)), B.run(1)
-                    })), Re(P.$$.fragment, e), V = !0
+                    for (let e = 0; e < ne.length; e += 1) Ve(Y[e]);
+                    e && ye((() => {
+                        B || (B = Ue(w, tn, {}, !0)), B.run(1)
+                    })), Ve(L.$$.fragment, e), V = !0
                 }
             },
             o(e) {
-                for (let t = 0; t < Y.length; t += 1) Ve(Y[t]);
-                e && (B || (B = Ue(w, Yt, {}, !1)), B.run(0)), Ve(P.$$.fragment, e), V = !1
+                for (let t = 0; t < Y.length; t += 1) Oe(Y[t]);
+                e && (B || (B = Ue(w, tn, {}, !1)), B.run(0)), Oe(L.$$.fragment, e), V = !1
             },
             d(e) {
                 e && R(t), _ && _.d(), ee && ee.d(), e && R(I), e && R(w), te && te.d();
                 for (let t = 0; t < Y.length; t += 1) Y[t].d();
-                e && B && B.end(), e && R(S), qe(P, e), z = !1, l(H)
+                e && B && B.end(), e && R(S), Me(L, e), U = !1, l(H)
             }
         }
     }
 
-    function Nn(e, t, n) {
+    function qn(e, t, n) {
         let i, a, r;
-        d(e, $e, (e => n(4, r = e)));
+        d(e, _e, (e => n(4, r = e)));
         let {
             team: l
         } = t, {
             players: o
         } = t, {
             selected: s = []
         } = t, {
             readOnly: c = !1
         } = t, u = !1;
-        const A = ue();
+        const A = de();
         console.log(l.length);
         return e.$$set = e => {
             "team" in e && n(0, l = e.team), "players" in e && n(1, o = e.players), "selected" in e && n(2, s = e.selected), "readOnly" in e && n(3, c = e.readOnly)
         }, e.$$.update = () => {
             5 & e.$$.dirty && n(7, i = s.filter((e => !l.players.includes(e)))), 18 & e.$$.dirty && n(6, a = o.length && (r.minimumPlayers && o.length < r.minimumPlayers || r.maximumPlayers && o.length > r.maximumPlayers))
         }, [l, o, s, c, r, u, a, i, A, () => {
             n(5, u = !0)
         }, () => {
             A("addPlayers")
         }, () => {
             n(5, u = !0)
         }, () => {
             A("delete")
         }, function(t) {
-            de.call(this, e, t)
+            Ae.call(this, e, t)
         }, function(t) {
-            de.call(this, e, t)
+            Ae.call(this, e, t)
         }, function(t) {
-            de.call(this, e, t)
+            Ae.call(this, e, t)
         }, function(e) {
             u = e, n(5, u)
         }, () => {
             n(5, u = !1)
         }, e => {
             A("rename", e.detail), n(5, u = !1)
         }]
     }
-    class Qn extends Ze {
+    class Mn extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Nn, Hn, s, {
+            super(), Ze(this, e, qn, jn, s, {
                 team: 0,
                 players: 1,
                 selected: 2,
                 readOnly: 3
             })
         }
     }
     const {
-        Map: Wn
+        Map: Kn
     } = ze;
 
-    function Jn(e, t, n) {
+    function Zn(e, t, n) {
         const i = e.slice();
         return i[33] = t[n][0], i[34] = t[n][1], i
     }
 
-    function jn(e, t, n) {
+    function Yn(e, t, n) {
         const i = e.slice();
         return i[30] = t[n], i[37] = t, i[38] = n, i
     }
 
-    function qn(e, t, n) {
+    function Gn(e, t, n) {
         const i = e.slice();
         return i[30] = t[n], i[31] = t, i[32] = n, i
     }
 
-    function Mn(e) {
+    function $n(e) {
         let t, n, i = [],
-            a = new Wn,
+            a = new Kn,
             r = [...e[6]];
         const l = e => e[33];
         for (let o = 0; o < r.length; o += 1) {
-            let t = Jn(e, r, o),
+            let t = Zn(e, r, o),
                 n = l(t);
-            a.set(n, i[o] = _n(n, t))
+            a.set(n, i[o] = ai(n, t))
         }
         return {
             c() {
                 for (let e = 0; e < i.length; e += 1) i[e].c();
-                t = z()
+                t = U()
             },
             l(e) {
                 for (let t = 0; t < i.length; t += 1) i[t].l(e);
-                t = z()
+                t = U()
             },
             m(e, a) {
                 for (let t = 0; t < i.length; t += 1) i[t].m(e, a);
                 k(e, t, a), n = !0
             },
             p(e, n) {
-                31297 & n[0] && (r = [...e[6]], xe(), i = Ne(i, n, l, 1, e, r, a, t.parentNode, De, _n, t, Jn), ke())
+                31297 & n[0] && (r = [...e[6]], ke(), i = Qe(i, n, l, 1, e, r, a, t.parentNode, He, ai, t, Zn), Re())
             },
             i(e) {
                 if (!n) {
-                    for (let e = 0; e < r.length; e += 1) Re(i[e]);
+                    for (let e = 0; e < r.length; e += 1) Ve(i[e]);
                     n = !0
                 }
             },
             o(e) {
-                for (let t = 0; t < i.length; t += 1) Ve(i[t]);
+                for (let t = 0; t < i.length; t += 1) Oe(i[t]);
                 n = !1
             },
             d(e) {
                 for (let t = 0; t < i.length; t += 1) i[t].d(e);
                 e && R(t)
             }
         }
     }
 
-    function Kn(e) {
+    function _n(e) {
         let t, n, i, a, r, l, o, s, c = e[7].length + "",
             u = [],
-            d = new Wn,
+            d = new Kn,
             A = e[7];
         const f = e => e[30].internalId || e[30].id;
         for (let h = 0; h < A.length; h += 1) {
-            let t = qn(e, A, h),
+            let t = Gn(e, A, h),
                 n = f(t);
-            d.set(n, u[h] = ei(n, t))
+            d.set(n, u[h] = ri(n, t))
         }
         return {
             c() {
-                t = O("div"), n = O("p"), i = F("Teams ("), a = F(c), r = F(")"), l = U(), o = O("div");
+                t = O("div"), n = O("p"), i = F("Teams ("), a = F(c), r = F(")"), l = T(), o = O("div");
                 for (let e = 0; e < u.length; e += 1) u[e].c();
                 this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
                     class: !0,
                     id: !0
@@ -3700,61 +3833,61 @@
             m(e, c) {
                 k(e, t, c), x(t, n), x(n, i), x(n, a), x(n, r), k(e, l, c), k(e, o, c);
                 for (let t = 0; t < u.length; t += 1) u[t].m(o, null);
                 s = !0
             },
             p(e, t) {
                 if ((!s || 128 & t[0]) && c !== (c = e[7].length + "") && K(a, c), 14984 & t[0]) {
-                    A = e[7], xe();
+                    A = e[7], ke();
                     for (let e = 0; e < u.length; e += 1) u[e].r();
-                    u = Ne(u, t, f, 1, e, A, d, o, He, ei, null, qn);
+                    u = Qe(u, t, f, 1, e, A, d, o, Ne, ri, null, Gn);
                     for (let e = 0; e < u.length; e += 1) u[e].a();
-                    ke()
+                    Re()
                 }
             },
             i(e) {
                 if (!s) {
-                    for (let e = 0; e < A.length; e += 1) Re(u[e]);
+                    for (let e = 0; e < A.length; e += 1) Ve(u[e]);
                     s = !0
                 }
             },
             o(e) {
-                for (let t = 0; t < u.length; t += 1) Ve(u[t]);
+                for (let t = 0; t < u.length; t += 1) Oe(u[t]);
                 s = !1
             },
             d(e) {
                 e && R(t), e && R(l), e && R(o);
                 for (let t = 0; t < u.length; t += 1) u[t].d()
             }
         }
     }
 
-    function Zn(e) {
+    function ei(e) {
         let t, n, i, a, r, l, o, s, c, u, d, A, f, h = e[34].length + "",
             m = 1 == e[34].length ? "team" : "teams",
             p = [],
-            g = new Wn;
+            g = new Kn;
 
         function v(e, t) {
-            return e[33] ? Gn : Yn
+            return e[33] ? ni : ti
         }
         let y = v(e),
             E = y(e),
             b = e[34];
         const I = e => e[30].internalId || e[30].id;
         for (let w = 0; w < b.length; w += 1) {
-            let t = jn(e, b, w),
+            let t = Yn(e, b, w),
                 n = I(t);
-            g.set(n, p[w] = $n(n, t))
+            g.set(n, p[w] = ii(n, t))
         }
         return {
             c() {
-                t = O("div"), n = O("div"), i = O("h3"), E.c(), a = F("\n          ("), r = F(h), l = U(), o = F(m), s = F(")"), u = U();
+                t = O("div"), n = O("div"), i = O("h3"), E.c(), a = F("\n          ("), r = F(h), l = T(), o = F(m), s = F(")"), u = T();
                 for (let e = 0; e < p.length; e += 1) p[e].c();
-                d = U(), this.h()
+                d = T(), this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
                     class: !0
                 });
                 var c = W(t);
                 n = j(c, "DIV", {
@@ -3775,41 +3908,41 @@
             },
             m(e, c) {
                 k(e, t, c), x(t, n), x(n, i), E.m(i, null), x(n, a), x(n, r), x(n, l), x(n, o), x(n, s), x(t, u);
                 for (let n = 0; n < p.length; n += 1) p[n].m(t, null);
                 x(t, d), f = !0
             },
             p(e, a) {
-                y === (y = v(e)) && E ? E.p(e, a) : (E.d(1), E = y(e), E && (E.c(), E.m(i, null))), (!f || 64 & a[0]) && h !== (h = e[34].length + "") && K(r, h), (!f || 64 & a[0]) && m !== (m = 1 == e[34].length ? "team" : "teams") && K(o, m), (!f || 64 & a[0] && c !== (c = `session-${e[33]}`)) && N(n, "id", c), 14912 & a[0] && (b = e[34], xe(), p = Ne(p, a, I, 1, e, b, g, t, De, $n, d, jn), ke())
+                y === (y = v(e)) && E ? E.p(e, a) : (E.d(1), E = y(e), E && (E.c(), E.m(i, null))), (!f || 64 & a[0]) && h !== (h = e[34].length + "") && K(r, h), (!f || 64 & a[0]) && m !== (m = 1 == e[34].length ? "team" : "teams") && K(o, m), (!f || 64 & a[0] && c !== (c = `session-${e[33]}`)) && N(n, "id", c), 14912 & a[0] && (b = e[34], ke(), p = Qe(p, a, I, 1, e, b, g, t, He, ii, d, Yn), Re())
             },
             i(e) {
                 if (!f) {
-                    for (let e = 0; e < b.length; e += 1) Re(p[e]);
-                    e && ve((() => {
-                        A || (A = Ue(t, Yt, {
+                    for (let e = 0; e < b.length; e += 1) Ve(p[e]);
+                    e && ye((() => {
+                        A || (A = Ue(t, tn, {
                             duration: 200
                         }, !0)), A.run(1)
                     })), f = !0
                 }
             },
             o(e) {
-                for (let t = 0; t < p.length; t += 1) Ve(p[t]);
-                e && (A || (A = Ue(t, Yt, {
+                for (let t = 0; t < p.length; t += 1) Oe(p[t]);
+                e && (A || (A = Ue(t, tn, {
                     duration: 200
                 }, !1)), A.run(0)), f = !1
             },
             d(e) {
                 e && R(t), E.d();
                 for (let t = 0; t < p.length; t += 1) p[t].d();
                 e && A && A.end()
             }
         }
     }
 
-    function Yn(e) {
+    function ti(e) {
         let n, i;
         return {
             c() {
                 n = O("em"), i = F("No Session Group")
             },
             l(e) {
                 n = j(e, "EM", {});
@@ -3822,15 +3955,15 @@
             p: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function Gn(e) {
+    function ni(e) {
         let t, n, i, a, r = e[14](e[33]) + "";
 
         function l() {
             return e[21](e[33])
         }
         return {
             c() {
@@ -3843,28 +3976,28 @@
                 var i = W(t);
                 n = q(i, r), i.forEach(R), this.h()
             },
             h() {
                 N(t, "href", ".")
             },
             m(e, r) {
-                k(e, t, r), x(t, n), i || (a = T(t, "click", D(l)), i = !0)
+                k(e, t, r), x(t, n), i || (a = z(t, "click", D(l)), i = !0)
             },
             p(t, i) {
                 e = t, 64 & i[0] && r !== (r = e[14](e[33]) + "") && K(n, r)
             },
             d(e) {
                 e && R(t), i = !1, a()
             }
         }
     }
 
-    function $n(e, t) {
+    function ii(e, t) {
         let n, i, a, r;
-        return i = new Qn({
+        return i = new Mn({
             props: {
                 team: t[30],
                 players: t[30].players.map(t[22]),
                 readOnly: !0
             }
         }), i.$on("delete", (function() {
             return t[23](t[30])
@@ -3874,89 +4007,89 @@
             return t[25](t[30], ...e)
         })), i.$on("unassignPlayer", (function(...e) {
             return t[26](t[30], t[37], t[38], ...e)
         })), {
             key: e,
             first: null,
             c() {
-                n = O("div"), We(i.$$.fragment), this.h()
+                n = O("div"), Je(i.$$.fragment), this.h()
             },
             l(e) {
                 n = j(e, "DIV", {
                     class: !0
                 });
                 var t = W(n);
-                Je(i.$$.fragment, t), t.forEach(R), this.h()
+                je(i.$$.fragment, t), t.forEach(R), this.h()
             },
             h() {
                 N(n, "class", "card player-card team-card"), this.first = n
             },
             m(e, t) {
-                k(e, n, t), je(i, n, null), r = !0
+                k(e, n, t), qe(i, n, null), r = !0
             },
             p(e, n) {
                 t = e;
                 const a = {};
                 64 & n[0] && (a.team = t[30]), 576 & n[0] && (a.players = t[30].players.map(t[22])), i.$set(a)
             },
             i(e) {
-                r || (Re(i.$$.fragment, e), e && ve((() => {
-                    a || (a = Ue(n, Zt, {
+                r || (Ve(i.$$.fragment, e), e && ye((() => {
+                    a || (a = Ue(n, en, {
                         duration: 200
                     }, !0)), a.run(1)
                 })), r = !0)
             },
             o(e) {
-                Ve(i.$$.fragment, e), e && (a || (a = Ue(n, Zt, {
+                Oe(i.$$.fragment, e), e && (a || (a = Ue(n, en, {
                     duration: 200
                 }, !1)), a.run(0)), r = !1
             },
             d(e) {
-                e && R(n), qe(i), e && a && a.end()
+                e && R(n), Me(i), e && a && a.end()
             }
         }
     }
 
-    function _n(e, t) {
-        let n, i, a, r = t[34].length && Zn(t);
+    function ai(e, t) {
+        let n, i, a, r = t[34].length && ei(t);
         return {
             key: e,
             first: null,
             c() {
-                n = z(), r && r.c(), i = z(), this.h()
+                n = U(), r && r.c(), i = U(), this.h()
             },
             l(e) {
-                n = z(), r && r.l(e), i = z(), this.h()
+                n = U(), r && r.l(e), i = U(), this.h()
             },
             h() {
                 this.first = n
             },
             m(e, t) {
                 k(e, n, t), r && r.m(e, t), k(e, i, t), a = !0
             },
             p(e, n) {
-                (t = e)[34].length ? r ? (r.p(t, n), 64 & n[0] && Re(r, 1)) : (r = Zn(t), r.c(), Re(r, 1), r.m(i.parentNode, i)) : r && (xe(), Ve(r, 1, 1, (() => {
+                (t = e)[34].length ? r ? (r.p(t, n), 64 & n[0] && Ve(r, 1)) : (r = ei(t), r.c(), Ve(r, 1), r.m(i.parentNode, i)) : r && (ke(), Oe(r, 1, 1, (() => {
                     r = null
-                })), ke())
+                })), Re())
             },
             i(e) {
-                a || (Re(r), a = !0)
+                a || (Ve(r), a = !0)
             },
             o(e) {
-                Ve(r), a = !1
+                Oe(r), a = !1
             },
             d(e) {
                 e && R(n), r && r.d(e), e && R(i)
             }
         }
     }
 
-    function ei(e, n) {
+    function ri(e, n) {
         let i, a, r, l, o, s, c = t;
-        return a = new Qn({
+        return a = new Mn({
             props: {
                 team: n[30],
                 players: n[30].players.map(n[15]).filter(Boolean),
                 selected: n[3]
             }
         }), a.$on("selectPlayer", n[16]), a.$on("delete", (function() {
             return n[17](n[30])
@@ -3966,152 +4099,152 @@
             return n[19](n[30], ...e)
         })), a.$on("unassignPlayer", (function(...e) {
             return n[20](n[30], n[31], n[32], ...e)
         })), {
             key: e,
             first: null,
             c() {
-                i = O("div"), We(a.$$.fragment), r = U(), this.h()
+                i = O("div"), Je(a.$$.fragment), r = T(), this.h()
             },
             l(e) {
                 i = j(e, "DIV", {
                     class: !0
                 });
                 var t = W(i);
-                Je(a.$$.fragment, t), r = M(t), t.forEach(R), this.h()
+                je(a.$$.fragment, t), r = M(t), t.forEach(R), this.h()
             },
             h() {
                 N(i, "class", "card player-card glow-shadow team-card"), this.first = i
             },
             m(e, t) {
-                k(e, i, t), je(a, i, null), x(i, r), s = !0
+                k(e, i, t), qe(a, i, null), x(i, r), s = !0
             },
             p(e, t) {
                 n = e;
                 const i = {};
                 128 & t[0] && (i.team = n[30]), 640 & t[0] && (i.players = n[30].players.map(n[15]).filter(Boolean)), 8 & t[0] && (i.selected = n[3]), a.$set(i)
             },
             r() {
                 o = i.getBoundingClientRect()
             },
             f() {
                 re(i), c(), le(i, o)
             },
             a() {
-                c(), c = ae(i, o, Tt, {
+                c(), c = ae(i, o, Dt, {
                     duration: 400
                 })
             },
             i(e) {
-                s || (Re(a.$$.fragment, e), e && ve((() => {
-                    l || (l = Ue(i, Zt, {
+                s || (Ve(a.$$.fragment, e), e && ye((() => {
+                    l || (l = Ue(i, en, {
                         duration: 200
                     }, !0)), l.run(1)
                 })), s = !0)
             },
             o(e) {
-                Ve(a.$$.fragment, e), e && (l || (l = Ue(i, Zt, {
+                Oe(a.$$.fragment, e), e && (l || (l = Ue(i, en, {
                     duration: 200
                 }, !1)), l.run(0)), s = !1
             },
             d(e) {
-                e && R(i), qe(a), e && l && l.end()
+                e && R(i), Me(a), e && l && l.end()
             }
         }
     }
 
-    function ti(e) {
+    function li(e) {
         let t, n;
-        return t = new Bn({
+        return t = new kn({
             props: {
                 showAutoBalance: e[5]
             }
         }), t.$on("clickCreateTeam", e[27]), t.$on("openAutoBalance", e[28]), {
             c() {
-                We(t.$$.fragment)
+                Je(t.$$.fragment)
             },
             l(e) {
-                Je(t.$$.fragment, e)
+                je(t.$$.fragment, e)
             },
             m(e, i) {
-                je(t, e, i), n = !0
+                qe(t, e, i), n = !0
             },
             p(e, n) {
                 const i = {};
                 32 & n[0] && (i.showAutoBalance = e[5]), t.$set(i)
             },
             i(e) {
-                n || (Re(t.$$.fragment, e), n = !0)
+                n || (Ve(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Ve(t.$$.fragment, e), n = !1
+                Oe(t.$$.fragment, e), n = !1
             },
             d(e) {
-                qe(t, e)
+                Me(t, e)
             }
         }
     }
 
-    function ni(e) {
+    function oi(e) {
         let t, n, i, a, r, l;
-        const o = [Kn, Mn],
+        const o = [_n, $n],
             s = [];
 
         function c(e, t) {
             return e[8] ? 1 : 0
         }
 
         function u(t) {
             e[29](t)
         }
         t = c(e), n = s[t] = o[t](e);
         let d = {
             $$slots: {
-                default: [ti]
+                default: [li]
             },
             $$scope: {
                 ctx: e
             }
         };
-        return void 0 !== e[10] && (d.open = e[10]), a = new Et({
+        return void 0 !== e[10] && (d.open = e[10]), a = new bt({
             props: d
-        }), fe.push((() => Qe(a, "open", u))), {
+        }), he.push((() => We(a, "open", u))), {
             c() {
-                n.c(), i = U(), We(a.$$.fragment)
+                n.c(), i = T(), Je(a.$$.fragment)
             },
             l(e) {
-                n.l(e), i = M(e), Je(a.$$.fragment, e)
+                n.l(e), i = M(e), je(a.$$.fragment, e)
             },
             m(e, n) {
-                s[t].m(e, n), k(e, i, n), je(a, e, n), l = !0
+                s[t].m(e, n), k(e, i, n), qe(a, e, n), l = !0
             },
             p(e, l) {
                 let u = t;
-                t = c(e), t === u ? s[t].p(e, l) : (xe(), Ve(s[u], 1, 1, (() => {
+                t = c(e), t === u ? s[t].p(e, l) : (ke(), Oe(s[u], 1, 1, (() => {
                     s[u] = null
-                })), ke(), n = s[t], n ? n.p(e, l) : (n = s[t] = o[t](e), n.c()), Re(n, 1), n.m(i.parentNode, i));
+                })), Re(), n = s[t], n ? n.p(e, l) : (n = s[t] = o[t](e), n.c()), Ve(n, 1), n.m(i.parentNode, i));
                 const d = {};
                 1586 & l[0] | 256 & l[1] && (d.$$scope = {
                     dirty: l,
                     ctx: e
-                }), !r && 1024 & l[0] && (r = !0, d.open = e[10], ye((() => r = !1))), a.$set(d)
+                }), !r && 1024 & l[0] && (r = !0, d.open = e[10], Ee((() => r = !1))), a.$set(d)
             },
             i(e) {
-                l || (Re(n), Re(a.$$.fragment, e), l = !0)
+                l || (Ve(n), Ve(a.$$.fragment, e), l = !0)
             },
             o(e) {
-                Ve(n), Ve(a.$$.fragment, e), l = !1
+                Oe(n), Oe(a.$$.fragment, e), l = !1
             },
             d(e) {
-                s[t].d(e), e && R(i), qe(a, e)
+                s[t].d(e), e && R(i), Me(a, e)
             }
         }
     }
 
-    function ii(e, n, i) {
+    function si(e, n, i) {
         let a, r, l, o = t,
             s = () => (o(), o = u(c, (e => i(9, l = e))), c);
         e.$$.on_destroy.push((() => o()));
         let {
             data: c
         } = n;
         s();
@@ -4122,15 +4255,15 @@
         } = n, {
             createTeam: f
         } = n, {
             showDialog: h
         } = n, {
             showAutoBalance: m
         } = n;
-        const p = ue();
+        const p = de();
         let v, y = new Map;
 
         function E(e) {
             g(c, l.teams = l.teams.filter((t => t !== e)), l)
         }
 
         function b(e, t) {
@@ -4139,15 +4272,15 @@
         return e.$$set = e => {
             "data" in e && s(i(2, c = e.data)), "currentSession" in e && i(0, d = e.currentSession), "currentSessionSelected" in e && i(3, A = e.currentSessionSelected), "createTeam" in e && i(4, f = e.createTeam), "showDialog" in e && i(1, h = e.showDialog), "showAutoBalance" in e && i(5, m = e.showAutoBalance)
         }, e.$$.update = () => {
             1 & e.$$.dirty[0] && i(8, a = null === d), 769 & e.$$.dirty[0] && i(7, r = a ? l.teams : l.teams.filter((e => !e.session || e.session === d || void 0 === d))), 960 & e.$$.dirty[0] && a && (i(6, y = new Map), l.sessions.forEach((e => y.set(e, []))), r.forEach((e => {
                 e.players.length && (y.has(e.session) || y.set(e.session, []), y.get(e.session).push(e))
             })))
         }, [d, h, c, A, f, m, y, r, a, l, v, p, E, b, e => l.sessions.find((t => t.id === e)).name, e => l.players.find((t => t.id === e)), function(t) {
-            de.call(this, e, t)
+            Ae.call(this, e, t)
         }, e => {
             E(e)
         }, (e, t) => {
             b(t, e)
         }, (e, t) => {
             const n = t.detail || {
                 team: e
@@ -4176,83 +4309,83 @@
             }), g(c, l.teams = [e, ...l.teams], l), i(10, v = !1)
         }, () => {
             i(1, h = !0), i(10, v = !1)
         }, function(e) {
             v = e, i(10, v)
         }]
     }
-    class ai extends Ze {
+    class ci extends Ye {
         constructor(e) {
-            super(), Ke(this, e, ii, ni, s, {
+            super(), Ze(this, e, si, oi, s, {
                 data: 2,
                 currentSession: 0,
                 currentSessionSelected: 3,
                 createTeam: 4,
                 showDialog: 1,
                 showAutoBalance: 5
             }, null, [-1, -1])
         }
     }
 
-    function ri(e, t, n) {
+    function ui(e, t, n) {
         const i = e.slice();
         return i[36] = t[n], i
     }
 
-    function li(e, t, n) {
+    function di(e, t, n) {
         const i = e.slice();
         return i[39] = t[n], i
     }
 
-    function oi(e, t, n) {
+    function Ai(e, t, n) {
         const i = e.slice();
         return i[42] = t[n], i
     }
 
-    function si(e) {
+    function fi(e) {
         let t, n;
-        return t = new Ot({
+        return t = new Xt({
             props: {
                 $$slots: {
-                    default: [di]
+                    default: [pi]
                 },
                 $$scope: {
                     ctx: e
                 }
             }
         }), {
             c() {
-                We(t.$$.fragment)
+                Je(t.$$.fragment)
             },
             l(e) {
-                Je(t.$$.fragment, e)
+                je(t.$$.fragment, e)
             },
             m(e, i) {
-                je(t, e, i), n = !0
+                qe(t, e, i), n = !0
             },
             p(e, n) {
                 const i = {};
                 8206 & n[0] | 16384 & n[1] && (i.$$scope = {
                     dirty: n,
                     ctx: e
                 }), t.$set(i)
             },
             i(e) {
-                n || (Re(t.$$.fragment, e), n = !0)
+                n || (Ve(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Ve(t.$$.fragment, e), n = !1
+                Oe(t.$$.fragment, e), n = !1
             },
             d(e) {
-                qe(t, e)
+                Me(t, e)
             }
         }
     }
 
-    function ci(e) {
+    function hi(e) {
         let t, n = (e[42] ? e[42].name : "Summary") + "";
         return {
             c() {
                 t = F(n)
             },
             l(e) {
                 t = q(e, n)
@@ -4265,127 +4398,127 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function ui(e, t) {
+    function mi(e, t) {
         var n, i, a;
         let r, l, o, s;
 
         function c(e) {
             t[20](e)
         }
         let u = {
-            badge: t[2][null == (n = t[42]) ? void 0 : n.id] && t[2][null == (i = t[42]) ? void 0 : i.id].filter(Pi).length || null,
+            badge: t[2][null == (n = t[42]) ? void 0 : n.id] && t[2][null == (i = t[42]) ? void 0 : i.id].filter(Vi).length || null,
             outline: !t[42] && !t[3].length,
             value: (null == (a = t[42]) ? void 0 : a.id) || null,
             $$slots: {
-                default: [ci]
+                default: [hi]
             },
             $$scope: {
                 ctx: t
             }
         };
         return void 0 !== t[1] && (u.state = t[1]), l = new Ut({
             props: u
-        }), fe.push((() => Qe(l, "state", c))), {
+        }), he.push((() => We(l, "state", c))), {
             key: e,
             first: null,
             c() {
-                r = z(), We(l.$$.fragment), this.h()
+                r = U(), Je(l.$$.fragment), this.h()
             },
             l(e) {
-                r = z(), Je(l.$$.fragment, e), this.h()
+                r = U(), je(l.$$.fragment, e), this.h()
             },
             h() {
                 this.first = r
             },
             m(e, t) {
-                k(e, r, t), je(l, e, t), s = !0
+                k(e, r, t), qe(l, e, t), s = !0
             },
             p(e, n) {
                 var i, a, r;
                 t = e;
                 const s = {};
-                8196 & n[0] && (s.badge = t[2][null == (i = t[42]) ? void 0 : i.id] && t[2][null == (a = t[42]) ? void 0 : a.id].filter(Pi).length || null), 8200 & n[0] && (s.outline = !t[42] && !t[3].length), 8192 & n[0] && (s.value = (null == (r = t[42]) ? void 0 : r.id) || null), 8192 & n[0] | 16384 & n[1] && (s.$$scope = {
+                8196 & n[0] && (s.badge = t[2][null == (i = t[42]) ? void 0 : i.id] && t[2][null == (a = t[42]) ? void 0 : a.id].filter(Vi).length || null), 8200 & n[0] && (s.outline = !t[42] && !t[3].length), 8192 & n[0] && (s.value = (null == (r = t[42]) ? void 0 : r.id) || null), 8192 & n[0] | 16384 & n[1] && (s.$$scope = {
                     dirty: n,
                     ctx: t
-                }), !o && 2 & n[0] && (o = !0, s.state = t[1], ye((() => o = !1))), l.$set(s)
+                }), !o && 2 & n[0] && (o = !0, s.state = t[1], Ee((() => o = !1))), l.$set(s)
             },
             i(e) {
-                s || (Re(l.$$.fragment, e), s = !0)
+                s || (Ve(l.$$.fragment, e), s = !0)
             },
             o(e) {
-                Ve(l.$$.fragment, e), s = !1
+                Oe(l.$$.fragment, e), s = !1
             },
             d(e) {
-                e && R(r), qe(l, e)
+                e && R(r), Me(l, e)
             }
         }
     }
 
-    function di(e) {
+    function pi(e) {
         let t, n, i = [],
             a = new Map,
             r = e[13];
         const l = e => {
             var t;
             return null == (t = e[42]) ? void 0 : t.id
         };
         for (let o = 0; o < r.length; o += 1) {
-            let t = oi(e, r, o),
+            let t = Ai(e, r, o),
                 n = l(t);
-            a.set(n, i[o] = ui(n, t))
+            a.set(n, i[o] = mi(n, t))
         }
         return {
             c() {
                 for (let e = 0; e < i.length; e += 1) i[e].c();
-                t = z()
+                t = U()
             },
             l(e) {
                 for (let t = 0; t < i.length; t += 1) i[t].l(e);
-                t = z()
+                t = U()
             },
             m(e, a) {
                 for (let t = 0; t < i.length; t += 1) i[t].m(e, a);
                 k(e, t, a), n = !0
             },
             p(e, n) {
-                8206 & n[0] && (r = e[13], xe(), i = Ne(i, n, l, 1, e, r, a, t.parentNode, De, ui, t, oi), ke())
+                8206 & n[0] && (r = e[13], ke(), i = Qe(i, n, l, 1, e, r, a, t.parentNode, He, mi, t, Ai), Re())
             },
             i(e) {
                 if (!n) {
-                    for (let e = 0; e < r.length; e += 1) Re(i[e]);
+                    for (let e = 0; e < r.length; e += 1) Ve(i[e]);
                     n = !0
                 }
             },
             o(e) {
-                for (let t = 0; t < i.length; t += 1) Ve(i[t]);
+                for (let t = 0; t < i.length; t += 1) Oe(i[t]);
                 n = !1
             },
             d(e) {
                 for (let t = 0; t < i.length; t += 1) i[t].d(e);
                 e && R(t)
             }
         }
     }
 
-    function Ai(e) {
+    function gi(e) {
         let n, i, a, r, l;
 
         function o(e, t) {
-            return e[5] && null !== e[1] ? pi : gi
+            return e[5] && null !== e[1] ? bi : Ii
         }
         let s = o(e),
             c = s(e);
         return {
             c() {
-                n = O("div"), i = X("svg"), a = X("path"), r = U(), l = O("p"), c.c(), this.h()
+                n = O("div"), i = X("svg"), a = X("path"), r = T(), l = O("p"), c.c(), this.h()
             },
             l(e) {
                 n = j(e, "DIV", {
                     class: !0
                 });
                 var t = W(n);
                 i = j(t, "svg", {
@@ -4416,19 +4549,19 @@
             o: t,
             d(e) {
                 e && R(n), c.d()
             }
         }
     }
 
-    function fi(e) {
+    function vi(e) {
         let n, i, a, r, l, o, s, c, u;
         return {
             c() {
-                n = O("div"), i = O("h3"), a = F("There are no players registered."), r = U(), l = O("p"), o = F("Once players have accepted their invitation from the marketplace, they\n          will appear in this list."), s = U(), c = O("p"), u = F("All unassigned players must either be assigned to teams or made\n          inactive before the game may begin."), this.h()
+                n = O("div"), i = O("h3"), a = F("There are no players registered."), r = T(), l = O("p"), o = F("Once players have accepted their invitation from the marketplace, they\n          will appear in this list."), s = T(), c = O("p"), u = F("All unassigned players must either be assigned to teams or made\n          inactive before the game may begin."), this.h()
             },
             l(e) {
                 n = j(e, "DIV", {
                     class: !0
                 });
                 var t = W(n);
                 i = j(t, "H3", {
@@ -4456,21 +4589,21 @@
             o: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function hi(e) {
+    function yi(e) {
         let n, i, a, r, l = e[11],
             o = [];
-        for (let t = 0; t < l.length; t += 1) o[t] = wi(li(e, l, t));
+        for (let t = 0; t < l.length; t += 1) o[t] = Pi(di(e, l, t));
         return {
             c() {
-                n = O("div"), i = X("svg"), a = X("path"), r = U();
+                n = O("div"), i = X("svg"), a = X("path"), r = T();
                 for (let e = 0; e < o.length; e += 1) o[e].c();
                 this.h()
             },
             l(e) {
                 n = j(e, "DIV", {
                     class: !0
                 });
@@ -4498,71 +4631,71 @@
                 k(e, n, t), x(n, i), x(i, a), x(n, r);
                 for (let i = 0; i < o.length; i += 1) o[i].m(n, null)
             },
             p(e, t) {
                 if (2112 & t[0]) {
                     let i;
                     for (l = e[11], i = 0; i < l.length; i += 1) {
-                        const a = li(e, l, i);
-                        o[i] ? o[i].p(a, t) : (o[i] = wi(a), o[i].c(), o[i].m(n, null))
+                        const a = di(e, l, i);
+                        o[i] ? o[i].p(a, t) : (o[i] = Pi(a), o[i].c(), o[i].m(n, null))
                     }
                     for (; i < o.length; i += 1) o[i].d(1);
                     o.length = l.length
                 }
             },
             i: t,
             o: t,
             d(e) {
                 e && R(n), V(o, e)
             }
         }
     }
 
-    function mi(e) {
+    function Ei(e) {
         let t, n, i;
-        return n = new on({
+        return n = new An({
             props: {
                 selected: e[4],
                 players: e[12],
                 unassignedIsError: e[5] && null === e[1]
             }
         }), n.$on("selectPlayer", e[23]), n.$on("addPlayers", e[24]), {
             c() {
-                t = O("div"), We(n.$$.fragment), this.h()
+                t = O("div"), Je(n.$$.fragment), this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
                     class: !0
                 });
                 var i = W(t);
-                Je(n.$$.fragment, i), i.forEach(R), this.h()
+                je(n.$$.fragment, i), i.forEach(R), this.h()
             },
             h() {
                 N(t, "class", "player-col")
             },
             m(e, a) {
-                k(e, t, a), je(n, t, null), i = !0
+                k(e, t, a), qe(n, t, null), i = !0
             },
             p(e, t) {
                 const i = {};
                 16 & t[0] && (i.selected = e[4]), 4096 & t[0] && (i.players = e[12]), 34 & t[0] && (i.unassignedIsError = e[5] && null === e[1]), n.$set(i)
             },
             i(e) {
-                i || (Re(n.$$.fragment, e), i = !0)
+                i || (Ve(n.$$.fragment, e), i = !0)
             },
             o(e) {
-                Ve(n.$$.fragment, e), i = !1
+                Oe(n.$$.fragment, e), i = !1
             },
             d(e) {
-                e && R(t), qe(n)
+                e && R(t), Me(n)
             }
         }
     }
 
-    function pi(e) {
+    function bi(e) {
         let n;
         return {
             c() {
                 n = F("All players are assigned for this session group.")
             },
             l(e) {
                 n = q(e, "All players are assigned for this session group.")
@@ -4573,42 +4706,42 @@
             p: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function gi(e) {
+    function Ii(e) {
         let t;
 
         function n(e, t) {
-            return e[10].length ? yi : vi
+            return e[10].length ? Ci : wi
         }
         let i = n(e),
             a = i(e);
         return {
             c() {
-                a.c(), t = z()
+                a.c(), t = U()
             },
             l(e) {
-                a.l(e), t = z()
+                a.l(e), t = U()
             },
             m(e, n) {
                 a.m(e, n), k(e, t, n)
             },
             p(e, r) {
                 i !== (i = n(e)) && (a.d(1), a = i(e), a && (a.c(), a.m(t.parentNode, t)))
             },
             d(e) {
                 a.d(e), e && R(t)
             }
         }
     }
 
-    function vi(e) {
+    function wi(e) {
         let t;
         return {
             c() {
                 t = F("All players are assigned to teams.")
             },
             l(e) {
                 t = q(e, "All players are assigned to teams.")
@@ -4618,15 +4751,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function yi(e) {
+    function Ci(e) {
         let t, n, i, a;
         return {
             c() {
                 t = F("All players are assigned to teams or marked "), n = O("a"), i = F("Inactive"), a = F("."), this.h()
             },
             l(e) {
                 t = q(e, "All players are assigned to teams or marked "), n = j(e, "A", {
@@ -4643,15 +4776,15 @@
             },
             d(e) {
                 e && R(t), e && R(n), e && R(a)
             }
         }
     }
 
-    function Ei(e) {
+    function Bi(e) {
         let t, n, i, a, r, l, o = e[39].name + "",
             s = e[6].maximumPlayers + "";
         return {
             c() {
                 t = O("strong"), n = F(o), i = F(" must have\n              "), a = O("strong"), r = F(s), l = F(" players to begin.")
             },
             l(e) {
@@ -4669,15 +4802,15 @@
             },
             d(e) {
                 e && R(t), e && R(i), e && R(a), e && R(l)
             }
         }
     }
 
-    function bi(e) {
+    function Si(e) {
         let t, n, i, a, r, l, o, s, c, u = e[39].name + "",
             d = e[6].minimumPlayers + "",
             A = e[6].maximumPlayers + "";
         return {
             c() {
                 t = O("strong"), n = F(u), i = F(" must have\n              "), a = O("strong"), r = F(d), l = F("\n              to\n              "), o = O("strong"), s = F(A), c = F(" players to begin.")
             },
@@ -4698,15 +4831,15 @@
             },
             d(e) {
                 e && R(t), e && R(i), e && R(a), e && R(l), e && R(o), e && R(c)
             }
         }
     }
 
-    function Ii(e) {
+    function Li(e) {
         let t, n, i, a, r, l, o = e[39].name + "",
             s = e[6].minimumPlayers + "";
         return {
             c() {
                 t = O("strong"), n = F(o), i = F(" must have\n              "), a = O("strong"), r = F(s), l = F(" players to begin.")
             },
             l(e) {
@@ -4724,25 +4857,25 @@
             },
             d(e) {
                 e && R(t), e && R(i), e && R(a), e && R(l)
             }
         }
     }
 
-    function wi(e) {
+    function Pi(e) {
         let t, n;
 
         function i(e, t) {
-            return !e[6].minimumPlayers || e[6].maximumPlayers && e[6].maximumPlayers !== e[6].minimumPlayers ? e[6].minimumPlayers && e[6].maximumPlayers ? bi : Ei : Ii
+            return !e[6].minimumPlayers || e[6].maximumPlayers && e[6].maximumPlayers !== e[6].minimumPlayers ? e[6].minimumPlayers && e[6].maximumPlayers ? Si : Bi : Li
         }
         let a = i(e),
             r = a(e);
         return {
             c() {
-                t = O("p"), r.c(), n = U(), this.h()
+                t = O("p"), r.c(), n = T(), this.h()
             },
             l(e) {
                 t = j(e, "P", {
                     class: !0
                 });
                 var i = W(t);
                 r.l(i), n = M(i), i.forEach(R), this.h()
@@ -4758,221 +4891,221 @@
             },
             d(e) {
                 e && R(t), r.d()
             }
         }
     }
 
-    function Ci(e) {
+    function xi(e) {
         let t, n, i, a, r;
-        return i = new on({
+        return i = new An({
             props: {
                 inactive: !0,
                 selected: e[4],
                 players: e[10],
                 unassignedIsError: e[5] && null === e[1]
             }
         }), i.$on("selectPlayer", e[33]), i.$on("addPlayers", e[34]), {
             c() {
-                t = O("div"), n = O("div"), We(i.$$.fragment), a = U(), this.h()
+                t = O("div"), n = O("div"), Je(i.$$.fragment), a = T(), this.h()
             },
             l(e) {
                 t = j(e, "DIV", {
                     class: !0
                 });
                 var r = W(t);
                 n = j(r, "DIV", {
                     class: !0
                 });
                 var l = W(n);
-                Je(i.$$.fragment, l), l.forEach(R), a = M(r), r.forEach(R), this.h()
+                je(i.$$.fragment, l), l.forEach(R), a = M(r), r.forEach(R), this.h()
             },
             h() {
                 N(n, "class", "player-col"), N(t, "class", "player-grid")
             },
             m(e, l) {
-                k(e, t, l), x(t, n), je(i, n, null), x(t, a), r = !0
+                k(e, t, l), x(t, n), qe(i, n, null), x(t, a), r = !0
             },
             p(e, t) {
                 const n = {};
                 16 & t[0] && (n.selected = e[4]), 1024 & t[0] && (n.players = e[10]), 34 & t[0] && (n.unassignedIsError = e[5] && null === e[1]), i.$set(n)
             },
             i(e) {
-                r || (Re(i.$$.fragment, e), r = !0)
+                r || (Ve(i.$$.fragment, e), r = !0)
             },
             o(e) {
-                Ve(i.$$.fragment, e), r = !1
+                Oe(i.$$.fragment, e), r = !1
             },
             d(e) {
-                e && R(t), qe(i)
+                e && R(t), Me(i)
             }
         }
     }
 
-    function Bi(e, t) {
+    function ki(e, t) {
         let n, i, a, r, l, o, s, c, u, d, A, f, h, m;
-        const p = [mi, hi, fi, Ai],
+        const p = [Ei, yi, vi, gi],
             g = [];
 
         function v(e, t) {
             var n, i;
             return e[12].length ? 0 : e[11].length ? 1 : (null == (i = null == (n = e[6]) ? void 0 : n.players) ? void 0 : i.length) ? 3 : 2
         }
 
         function y(e) {
             t[25](e)
         }
         i = v(t), a = g[i] = p[i](t);
         let E = {
             unassigned: t[3].length,
-            data: $e,
+            data: _e,
             inactive: t[10].length,
             downloadPlayersUrl: t[0],
             showAutoBalance: t[9],
             allowCreate: !t[5] || null !== t[1]
         };
 
         function b(e) {
             t[28](e)
         }
 
         function I(e) {
             t[29](e)
         }
-        void 0 !== t[1] && (E.currentSession = t[1]), o = new En({
+        void 0 !== t[1] && (E.currentSession = t[1]), o = new Bn({
             props: E
-        }), fe.push((() => Qe(o, "currentSession", y))), o.$on("clickCreateTeam", t[26]), o.$on("openAutoBalance", t[27]);
+        }), he.push((() => We(o, "currentSession", y))), o.$on("clickCreateTeam", t[26]), o.$on("openAutoBalance", t[27]);
         let w = {
-            data: $e,
+            data: _e,
             currentSessionSelected: t[8],
             createTeam: t[14],
             showAutoBalance: t[9]
         };
-        void 0 !== t[1] && (w.currentSession = t[1]), void 0 !== t[7] && (w.showDialog = t[7]), u = new ai({
+        void 0 !== t[1] && (w.currentSession = t[1]), void 0 !== t[7] && (w.showDialog = t[7]), u = new ci({
             props: w
-        }), fe.push((() => Qe(u, "currentSession", b))), fe.push((() => Qe(u, "showDialog", I))), u.$on("selectPlayer", t[30]), u.$on("unassignPlayer", t[31]), u.$on("addPlayers", t[32]);
-        let C = t[10].length && Ci(t);
+        }), he.push((() => We(u, "currentSession", b))), he.push((() => We(u, "showDialog", I))), u.$on("selectPlayer", t[30]), u.$on("unassignPlayer", t[31]), u.$on("addPlayers", t[32]);
+        let C = t[10].length && xi(t);
         return {
             key: e,
             first: null,
             c() {
-                n = O("div"), a.c(), r = U(), l = O("div"), We(o.$$.fragment), c = U(), We(u.$$.fragment), f = U(), C && C.c(), h = z(), this.h()
+                n = O("div"), a.c(), r = T(), l = O("div"), Je(o.$$.fragment), c = T(), Je(u.$$.fragment), f = T(), C && C.c(), h = U(), this.h()
             },
             l(e) {
                 n = j(e, "DIV", {
                     class: !0
                 });
                 var t = W(n);
                 a.l(t), r = M(t), l = j(t, "DIV", {
                     class: !0
                 });
                 var i = W(l);
-                Je(o.$$.fragment, i), i.forEach(R), t.forEach(R), c = M(e), Je(u.$$.fragment, e), f = M(e), C && C.l(e), h = z(), this.h()
+                je(o.$$.fragment, i), i.forEach(R), t.forEach(R), c = M(e), je(u.$$.fragment, e), f = M(e), C && C.l(e), h = U(), this.h()
             },
             h() {
                 N(l, "class", "player-col"), N(n, "class", "player-grid"), this.first = n
             },
             m(e, t) {
-                k(e, n, t), g[i].m(n, null), x(n, r), x(n, l), je(o, l, null), k(e, c, t), je(u, e, t), k(e, f, t), C && C.m(e, t), k(e, h, t), m = !0
+                k(e, n, t), g[i].m(n, null), x(n, r), x(n, l), qe(o, l, null), k(e, c, t), qe(u, e, t), k(e, f, t), C && C.m(e, t), k(e, h, t), m = !0
             },
             p(e, l) {
                 let c = i;
-                i = v(t = e), i === c ? g[i].p(t, l) : (xe(), Ve(g[c], 1, 1, (() => {
+                i = v(t = e), i === c ? g[i].p(t, l) : (ke(), Oe(g[c], 1, 1, (() => {
                     g[c] = null
-                })), ke(), a = g[i], a ? a.p(t, l) : (a = g[i] = p[i](t), a.c()), Re(a, 1), a.m(n, r));
+                })), Re(), a = g[i], a ? a.p(t, l) : (a = g[i] = p[i](t), a.c()), Ve(a, 1), a.m(n, r));
                 const f = {};
-                8 & l[0] && (f.unassigned = t[3].length), 1024 & l[0] && (f.inactive = t[10].length), 1 & l[0] && (f.downloadPlayersUrl = t[0]), 512 & l[0] && (f.showAutoBalance = t[9]), 34 & l[0] && (f.allowCreate = !t[5] || null !== t[1]), !s && 2 & l[0] && (s = !0, f.currentSession = t[1], ye((() => s = !1))), o.$set(f);
+                8 & l[0] && (f.unassigned = t[3].length), 1024 & l[0] && (f.inactive = t[10].length), 1 & l[0] && (f.downloadPlayersUrl = t[0]), 512 & l[0] && (f.showAutoBalance = t[9]), 34 & l[0] && (f.allowCreate = !t[5] || null !== t[1]), !s && 2 & l[0] && (s = !0, f.currentSession = t[1], Ee((() => s = !1))), o.$set(f);
                 const m = {};
-                256 & l[0] && (m.currentSessionSelected = t[8]), 512 & l[0] && (m.showAutoBalance = t[9]), !d && 2 & l[0] && (d = !0, m.currentSession = t[1], ye((() => d = !1))), !A && 128 & l[0] && (A = !0, m.showDialog = t[7], ye((() => A = !1))), u.$set(m), t[10].length ? C ? (C.p(t, l), 1024 & l[0] && Re(C, 1)) : (C = Ci(t), C.c(), Re(C, 1), C.m(h.parentNode, h)) : C && (xe(), Ve(C, 1, 1, (() => {
+                256 & l[0] && (m.currentSessionSelected = t[8]), 512 & l[0] && (m.showAutoBalance = t[9]), !d && 2 & l[0] && (d = !0, m.currentSession = t[1], Ee((() => d = !1))), !A && 128 & l[0] && (A = !0, m.showDialog = t[7], Ee((() => A = !1))), u.$set(m), t[10].length ? C ? (C.p(t, l), 1024 & l[0] && Ve(C, 1)) : (C = xi(t), C.c(), Ve(C, 1), C.m(h.parentNode, h)) : C && (ke(), Oe(C, 1, 1, (() => {
                     C = null
-                })), ke())
+                })), Re())
             },
             i(e) {
-                m || (Re(a), Re(o.$$.fragment, e), Re(u.$$.fragment, e), Re(C), m = !0)
+                m || (Ve(a), Ve(o.$$.fragment, e), Ve(u.$$.fragment, e), Ve(C), m = !0)
             },
             o(e) {
-                Ve(a), Ve(o.$$.fragment, e), Ve(u.$$.fragment, e), Ve(C), m = !1
+                Oe(a), Oe(o.$$.fragment, e), Oe(u.$$.fragment, e), Oe(C), m = !1
             },
             d(e) {
-                e && R(n), g[i].d(), qe(o), e && R(c), qe(u, e), e && R(f), C && C.d(e), e && R(h)
+                e && R(n), g[i].d(), Me(o), e && R(c), Me(u, e), e && R(f), C && C.d(e), e && R(h)
             }
         }
     }
 
-    function Si(e) {
+    function Ri(e) {
         var t;
         let n, i, a, r, l, o, s = [],
             c = new Map,
-            u = e[6].sessions && e[5] && si(e);
+            u = e[6].sessions && e[5] && fi(e);
 
         function d(t) {
             e[21](t)
         }
         let A = {
-            unassigned: (null == (t = e[2][e[1]]) ? void 0 : t.filter(Li)) || []
+            unassigned: (null == (t = e[2][e[1]]) ? void 0 : t.filter(Oi)) || []
         };
-        void 0 !== e[7] && (A.open = e[7]), i = new kt({
+        void 0 !== e[7] && (A.open = e[7]), i = new Rt({
             props: A
-        }), fe.push((() => Qe(i, "open", d))), i.$on("submit", e[22]);
+        }), he.push((() => We(i, "open", d))), i.$on("submit", e[22]);
         let f = [e[1]];
         const h = e => e[36];
         for (let m = 0; m < 1; m += 1) {
-            let t = ri(e, f, m),
+            let t = ui(e, f, m),
                 n = h(t);
-            c.set(n, s[m] = Bi(n, t))
+            c.set(n, s[m] = ki(n, t))
         }
         return {
             c() {
-                u && u.c(), n = U(), We(i.$$.fragment), r = U();
+                u && u.c(), n = T(), Je(i.$$.fragment), r = T();
                 for (let e = 0; e < 1; e += 1) s[e].c();
-                l = z()
+                l = U()
             },
             l(e) {
-                u && u.l(e), n = M(e), Je(i.$$.fragment, e), r = M(e);
+                u && u.l(e), n = M(e), je(i.$$.fragment, e), r = M(e);
                 for (let t = 0; t < 1; t += 1) s[t].l(e);
-                l = z()
+                l = U()
             },
             m(e, t) {
-                u && u.m(e, t), k(e, n, t), je(i, e, t), k(e, r, t);
+                u && u.m(e, t), k(e, n, t), qe(i, e, t), k(e, r, t);
                 for (let n = 0; n < 1; n += 1) s[n].m(e, t);
                 k(e, l, t), o = !0
             },
             p(e, t) {
                 var r;
-                e[6].sessions && e[5] ? u ? (u.p(e, t), 96 & t[0] && Re(u, 1)) : (u = si(e), u.c(), Re(u, 1), u.m(n.parentNode, n)) : u && (xe(), Ve(u, 1, 1, (() => {
+                e[6].sessions && e[5] ? u ? (u.p(e, t), 96 & t[0] && Ve(u, 1)) : (u = fi(e), u.c(), Ve(u, 1), u.m(n.parentNode, n)) : u && (ke(), Oe(u, 1, 1, (() => {
                     u = null
-                })), ke());
+                })), Re());
                 const o = {};
-                6 & t[0] && (o.unassigned = (null == (r = e[2][e[1]]) ? void 0 : r.filter(Li)) || []), !a && 128 & t[0] && (a = !0, o.open = e[7], ye((() => a = !1))), i.$set(o), 253947 & t[0] && (f = [e[1]], xe(), s = Ne(s, t, h, 1, e, f, c, l.parentNode, De, Bi, l, ri), ke())
+                6 & t[0] && (o.unassigned = (null == (r = e[2][e[1]]) ? void 0 : r.filter(Oi)) || []), !a && 128 & t[0] && (a = !0, o.open = e[7], Ee((() => a = !1))), i.$set(o), 253947 & t[0] && (f = [e[1]], ke(), s = Qe(s, t, h, 1, e, f, c, l.parentNode, He, ki, l, ui), Re())
             },
             i(e) {
                 if (!o) {
-                    Re(u), Re(i.$$.fragment, e);
-                    for (let e = 0; e < 1; e += 1) Re(s[e]);
+                    Ve(u), Ve(i.$$.fragment, e);
+                    for (let e = 0; e < 1; e += 1) Ve(s[e]);
                     o = !0
                 }
             },
             o(e) {
-                Ve(u), Ve(i.$$.fragment, e);
-                for (let t = 0; t < 1; t += 1) Ve(s[t]);
+                Oe(u), Oe(i.$$.fragment, e);
+                for (let t = 0; t < 1; t += 1) Oe(s[t]);
                 o = !1
             },
             d(e) {
-                u && u.d(e), e && R(n), qe(i, e), e && R(r);
+                u && u.d(e), e && R(n), Me(i, e), e && R(r);
                 for (let t = 0; t < 1; t += 1) s[t].d(e);
                 e && R(l)
             }
         }
     }
-    const Pi = e => !e.inactive,
-        Li = e => !e.inactive;
+    const Vi = e => !e.inactive,
+        Oi = e => !e.inactive;
 
-    function xi(e, t, n) {
+    function Xi(e, t, n) {
         let i, a, r, l, o, s, c;
-        d(e, $e, (e => n(6, c = e)));
+        d(e, _e, (e => n(6, c = e)));
         let u = !1,
             {
                 nextStep: A = null
             } = t,
             {
                 downloadPlayersUrl: f = null
             } = t;
@@ -5031,15 +5164,15 @@
             minimumPlayers: 2,
             maximumPlayers: 4
         };
         h.players.map((e => e.email = `${e.name.replace(" ",".").toLowerCase()}@wharton.edu`));
         let m, {
             example: p = null
         } = t;
-        p && g($e, c = h, c);
+        p && g(_e, c = h, c);
         let v = {},
             y = [];
         const E = ({
             name: e = null,
             session: t = null
         } = {}) => {
             if (!e) {
@@ -5056,35 +5189,35 @@
         let b = [];
         const I = e => {
             b.includes(e) ? n(4, b = b.filter((t => t !== e))) : n(4, b = [...b, e])
         };
         let w = [];
         const C = e => {
                 for (const t of c.teams) t.players = t.players.filter((t => t !== e));
-                $e.set(c)
+                _e.set(c)
             },
             B = ({
                 team: e,
                 onlyUnassigned: t = !1,
                 adding: i = null,
                 session: a = null
             }) => {
                 const l = c.teams;
                 if (e || (e = E({
                         session: a
-                    }), g($e, c.teams = [...c.teams, e], c)), null === i && (i = w, t)) {
+                    }), g(_e, c.teams = [...c.teams, e], c)), null === i && (i = w, t)) {
                     const e = l.flatMap((e => e.players)),
                         t = i.filter((t => e.includes(t)));
                     i = i.filter((e => !t.includes(e) && !r.map((e => e.id)).includes(e)))
                 }
                 e.players = [...e.players, ...i.filter((t => !e.players.includes(t)))];
                 for (const n of l.filter((t => t !== e))) n.players = n.players.filter((e => !i.includes(e)));
                 r.filter((e => i.includes(e.id))).map((e => {
                     e.inactive = !1
-                })), $e.set(c), n(4, b = b.filter((t => !e.players.includes(t)))), a && m && n(1, m = a)
+                })), _e.set(c), n(4, b = b.filter((t => !e.players.includes(t)))), a && m && n(1, m = a)
             };
         return e.$$set = e => {
             "nextStep" in e && n(18, A = e.nextStep), "downloadPlayersUrl" in e && n(0, f = e.downloadPlayersUrl), "example" in e && n(19, p = e.example)
         }, e.$$.update = () => {
             var t, u, d, A;
             if (64 & e.$$.dirty[0] && n(5, i = (null == (t = null == c ? void 0 : c.sessions) ? void 0 : t.length) > 1), 96 & e.$$.dirty[0] && n(13, a = i ? [...c.sessions, null] : c.sessions), 106 & e.$$.dirty[0] && (null == c ? void 0 : c.players)) {
                 const e = c.teams.flatMap((e => e.players));
@@ -5116,24 +5249,24 @@
                         i = e[t];
                     e[t] = e[n], e[n] = i
                 }
             }(r);
             for (const n of r) i.length ? a = i.shift() : (a = E(), c.teams.unshift(a)), a.players.push(n.id), a.players.length < t && i.unshift(a);
             c.teams.forEach((e => {
                 delete e.ready
-            })), $e.set(c), n(4, b = [])
+            })), _e.set(c), n(4, b = [])
         }, e => {
             I(e.detail.id)
         }, e => {
             B(e.detail)
         }, function(e) {
             m = e, n(1, m), n(6, c), n(5, i), n(3, y)
         }, () => {
             const e = E();
-            g($e, c.teams = [...c.teams, e], c), B({
+            g(_e, c.teams = [...c.teams, e], c), B({
                 team: e,
                 onlyUnassigned: !0
             })
         }, () => {
             n(7, u = !0)
         }, function(e) {
             m = e, n(1, m), n(6, c), n(5, i), n(3, y)
@@ -5147,46 +5280,46 @@
             B(e.detail)
         }, e => {
             I(e.detail.id)
         }, e => {
             B(e.detail)
         }]
     }
-    class ki extends Ze {
+    class Fi extends Ye {
         constructor(e) {
-            super(), Ke(this, e, xi, Si, s, {
+            super(), Ze(this, e, Xi, Ri, s, {
                 nextStep: 18,
                 downloadPlayersUrl: 0,
                 example: 19
             }, null, [-1, -1])
         }
     }
-    var Ri = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
+    var Ti = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : "undefined" != typeof global ? global : "undefined" != typeof self ? self : {};
 
-    function Vi(e) {
+    function Ui(e) {
         if (e.__esModule) return e;
         var t = Object.defineProperty({}, "__esModule", {
             value: !0
         });
         return Object.keys(e).forEach((function(n) {
             var i = Object.getOwnPropertyDescriptor(e, n);
             Object.defineProperty(t, n, i.get ? i : {
                 enumerable: !0,
                 get: function() {
                     return e[n]
                 }
             })
         })), t
     }
-    var Oi = {},
-        Xi = {
+    var zi = {},
+        Di = {
             exports: {}
         };
     ! function(e, t) {
-        var n, i = "undefined" != typeof self ? self : Ri,
+        var n, i = "undefined" != typeof self ? self : Ti,
             a = function() {
                 function e() {
                     this.fetch = !1, this.DOMException = i.DOMException
                 }
                 return e.prototype = i, new e
             }();
         n = a,
@@ -5432,51 +5565,51 @@
                 }
                 w.polyfill = !0, n.fetch || (n.fetch = w, n.Headers = A, n.Request = y, n.Response = b), e.Headers = A, e.Request = y, e.Response = b, e.fetch = w, Object.defineProperty(e, "__esModule", {
                     value: !0
                 })
             }({}), a.fetch.ponyfill = !0, delete a.fetch.polyfill;
         var r = a;
         (t = r.fetch).default = r.fetch, t.fetch = r.fetch, t.Headers = r.Headers, t.Request = r.Request, t.Response = r.Response, e.exports = t
-    }(Xi, Xi.exports);
-    var Fi = "function" == typeof Symbol && "function" == typeof Symbol.for ? Symbol.for("nodejs.util.inspect.custom") : void 0;
+    }(Di, Di.exports);
+    var Hi = "function" == typeof Symbol && "function" == typeof Symbol.for ? Symbol.for("nodejs.util.inspect.custom") : void 0;
 
-    function Ui(e) {
-        return (Ui = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Ni(e) {
+        return (Ni = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function zi(e) {
-        return Ti(e, [])
+    function Qi(e) {
+        return Wi(e, [])
     }
 
-    function Ti(e, t) {
-        switch (Ui(e)) {
+    function Wi(e, t) {
+        switch (Ni(e)) {
             case "string":
                 return JSON.stringify(e);
             case "function":
                 return e.name ? "[function ".concat(e.name, "]") : "[function]";
             case "object":
                 return null === e ? "null" : function(e, t) {
                     if (-1 !== t.indexOf(e)) return "[Circular]";
                     var n = [].concat(t, [e]),
                         i = function(e) {
-                            var t = e[String(Fi)];
+                            var t = e[String(Hi)];
                             if ("function" == typeof t) return t;
                             if ("function" == typeof e.inspect) return e.inspect
                         }(e);
                     if (void 0 !== i) {
                         var a = i.call(e);
-                        if (a !== e) return "string" == typeof a ? a : Ti(a, n)
+                        if (a !== e) return "string" == typeof a ? a : Wi(a, n)
                     } else if (Array.isArray(e)) return function(e, t) {
                         if (0 === e.length) return "[]";
                         if (t.length > 2) return "[Array]";
-                        for (var n = Math.min(10, e.length), i = e.length - n, a = [], r = 0; r < n; ++r) a.push(Ti(e[r], t));
+                        for (var n = Math.min(10, e.length), i = e.length - n, a = [], r = 0; r < n; ++r) a.push(Wi(e[r], t));
                         1 === i ? a.push("... 1 more item") : i > 1 && a.push("... ".concat(i, " more items"));
                         return "[" + a.join(", ") + "]"
                     }(e, n);
                     return function(e, t) {
                         var n = Object.keys(e);
                         if (0 === n.length) return "{}";
                         if (t.length > 2) return "[" + function(e) {
@@ -5484,57 +5617,57 @@
                             if ("Object" === t && "function" == typeof e.constructor) {
                                 var n = e.constructor.name;
                                 if ("string" == typeof n && "" !== n) return n
                             }
                             return t
                         }(e) + "]";
                         return "{ " + n.map((function(n) {
-                            return n + ": " + Ti(e[n], t)
+                            return n + ": " + Wi(e[n], t)
                         })).join(", ") + " }"
                     }(e, n)
                 }(e, t);
             default:
                 return String(e)
         }
     }
 
-    function Di(e) {
+    function Ji(e) {
         var t = e.prototype.toJSON;
         "function" == typeof t || function(e, t) {
             if (!Boolean(e)) throw new Error(null != t ? t : "Unexpected invariant triggered.")
-        }(0), e.prototype.inspect = t, Fi && (e.prototype[Fi] = t)
+        }(0), e.prototype.inspect = t, Hi && (e.prototype[Hi] = t)
     }
 
-    function Hi(e) {
+    function ji(e) {
         return null != e && "string" == typeof e.kind
     }
-    Di(function() {
+    Ji(function() {
         function e(e, t, n) {
             this.start = e.start, this.end = t.end, this.startToken = e, this.endToken = t, this.source = n
         }
         return e.prototype.toJSON = function() {
             return {
                 start: this.start,
                 end: this.end
             }
         }, e
-    }()), Di(function() {
+    }()), Ji(function() {
         function e(e, t, n, i, a, r, l) {
             this.kind = e, this.start = t, this.end = n, this.line = i, this.column = a, this.value = l, this.prev = r, this.next = null
         }
         return e.prototype.toJSON = function() {
             return {
                 kind: this.kind,
                 value: this.value,
                 line: this.line,
                 column: this.column
             }
         }, e
     }());
-    var Ni = {
+    var qi = {
             Name: [],
             Document: ["definitions"],
             OperationDefinition: ["name", "variableDefinitions", "directives", "selectionSet"],
             VariableDefinition: ["variable", "type", "defaultValue", "directives"],
             Variable: ["name"],
             SelectionSet: ["selections"],
             Field: ["alias", "name", "arguments", "directives", "selectionSet"],
@@ -5571,88 +5704,88 @@
             ScalarTypeExtension: ["name", "directives"],
             ObjectTypeExtension: ["name", "interfaces", "directives", "fields"],
             InterfaceTypeExtension: ["name", "interfaces", "directives", "fields"],
             UnionTypeExtension: ["name", "directives", "types"],
             EnumTypeExtension: ["name", "directives", "values"],
             InputObjectTypeExtension: ["name", "directives", "fields"]
         },
-        Qi = Object.freeze({});
+        Mi = Object.freeze({});
 
-    function Wi(e, t, n) {
+    function Ki(e, t, n) {
         var i = e[t];
         if (i) {
             if (!n && "function" == typeof i) return i;
             var a = n ? i.leave : i.enter;
             if ("function" == typeof a) return a
         } else {
             var r = n ? e.leave : e.enter;
             if (r) {
                 if ("function" == typeof r) return r;
                 var l = r[t];
                 if ("function" == typeof l) return l
             }
         }
     }
-    var Ji = {
+    var Zi = {
         Name: function(e) {
             return e.value
         },
         Variable: function(e) {
             return "$" + e.name
         },
         Document: function(e) {
-            return qi(e.definitions, "\n\n") + "\n"
+            return Gi(e.definitions, "\n\n") + "\n"
         },
         OperationDefinition: function(e) {
             var t = e.operation,
                 n = e.name,
-                i = Ki("(", qi(e.variableDefinitions, ", "), ")"),
-                a = qi(e.directives, " "),
+                i = _i("(", Gi(e.variableDefinitions, ", "), ")"),
+                a = Gi(e.directives, " "),
                 r = e.selectionSet;
-            return n || a || i || "query" !== t ? qi([t, qi([n, i]), a, r], " ") : r
+            return n || a || i || "query" !== t ? Gi([t, Gi([n, i]), a, r], " ") : r
         },
         VariableDefinition: function(e) {
             var t = e.variable,
                 n = e.type,
                 i = e.defaultValue,
                 a = e.directives;
-            return t + ": " + n + Ki(" = ", i) + Ki(" ", qi(a, " "))
+            return t + ": " + n + _i(" = ", i) + _i(" ", Gi(a, " "))
         },
         SelectionSet: function(e) {
-            return Mi(e.selections)
+            return $i(e.selections)
         },
         Field: function(e) {
             var t = e.alias,
                 n = e.name,
                 i = e.arguments,
                 a = e.directives,
                 r = e.selectionSet,
-                l = Ki("", t, ": ") + n,
-                o = l + Ki("(", qi(i, ", "), ")");
-            return o.length > 80 && (o = l + Ki("(\n", Zi(qi(i, "\n")), "\n)")), qi([o, qi(a, " "), r], " ")
+                l = _i("", t, ": ") + n,
+                o = l + _i("(", Gi(i, ", "), ")");
+            return o.length > 80 && (o = l + _i("(\n", ea(Gi(i, "\n")), "\n)")), Gi([o, Gi(a, " "), r], " ")
         },
         Argument: function(e) {
             return e.name + ": " + e.value
         },
         FragmentSpread: function(e) {
-            return "..." + e.name + Ki(" ", qi(e.directives, " "))
+            return "..." + e.name + _i(" ", Gi(e.directives, " "))
         },
         InlineFragment: function(e) {
             var t = e.typeCondition,
                 n = e.directives,
                 i = e.selectionSet;
-            return qi(["...", Ki("on ", t), qi(n, " "), i], " ")
+            return Gi(["...", _i("on ", t), Gi(n, " "), i], " ")
         },
         FragmentDefinition: function(e) {
             var t = e.name,
                 n = e.typeCondition,
                 i = e.variableDefinitions,
                 a = e.directives,
                 r = e.selectionSet;
-            return "fragment ".concat(t).concat(Ki("(", qi(i, ", "), ")"), " ") + "on ".concat(n, " ").concat(Ki("", qi(a, " "), " ")) + r
+            return "fragment ".concat(t).concat(_i("(", Gi(i, ", "), ")"), " ") + "on ".concat(n, " ").concat(_i("", Gi(a, " "), " ")) + r
         },
         IntValue: function(e) {
             return e.value
         },
         FloatValue: function(e) {
             return e.value
         },
@@ -5676,182 +5809,182 @@
         NullValue: function() {
             return "null"
         },
         EnumValue: function(e) {
             return e.value
         },
         ListValue: function(e) {
-            return "[" + qi(e.values, ", ") + "]"
+            return "[" + Gi(e.values, ", ") + "]"
         },
         ObjectValue: function(e) {
-            return "{" + qi(e.fields, ", ") + "}"
+            return "{" + Gi(e.fields, ", ") + "}"
         },
         ObjectField: function(e) {
             return e.name + ": " + e.value
         },
         Directive: function(e) {
-            return "@" + e.name + Ki("(", qi(e.arguments, ", "), ")")
+            return "@" + e.name + _i("(", Gi(e.arguments, ", "), ")")
         },
         NamedType: function(e) {
             return e.name
         },
         ListType: function(e) {
             return "[" + e.type + "]"
         },
         NonNullType: function(e) {
             return e.type + "!"
         },
-        SchemaDefinition: ji((function(e) {
+        SchemaDefinition: Yi((function(e) {
             var t = e.directives,
                 n = e.operationTypes;
-            return qi(["schema", qi(t, " "), Mi(n)], " ")
+            return Gi(["schema", Gi(t, " "), $i(n)], " ")
         })),
         OperationTypeDefinition: function(e) {
             return e.operation + ": " + e.type
         },
-        ScalarTypeDefinition: ji((function(e) {
-            return qi(["scalar", e.name, qi(e.directives, " ")], " ")
+        ScalarTypeDefinition: Yi((function(e) {
+            return Gi(["scalar", e.name, Gi(e.directives, " ")], " ")
         })),
-        ObjectTypeDefinition: ji((function(e) {
+        ObjectTypeDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.interfaces,
                 i = e.directives,
                 a = e.fields;
-            return qi(["type", t, Ki("implements ", qi(n, " & ")), qi(i, " "), Mi(a)], " ")
+            return Gi(["type", t, _i("implements ", Gi(n, " & ")), Gi(i, " "), $i(a)], " ")
         })),
-        FieldDefinition: ji((function(e) {
+        FieldDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.arguments,
                 i = e.type,
                 a = e.directives;
-            return t + (Gi(n) ? Ki("(\n", Zi(qi(n, "\n")), "\n)") : Ki("(", qi(n, ", "), ")")) + ": " + i + Ki(" ", qi(a, " "))
+            return t + (na(n) ? _i("(\n", ea(Gi(n, "\n")), "\n)") : _i("(", Gi(n, ", "), ")")) + ": " + i + _i(" ", Gi(a, " "))
         })),
-        InputValueDefinition: ji((function(e) {
+        InputValueDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.type,
                 i = e.defaultValue,
                 a = e.directives;
-            return qi([t + ": " + n, Ki("= ", i), qi(a, " ")], " ")
+            return Gi([t + ": " + n, _i("= ", i), Gi(a, " ")], " ")
         })),
-        InterfaceTypeDefinition: ji((function(e) {
+        InterfaceTypeDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.interfaces,
                 i = e.directives,
                 a = e.fields;
-            return qi(["interface", t, Ki("implements ", qi(n, " & ")), qi(i, " "), Mi(a)], " ")
+            return Gi(["interface", t, _i("implements ", Gi(n, " & ")), Gi(i, " "), $i(a)], " ")
         })),
-        UnionTypeDefinition: ji((function(e) {
+        UnionTypeDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.directives,
                 i = e.types;
-            return qi(["union", t, qi(n, " "), i && 0 !== i.length ? "= " + qi(i, " | ") : ""], " ")
+            return Gi(["union", t, Gi(n, " "), i && 0 !== i.length ? "= " + Gi(i, " | ") : ""], " ")
         })),
-        EnumTypeDefinition: ji((function(e) {
+        EnumTypeDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.directives,
                 i = e.values;
-            return qi(["enum", t, qi(n, " "), Mi(i)], " ")
+            return Gi(["enum", t, Gi(n, " "), $i(i)], " ")
         })),
-        EnumValueDefinition: ji((function(e) {
-            return qi([e.name, qi(e.directives, " ")], " ")
+        EnumValueDefinition: Yi((function(e) {
+            return Gi([e.name, Gi(e.directives, " ")], " ")
         })),
-        InputObjectTypeDefinition: ji((function(e) {
+        InputObjectTypeDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.directives,
                 i = e.fields;
-            return qi(["input", t, qi(n, " "), Mi(i)], " ")
+            return Gi(["input", t, Gi(n, " "), $i(i)], " ")
         })),
-        DirectiveDefinition: ji((function(e) {
+        DirectiveDefinition: Yi((function(e) {
             var t = e.name,
                 n = e.arguments,
                 i = e.repeatable,
                 a = e.locations;
-            return "directive @" + t + (Gi(n) ? Ki("(\n", Zi(qi(n, "\n")), "\n)") : Ki("(", qi(n, ", "), ")")) + (i ? " repeatable" : "") + " on " + qi(a, " | ")
+            return "directive @" + t + (na(n) ? _i("(\n", ea(Gi(n, "\n")), "\n)") : _i("(", Gi(n, ", "), ")")) + (i ? " repeatable" : "") + " on " + Gi(a, " | ")
         })),
         SchemaExtension: function(e) {
             var t = e.directives,
                 n = e.operationTypes;
-            return qi(["extend schema", qi(t, " "), Mi(n)], " ")
+            return Gi(["extend schema", Gi(t, " "), $i(n)], " ")
         },
         ScalarTypeExtension: function(e) {
-            return qi(["extend scalar", e.name, qi(e.directives, " ")], " ")
+            return Gi(["extend scalar", e.name, Gi(e.directives, " ")], " ")
         },
         ObjectTypeExtension: function(e) {
             var t = e.name,
                 n = e.interfaces,
                 i = e.directives,
                 a = e.fields;
-            return qi(["extend type", t, Ki("implements ", qi(n, " & ")), qi(i, " "), Mi(a)], " ")
+            return Gi(["extend type", t, _i("implements ", Gi(n, " & ")), Gi(i, " "), $i(a)], " ")
         },
         InterfaceTypeExtension: function(e) {
             var t = e.name,
                 n = e.interfaces,
                 i = e.directives,
                 a = e.fields;
-            return qi(["extend interface", t, Ki("implements ", qi(n, " & ")), qi(i, " "), Mi(a)], " ")
+            return Gi(["extend interface", t, _i("implements ", Gi(n, " & ")), Gi(i, " "), $i(a)], " ")
         },
         UnionTypeExtension: function(e) {
             var t = e.name,
                 n = e.directives,
                 i = e.types;
-            return qi(["extend union", t, qi(n, " "), i && 0 !== i.length ? "= " + qi(i, " | ") : ""], " ")
+            return Gi(["extend union", t, Gi(n, " "), i && 0 !== i.length ? "= " + Gi(i, " | ") : ""], " ")
         },
         EnumTypeExtension: function(e) {
             var t = e.name,
                 n = e.directives,
                 i = e.values;
-            return qi(["extend enum", t, qi(n, " "), Mi(i)], " ")
+            return Gi(["extend enum", t, Gi(n, " "), $i(i)], " ")
         },
         InputObjectTypeExtension: function(e) {
             var t = e.name,
                 n = e.directives,
                 i = e.fields;
-            return qi(["extend input", t, qi(n, " "), Mi(i)], " ")
+            return Gi(["extend input", t, Gi(n, " "), $i(i)], " ")
         }
     };
 
-    function ji(e) {
+    function Yi(e) {
         return function(t) {
-            return qi([t.description, e(t)], "\n")
+            return Gi([t.description, e(t)], "\n")
         }
     }
 
-    function qi(e) {
+    function Gi(e) {
         var t, n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
         return null !== (t = null == e ? void 0 : e.filter((function(e) {
             return e
         })).join(n)) && void 0 !== t ? t : ""
     }
 
-    function Mi(e) {
-        return Ki("{\n", Zi(qi(e, "\n")), "\n}")
+    function $i(e) {
+        return _i("{\n", ea(Gi(e, "\n")), "\n}")
     }
 
-    function Ki(e, t) {
+    function _i(e, t) {
         var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "";
         return null != t && "" !== t ? e + t + n : ""
     }
 
-    function Zi(e) {
-        return Ki("  ", e.replace(/\n/g, "\n  "))
+    function ea(e) {
+        return _i("  ", e.replace(/\n/g, "\n  "))
     }
 
-    function Yi(e) {
+    function ta(e) {
         return -1 !== e.indexOf("\n")
     }
 
-    function Gi(e) {
-        return null != e && e.some(Yi)
+    function na(e) {
+        return null != e && e.some(ta)
     }
-    var $i = Vi(Object.freeze({
+    var ia = Ui(Object.freeze({
             __proto__: null,
             [Symbol.toStringTag]: "Module",
             print: function(e) {
                 return function(e, t) {
-                    var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : Ni,
+                    var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : qi,
                         i = void 0,
                         a = Array.isArray(e),
                         r = [e],
                         l = -1,
                         o = [],
                         s = void 0,
                         c = void 0,
@@ -5881,25 +6014,25 @@
                             l = i.index, r = i.keys, o = i.edits, a = i.inArray, i = i.prev
                         } else {
                             if (c = u ? a ? l : r[l] : void 0, null == (s = u ? u[c] : f)) continue;
                             u && d.push(c)
                         }
                         var C, B = void 0;
                         if (!Array.isArray(s)) {
-                            if (!Hi(s)) throw new Error("Invalid AST Node: ".concat(zi(s), "."));
-                            var S = Wi(t, s.kind, h);
+                            if (!ji(s)) throw new Error("Invalid AST Node: ".concat(Qi(s), "."));
+                            var S = Ki(t, s.kind, h);
                             if (S) {
-                                if ((B = S.call(t, s, c, u, d, A)) === Qi) break;
+                                if ((B = S.call(t, s, c, u, d, A)) === Mi) break;
                                 if (!1 === B) {
                                     if (!h) {
                                         d.pop();
                                         continue
                                     }
                                 } else if (void 0 !== B && (o.push([c, B]), !h)) {
-                                    if (!Hi(B)) {
+                                    if (!ji(B)) {
                                         d.pop();
                                         continue
                                     }
                                     s = B
                                 }
                             }
                         }
@@ -5909,34 +6042,34 @@
                             keys: r,
                             edits: o,
                             prev: i
                         }, r = (a = Array.isArray(s)) ? s : null !== (C = n[s.kind]) && void 0 !== C ? C : [], l = -1, o = [], u && A.push(u), u = s)
                     } while (void 0 !== i);
                     return 0 !== o.length && (f = o[o.length - 1][1]), f
                 }(e, {
-                    leave: Ji
+                    leave: Zi
                 })
             }
         })),
-        _i = {},
-        ea = {},
-        ta = function(e) {
+        aa = {},
+        ra = {},
+        la = function(e) {
             var t = e.uri,
                 n = e.name,
                 i = e.type;
             this.uri = t, this.name = n, this.type = i
         },
-        na = ta,
-        ia = function(e) {
-            return "undefined" != typeof File && e instanceof File || "undefined" != typeof Blob && e instanceof Blob || e instanceof na
+        oa = la,
+        sa = function(e) {
+            return "undefined" != typeof File && e instanceof File || "undefined" != typeof Blob && e instanceof Blob || e instanceof oa
         },
-        aa = ia;
-    ea.ReactNativeFile = ta, ea.extractFiles = function e(t, n, i) {
+        ca = sa;
+    ra.ReactNativeFile = la, ra.extractFiles = function e(t, n, i) {
         var a;
-        void 0 === n && (n = ""), void 0 === i && (i = aa);
+        void 0 === n && (n = ""), void 0 === i && (i = ca);
         var r = new Map;
 
         function l(e, t) {
             var n = r.get(t);
             n ? n.push.apply(n, e) : r.set(t, e)
         }
         if (i(t)) a = null, l([n], t);
@@ -5955,118 +6088,118 @@
                     c.files.forEach(l), a[s] = c.clone
                 } else a = t
         }
         return {
             clone: a,
             files: r
         }
-    }, ea.isExtractableFile = ia;
-    var ra = "object" == typeof self ? self.FormData : window.FormData,
-        la = Ri && Ri.__importDefault || function(e) {
+    }, ra.isExtractableFile = sa;
+    var ua = "object" == typeof self ? self.FormData : window.FormData,
+        da = Ti && Ti.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
-    Object.defineProperty(_i, "__esModule", {
+    Object.defineProperty(aa, "__esModule", {
         value: !0
     });
-    var oa = ea,
-        sa = la(ra),
-        ca = function(e) {
-            return oa.isExtractableFile(e) || null !== e && "object" == typeof e && "function" == typeof e.pipe
+    var Aa = ra,
+        fa = da(ua),
+        ha = function(e) {
+            return Aa.isExtractableFile(e) || null !== e && "object" == typeof e && "function" == typeof e.pipe
         };
-    _i.default = function(e, t) {
-        var n = oa.extractFiles({
+    aa.default = function(e, t) {
+        var n = Aa.extractFiles({
                 query: e,
                 variables: t
-            }, "", ca),
+            }, "", ha),
             i = n.clone,
             a = n.files;
         if (0 === a.size) return JSON.stringify(i);
-        var r = new("undefined" == typeof FormData ? sa.default : FormData);
+        var r = new("undefined" == typeof FormData ? fa.default : FormData);
         r.append("operations", JSON.stringify(i));
         var l = {},
             o = 0;
         return a.forEach((function(e) {
             l[++o] = e
         })), r.append("map", JSON.stringify(l)), o = 0, a.forEach((function(e, t) {
             r.append("" + ++o, t)
         })), r
     };
-    var ua, da = {},
-        Aa = Ri && Ri.__extends || (ua = function(e, t) {
-            return (ua = Object.setPrototypeOf || {
+    var ma, pa = {},
+        ga = Ti && Ti.__extends || (ma = function(e, t) {
+            return (ma = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
                 })(e, t)
         }, function(e, t) {
             function n() {
                 this.constructor = e
             }
-            ua(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            ma(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         });
-    Object.defineProperty(da, "__esModule", {
+    Object.defineProperty(pa, "__esModule", {
         value: !0
-    }), da.ClientError = void 0;
-    var fa = function(e) {
+    }), pa.ClientError = void 0;
+    var va = function(e) {
         function t(n, i) {
             var a = this,
                 r = t.extractMessage(n) + ": " + JSON.stringify({
                     response: n,
                     request: i
                 });
             return a = e.call(this, r) || this, Object.setPrototypeOf(a, t.prototype), a.response = n, a.request = i, "function" == typeof Error.captureStackTrace && Error.captureStackTrace(a, t), a
         }
-        return Aa(t, e), t.extractMessage = function(e) {
+        return ga(t, e), t.extractMessage = function(e) {
             try {
                 return e.errors[0].message
             } catch (t) {
                 return "GraphQL Error (Code: " + e.status + ")"
             }
         }, t
     }(Error);
-    da.ClientError = fa,
+    pa.ClientError = va,
         function(e) {
-            var t = Ri && Ri.__assign || function() {
+            var t = Ti && Ti.__assign || function() {
                     return (t = Object.assign || function(e) {
                         for (var t, n = 1, i = arguments.length; n < i; n++)
                             for (var a in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, a) && (e[a] = t[a]);
                         return e
                     }).apply(this, arguments)
                 },
-                n = Ri && Ri.__createBinding || (Object.create ? function(e, t, n, i) {
+                n = Ti && Ti.__createBinding || (Object.create ? function(e, t, n, i) {
                     void 0 === i && (i = n), Object.defineProperty(e, i, {
                         enumerable: !0,
                         get: function() {
                             return t[n]
                         }
                     })
                 } : function(e, t, n, i) {
                     void 0 === i && (i = n), e[i] = t[n]
                 }),
-                i = Ri && Ri.__setModuleDefault || (Object.create ? function(e, t) {
+                i = Ti && Ti.__setModuleDefault || (Object.create ? function(e, t) {
                     Object.defineProperty(e, "default", {
                         enumerable: !0,
                         value: t
                     })
                 } : function(e, t) {
                     e.default = t
                 }),
-                a = Ri && Ri.__importStar || function(e) {
+                a = Ti && Ti.__importStar || function(e) {
                     if (e && e.__esModule) return e;
                     var t = {};
                     if (null != e)
                         for (var a in e) "default" !== a && Object.prototype.hasOwnProperty.call(e, a) && n(t, e, a);
                     return i(t, e), t
                 },
-                r = Ri && Ri.__awaiter || function(e, t, n, i) {
+                r = Ti && Ti.__awaiter || function(e, t, n, i) {
                     return new(n || (n = Promise))((function(a, r) {
                         function l(e) {
                             try {
                                 s(i.next(e))
                             } catch (t) {
                                 r(t)
                             }
@@ -6085,15 +6218,15 @@
                             e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(l, o)
                         }
                         s((i = i.apply(e, t || [])).next())
                     }))
                 },
-                l = Ri && Ri.__generator || function(e, t) {
+                l = Ti && Ti.__generator || function(e, t) {
                     var n, i, a, r, l = {
                         label: 0,
                         sent: function() {
                             if (1 & a[0]) throw a[1];
                             return a[1]
                         },
                         trys: [],
@@ -6160,37 +6293,37 @@
                                     value: r[0] ? r[1] : void 0,
                                     done: !0
                                 }
                             }([r, o])
                         }
                     }
                 },
-                o = Ri && Ri.__rest || function(e, t) {
+                o = Ti && Ti.__rest || function(e, t) {
                     var n = {};
                     for (var i in e) Object.prototype.hasOwnProperty.call(e, i) && t.indexOf(i) < 0 && (n[i] = e[i]);
                     if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                         var a = 0;
                         for (i = Object.getOwnPropertySymbols(e); a < i.length; a++) t.indexOf(i[a]) < 0 && Object.prototype.propertyIsEnumerable.call(e, i[a]) && (n[i[a]] = e[i[a]])
                     }
                     return n
                 },
-                s = Ri && Ri.__importDefault || function(e) {
+                s = Ti && Ti.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
             Object.defineProperty(e, "__esModule", {
                 value: !0
             }), e.gql = e.request = e.rawRequest = e.GraphQLClient = e.ClientError = void 0;
-            var c = a(Xi.exports),
+            var c = a(Di.exports),
                 u = c,
-                d = $i,
-                A = s(_i),
-                f = da,
-                h = da;
+                d = ia,
+                A = s(aa),
+                f = pa,
+                h = pa;
             Object.defineProperty(e, "ClientError", {
                 enumerable: !0,
                 get: function() {
                     return h.ClientError
                 }
             });
             var m = function(e) {
@@ -6300,44 +6433,44 @@
                 }))
             }, e.request = g, e.default = g, e.gql = function(e) {
                 for (var t = [], n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
                 return e.reduce((function(e, n, i) {
                     return "" + e + n + (i in t ? t[i] : "")
                 }), "")
             }
-        }(Oi);
+        }(zi);
 
-    function ha(e) {
+    function ya(e) {
         let t;
 
         function n(e, t) {
-            return e[2] ? va : ga
+            return e[2] ? wa : Ia
         }
         let i = n(e),
             a = i(e);
         return {
             c() {
-                a.c(), t = z()
+                a.c(), t = U()
             },
             l(e) {
-                a.l(e), t = z()
+                a.l(e), t = U()
             },
             m(e, n) {
                 a.m(e, n), k(e, t, n)
             },
             p(e, r) {
                 i !== (i = n(e)) && (a.d(1), a = i(e), a && (a.c(), a.m(t.parentNode, t)))
             },
             d(e) {
                 a.d(e), e && R(t)
             }
         }
     }
 
-    function ma(e) {
+    function Ea(e) {
         let n, i;
         return {
             c() {
                 n = O("p"), i = F("Saving..."), this.h()
             },
             l(e) {
                 n = j(e, "P", {
@@ -6355,15 +6488,15 @@
             p: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function pa(e) {
+    function ba(e) {
         let n, i;
         return {
             c() {
                 n = O("p"), i = F("Loading..."), this.h()
             },
             l(e) {
                 n = j(e, "P", {
@@ -6381,15 +6514,15 @@
             p: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function ga(e) {
+    function Ia(e) {
         let t, n;
         return {
             c() {
                 t = O("p"), n = F("Disconnected"), this.h()
             },
             l(e) {
                 t = j(e, "P", {
@@ -6406,15 +6539,15 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function va(e) {
+    function wa(e) {
         let t, n;
         return {
             c() {
                 t = O("p"), n = F("Connected"), this.h()
             },
             l(e) {
                 t = j(e, "P", {
@@ -6431,28 +6564,28 @@
             },
             d(e) {
                 e && R(t)
             }
         }
     }
 
-    function ya(e) {
+    function Ca(e) {
         let n;
 
         function i(e, t) {
-            return e[0] ? e[1] ? ma : null !== e[2] ? ha : void 0 : pa
+            return e[0] ? e[1] ? Ea : null !== e[2] ? ya : void 0 : ba
         }
         let a = i(e),
             r = a && a(e);
         return {
             c() {
-                r && r.c(), n = z()
+                r && r.c(), n = U()
             },
             l(e) {
-                r && r.l(e), n = z()
+                r && r.l(e), n = U()
             },
             m(e, t) {
                 r && r.m(e, t), k(e, n, t)
             },
             p(e, [t]) {
                 a === (a = i(e)) && r ? r.p(e, t) : (r && r.d(1), r = a && a(e), r && (r.c(), r.m(n.parentNode, n)))
             },
@@ -6460,36 +6593,36 @@
             o: t,
             d(e) {
                 r && r.d(e), e && R(n)
             }
         }
     }
 
-    function Ea(e, t, n) {
+    function Ba(e, t, n) {
         let {
             loaded: i
         } = t, {
             saving: a = !1
         } = t, {
             listening: r = null
         } = t;
         return e.$$set = e => {
             "loaded" in e && n(0, i = e.loaded), "saving" in e && n(1, a = e.saving), "listening" in e && n(2, r = e.listening)
         }, [i, a, r]
     }
-    class ba extends Ze {
+    class Sa extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Ea, ya, s, {
+            super(), Ze(this, e, Ba, Ca, s, {
                 loaded: 0,
                 saving: 1,
                 listening: 2
             })
         }
     }
-    var Ia = {
+    var La = {
         kind: "Document",
         definitions: [{
             kind: "OperationDefinition",
             operation: "query",
             name: {
                 kind: "Name",
                 value: "Balancing"
@@ -6704,75 +6837,75 @@
         }],
         loc: {
             start: 0,
             end: 312
         }
     };
 
-    function wa(e, t) {
+    function Pa(e, t) {
         if ("FragmentSpread" === e.kind) t.add(e.name.value);
         else if ("VariableDefinition" === e.kind) {
             var n = e.type;
             "NamedType" === n.kind && t.add(n.name.value)
         }
         e.selectionSet && e.selectionSet.selections.forEach((function(e) {
-            wa(e, t)
+            Pa(e, t)
         })), e.variableDefinitions && e.variableDefinitions.forEach((function(e) {
-            wa(e, t)
+            Pa(e, t)
         })), e.definitions && e.definitions.forEach((function(e) {
-            wa(e, t)
+            Pa(e, t)
         }))
     }
-    Ia.loc.source = {
+    La.loc.source = {
         body: "query Balancing($run: ID!) {\n  balancing(runId: $run) {\n    sessions {\n      id\n      name\n    }\n    players {\n      id\n      session\n      name\n      email\n      inactive\n      ready\n    }\n    teams {\n      id\n      session\n      name\n      ready\n      players\n    }\n    minimumPlayers\n    maximumPlayers\n  }\n}\n",
         name: "GraphQL request",
         locationOffset: {
             line: 1,
             column: 1
         }
     };
-    var Ca = {};
+    var xa = {};
 
-    function Ba(e, t) {
+    function ka(e, t) {
         for (var n = 0; n < e.definitions.length; n++) {
             var i = e.definitions[n];
             if (i.name && i.name.value == t) return i
         }
     }
-    Ia.definitions.forEach((function(e) {
+    La.definitions.forEach((function(e) {
             if (e.name) {
                 var t = new Set;
-                wa(e, t), Ca[e.name.value] = t
+                Pa(e, t), xa[e.name.value] = t
             }
         })),
         function(e, t) {
             var n = {
                 kind: e.kind,
-                definitions: [Ba(e, t)]
+                definitions: [ka(e, t)]
             };
             e.hasOwnProperty("loc") && (n.loc = e.loc);
-            var i = Ca[t] || new Set,
+            var i = xa[t] || new Set,
                 a = new Set,
                 r = new Set;
             for (i.forEach((function(e) {
                     r.add(e)
                 })); r.size > 0;) {
                 var l = r;
                 r = new Set, l.forEach((function(e) {
-                    a.has(e) || (a.add(e), (Ca[e] || new Set).forEach((function(e) {
+                    a.has(e) || (a.add(e), (xa[e] || new Set).forEach((function(e) {
                         r.add(e)
                     })))
                 }))
             }
             a.forEach((function(t) {
-                var i = Ba(e, t);
+                var i = ka(e, t);
                 i && n.definitions.push(i)
             }))
-        }(Ia, "Balancing");
-    var Sa = {
+        }(La, "Balancing");
+    var Ra = {
         kind: "Document",
         definitions: [{
             kind: "OperationDefinition",
             operation: "mutation",
             name: {
                 kind: "Name",
                 value: "AlterPlayer"
@@ -6904,75 +7037,75 @@
         }],
         loc: {
             start: 0,
             end: 169
         }
     };
 
-    function Pa(e, t) {
+    function Va(e, t) {
         if ("FragmentSpread" === e.kind) t.add(e.name.value);
         else if ("VariableDefinition" === e.kind) {
             var n = e.type;
             "NamedType" === n.kind && t.add(n.name.value)
         }
         e.selectionSet && e.selectionSet.selections.forEach((function(e) {
-            Pa(e, t)
+            Va(e, t)
         })), e.variableDefinitions && e.variableDefinitions.forEach((function(e) {
-            Pa(e, t)
+            Va(e, t)
         })), e.definitions && e.definitions.forEach((function(e) {
-            Pa(e, t)
+            Va(e, t)
         }))
     }
-    Sa.loc.source = {
+    Ra.loc.source = {
         body: "mutation AlterPlayer($playerId: ID!, $active: Boolean!) {\n  alterPlayer(playerId: $playerId, active: $active) {\n    id\n    session\n    name\n    email\n    inactive\n  }\n}\n",
         name: "GraphQL request",
         locationOffset: {
             line: 1,
             column: 1
         }
     };
-    var La = {};
+    var Oa = {};
 
-    function xa(e, t) {
+    function Xa(e, t) {
         for (var n = 0; n < e.definitions.length; n++) {
             var i = e.definitions[n];
             if (i.name && i.name.value == t) return i
         }
     }
-    Sa.definitions.forEach((function(e) {
+    Ra.definitions.forEach((function(e) {
             if (e.name) {
                 var t = new Set;
-                Pa(e, t), La[e.name.value] = t
+                Va(e, t), Oa[e.name.value] = t
             }
         })),
         function(e, t) {
             var n = {
                 kind: e.kind,
-                definitions: [xa(e, t)]
+                definitions: [Xa(e, t)]
             };
             e.hasOwnProperty("loc") && (n.loc = e.loc);
-            var i = La[t] || new Set,
+            var i = Oa[t] || new Set,
                 a = new Set,
                 r = new Set;
             for (i.forEach((function(e) {
                     r.add(e)
                 })); r.size > 0;) {
                 var l = r;
                 r = new Set, l.forEach((function(e) {
-                    a.has(e) || (a.add(e), (La[e] || new Set).forEach((function(e) {
+                    a.has(e) || (a.add(e), (Oa[e] || new Set).forEach((function(e) {
                         r.add(e)
                     })))
                 }))
             }
             a.forEach((function(t) {
-                var i = xa(e, t);
+                var i = Xa(e, t);
                 i && n.definitions.push(i)
             }))
-        }(Sa, "AlterPlayer");
-    var ka = {
+        }(Ra, "AlterPlayer");
+    var Fa = {
         kind: "Document",
         definitions: [{
             kind: "OperationDefinition",
             operation: "mutation",
             name: {
                 kind: "Name",
                 value: "UpdateBalancing"
@@ -7259,178 +7392,178 @@
         }],
         loc: {
             start: 0,
             end: 409
         }
     };
 
-    function Ra(e, t) {
+    function Ta(e, t) {
         if ("FragmentSpread" === e.kind) t.add(e.name.value);
         else if ("VariableDefinition" === e.kind) {
             var n = e.type;
             "NamedType" === n.kind && t.add(n.name.value)
         }
         e.selectionSet && e.selectionSet.selections.forEach((function(e) {
-            Ra(e, t)
+            Ta(e, t)
         })), e.variableDefinitions && e.variableDefinitions.forEach((function(e) {
-            Ra(e, t)
+            Ta(e, t)
         })), e.definitions && e.definitions.forEach((function(e) {
-            Ra(e, t)
+            Ta(e, t)
         }))
     }
-    ka.loc.source = {
+    Fa.loc.source = {
         body: "mutation UpdateBalancing($run: ID!, $teams: [TeamInput!], $deleteTeams: [ID!]) {\n  balanceTeams(runId: $run, teams: $teams, deleteTeams: $deleteTeams) {\n    sessions {\n      id\n      name\n    }\n    players {\n      id\n      session\n      name\n      email\n      inactive\n      ready\n    }\n    teams {\n      id\n      session\n      name\n      players\n      ready\n    }\n    minimumPlayers\n    maximumPlayers\n  }\n}\n",
         name: "GraphQL request",
         locationOffset: {
             line: 1,
             column: 1
         }
     };
-    var Va = {};
+    var Ua = {};
 
-    function Oa(e, t) {
+    function za(e, t) {
         for (var n = 0; n < e.definitions.length; n++) {
             var i = e.definitions[n];
             if (i.name && i.name.value == t) return i
         }
     }
 
-    function Xa(e) {
+    function Da(e) {
         let t, n;
-        return t = new ba({
+        return t = new Sa({
             props: {
                 loaded: e[1],
                 saving: e[0]
             }
         }), {
             c() {
-                We(t.$$.fragment)
+                Je(t.$$.fragment)
             },
             l(e) {
-                Je(t.$$.fragment, e)
+                je(t.$$.fragment, e)
             },
             m(e, i) {
-                je(t, e, i), n = !0
+                qe(t, e, i), n = !0
             },
             p(e, [n]) {
                 const i = {};
                 2 & n && (i.loaded = e[1]), 1 & n && (i.saving = e[0]), t.$set(i)
             },
             i(e) {
-                n || (Re(t.$$.fragment, e), n = !0)
+                n || (Ve(t.$$.fragment, e), n = !0)
             },
             o(e) {
-                Ve(t.$$.fragment, e), n = !1
+                Oe(t.$$.fragment, e), n = !1
             },
             d(e) {
-                qe(t, e)
+                Me(t, e)
             }
         }
     }
 
-    function Fa(e, t, n) {
+    function Ha(e, t, n) {
         let i, a;
-        d(e, $e, (e => n(4, i = e))), d(e, _e, (e => n(1, a = e)));
+        d(e, _e, (e => n(4, i = e))), d(e, et, (e => n(1, a = e)));
         let {
             endpoint: r = "/graphql/"
         } = t, {
             run: l
         } = t, o = !1;
-        const s = new Oi.GraphQLClient(r, {
+        const s = new zi.GraphQLClient(r, {
             credentials: "include"
         });
-        var c, u = {};
+        var c = {};
         return ce((() => {
-            g(_e, a = !1, a), s.request(Ia, {
+            g(et, a = !1, a), s.request(La, {
                 run: l
             }).then((e => {
-                (null == e ? void 0 : e.balancing) && (u = JSON.parse(JSON.stringify(e.balancing)), g($e, i = e.balancing, i)), g(_e, a = !0, a)
+                (null == e ? void 0 : e.balancing) && (c = JSON.parse(JSON.stringify(e.balancing)), g(_e, i = e.balancing, i)), g(et, a = !0, a)
             }))
-        })), c = et.subscribe((async e => {
+        })), ue(tt.subscribe((async e => {
             if (!e) return;
-            let t = await s.request(Sa, e);
-            (null == t ? void 0 : t.alterPlayer) && g($e, i.players = i.players.map((e => e.id == t.alterPlayer.id ? Object.assign(e, t.alterPlayer) : e)), i)
-        })), se().$$.on_destroy.push(c), e.$$set = e => {
+            let t = await s.request(Ra, e);
+            (null == t ? void 0 : t.alterPlayer) && g(_e, i.players = i.players.map((e => e.id == t.alterPlayer.id ? Object.assign(e, t.alterPlayer) : e)), i)
+        }))), e.$$set = e => {
             "endpoint" in e && n(2, r = e.endpoint), "run" in e && n(3, l = e.run)
         }, e.$$.update = () => {
             19 & e.$$.dirty && a && i && !o && (console.debug("checking for changes"), function() {
-                if (!u.teams) return;
+                if (!c.teams) return;
                 const e = i.teams.map((e => e.id)),
                     t = {
                         run: l,
-                        deleteTeams: u.teams.map((e => e.id)).filter((t => t && !e.includes(t))),
+                        deleteTeams: c.teams.map((e => e.id)).filter((t => t && !e.includes(t))),
                         teams: i.teams.filter((e => {
-                            const t = u.teams.find((t => t.id === e.id));
+                            const t = c.teams.find((t => t.id === e.id));
                             return !t || t.name !== e.name || t.players.length !== e.players.length || !t.players.every((t => e.players.includes(t)))
                         })).map((e => __spreadProps(__spreadValues({}, e), {
                             ready: void 0,
                             internalId: void 0
                         })))
                     };
-                (t.deleteTeams.length || t.teams.length) && (console.debug("updating data"), n(0, o = !0), u = JSON.parse(JSON.stringify(i)), s.request(ka, t).then((e => {
+                (t.deleteTeams.length || t.teams.length) && (console.debug("updating data"), n(0, o = !0), c = JSON.parse(JSON.stringify(i)), s.request(Fa, t).then((e => {
                     if (null == e ? void 0 : e.balanceTeams) {
                         const t = i.teams.filter((e => e.internalId));
-                        g($e, i = __spreadProps(__spreadValues({}, e.balanceTeams), {
+                        g(_e, i = __spreadProps(__spreadValues({}, e.balanceTeams), {
                             teams: e.balanceTeams.teams.map((e => {
                                 var n = t.find((t => t.id === e.id)) || t.find((t => t.name === e.name));
                                 return n ? __spreadProps(__spreadValues({}, e), {
                                     internalId: n.internalId
                                 }) : e
                             }))
-                        }), i), u = JSON.parse(JSON.stringify(i))
+                        }), i), c = JSON.parse(JSON.stringify(i))
                     }
                     n(0, o = !1)
                 })))
             }())
         }, [o, a, r, l, i]
     }
-    ka.definitions.forEach((function(e) {
+    Fa.definitions.forEach((function(e) {
             if (e.name) {
                 var t = new Set;
-                Ra(e, t), Va[e.name.value] = t
+                Ta(e, t), Ua[e.name.value] = t
             }
         })),
         function(e, t) {
             var n = {
                 kind: e.kind,
-                definitions: [Oa(e, t)]
+                definitions: [za(e, t)]
             };
             e.hasOwnProperty("loc") && (n.loc = e.loc);
-            var i = Va[t] || new Set,
+            var i = Ua[t] || new Set,
                 a = new Set,
                 r = new Set;
             for (i.forEach((function(e) {
                     r.add(e)
                 })); r.size > 0;) {
                 var l = r;
                 r = new Set, l.forEach((function(e) {
-                    a.has(e) || (a.add(e), (Va[e] || new Set).forEach((function(e) {
+                    a.has(e) || (a.add(e), (Ua[e] || new Set).forEach((function(e) {
                         r.add(e)
                     })))
                 }))
             }
             a.forEach((function(t) {
-                var i = Oa(e, t);
+                var i = za(e, t);
                 i && n.definitions.push(i)
             }))
-        }(ka, "UpdateBalancing");
-    class Ua extends Ze {
+        }(Fa, "UpdateBalancing");
+    class Na extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Fa, Xa, s, {
+            super(), Ze(this, e, Ha, Da, s, {
                 endpoint: 2,
                 run: 3
             })
         }
     }
 
-    function za(e) {
+    function Qa(e) {
         let t;
 
         function n(e, t) {
-            return 1 == e[3] ? Da : Ta
+            return 1 == e[3] ? Ja : Wa
         }
         let i = n(e),
             a = i(e);
         return {
             c() {
                 t = O("span"), a.c(), this.h()
             },
@@ -7452,15 +7585,15 @@
             },
             d(e) {
                 e && R(t), a.d()
             }
         }
     }
 
-    function Ta(e) {
+    function Wa(e) {
         let t, n;
         return {
             c() {
                 t = F(e[3]), n = F(" players need balancing")
             },
             l(i) {
                 t = q(i, e[3]), n = q(i, " players need balancing")
@@ -7473,15 +7606,15 @@
             },
             d(e) {
                 e && R(t), e && R(n)
             }
         }
     }
 
-    function Da(e) {
+    function Ja(e) {
         let t, n;
         return {
             c() {
                 t = F(e[3]), n = F(" player needs balancing")
             },
             l(i) {
                 t = q(i, e[3]), n = q(i, " player needs balancing")
@@ -7494,19 +7627,19 @@
             },
             d(e) {
                 e && R(t), e && R(n)
             }
         }
     }
 
-    function Ha(e) {
-        let n, i, a, r, l, o = e[3] && za(e);
+    function ja(e) {
+        let n, i, a, r, l, o = e[3] && Qa(e);
         return {
             c() {
-                n = O("li"), i = O("a"), a = O("span"), r = F("Manage Teams"), l = U(), o && o.c(), this.h()
+                n = O("li"), i = O("a"), a = O("span"), r = F("Manage Teams"), l = T(), o && o.c(), this.h()
             },
             l(e) {
                 n = j(e, "LI", {
                     class: !0
                 });
                 var t = W(n);
                 i = j(t, "A", {
@@ -7523,51 +7656,51 @@
             h() {
                 N(a, "class", "todo-link-title"), N(i, "class", "todo-link"), N(i, "href", e[1]), G(i, "is-active", e[0]), G(i, "is-alert", e[3]), G(i, "is-complete", !e[3] && e[2].length), N(n, "class", "todo-item")
             },
             m(e, t) {
                 k(e, n, t), x(n, i), x(i, a), x(a, r), x(i, l), o && o.m(i, null)
             },
             p(e, [t]) {
-                e[3] ? o ? o.p(e, t) : (o = za(e), o.c(), o.m(i, null)) : o && (o.d(1), o = null), 2 & t && N(i, "href", e[1]), 1 & t && G(i, "is-active", e[0]), 8 & t && G(i, "is-alert", e[3]), 12 & t && G(i, "is-complete", !e[3] && e[2].length)
+                e[3] ? o ? o.p(e, t) : (o = Qa(e), o.c(), o.m(i, null)) : o && (o.d(1), o = null), 2 & t && N(i, "href", e[1]), 1 & t && G(i, "is-active", e[0]), 8 & t && G(i, "is-alert", e[3]), 12 & t && G(i, "is-complete", !e[3] && e[2].length)
             },
             i: t,
             o: t,
             d(e) {
                 e && R(n), o && o.d()
             }
         }
     }
 
-    function Na(e, t, n) {
+    function qa(e, t, n) {
         let i;
-        d(e, $e, (e => n(4, i = e)));
+        d(e, _e, (e => n(4, i = e)));
         let a, {
                 active: r = !1
             } = t,
             {
                 href: l
             } = t,
             o = [];
         return e.$$set = e => {
             "active" in e && n(0, r = e.active), "href" in e && n(1, l = e.href)
         }, e.$$.update = () => {
             var t;
             20 & e.$$.dirty && (n(2, o = i.teams.flatMap((e => e.players))), n(3, a = null == (t = i.players) ? void 0 : t.filter((e => !o.includes(e.id) && !e.inactive)).length))
         }, [r, l, o, a, i]
     }
-    class Qa extends Ze {
+    class Ma extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Na, Ha, s, {
+            super(), Ze(this, e, qa, ja, s, {
                 active: 0,
                 href: 1
             })
         }
     }
 
-    function Wa(e) {
+    function Ka(e) {
         let n, i, a, r;
         return {
             c() {
                 n = O("li"), i = O("a"), a = O("span"), r = F("Start Game"), this.h()
             },
             l(e) {
                 n = j(e, "LI", {
@@ -7598,36 +7731,36 @@
             o: t,
             d(e) {
                 e && R(n)
             }
         }
     }
 
-    function Ja(e, t, n) {
+    function Za(e, t, n) {
         let i;
-        d(e, $e, (e => n(3, i = e)));
+        d(e, _e, (e => n(3, i = e)));
         let a, {
                 href: r = null
             } = t,
             l = [];
         return e.$$set = e => {
             "href" in e && n(0, r = e.href)
         }, e.$$.update = () => {
             var t;
             10 & e.$$.dirty && (n(1, l = i.teams.flatMap((e => e.players))), n(2, a = null == (t = i.players) ? void 0 : t.filter((e => !l.includes(e.id))).length))
         }, [r, l, a, i]
     }
-    class ja extends Ze {
+    class Ya extends Ye {
         constructor(e) {
-            super(), Ke(this, e, Ja, Wa, s, {
+            super(), Ze(this, e, Za, Ka, s, {
                 href: 0
             })
         }
     }
-    class qa {
+    class Ga {
         constructor() {
             this.buttonAttr = "data-toggle-elements", document.querySelectorAll(`[${this.buttonAttr}]`).forEach(this.initComponent, this)
         }
         toggleEl(e) {
             document.querySelectorAll(e).forEach((e => {
                 e.classList.contains("hide") ? e.classList.remove("hide") : e.classList.add("hide")
             }))
@@ -7635,15 +7768,15 @@
         initComponent(e) {
             const t = e.getAttribute(this.buttonAttr);
             e.addEventListener("click", (e => {
                 e.preventDefault(), this.toggleEl(t)
             }))
         }
     }
-    class Ma {
+    class $a {
         constructor() {
             this.collapsibleAttr = "data-is-accordion", this.toggleButtonAttr = "data-toggle-collapsible", this.expandAllAttr = "data-expand-all", this.collapseAllAttr = "data-collapse-all", this.allCollapsibles = document.querySelectorAll(`[${this.collapsibleAttr}]`), this.toggleButtons = document.querySelectorAll(`[${this.toggleButtonAttr}]`), this.expandAllButtons = document.querySelectorAll(`[${this.expandAllAttr}]`), this.collapseAllButtons = document.querySelectorAll(`[${this.collapseAllAttr}]`), this.toggleButtons.forEach((e => e.addEventListener("click", (t => this.toggleCollapsible(e))))), this.expandAllButtons.forEach((e => e.addEventListener("click", (e => this.expandAll())))), this.collapseAllButtons.forEach((e => e.addEventListener("click", (e => this.collapseAll()))))
         }
         hide(e) {
             e.classList.add("hide")
         }
         show(e) {
@@ -7665,74 +7798,74 @@
         expandAll() {
             this.expandAllButtons.forEach((e => this.hide(e))), this.collapseAllButtons.forEach((e => this.show(e))), this.allCollapsibles.forEach((e => this.show(e))), this.toggleButtons.forEach((e => this.setExpanded(e)))
         }
         collapseAll() {
             this.collapseAllButtons.forEach((e => this.hide(e))), this.expandAllButtons.forEach((e => this.show(e))), this.allCollapsibles.forEach((e => this.hide(e))), this.toggleButtons.forEach((e => this.removeExpanded(e)))
         }
     }
-    class Ka {
+    class _a {
         constructor() {
             this.selector = "[data-toast]", document.querySelectorAll(this.selector).forEach(this.initComponent, this)
         }
         initComponent(e) {
             const t = parseInt(e.getAttribute("data-timeout")) || 5e3;
             setTimeout((() => {
                 e.classList.contains("collapse") ? e.classList.remove("in") : e.classList.add("hide")
             }), t)
         }
     }
-    class Za {
+    class er {
         constructor() {
             this.selector = ".field-pair", document.querySelectorAll(this.selector).forEach(this.initComponent, this)
         }
         toggleCheckboxes(e) {
             this.checkbox = e.querySelector("[type=checkbox]"), this.willDisable = e.querySelector("[data-disabled-when-unchecked]"), this.willDisableFields = this.willDisable.querySelectorAll("input");
             let t = !!e.querySelector("[data-disable-fields]:checked");
             t ? this.willDisableFields.forEach((e => e.removeAttribute("disabled"))) : this.willDisableFields.forEach((e => e.setAttribute("disabled", "disabled"))), this.willDisable.classList.toggle("is-disabled", !t), e.classList.toggle("has-checked", t)
         }
         initComponent(e) {
             this.toggleCheckboxes(e), this.checkbox.addEventListener("change", (() => {
                 this.toggleCheckboxes(e)
             }))
         }
     }
-    e.ToggleElement = qa, e.initBalancing = function(e) {
-        e || (e = document.getElementById("app")), new ki({
+    e.ToggleElement = Ga, e.initBalancing = function(e) {
+        e || (e = document.getElementById("app")), new Fi({
             target: e,
             props: e.dataset
         });
         const t = document.getElementById("loader");
-        t && new Ua({
+        t && new Na({
             target: t,
             props: t.dataset
-        }), $e.subscribe((e => {
+        }), _e.subscribe((e => {
             if (!e.players) return;
             const t = document.getElementById("simpl-team-nav");
             if (t) {
                 const e = t.getElementsByTagName("A")[0];
-                new Qa({
+                new Ma({
                     target: t,
                     hydrate: !0,
                     props: {
                         href: e.href,
                         active: e.classList.contains("is-active")
                     }
                 })
             }
             const n = document.getElementById("simpl-start-nav");
             if (n) {
                 const e = n.getElementsByTagName("A")[0].href;
-                new ja({
+                new Ya({
                     target: n,
                     hydrate: !0,
                     props: {
                         href: e
                     }
                 })
             }
         }))
     }, e.initComponents = function() {
-        new qa, new Ka, new Za, new Ma
+        new Ga, new _a, new er, new $a
     }, Object.defineProperty(e, "__esModule", {
         value: !0
     }), e[Symbol.toStringTag] = "Module"
 }));
```

### Comparing `simpl-cloud-1.2.4/simpl/static/simpl/style.css` & `simpl-cloud-1.3.0/simpl/static/simpl/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
     90deg,
     #dd0847 18.26%,
     #2b66b2 81.94%
   );--brand-gradient-2:linear-gradient(
     90deg,
     #042441 18.26%,
     #2b66b2 81.94%
-  );--global-font-family:"Lato",sans-serif;--global-weight-semibold:700;--global-weight-normal:400;--font-size-base:1rem;--font-size-small:0.875rem;--code-font-family:Menlo,"Ubuntu Mono","Lucida Console","Courier New",Courier,monospace;--body-bg-color:#ecf0f3;--body-bg-shade:#e0e6ea;--body-bg-shade2:#c9d1d8;--body-bg-shade-half:#e7ecef;--body-bg-tint:#f6f8f9;--body-bg-image:url(/static/dots.svg),linear-gradient(to bottom, #fff 10%, #ecf0f3 100%);--body-bg-image-size:auto,100% 500px;--body-bg-image-attachment:fixed,fixed;--body-bg-image-repeat:repeat-x,no-repeat;--header-bg:transparent;--header-border-bottom:0 none;--sidebar-background:var(--card-bg);--sidebar-link-hover-bg:var(--body-bg-shade-half);--site-header-grid-cols-xl:13.5rem 1fr auto;--stat-card-bg:var(--caution-color-tint5);--stat-card-bg-alt1:var(--success-color-tint5);--stat-card-bg-alt2:var(--info-color-tint5);--stat-card-color:var(--link-color);--stat-card-radius:var(--global-radius);--site-nav-background:var(--tint);--site-nav-background-alt:var(--site-nav-background);--site-nav-link-color:var(--text-color);--site-nav-link-color-hover:var(--alert-color);--site-nav-link-hover-bg-color:transparent;--site-nav-text-transform:none;--site-nav-letter-spacing:0;--site-nav-font-size:0.875rem;--site-nav-font-size-xl:var(--site-nav-font-size);--site-nav-font-size-xxl:var(--site-nav-font-size);--site-nav-font-weight:var(--global-weight-semibold);--site-nav-logo-color:var(--site-nav-link-color);--site-nav-link-current-bg:var(--brand-color-tint5);--site-nav-link-current-color:var(--site-nav-link-color-hover);--site-nav-height:4rem;--site-nav-height-open:6.25rem;--site-subheader-height:2.5625rem;--site-nav-mobile-nav-background:var(--brand-color-tint1);--site-nav-mobile-nav-thin-height:1.875rem;--site-nav-border-bottom:1px solid var(--card-border-color-default);--site-nav-button-border:1px solid var(--card-border-color-default);--subnav-background:var(--brand-color-tint5);--v-nav-bg:#F5F5F6;--v-nav-color:var(--text-color);--v-nav-active-color:var(--v-nav-color);--v-nav-active-bg:#fff;--v-nav-active-bg-alt:var(--v-nav-active-bg);--well-bg:var(--body-bg-shade);--well-bg-shade:var(--body-bg-shade2);--action-list-border-color:var(--body-bg-shade-half);--action-list-link-hover-bg:var(--success-color-tint4);--todo-aside:#fff;--link-color:var(--brand-color);--primary-heading-color:var(--text-color);--heading-color:var(--primary-heading-color);--link-color-tint:#b4bdc6;--knockout-color:#fff;--unread-color:var(--alert-color);--unread-tint1:var(--alert-color-tint5);--unread-tint2:var(--alert-color-tint4);--unread-bg-color:var(--card-bg);--selected-color:var(--brand-color);--selected-bg-color:var(--info-color-tint5);--leader-color:var(--brand-color);--unread-border-top-height:5px;--unread-top-border-bg:var(--brand-gradient);--card-bg:var(--knockout-color);--card-bg-shade:var(--body-bg-shade-half);--card-bg-shade2:var(--body-bg-shade-half);--card-bg-unread:var(--card-bg);--card-border-color-default:var(--body-bg-shade-half);--card-shadow-default:var(--base-shadow);--card-radius:var(--global-radius);--card-unread-border-top:4px solid var(--unread-color);--card-border-width:0;--feature-card-heading-weight:var(--global-weight-normal);--feature-card-heading-size:1.5rem;--feature-card-heading-margin:0 0 1rem 0;--modal-bg:var(--card-bg);--modal-header-bg:var(--brand-color-tint5);--modal-shade-bg:var(--body-bg-color);--dropdown-bg:var(--knockout-color);--dropdown-border-color:var(--card-border-color-default);--dropdown-hover-color:var(--card-bg-shade);--dropdown-hover-bg:var(--success-color-tint4);--compose-footer-color:#ecf0f3;--sidebar-link-hover-bg:var(--success-color-tint4);--carousel-arrow-bg-color-hover:var(--body-bg-shade-half);--button-transition:background-image 0.25s ease-out,box-shadow 0.25s ease-out,border-color 0.25s ease-out,color 0.25s ease-out,background-color 0.25s ease-out,background-position 0.25s ease-out,transform 0.25s ease-out}:root{--field-border-color:#ddd;--mobile-sub-nav-expanded-bg:#fff}:root{--brand-color:#2b66b2;--brand-color-tint1:#5585c1;--brand-color-tint2:#80a3d1;--brand-color-tint3:#aac2e0;--brand-color-tint4:#d5e0f0;--brand-color-tint5:#eaf0f7;--brand-color-tint:#5585c1;--brand-color-alpha:rgba(43, 102, 178, 0.2);--brand-color-alpha-shade:rgba(27, 76, 133, 0.4);--brand-color-shade:#1e477d;--brand-color-spin:#2b5bb2;--info-color:#2b66b2;--info-color-tint1:#5585c1;--info-color-tint2:#80a3d1;--info-color-tint3:#aac2e0;--info-color-tint4:#d5e0f0;--info-color-tint5:#eaf0f7;--info-color-tint6:#f4f7fb;--info-color-tint7:#f9fafd;--info-color-tint8:#fbfcfd;--info-color-tint:#aac2e0;--info-color-alpha:rgba(43, 102, 178, 0.2);--info-color-alpha-40:rgba(43, 102, 178, 0.4);--info-color-shade:#23599b;--info-color-alpha-shade:rgba(27, 76, 133, 0.4);--info-color-spin:#2b5bb2;--success-color:#00D86B;--success-color-tint1:#33e089;--success-color-tint2:#66e8a6;--success-color-tint3:#99efc4;--success-color-tint4:#ccf7e1;--success-color-tint5:#e6fbf0;--success-color-tint:#99efc4;--success-color-alpha:rgba(0, 216, 107, 0.2);--success-color-alpha-shade:rgba(2, 144, 90, 0.4);--success-color-shade:#02905a;--success-color-spin:#00d87d;--caution-color:#FFBE15;--caution-color-tint1:#ffcb44;--caution-color-tint2:#ffd873;--caution-color-tint3:#ffe5a1;--caution-color-tint4:#fff2d0;--caution-color-tint5:#fff9e8;--caution-color-tint:#ffe5a1;--caution-color-alpha:rgba(255, 190, 21, 0.2);--caution-color-alpha-shade:rgba(155, 128, 39, 0.4);--caution-color-shade:#cd9f1e;--caution-color-spin:#ffd215;--alert-color:#dd0847;--alert-color-tint1:#e4396c;--alert-color-tint2:#eb6b91;--alert-color-tint3:#f19cb5;--alert-color-tint4:#f8ceda;--alert-color-tint5:#fce6ed;--alert-color-tint:#f8ceda;--alert-color-alpha:rgba(221, 8, 71, 0.2);--alert-color-alpha-shade:rgba(134, 19, 69, 0.4);--alert-color-shade:#861345;--alert-color-spin:#dd0835;--text-color:#2e373f;--text-color-alpha:rgba(46, 55, 63, 0.9);--text-color-subdued:rgba(46, 55, 63, 0.7);--tint:#fff;--normal:#2b66b2;--normal-tint1:#5585c1;--normal-tint2:#80a3d1;--normal-tint3:#aac2e0;--normal-tint4:#d5e0f0;--normal-tint5:#eaf0f7;--normal-tint:#aac2e0;--normal-alpha:rgba(43, 102, 178, 0.2);--normal-alpha-shade:rgba(27, 76, 133, 0.4);--normal-shade:#23599b;--important:#FFBE15;--important-tint1:#ffcb44;--important-tint2:#ffd873;--important-tint3:#ffe5a1;--important-tint4:#fff2d0;--important-tint5:#fff9e8;--important-tint:#ffe5a1;--important-alpha:rgba(255, 190, 21, 0.2);--important-alpha-shade:rgba(155, 128, 39, 0.4);--important-shade:#cd9f1e;--critical:#dd0847;--critical-tint1:#e4396c;--critical-tint2:#eb6b91;--critical-tint3:#f19cb5;--critical-tint4:#f8ceda;--critical-tint5:#fce6ed;--critical-tint:#f8ceda;--critical-alpha:rgba(221, 8, 71, 0.2);--critical-alpha-shade:rgba(134, 19, 69, 0.4);--critical-shade:#861345}.theme-brand-color{--theme-color:var(--brand-color);--theme-debug-brand-color:43.3333333333%;--theme-text-color:var(--theme-brand-color-text-color, var(--tint));--theme-color-tint1:var(--brand-color-tint1);--theme-color-tint2:var(--brand-color-tint2);--theme-color-tint3:var(--brand-color-tint3);--theme-color-tint4:var(--brand-color-tint4);--theme-color-tint5:var(--brand-color-tint5);--theme-color-tint:var(--brand-color-tint);--theme-color-alpha:var(--brand-color-alpha);--theme-color-alpha-shade:var(--brand-color-alpha-shade);--theme-color-shade:var(--brand-color-shade);--theme-color-spin:var(--brand-color-spin)}.theme-info-color{--theme-color:var(--info-color);--theme-debug-info-color:43.3333333333%;--theme-text-color:var(--theme-info-color-text-color, var(--tint));--theme-color-tint1:var(--info-color-tint1);--theme-color-tint2:var(--info-color-tint2);--theme-color-tint3:var(--info-color-tint3);--theme-color-tint4:var(--info-color-tint4);--theme-color-tint5:var(--info-color-tint5);--theme-color-tint6:var(--info-color-tint6);--theme-color-tint7:var(--info-color-tint7);--theme-color-tint8:var(--info-color-tint8);--theme-color-tint:var(--info-color-tint);--theme-color-alpha:var(--info-color-alpha);--theme-color-alpha-40:var(--info-color-alpha-40);--theme-color-shade:var(--info-color-shade);--theme-color-alpha-shade:var(--info-color-alpha-shade);--theme-color-spin:var(--info-color-spin)}.theme-success-color{--theme-color:var(--success-color);--theme-debug-success-color:42.3529411765%;--theme-text-color:var(--theme-success-color-text-color, var(--text-color));--theme-color-tint1:var(--success-color-tint1);--theme-color-tint2:var(--success-color-tint2);--theme-color-tint3:var(--success-color-tint3);--theme-color-tint4:var(--success-color-tint4);--theme-color-tint5:var(--success-color-tint5);--theme-color-tint:var(--success-color-tint);--theme-color-alpha:var(--success-color-alpha);--theme-color-alpha-shade:var(--success-color-alpha-shade);--theme-color-shade:var(--success-color-shade);--theme-color-spin:var(--success-color-spin)}.theme-caution-color{--theme-color:var(--caution-color);--theme-debug-caution-color:54.1176470588%;--theme-text-color:var(--theme-caution-color-text-color, var(--text-color));--theme-color-tint1:var(--caution-color-tint1);--theme-color-tint2:var(--caution-color-tint2);--theme-color-tint3:var(--caution-color-tint3);--theme-color-tint4:var(--caution-color-tint4);--theme-color-tint5:var(--caution-color-tint5);--theme-color-tint:var(--caution-color-tint);--theme-color-alpha:var(--caution-color-alpha);--theme-color-alpha-shade:var(--caution-color-alpha-shade);--theme-color-shade:var(--caution-color-shade);--theme-color-spin:var(--caution-color-spin)}.theme-alert-color{--theme-color:var(--alert-color);--theme-debug-alert-color:44.9019607843%;--theme-text-color:var(--theme-alert-color-text-color, var(--tint));--theme-color-tint1:var(--alert-color-tint1);--theme-color-tint2:var(--alert-color-tint2);--theme-color-tint3:var(--alert-color-tint3);--theme-color-tint4:var(--alert-color-tint4);--theme-color-tint5:var(--alert-color-tint5);--theme-color-tint:var(--alert-color-tint);--theme-color-alpha:var(--alert-color-alpha);--theme-color-alpha-shade:var(--alert-color-alpha-shade);--theme-color-shade:var(--alert-color-shade);--theme-color-spin:var(--alert-color-spin)}.theme-text-color{--theme-color:var(--text-color);--theme-debug-text-color:21.3725490196%;--theme-text-color:var(--theme-text-color-text-color, var(--tint));--theme-color-alpha:var(--text-color-alpha);--theme-color-subdued:var(--text-color-subdued)}.theme-tint{--theme-color:var(--tint);--theme-debug-tint:100%;--theme-text-color:var(--theme-tint-text-color, var(--text-color))}.theme-normal{--theme-color:var(--normal);--theme-debug-normal:43.3333333333%;--theme-text-color:var(--theme-normal-text-color, var(--tint));--theme-color-tint1:var(--normal-tint1);--theme-color-tint2:var(--normal-tint2);--theme-color-tint3:var(--normal-tint3);--theme-color-tint4:var(--normal-tint4);--theme-color-tint5:var(--normal-tint5);--theme-color-tint:var(--normal-tint);--theme-color-alpha:var(--normal-alpha);--theme-color-alpha-shade:var(--normal-alpha-shade);--theme-color-shade:var(--normal-shade)}.theme-important{--theme-color:var(--important);--theme-debug-important:54.1176470588%;--theme-text-color:var(--theme-important-text-color, var(--text-color));--theme-color-tint1:var(--important-tint1);--theme-color-tint2:var(--important-tint2);--theme-color-tint3:var(--important-tint3);--theme-color-tint4:var(--important-tint4);--theme-color-tint5:var(--important-tint5);--theme-color-tint:var(--important-tint);--theme-color-alpha:var(--important-alpha);--theme-color-alpha-shade:var(--important-alpha-shade);--theme-color-shade:var(--important-shade)}.theme-critical{--theme-color:var(--critical);--theme-debug-critical:44.9019607843%;--theme-text-color:var(--theme-critical-text-color, var(--tint));--theme-color-tint1:var(--critical-tint1);--theme-color-tint2:var(--critical-tint2);--theme-color-tint3:var(--critical-tint3);--theme-color-tint4:var(--critical-tint4);--theme-color-tint5:var(--critical-tint5);--theme-color-tint:var(--critical-tint);--theme-color-alpha:var(--critical-alpha);--theme-color-alpha-shade:var(--critical-alpha-shade);--theme-color-shade:var(--critical-shade)}html *{box-sizing:border-box}img{max-width:100%}.icon{pointer-events:none}.icon use{pointer-events:none}.bottomless>:last-child{margin-bottom:0}.ellipsis{text-overflow:ellipsis;white-space:nowrap;overflow:hidden}.ellipsis-two-lines{display:-webkit-box;overflow:hidden;-webkit-line-clamp:2;-webkit-box-orient:vertical}.ellipsis-three-lines{display:-webkit-box;overflow:hidden;-webkit-line-clamp:3;-webkit-box-orient:vertical}.read-more{display:flex}.read-more.is-expanded{display:block}.read-more.is-expanded .clamp-button{display:block;margin-top:.5rem}.read-more:not(.is-expanded) .clamp-text{flex:1 1 100%;display:-webkit-box;overflow:hidden;-webkit-line-clamp:1;-webkit-box-orient:vertical}.read-more:not(.is-expanded) .clamp-button{flex:0 0 auto}.nowrap{white-space:nowrap}.normal-weight{font-weight:var(--global-weight-normal)}.show-on-toggle{display:none}.is-toggled .hide-on-toggle{display:none}.is-toggled .show-on-toggle{display:block}[data-toggle-this].is-expanded{display:block}.v-pad{padding-top:calc(var(--global-margin)/ 2);padding-bottom:calc(var(--global-margin)/ 2)}.mb,.mb-1{margin-bottom:var(--global-margin)!important}.mt{display:block;margin-top:var(--global-margin)!important}.mt-0{margin-top:0!important}.mb-0{margin-bottom:0!important}.m-0{margin:0!important}.mt-2{margin-top:calc(var(--global-margin) * 2)!important}.mb-2{margin-bottom:calc(var(--global-margin) * 2)!important}.pad-right{padding-right:var(--global-margin)}.zero-text-margins h1,.zero-text-margins h2,.zero-text-margins h3,.zero-text-margins h4,.zero-text-margins h5,.zero-text-margins h6,.zero-text-margins li,.zero-text-margins ol,.zero-text-margins p,.zero-text-margins ul{margin:0}.float-right{float:right;margin:0 0 .625rem .625rem}.default-case{text-transform:none}.text-right{text-align:right}.text-center{text-align:center}.knockout,.knockout a,.knockout h1,.knockout h2,.knockout h3,.knockout h4,.knockout h5,.knockout h6,.knockout li,.knockout p,.knockout table{color:var(--knockout-color)}.show-for-sr-only{position:absolute;left:-1000px;padding:0;width:1px;height:1px;border:0;overflow:hidden;clip:rect(0 0 0 0)}.is-disabled{opacity:.4;pointer-events:none}.reverse-links a,a.reverse-link{text-decoration:none}.reverse-links a:hover,a.reverse-link:hover{text-decoration:underline}.fullscreen-only{display:none!important}:-webkit-full-screen .fullscreen-only{display:flex!important}:-ms-fullscreen .fullscreen-only{display:flex!important}:fullscreen .fullscreen-only{display:flex!important}@media (min-width:980px){.mobile-only{display:none!important}}@media (max-width:979px){.hide-on-mobile{display:none!important}}@media (max-width:569px){.show-on-smedium{display:none}}.hide{display:none!important}.expand-this-link:after{position:absolute;top:0;right:0;bottom:0;left:0;z-index:1;content:""}.expand-this-link:focus{box-shadow:none}.expand-this-link:focus:after{box-shadow:var(--focus-shadow)}.is-open .expand-this-link:not(.attachment-title):after{content:none}.show-on-focus{position:absolute!important;width:1px;height:1px;white-space:nowrap;overflow:hidden}.show-on-focus:focus{position:relative!important;top:calc(var(--site-nav-height) * -1 - -18px);left:16px;z-index:6;padding:10px;width:auto;height:auto;background-color:var(--card-bg)}.max-760{max-width:760px}[data-truncate] [data-expand-this]{display:none}[data-truncate] [data-expand-label]{cursor:pointer}[data-truncate].is-expanded [data-expand-this]{display:inline}[data-truncate].is-expanded [data-expand-label]{display:none}.video-wrap{position:relative;padding-bottom:56.25%;height:0}.video-wrap iframe{position:absolute;top:0;left:0;width:100%;height:100%}.slide-in-enter{transition:all .3s}.slide-in-enter-active{transform:translateX(0)}.slide-in-enter-done{transform:translateX(0)}.slide-in-exit{transition:all .3s}.slide-in-exit-active{transform:translateX(120%)}.slide-in-exit-done{transform:translateX(120%)}.collapse{transition:all .3s}.collapse:not(.in){height:0;opacity:0;padding:0!important;margin:0!important}.collapse.in{height:initial;opacity:1}:root{scrollbar-color:var(--scrollbar-color,red) var(--scrollbar-bg,blue)}::-webkit-scrollbar-track{border-radius:10px}::-webkit-scrollbar{width:12px;background-color:var(--scrollbar-bg,auto)}::-webkit-scrollbar-thumb{border-radius:10px;border:2px solid var(--scrollbar-bg,auto);background:var(--scrollbar-color)}.hidden{display:none!important}.fullscreen-only{display:none!important}:-webkit-full-screen .fullscreen-only{display:flex!important}:-ms-fullscreen .fullscreen-only{display:flex!important}:fullscreen .fullscreen-only{display:flex!important}.animate-in{-webkit-animation:pulse;animation:pulse;-webkit-animation-duration:1s;animation-duration:1s;-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out}@-webkit-keyframes pulse{from{box-shadow:none;opacity:0}25%{box-shadow:0 0 0 10px rgba(255,255,255,.6);opacity:1}to{box-shadow:none}}@keyframes pulse{from{box-shadow:none;opacity:0}25%{box-shadow:0 0 0 10px rgba(255,255,255,.6);opacity:1}to{box-shadow:none}}/*! normalize.css v8.0.0 | MIT License | github.com/necolas/normalize.css */html{line-height:1.15;-webkit-text-size-adjust:100%}body{margin:0}h1{margin:.67em 0;font-size:2em}hr{box-sizing:content-box;height:0;overflow:visible}pre{font-family:monospace;font-size:1em}a{background-color:transparent}abbr[title]{border-bottom:none;text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}b,strong{font-weight:bolder}code,kbd,samp{font-family:monospace;font-size:1em}small{font-size:80%}sub,sup{position:relative;font-size:75%;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}img{border-style:none}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:100%;line-height:1.15}button,input{overflow:visible}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner,button::-moz-focus-inner{border-style:none;padding:0}[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring,button:-moz-focusring{outline:1px dotted ButtonText}fieldset{padding:.35em .75em .625em}legend{display:table;box-sizing:border-box;padding:0;max-width:100%;white-space:normal;color:inherit}progress{vertical-align:baseline}textarea{overflow:auto}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}[type=search]::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}details{display:block}summary{display:list-item}template{display:none}[hidden]{display:none}body{background-color:var(--body-bg-color);font-family:var(--global-font-family);line-height:1.5;color:var(--text-color);background-image:var(--body-bg-image,none);background-size:var(--body-bg-image-size,auto);background-attachment:var(--body-bg-image-attachment,scroll);background-repeat:var(--body-bg-image-repeat,repeat)}h1,h2,h3,h4,h5,h6{margin:0;font-weight:var(--global-weight-semibold);line-height:1.2;color:var(--heading-color);font-family:var(--heading-font-family, var(--global-font-family))}h1 small,h2 small,h3 small,h4 small,h5 small,h6 small{margin-left:6px}small[class*=theme-]{color:var(--theme-color)}ol,p,ul{margin:0 0 1em 0}h1[class*=theme-],h2[class*=theme-],h3[class*=theme-],h4[class*=theme-],h5[class*=theme-],h6[class*=theme-],ol[class*=theme-],p[class*=theme-],ul[class*=theme-]{color:var(--theme-color)}ol,ul{padding-left:20px}hr{margin:1em 0;border:0;border-top:1px solid var(--body-bg-shade2)}.body-size,body{font-size:calc(var(--font-size-normal) * .85)}h1{font-size:1.9125rem}h2{font-size:1.7rem}h3{font-size:1.59375rem}h4{font-size:1.38125rem}h5{font-size:1.275rem}h6{font-size:1.0625rem}h1{margin:0;font-size:1.375rem}@media (min-width:980px){.body-size,body{font-size:calc(var(--font-size-normal) * 1)}h1{font-size:2.25rem}h2{font-size:2rem}h3{font-size:1.875rem}h4{font-size:1.625rem}h5{font-size:1.5rem}h6{font-size:1.25rem}}a{color:var(--link-color)}a:focus{box-shadow:var(--focus-shadow);outline:0}a:hover{text-decoration:none}.small{font-size:var(--font-size-small)}.subdued{opacity:.7}blockquote{margin-left:0;padding-left:var(--global-margin);border-left:2px solid var(--text-color)}.prose{max-width:65ch}.hr-with-title{display:flex;justify-content:center;align-items:center;margin:2rem 0;font-size:var(--font-size-normal);text-transform:uppercase;color:var(--theme-color,var(--text-color))}.hr-with-title:after,.hr-with-title:before{display:block;flex:1 1 auto;margin-right:.625rem;height:1px;background-color:var(--theme-color,var(--text-color));opacity:.4;content:""}.hr-with-title:after{margin-right:0;margin-left:.625rem}.hr-with-title a{color:var(--theme-color,var(--text-color))}button.hr-with-title{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;border:none;background:0 0;font-weight:var(--global-weight-semibold);text-decoration:underline;color:var(--theme-color,var(--text-color));cursor:pointer}button.hr-with-title:hover{text-decoration:none}code:not(:empty),pre:not(:empty){padding:2px 4px;border:1px solid rgba(0,0,0,.05);border-radius:4px;background-color:rgba(255,190,21,.075);font-family:var(--code-font-family);font-size:.8rem;color:inherit}.no-bullets{list-style:none;padding-left:0}.ace_gutter,.ace_layer{min-width:62px!important}.ace_scroller{left:62px!important}:root{--field-background:var(--knockout-color);--field-border-color:var(--text-color-subdued);--select-border-color:var(--text-color-subdued);--field-focus-border-color:var(--brand-color);--field-focus-background:var(--knockout-color);--field-radius:var(--global-radius);--field-font-size:0.875rem;--label-font-size:0.875rem;--error-color:var(--alert-color);--radio-size:1.125rem;--max-field-width:25rem;--focus-shadow-color:rgba(43, 102, 178, 0.4);--focus-shadow:0 0 0 3px var(--focus-shadow-color);--error-shadow:0 0 0 3px var(--alert-color-tint);--checkbox-radio-color:var(--brand-color);--checkbox-radio-selected-color:var(--brand-color-shade)}label:not(.button),span.label{display:block;margin-bottom:4px;font-size:var(--label-font-size);font-weight:var(--global-weight-normal)}.page-heading+label:not(.button),.page-heading+span.label{margin-top:1rem}.django-as-p>p,.field{position:relative;margin-bottom:var(--global-margin);max-width:var(--max-field-width)}.django-as-p>p .error-message,.field .error-message{display:none}.django-as-p>p.error,.field.error{--field-border-color:var(--error-border-color, var(--error-color));--select-border-color:var(--error-border-color, var(--error-color))}.django-as-p>p.error [type=checkbox]+label .values:before,.django-as-p>p.error label:not(.file-label-button),.field.error [type=checkbox]+label .values:before,.field.error label:not(.file-label-button){color:var(--error-color)}.django-as-p>p.error.toggle label:before,.field.error.toggle label:before{background-color:var(--error-color)}.django-as-p>p.error .error-message,.field.error .error-message{display:block}.django-as-p>p.error .checkbox [type=checkbox]+label:before,.field.error .checkbox [type=checkbox]+label:before{border-color:var(--error-color)}.django-as-p>p.error .upload-preview,.django-as-p>p.error input:not([type=submit]):not([type=checkbox]):not([type=radio]),.django-as-p>p.error select,.django-as-p>p.error textarea,.django-as-p>p.error.checkbox label:before,.django-as-p>p.error.radio label:before,.django-as-p>p.error.toggle label:before,.field.error .upload-preview,.field.error input:not([type=submit]):not([type=checkbox]):not([type=radio]),.field.error select,.field.error textarea,.field.error.checkbox label:before,.field.error.radio label:before,.field.error.toggle label:before{box-shadow:var(--error-shadow)}.django-as-p>p.required label,.field.required label{font-weight:var(--global-weight-semibold)}.django-as-p>p.required label:after,.field.required label:after{content:"*"}.django-as-p>p.has-focus label.is-checked:before,.django-as-p>p.has-focus.checkbox label:before,.django-as-p>p.has-focus.radio label:before,.django-as-p>p.has-focus.toggle label:before,.django-as-p>p:not(.toggle):focus-within label.is-checked:before,.django-as-p>p:not(.toggle):focus-within.checkbox label:before,.django-as-p>p:not(.toggle):focus-within.radio label:before,.django-as-p>p:not(.toggle):focus-within.toggle label:before,.field.has-focus label.is-checked:before,.field.has-focus.checkbox label:before,.field.has-focus.radio label:before,.field.has-focus.toggle label:before,.field:not(.toggle):focus-within label.is-checked:before,.field:not(.toggle):focus-within.checkbox label:before,.field:not(.toggle):focus-within.radio label:before,.field:not(.toggle):focus-within.toggle label:before{box-shadow:var(--focus-shadow)}.django-as-p>p.has-focus [type=checkbox]:checked+label:after,.django-as-p>p.has-focus [type=radio]+label:after,.django-as-p>p:not(.toggle):focus-within [type=checkbox]:checked+label:after,.django-as-p>p:not(.toggle):focus-within [type=radio]+label:after,.field.has-focus [type=checkbox]:checked+label:after,.field.has-focus [type=radio]+label:after,.field:not(.toggle):focus-within [type=checkbox]:checked+label:after,.field:not(.toggle):focus-within [type=radio]+label:after{position:absolute;top:4px;left:1px;z-index:0;width:14px;height:13px;box-shadow:var(--focus-shadow);content:""}.django-as-p>p.has-focus [type=radio]+label:after,.django-as-p>p:not(.toggle):focus-within [type=radio]+label:after,.field.has-focus [type=radio]+label:after,.field:not(.toggle):focus-within [type=radio]+label:after{top:2px;left:2px;width:calc(var(--radio-size) - 4px);height:calc(var(--radio-size) - 4px);border-radius:50%}.django-as-p>p [type=checkbox]:invalid:focus+label:after,.django-as-p>p [type=radio]:invalid:focus+label:after,.field [type=checkbox]:invalid:focus+label:after,.field [type=radio]:invalid:focus+label:after{position:absolute;top:4px;left:1px;z-index:0;width:14px;height:13px;box-shadow:var(--error-shadow);content:""}.django-as-p>p [type=radio]:invalid:focus+label:after,.field [type=radio]:invalid:focus+label:after{top:2px;left:2px;width:calc(var(--radio-size) - 4px);height:calc(var(--radio-size) - 4px);border-radius:50%}.django-as-p>p.no-text.checkbox label,.field.no-text.checkbox label{margin-bottom:0;height:16px;vertical-align:top}.django-as-p>p.no-text.checkbox label:before,.field.no-text.checkbox label:before{margin:0}.django-as-p>p.inline-label,.field.inline-label{display:flex;align-items:center;flex-wrap:wrap}.django-as-p>p.inline-label label,.field.inline-label label{margin-right:.625rem;white-space:nowrap}.django-as-p>p.inline-label select,.field.inline-label select{width:auto}.django-as-p>p.inline-label.reverse-label label,.field.inline-label.reverse-label label{order:2;margin-left:10px}.django-as-p>p.inline-label .error-message,.field.inline-label .error-message{order:3;width:100%}@media (min-width:570px){.django-as-p>p.inline-label,.field.inline-label{flex-wrap:nowrap}}.django-as-p>p.full,.field.full{max-width:none}.django-as-p>p.large-label label,.field.large-label label{font-size:1.125rem;font-weight:var(--global-weight-semibold)}.django-as-p>p.medium-label label,.field.medium-label label{font-size:var(--font-size-base)}.dark-fields{--field-background:var(--dark-field-bg, var(--body-bg-shade-half));--field-border-color:var(--dark-field-border-color, var(--field-background))}.disabled .help-text,.disabled button,.disabled input,.disabled label,.disabled select,.disabled textarea,:disabled,:disabled~label{opacity:.4;pointer-events:none}input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]),select,textarea{-webkit-appearance:none;-moz-appearance:none;appearance:none;box-sizing:border-box;padding:.625rem;width:100%;min-height:38px;box-shadow:none;border:1px solid var(--field-border-color);border-width:var(--field-border-width,1px);border-radius:var(--field-radius);background-color:var(--field-background);font-family:var(--field-font-family, var(--global-font-family));font-size:var(--field-font-size);color:var(--field-color,var(--text-color));letter-spacing:var(--field-letter-spacing, normal)}.has-focus input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]),.has-focus select,.has-focus textarea,input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]):focus,select:focus,textarea:focus{box-shadow:var(--focus-shadow);border-color:var(--field-focus-border-color);background-color:var(--field-focus-background);outline:0}input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]):invalid:focus,select:invalid:focus,textarea:invalid:focus{--field-focus-border-color:var(--error-color);--select-border-color:var(--error-color);box-shadow:var(--error-shadow)}input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file])[required]+label:after,select[required]+label:after,textarea[required]+label:after{content:"*"}.m-input input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]),.m-input select,.m-input textarea,input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]).m-input,select.m-input,textarea.m-input{width:120px}.sm-input input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]),.sm-input select,.sm-input textarea,input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]).sm-input,select.sm-input,textarea.sm-input{width:80px}.xs-input input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]),.xs-input select,.xs-input textarea,input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]).xs-input,select.xs-input,textarea.xs-input{width:60px}input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]).auto-assign-input,select.auto-assign-input,textarea.auto-assign-input{width:60px;margin:0 4px;padding-right:4px;text-align:center}.field.has-button{display:flex;flex-flow:row wrap;align-items:center}.field.has-button label{width:100%}.field.has-button input:not([type=submit]):not([type=checkbox]):not([type=radio]):not([type=file]),.field.has-button select,.field.has-button textarea{flex:1 1 auto;max-width:16.25rem}.field.has-button .button{margin-left:.5rem}.field-pair{display:flex;gap:1rem;justify-content:space-between;align-items:center;border-radius:var(--global-radius);padding:8px 12px;margin-bottom:8px}.field-pair .inline-label{width:calc(100% - 160px)}.field-pair .field{margin:0}.field-pair.has-checked{background-color:var(--info-color-tint4)}input[type=file]{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;border-color:transparent;font-size:var(--field-font-size)}.hide-file-input{position:absolute;z-index:-1;width:.1px;height:.1px;overflow:hidden;opacity:0}fieldset{margin:0;padding:0;border:none}legend{margin:0;padding:1em 0 .5em;font-size:1.5rem;font-weight:var(--global-weight-semibold);color:var(--primary-heading-color)}select{position:relative;padding-right:2.5rem;border-color:var(--select-border-color);background-image:var(--select-bg-image, url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 18 10'%3E%3Cpath fill='none' vector-effect='non-scaling-stroke' stroke='%232e373f' stroke-width='2' stroke-linecap='round' stroke-linejoin='round' stroke-miterlimit='10' d='M1 1l8 8 8-8'/%3E%3C/svg%3E"));background-color:transparent;background-position:top 14px right 14px;background-repeat:no-repeat;background-size:12px 12px}select[multiple]{background-image:none;padding-right:.625rem}select option{background-color:var(--select-option-bg-color,var(--body-bg-color))}textarea{display:block;min-height:5.625rem;font-family:var(--textarea-font-family, var(--global-font-family));letter-spacing:0}.checkbox [type=checkbox]{position:absolute;left:0;opacity:0}.checkbox label:before{width:14px;height:14px;display:inline-block;margin-right:6px;margin-bottom:-3px;border:1px solid var(--checkbox-radio-color);vertical-align:baseline;content:""}.checkbox [type=checkbox]:checked+label:before,.checkbox label.is-checked:before{width:16px;height:16px;z-index:1;border:none;background-color:var(--checkbox-radio-selected-color);-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 16 16' id='checkbox_selected' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M8 12L3 7l2-2 3 3 8-8H0v16h16V4z'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 16 16' id='checkbox_selected' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M8 12L3 7l2-2 3 3 8-8H0v16h16V4z'/%3E%3C/svg%3E");-webkit-mask-position:center center;mask-position:center center;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:18px 18px;mask-size:18px 18px}.checkbox.checkbox-only label{width:16px;height:16px;display:block;margin:0}.checkbox-group .field:not(:last-child),.radio-group .field:not(:last-child){margin-bottom:.625rem}.radio [type=radio]{position:absolute;top:0;left:0;opacity:0}.radio.priority-label{padding-left:24px}.radio.priority-label label{font-size:1.125rem;color:var(--primary-heading-color);font-weight:var(--global-weight-semibold);padding-left:0}.radio.priority-label label:before{left:-24px;top:4px}.radio.priority-label:focus-within [type=radio]+label:after{top:6px;left:-22px}.radio label{position:relative;padding-left:calc(var(--radio-size) * 1.4)}.radio label:before{position:absolute;top:0;left:0;z-index:1;display:block;margin-right:6px;width:var(--radio-size);height:var(--radio-size);border:none;background-color:var(--checkbox-radio-color);background-position:top center;-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 21.75 21.75' xmlns='http://www.w3.org/2000/svg'%3E%3Ccircle cx='10.88' cy='10.88' r='10.38' fill='transparent' vector-effect='non-scaling-stroke' stroke='currentColor'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 21.75 21.75' xmlns='http://www.w3.org/2000/svg'%3E%3Ccircle cx='10.88' cy='10.88' r='10.38' fill='transparent' vector-effect='non-scaling-stroke' stroke='currentColor'/%3E%3C/svg%3E");-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:top;content:""}.radio [type=radio]:checked+label:before,.radio label.is-checked:before{-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 21.75 21.75' xmlns='http://www.w3.org/2000/svg'%3E%3Ccircle cx='10.88' cy='10.88' r='10.38' fill='transparent' vector-effect='non-scaling-stroke' stroke='currentColor'/%3E%3Ccircle cx='10.88' cy='10.88' r='7.34' fill='currentColor'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 21.75 21.75' xmlns='http://www.w3.org/2000/svg'%3E%3Ccircle cx='10.88' cy='10.88' r='10.38' fill='transparent' vector-effect='non-scaling-stroke' stroke='currentColor'/%3E%3Ccircle cx='10.88' cy='10.88' r='7.34' fill='currentColor'/%3E%3C/svg%3E");background-color:var(--checkbox-radio-selected-color)}.field-row{--max-field-width:none;display:grid;grid-gap:0 20px;grid-template-columns:repeat(auto-fit,minmax(200px,1fr))}.field-row.full{display:block}.field-row.compact{grid-template-columns:minmax(160px,-webkit-min-content) 1fr;grid-template-columns:minmax(160px,min-content) 1fr;grid-gap:0 40px}.field-row.narrow{grid-template-columns:repeat(auto-fit,minmax(160px,1fr))}@media (min-width:570px){.field-row.priority{grid-template-columns:5fr 4fr}}.field-row.inline-fields{display:flex;flex-wrap:wrap;margin-bottom:var(--global-margin);gap:0}.field-row.inline-fields>.field{margin:0 .625rem .75rem 0}.field-row.inline-fields>.field .field{margin:0}.field-row.inline-fields [type=text]{margin-bottom:.5rem}.field-row.pill-labels{gap:0}.field-row.pill-labels .field{margin:0 8px 8px 0}.field-row.pill-labels .checkbox>label,.field-row.pill-labels .radio>label{background-color:var(--card-bg-shade);border-radius:var(--global-radius);padding:8px 12px;margin:0}.field-row.pill-labels .checkbox>label:before,.field-row.pill-labels .radio>label:before{top:9px;left:9px}.field-row.pill-labels .checkbox [type=checkbox]:checked+label,.field-row.pill-labels .checkbox [type=radio]:checked+label,.field-row.pill-labels .radio [type=checkbox]:checked+label,.field-row.pill-labels .radio [type=radio]:checked+label{background-color:var(--info-color-tint4)}.field-row.pill-labels .checkbox [type=radio]:checked+label:after,.field-row.pill-labels .radio [type=radio]:checked+label:after{top:11px;left:11px}.field-row.pill-labels .checkbox [type=checkbox]:checked+label:after,.field-row.pill-labels .radio [type=checkbox]:checked+label:after{top:13px;left:13px}.field-row.pill-labels .radio>label{padding:8px 12px 8px calc(var(--radio-size) * 1.8)}.subfield{display:flex;align-items:flex-start}.subfield .field{margin:0 0 0 .625rem}.subfield.checkbox .field,.subfield.radio .field{margin-top:-.875rem}.help-text,.helptext{display:block;margin:4px 0 8px;font-size:var(--label-font-size);font-style:italic}.help-text ul,.helptext ul{font-style:normal}.error-message,.errorlist{margin:4px 0 8px;font-size:var(--label-font-size);color:var(--error-color)}.reporting-description{max-width:600px;padding:2.5rem 0}.button{--icon-size:1.25rem;-webkit-appearance:none;-moz-appearance:none;appearance:none;display:inline-flex;box-sizing:border-box;justify-content:center;align-items:center;margin:0;padding:var(--button-padding,0 1.25rem);width:auto;min-height:var(--button-min-height,2.5rem);border:var(--button-border,1px solid transparent);border-bottom-width:var(--button-border-bottom-width,1px);border-radius:var(--button-radius,var(--global-radius));background-color:var(--theme-color,var(--button-bg-default-color,var(--info-color)));background-image:var(--button-bg-image,none);background-size:105% 105%;background-repeat:no-repeat;background-position:var(--button-initial-bg-position,0 calc(var(--button-min-height,2.5rem) * 1.3));box-shadow:var(--button-box-shadow,none);font-size:var(--button-font-size, .75rem);font-family:var(--button-font-family, var(--global-font-family));line-height:1.1;text-align:center;text-decoration:none;vertical-align:top;color:var(--theme-text-color,var(--button-color-default,var(--knockout-color)));text-transform:var(--button-text-transform,normal);text-shadow:var(--button-text-shadow,none);letter-spacing:var(--button-letter-spacing, normal);transition:var(--button-transition, none);cursor:pointer}.button:not(:disabled):focus,.button:not(:disabled):hover{background-color:var(--button-bg-default-color-hover,var(--button-bg-default-color,transparent));background-image:var(--button-bg-image-hover,none);box-shadow:var(--button-box-shadow-hover,none);border-color:var(--theme-color,var(--button-bg-default-color,var(--info-color)));background-position:0 0;color:var(--button-color-hover-force,var(--theme-color,var(--button-bg-default-color,var(--info-color))))}.button.is-disabled,.button:disabled{opacity:.4;pointer-events:none}.button:not(.dropdown-button):active{transform:translateY(1px)}.button.hollow,.button.no-border{border-color:var(--theme-color,var(--button-bg-default-color,var(--info-color-shade)));background-color:var(--button-hollow-bg-color,transparent);color:var(--theme-color,var(--button-hollow-color,var(--info-color-shade)))}.button.hollow:not(:disabled):focus,.button.hollow:not(:disabled):hover,.button.no-border:not(:disabled):focus,.button.no-border:not(:disabled):hover{background-color:var(--theme-color,var(--button-bg-default-color,var(--info-color)));color:var(--theme-text-color,var(--button-color-default,var(--knockout-color)))}.button.strong{font-weight:var(--global-weight-semibold);font-size:.875rem}.button.no-border{padding-right:0;padding-left:0;min-width:0;border-width:0;background-color:transparent;background-image:none;text-align:left;color:var(--theme-color,var(--text-color));box-shadow:none}.button.no-border:not(:disabled):focus,.button.no-border:not(:disabled):hover{background-image:none;background-color:transparent;text-decoration:underline;color:var(--theme-color-shade,var(--text-color));box-shadow:none}.button.knockout{border:var(--button-border,1px solid var(--knockout-color));background-color:transparent;font-weight:var(--global-weight-semibold);color:var(--knockout-button-color,var(--knockout-color))}.button.knockout:not(:disabled):focus,.button.knockout:not(:disabled):hover{background-color:var(--knockout-button-color,var(--knockout-color))}.button.small{--icon-size:0.75rem;padding:0 16px;min-width:0;min-height:1.875rem;font-size:.75rem}.button.large{min-height:3.125rem;font-size:1rem}.button.full-width{display:flex}.button.alert-on-hover:not(:disabled):hover{border-color:var(--alert-color);background-color:var(--alert-color-tint3);color:var(--alert-color-shade);box-shadow:var(--button-alert-on-hover-box-shadow,none)}.button.success-on-hover:not(:disabled):hover{border-color:var(--success-color);background-color:var(--success-color-tint3);color:var(--success-color-shade);box-shadow:var(--button-success-on-hover-box-shadow,none)}.button .quantity{font-weight:var(--global-weight-normal);color:var(--theme-text-color,var(--knockout-color))}.button.hollow .quantity{color:var(--theme-color,var(--info-color))}.button.card-button{--icon-size:2rem;flex-direction:column}.button.card-button .icon{margin-bottom:.625rem}@media (min-width:768px){.button{width:auto;min-width:6.25rem;max-width:22.5rem}}.button:focus,button:focus,input[type=file]:focus+.file-label-button,input[type=submit]:focus{box-shadow:var(--focus-shadow);outline:0}.button:not(.icon-button) .icon,.button:not(.icon-button) .icon-wrap{flex:0 0 auto;margin-right:6px}.button:not(.icon-button) .icon-wrap.inside-button,.button:not(.icon-button) .icon.inside-button{--icon-size:1rem;margin:0 6px 0 10px}.button:not(.icon-button) .icon-wrap .icon{margin-right:0}.button.no-border .icon{margin-left:0}.button.icon-button{padding:0;min-width:0;border:none}.button.icon-button:not(.circle){--icon-size:0.9375rem;--icon-color:var(--theme-color, var(--info-color));background-color:transparent;background-image:none;box-shadow:none}.button.icon-button:not(.circle):not(:disabled):focus,.button.icon-button:not(.circle):not(:disabled):hover{--icon-color:var(--theme-color-shade, var(--info-color-shade));background-color:transparent}.button.icon-button.circle{--icon-size:1.125rem;width:30px;height:30px;min-height:0;border-radius:50%;box-shadow:none}.button.icon-button.circle.large{--icon-size:1.5rem;width:36px;height:36px}.button.icon-button.subdued{opacity:.7}.button.icon-button.subdued:hover{opacity:1}.has-close-button,.has-help-button{position:relative}.has-close-button .close-button,.has-close-button .help-button,.has-help-button .close-button,.has-help-button .help-button{position:absolute;top:5px;right:5px;z-index:2}.has-close-button .close-button.center,.has-close-button .help-button.center,.has-help-button .close-button.center,.has-help-button .help-button.center{top:calc(50% - 10px)}.close-button,.help-button{--icon-size:0.5rem;--icon-color:var(--close-button-color, var(--knockout-color));width:1.25rem;height:1.25rem;-webkit-appearance:none;-moz-appearance:none;appearance:none;position:relative;display:flex;justify-content:center;align-items:center;padding:0;border:none;border-radius:50%;background-color:var(--close-button-bg-color,var(--text-color));font-weight:var(--global-weight-semibold);color:var(--close-button-color,var(--knockout-color));cursor:pointer;box-shadow:none}.close-button:hover,.help-button:hover{opacity:.8;box-shadow:none}.close-button:after,.help-button:after{width:2.5rem;height:2.5rem;position:absolute;top:-10px;left:-10px;content:""}.close-button.inverse,.help-button.inverse{background-color:var(--close-button-color,var(--knockout-color));--icon-color:var(--close-button-bg-color, var(--text-color));color:var(--close-button-bg-color,var(--text-color))}.close-button.transparent,.help-button.transparent{background-color:transparent;--icon-color:var(--close-button-bg-color, var(--text-color));color:var(--close-button-bg-color,var(--text-color))}.close-button.hollow,.help-button.hollow{border:2px solid var(--theme-color,var(--button-bg-default-color,var(--info-color)));color:var(--theme-color,var(--button-bg-default-color,var(--info-color)));background-color:var(--knockout-color);width:2rem;height:2rem}.close-button.hollow:hover,.help-button.hollow:hover{background-color:var(--theme-color,var(--button-bg-default-color,var(--info-color)));color:var(--knockout-color)}.add-button{--icon-color:var(--text-color);--icon-size:0.5rem;width:1.5rem;height:1.5rem;-webkit-appearance:none;-moz-appearance:none;appearance:none;position:relative;padding:0;border:1px solid var(--card-border-color-default);border-radius:4px;background-color:transparent;font:0/0 a;color:transparent;cursor:pointer}.add-button:hover{border-color:var(--success-color);background-color:var(--success-color-tint)}.add-button:after{position:absolute;top:-8px;right:-4px;bottom:-8px;left:-8px;display:block;content:""}.button-wrap{display:flex;justify-content:flex-start;align-items:center;flex-wrap:wrap;padding:.625rem 0;gap:var(--button-wrap-margin,.625rem)}.button-wrap.align-end{justify-content:flex-end}.button-wrap.align-full{justify-content:space-between}.button-wrap.align-center{justify-content:center}.button-wrap.stack{flex-direction:column}.button-wrap.stack .button+.button{margin-top:.625rem}.button-wrap.field-max-width{max-width:var(--max-field-width)}.button-wrap.tall{padding-top:1.875rem;padding-bottom:1.875rem}.button-wrap.feature-color{background:var(--success-color-tint5);margin-top:2.25rem;padding-right:1.875rem;padding-left:1.875rem}.button-wrap.pad-0{padding:0}.button-wrap>*{margin-bottom:0}.button-wrap>.field{margin-right:1.875rem}.button-wrap .checkbox label{margin-bottom:0}.button-wrap .checkbox label:before{margin-top:3px}.button-wrap .button-help-text{margin:auto .625rem auto 0;font-size:var(--font-size-small);font-style:italic}.button-wrap .push-right{margin-left:auto}.button-wrap .push-left{margin-right:auto}@media (max-width:569px){.button-wrap>.has-dropdown{margin-right:0;width:100%}.button-wrap.inline-on-small>.button:not(.no-border),.button-wrap.inline-on-small>.has-dropdown{margin-right:inherit;width:auto}.button-wrap.inline-on-small>*,.button-wrap.inline-on-small>:not(:last-child){margin-bottom:0}.button-wrap .last-on-mobile{order:100;margin-top:.625rem}}@media (min-width:570px){.button-wrap.reverse-on-desktop{flex-direction:row-reverse;justify-content:flex-end}.button-wrap.reverse-on-desktop.align-full{justify-content:space-between}.button-wrap.reverse-on-desktop.align-center{justify-content:center}.button-wrap.reverse-on-desktop.align-end{justify-content:flex-start}}.back-button{-webkit-appearance:none;-moz-appearance:none;appearance:none;display:inline-block;width:40px;height:40px;border:none;background:0 0;cursor:pointer}.back-button:hover{color:var(--info-color)}table{--avatar-size:1.875rem;--avatar-font-size:0.6875rem;margin-bottom:1rem;width:100%;border-color:var(--theme-color,var(--body-bg-shade2));border-radius:0;border-collapse:collapse;font-size:.95rem}table td,table th{padding:4px 8px;border-bottom:1px solid var(--theme-color-tint2,var(--body-bg-shade2));text-align:left}table td:first-child,table th:first-child{padding-left:.5rem}table td:last-child,table th:last-child{padding-right:.5rem}table td.border-bottom,table th.border-bottom{border-bottom:1px solid var(--theme-color,var(--brand-color))}table td.no-bottom-border,table th.no-bottom-border{border-bottom:0}table td.top-pad,table th.top-pad{padding-top:1.25rem}table td.stretch-column,table th.stretch-column{width:100%}table td.shrink-column,table th.shrink-column{width:1px}table td.highlight-row,table th.highlight-row{background-color:var(--theme-color-tint3,var(--well-bg))}table td.col-actions,table th.col-actions{text-align:right}@media (min-width:768px){table td:first-child,table th:first-child{padding-left:1rem}table td:last-child,table th:last-child{padding-right:1rem}}table th{white-space:nowrap}table .ellipsis,table thead th{font-weight:300;color:var(--text-color-highlight1,var(--text-color))}table.no-header-shade thead th:not(.highlight-row){background-color:transparent}table thead th.highlight-row{border-radius:var(--global-radius) var(--global-radius) 0 0}table tbody tr:last-child .highlight-row,table tfoot th:last-child .highlight-row{border-radius:0 0 var(--global-radius) var(--global-radius)}table thead th{background-color:var(--theme-color,var(--body-bg-shade));color:var(--theme-text-color,var(--text-color))}table tfoot th{background-color:var(--theme-color-tint3,var(--body-bg-shade))}table.condensed td,table.condensed th{padding:0 4px}table.expanded td,table.expanded th{padding-top:.75rem;padding-bottom:.75rem}table.large-text{font-size:1.25rem}table.large-text .field.checkbox{margin:.375rem 0 .5rem 0}table.large-text .field.checkbox label{vertical-align:middle}table.small-header-text thead th{font-size:.8rem}table.striped tbody tr:nth-child(even) td,table.striped tbody tr:nth-child(even) th{background:var(--theme-color-tint4,var(--body-bg-shade-half))}table.striped.hover-rows tbody tr:not(.no-hover):hover td,table.striped.hover-rows tbody tr:not(.no-hover):hover th{background:var(--theme-color-tint3,var(--body-bg-shade))}table.hover-rows tr:not(.no-hover):hover{background:var(--theme-color-tint4,var(--body-bg-shade))}table.no-h-pad td:first-child,table.no-h-pad th:first-child{padding-left:0}table.no-h-pad td:last-child,table.no-h-pad th:last-child{padding-right:0}table.no-h-pad td.highlight-row,table.no-h-pad th.highlight-row{padding-right:.5rem;padding-left:.5rem}table.no-borders td,table.no-borders th{border-bottom:none}table.no-color td,table.no-color th{border-bottom:var(--table-no-color-border,1px solid var(--theme-color-tint3,var(--body-bg-shade2)))}table.no-color tbody:last-child tr:last-child td,table.no-color tbody:last-child tr:last-child th{border-bottom:1px solid transparent}table.no-color tfoot th,table.no-color thead th{background-color:transparent}table .checkbox{margin:.375rem 0 0 0}table .icon-cell{width:50px;text-align:right}table .has-error{color:var(--error-color)}table .has-error .error-message{display:block;margin:0;font-size:.8em}table[class*=theme-] thead th:after,table[class*=theme-] thead th:before{background-color:var(--knockout-color)}table .table-header-row td,table .table-header-row th{padding-top:1rem;padding-bottom:.8rem;font-size:1.3rem}.table-scroll{position:relative;margin-right:-.625rem;margin-bottom:1rem;max-width:calc(100% + .625rem);overflow:auto;-webkit-overflow-scrolling:touch}.table-scroll table{margin-bottom:0}.table-scroll table td{position:relative}.table-scroll table td:last-child:after{position:absolute;right:-.625rem;display:block;width:.625rem;height:1px;content:""}.table-scroll .filename{color:var(--text-color-highlight1,var(--text-color))}@media (min-width:980px){.table-scroll{margin-right:0}.table-scroll table td:last-child:after{content:none}}.page-team table td,.page-team table th{display:var(--team-page-sub-column-display,table-cell)}.page-team table td:first-child,.page-team table th:first-child{display:table-cell}.page-team table tr.card-shade{display:var(--team-page-sub-column-display,table-row)}.sticky-col-table td:first-child,.sticky-col-table th:first-child{position:sticky;left:0;z-index:1}.sticky-col-table td.is-not-sticky,.sticky-col-table th.is-not-sticky{position:static}.sticky-col-table.budget-theme td,.sticky-col-table.budget-theme th{text-align:right}.sticky-col-table.budget-theme td:first-child,.sticky-col-table.budget-theme th:first-child{background-color:var(--theme-color,var(--body-bg-shade2));text-align:left}.sticky-col-table.budget-theme .subhead-row td,.sticky-col-table.budget-theme .subhead-row th{padding-top:22px;min-height:53px}.sticky-col-table.budget-theme thead th:first-child{background-color:var(--theme-color,var(--body-bg-shade2))}@media (max-width:569px){.sticky-col-table.disable-on-mobile td:first-child,.sticky-col-table.disable-on-mobile th:first-child{position:static}.sticky-col-table.card-theme td:first-child:after,.sticky-col-table.card-theme th:first-child:after{position:absolute;top:0;right:-8px;bottom:0;width:8px;background:linear-gradient(to right,rgba(0,0,0,.05) 0,rgba(255,255,255,0) 100%);content:""}.sticky-col-table.card-theme th:first-child:after{right:-12px;width:12px;background:radial-gradient(farthest-side at 0 50%,rgba(0,0,0,.05) 0,rgba(255,255,255,0) 100%)}.sticky-col-table.card-theme td.is-not-sticky:first-child:after{content:none}}:root{--first-sticky-col-width:200px}.card-theme{--avatar-size:2.25rem;--avatar-font-size:1rem;border-spacing:0 0.375rem;border-collapse:separate}.card-theme thead th{border:none;background:var(--body-bg-color);font-size:1.25rem;white-space:nowrap}.card-theme td,.card-theme th{padding:.625rem;border:1px solid var(--theme-color-tint3,var(--card-border-color-default));border-width:1px 0 1px 0;background:var(--card-bg)}.card-theme td:first-child,.card-theme th:first-child{width:50%;min-width:var(--first-sticky-col-width);border-radius:var(--card-radius) 0 0 var(--card-radius);border-width:1px 0 1px 1px}.card-theme td.text-right,.card-theme th.text-right{text-align:right}.card-theme td:last-child,.card-theme th:last-child{border-radius:0 var(--card-radius) var(--card-radius) 0;border-width:1px 1px 1px 0}.card-theme td.inactive,.card-theme th.inactive{padding-left:1.25rem;background:var(--info-color);color:var(--knockout-color);text-align:left}.card-theme td.inactive>:last-child,.card-theme th.inactive>:last-child{margin-bottom:0}.card-theme td.inactive .page-subheading,.card-theme th.inactive .page-subheading{margin:0;font-size:1.25rem;color:var(--knockout-color)}.card-theme .card-shade td,.card-theme .card-shade th{background:var(--card-bg-shade2)}@media (min-width:980px){.card-theme{--avatar-size:2.875rem}}.table-item-label{color:var(--theme-color-shade,var(--text-color))}.table-item-val{display:block;font-size:1.25rem;color:var(--text-color-highlight2,var(--text-color))}.table-item-label{--icon-size:0.75rem;display:flex;justify-content:center;align-items:center;font-size:var(--font-size-small)}.table-item-label.pull-down{margin-bottom:-1.25rem}:root{--avatar-size:2.5rem}.avatar{position:relative;display:flex;justify-content:center;align-items:center;width:var(--avatar-size);height:var(--avatar-size);border-radius:var(--avatar-radius,50%);background-color:var(--theme-color,var(--avatar-bg-color,var(--success-color)));font-size:var(--avatar-font-size, 1rem);font-weight:var(--global-weight-semibold);text-align:center;color:var(--knockout-color)}.avatar img,.avatar-initials,.avatar-inner{display:flex;align-items:center;justify-content:center;width:100%;height:100%;border-radius:var(--avatar-radius,50%);line-height:var(--avatar-size);-webkit-mask-image:var(--avatar-inner-mask-image,unset);mask-image:var(--avatar-inner-mask-image,unset)}.avatar-inner{background-color:var(--avatar-inner-bg-color,transparent);padding:var(--avatar-inner-padding,0)}.avatar img{z-index:1;width:100%;height:100%;-o-object-fit:cover;object-fit:cover}.avatar.small{--avatar-size:1.875rem;--avatar-font-size:0.75rem}.avatar.medium{--avatar-size:3.125rem;--avatar-font-size:1.25rem}.avatar.large{--avatar-size:8rem;--avatar-font-size:2.125rem}.avatar.has-icon{position:relative}.avatar.has-icon .icon-button{position:absolute;right:-4px;bottom:-4px;z-index:2}.avatar[data-online=true]:after{position:absolute;top:-2px;right:-2px;z-index:1;display:block;width:calc(var(--avatar-size)/ 2.7);height:calc(var(--avatar-size)/ 2.7);border-radius:50%;background:var(--theme-color,var(--success-color));content:""}.avatar-detail{display:flex;justify-content:flex-start;align-items:center;width:100%;min-width:0}.avatar-detail-meta{margin:0;padding-left:.625rem;overflow:hidden;text-overflow:ellipsis}.avatar-detail-meta .tag-list{margin:5px 0 0 0}.avatar-detail-meta .tag{line-height:1.2}.avatar-detail-desc{display:block;font-weight:var(--global-weight-normal);opacity:.8;overflow:hidden;text-overflow:ellipsis}.avatar-detail .avatar{flex:0 0 auto}.avatar-detail .button,.avatar-detail .card-time,.avatar-detail .icon-link{margin-left:auto}.avatar-detail.inline-title .avatar-detail-meta{line-height:1}.avatar-detail.inline-title .avatar-detail-meta .notification-flag{margin:0;font-size:.625rem}.avatar-detail.inline-title .avatar-detail-desc{display:inline;font-size:.8em}.avatar-detail+.tag-list{margin:.625rem 0 0 0}@media (min-width:980px){.avatar-detail+.tag-list{margin-left:calc(var(--avatar-size) + .625rem)}}.card{position:relative;padding:var(--card-padding,.625rem);border:1px solid var(--card-border-color-force,var(--theme-color-tint3,var(--card-border-color-default)));border-width:var(--card-border-width,1px);border-radius:var(--card-radius);background:var(--card-bg);box-shadow:var(--card-shadow-default,none)}.card.priority{border-color:var(--theme-color,var(--text-color))}.card.fill{--card-bg-shade:var(--theme-color-tint5, var(--card-bg-shade2));--card-bg:var(--theme-color-alpha, var(--card-bg-shade));--card-border-color:var(--theme-color-tint3, var(--text-color))}.card.fill .button,.card.fill .card-heading{color:var(--theme-color-shade)}.card-padding{position:relative;padding:.625rem}.card-thumbnail{max-height:11.25rem;display:block;margin:0 auto}.card-button-wrap{display:flex;justify-content:center;align-items:center}.card-set .card{margin-bottom:.625rem}.card-numbered{margin-left:40px;margin-bottom:40px;border-top-left-radius:0}.card-numbered-indent{margin-left:40px}.card-number{position:absolute;top:0;left:-40px;padding:10px;width:40px;border-radius:var(--global-radius-tl) 0 0 var(--global-radius-bl);font-size:1.25rem;text-align:center;font-weight:var(--global-weight-semibold);background:var(--card-bg);color:var(--text-color-subdued);z-index:-1}.glow-shadow .card-number{box-shadow:var(--glow-shadow)}.card-offset-button{position:absolute;right:-10px;top:-10px}.card-html-content{--heading-margin-default:0.5rem 0;font-size:.875rem}.card .darken{margin:0 -.625rem -.625rem;padding:.625rem 1.25rem;border-top:1px solid var(--card-bg-shade2);background:var(--card-bg-shade)}.card.is-unread{--card-bg:var(--card-bg-unread, var(--unread-tint1));--card-bg-shade:var(--unread-tint2);position:relative}.card.is-unread .card-heading:before{width:12px;height:12px;display:inline-block;margin:0 .25rem .125rem 0;border-radius:50%;background-color:var(--unread-color);vertical-align:middle;content:""}.card.is-unread:before{position:absolute;top:-1px;right:-1px;left:-1px;height:var(--unread-border-top-height,0);background:var(--unread-top-border-bg,none);border-radius:var(--global-radius-tl) var(--global-radius-tr) 0 0;content:""}.card.is-inactive.has-shadow-on-hover:hover{box-shadow:none}.card.is-inactive>*{opacity:.8}.card[class*=theme]{padding-top:var(--card-with-theme-padding-top,var(--card-padding,.625rem));border-width:var(--card-with-theme-border-width,1px)}.card[class*=theme]:before{position:absolute;top:0;left:0;right:0;height:6px;background-image:var(--card-top-stripe-bg-image,none);background-color:var(--theme-color,var(--brand-color-tint5));border-radius:var(--card-top-stripe-radius,0);content:var(--card-with-theme-top-stripe,unset)}.card[class*=theme].theme-low{padding-top:.625rem}.card[class*=theme].theme-low:before{content:none}.card[class*=theme].no-h-pad{padding-left:0;padding-right:0}.card td.ellipsis,.card td.ellipsis-three-lines,.card td.ellipsis-two-lines{max-width:6.875rem}.card.icon-card{margin-top:calc((var(--icon-size)/ 2) + .625rem + 2px);text-align:center}.card.icon-card .card-header{--icon-size:3.75rem;flex-direction:column;align-items:center;margin:calc((var(--icon-size)/ -2) - .625rem) 0 0}.card.icon-card .card-header .icon-wrap{margin-bottom:var(--global-margin)}.card.icon-card .card-header .icon{margin:0}.card.icon-card .card-footer{justify-content:center}.card-header{--icon-size:1.5rem;display:flex;justify-content:space-between;margin:0 0 .625rem 0}.card-header+.card-details{margin-top:0}.card-header .icon{margin-left:.625rem}.card-header-details{flex:1 1 100%}.card-heading{grid-area:heading;font-size:var(--card-heading-size, var(--font-size-base))}.card-heading.feature-size{font-size:1.5rem}.card-heading a{text-decoration:none;color:var(--info-color-shade)}.card-heading a:hover{color:var(--brand-color)}.theme-brand-light .card-heading{color:var(--theme-color)}.card-heading,.card-time,.card-var-label{color:var(--card-heading-default-color,var(--text-color-highlight2,var(--theme-color-shade,var(--text-color))));text-transform:var(--card-text-transform,none);font-family:var(--card-heading-font-family, var(--global-font-family))}.card-subheading{margin-bottom:.625rem;font-size:.75rem;text-transform:uppercase;color:var(--theme-color,var(--text-color))}.feature-card .card-subheading{font-size:1rem;text-transform:none}.card-time{font-size:var(--font-size-small);white-space:nowrap;opacity:.8}.card-list .card{margin-bottom:.625rem}.card .well{padding:.625rem;border:0 none;border-radius:var(--global-radius)}.card .button-wrap{padding-bottom:0}.card .world-logo{--icon-size:40px;max-width:100px;max-height:60px;color:var(--brand-color)}.card .substats{margin:1em 0 0 0}.card.has-shadow{box-shadow:var(--card-shadow)}.card.has-shadow-on-hover:hover{box-shadow:var(--card-shadow)}.card.heavy-shadow{box-shadow:0 0 0 8px var(--success-color-tint3)}.card.glow-shadow{box-shadow:var(--glow-shadow);border:0 none}.card.feature-shadow{box-shadow:var(--feature-shadow);border:0 none}.card-details{display:flex;justify-content:space-between;align-items:center;margin:.625rem 0}.card-details .icon{margin-left:auto}.card-content.has-actions{display:flex}.card-content.has-actions .card-actions{display:flex;flex-direction:column;margin-left:auto}.card-content.has-actions .card-actions .button+.button{margin-top:.375rem}.card-media,.card-media .video-wrap{margin-bottom:.625rem}.card-footer{--icon-size:1.125rem;display:flex;justify-content:space-between;align-items:center;margin-top:auto;padding:.625rem 0;font-size:var(--font-size-small)}.card-footer-tag{display:flex;align-items:center;font-weight:var(--global-weight-semibold)}.card-footer-tag .tag-link{text-decoration:none}.card-footer-tag .tag-link:hover{text-decoration:underline}.card-footer-tag .icon{margin-right:.375rem}.card-footer-tag .icon.circles_1{width:.875rem}.card-footer-tag .icon.circles_2{width:1.375rem}.card-footer-tag .icon.circles_3{width:1.875rem}.card-footer-tag .icon.circles_4{width:2.5rem}.card[data-card-flag]:after{position:absolute;top:0;right:0;width:var(--card-flag-width,auto);border-radius:var(--card-flag-radius,0 0 0 var(--global-radius-bl));padding:4px 16px;font-size:.875rem;color:var(--card-flag-color,var(--text-color));text-align:center;background:var(--card-flag-bg-color,var(--caution-color-tint));font-weight:var(--global-weight-semibold);content:attr(data-card-flag)}@media (min-width:570px){.card-list .card{margin-bottom:1.875rem}.card-list .card .card{margin-bottom:.625rem}.card.large{padding:1.25rem}.card.feature-card{padding:1.875rem}.card.feature-card .card-header{align-items:flex-start;margin:0 0 .625rem}.card.feature-card .card-header+.card-media{margin-top:1.25rem}.card.feature-card .card-heading{font-size:var(--feature-card-heading-size, 1.75rem);font-family:var(--heading-font-family);font-weight:var(--feature-card-heading-weight,var(--global-weight-semibold));margin:var(--feature-card-heading-margin,inherit)}.card.feature-card .card-footer{padding-bottom:0}.card.feature-card .darken{margin:0 -1.875rem -1.875rem;padding:1.875rem}.card .card-media,.card .card-media .video-wrap{margin-bottom:1.25rem}}:root{--checkmark-size:1rem;--new-badge-size:0.625rem}.has-dropdown{position:relative;display:inline-flex;font-weight:var(--global-weight-normal)}.has-dropdown.is-expanded .dropdown,.has-dropdown.is-expanded .dropdown-button:before,.has-dropdown.tooltip-dropdown:hover .dropdown,.has-dropdown.tooltip-dropdown:hover .dropdown-button:before,.has-dropdown:not(.disable-focus-within):focus-within .dropdown,.has-dropdown:not(.disable-focus-within):focus-within .dropdown-button:before{display:block}.has-dropdown.is-expanded .dropdown-button:after,.has-dropdown.tooltip-dropdown:hover .dropdown-button:after,.has-dropdown:not(.disable-focus-within):focus-within .dropdown-button:after{transform:rotate(180deg);padding-right:8px;padding-left:0;-webkit-mask-position:top left;mask-position:top left}.has-dropdown.is-expanded .star-toggle.dropdown-button:after,.has-dropdown.tooltip-dropdown:hover .star-toggle.dropdown-button:after,.has-dropdown:not(.disable-focus-within):focus-within .star-toggle.dropdown-button:after{padding-right:0}.has-dropdown.is-expanded.align-above .dropdown-button:before,.has-dropdown.tooltip-dropdown:hover.align-above .dropdown-button:before,.has-dropdown:not(.disable-focus-within):focus-within.align-above .dropdown-button:before{top:auto;bottom:100%;transform:rotate(180deg)}.has-dropdown.tooltip-dropdown .dropdown{padding:.5rem}.has-dropdown.is-heading-select{outline:0}.has-dropdown.is-heading-select .dropdown-button{padding-left:.5rem;padding-right:2.5rem;font-size:1.5rem;font-family:var(--heading-font-family);color:var(--primary-heading-color);text-decoration:none;border:1px solid var(--brand-color-tint4);background-image:var(--select-bg-image, url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 18 10'%3E%3Cpath fill='none' vector-effect='non-scaling-stroke' stroke='%232e373f' stroke-width='2' stroke-linecap='round' stroke-linejoin='round' stroke-miterlimit='10' d='M1 1l8 8 8-8'/%3E%3C/svg%3E"));background-color:transparent;background-position:top 14px right 9px;background-repeat:no-repeat;background-size:12px 12px}.has-dropdown.is-heading-select .dropdown-button:after{content:none}@media (max-width:569px){.has-dropdown{margin-bottom:.625rem}.has-dropdown.is-heading-select .dropdown-button{padding-left:.5rem;font-size:1.25rem;background-position:top 10px right 14px}.has-dropdown .dropdown-button{margin-right:0;width:100%}.has-dropdown .dropdown{width:100%;min-width:80vw}.has-dropdown.align-left .dropdown{max-width:none}}.dropdown{position:absolute;top:calc(100% + .625rem);right:-8px;z-index:3;display:none;padding:.5rem 0;width:80vh;max-width:18.75rem;box-shadow:var(--heavy-shadow);border-radius:var(--global-radius);background:var(--dropdown-bg);font-size:1rem}.align-above .dropdown{top:auto;bottom:calc(100% + .625rem)}.align-left .dropdown{right:auto;left:0;min-width:100%}.align-right .dropdown{left:calc(100% + .75rem);top:-50%}.narrow-dropdown .dropdown{max-width:11.25rem}.small-dropdown .dropdown{max-width:12.5rem}.dropdown-details,.dropdown-link,.dropdown-main-heading,.dropdown-section-heading{color:var(--theme-color,var(--dropdown-color,var(--text-color)))}.dropdown,.dropdown a{color:var(--theme-text-color,var(--button-color-default,var(--text-color)))}.dropdown a:hover,.dropdown:hover{color:var(--theme-text-color,var(--button-color-default,var(--text-color)))}.dropdown-button{display:inline-flex;align-items:center;margin:0}.dropdown-button:after{display:block;margin-right:-4px;margin-left:auto;padding-left:8px;width:10px;height:8px;background-color:var(--theme-text-color,var(--button-color-default,var(--knockout-color)));-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 14 8.84' id='arrow_down' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M11.61 0H.73A.73.73 0 000 .72a.7.7 0 00.13.42l.08.1 6 7.21a1.09 1.09 0 001.54.14l.15-.14 5.94-7.2.1-.12a.8.8 0 00.06-.4.73.73 0 00-.72-.73z'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 14 8.84' id='arrow_down' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M11.61 0H.73A.73.73 0 000 .72a.7.7 0 00.13.42l.08.1 6 7.21a1.09 1.09 0 001.54.14l.15-.14 5.94-7.2.1-.12a.8.8 0 00.06-.4.73.73 0 00-.72-.73z'/%3E%3C/svg%3E");-webkit-mask-position:top right;mask-position:top right;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:10px 10px;mask-size:10px 10px;content:""}.dropdown-button:before{position:absolute;top:100%;right:13px;left:auto;z-index:4;display:none;width:16px;height:16px;background-color:var(--dropdown-bg);-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 15.6 11.2' id='dropdown_pip' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1 8.6l5.9-7.2c.2-.2.5-.4.8-.4s.6.2.8.4l5.9 7.2s-1 2.6-6.8 2.6S1 8.6 1 8.6z' fill='currentColor'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 15.6 11.2' id='dropdown_pip' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1 8.6l5.9-7.2c.2-.2.5-.4.8-.4s.6.2.8.4l5.9 7.2s-1 2.6-6.8 2.6S1 8.6 1 8.6z' fill='currentColor'/%3E%3C/svg%3E");-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;content:""}.dropdown-button.button.hollow{border-color:rgba(0,0,0,.4);color:var(--text-color)}.dropdown-button:hover:after{background-color:var(--button-color-hover-force,var(--theme-color,var(--button-bg-default-color,var(--info-color))))}.dropdown-list{list-style:none;margin:0;padding:0}.dropdown-action-item,.dropdown-item{margin:0;border-bottom:1px solid var(--dropdown-border-color)}.dropdown-action-item label,.dropdown-item label{margin:0;padding:.375rem 0}.dropdown-item:last-child{border-bottom:none}.dropdown-group{padding:.375rem 1rem;font-weight:var(--global-weight-semibold);background:var(--body-bg-shade);display:flex;align-items:center;gap:.5rem}.dropdown-link{display:flex;align-items:center;gap:4px;margin-bottom:0;padding:.375rem 1rem;text-decoration:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;border:0 none;background:0 0;width:100%}.dropdown-link.is-checked{position:relative;padding-left:calc(var(--checkmark-size) + 24px);font-weight:var(--global-weight-semibold)}.dropdown-link.is-checked:after{position:absolute;top:50%;left:16px;display:block;margin-right:6px;width:var(--checkmark-size);height:var(--checkmark-size);background-color:var(--text-color);-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 23.043 17.154' id='check' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M22.501.542a1.852 1.852 0 00-2.526-.086l-.178.179-7.551 7.554-3.383 3.384c-.019.021-.038.043-.059.063l-.063.058-.007.006-.008.006a1.022 1.022 0 01-1.325-.027l-.009-.008a1.19 1.19 0 01-.073-.073l-.007-.009-3.404-3.403-.737-.738a1.855 1.855 0 00-2.627 0 1.852 1.852 0 00-.042 2.58l.087.088 6.7 6.7.056.057.019.018c.383.344.962.352 1.351.021l.12-.121 1.84-1.839-.001-.001.535-.534 4.7-4.699.042-.045.046-.042.678-.68.006.005L22.347 3.3l.291-.292a1.852 1.852 0 00-.137-2.466z'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 23.043 17.154' id='check' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M22.501.542a1.852 1.852 0 00-2.526-.086l-.178.179-7.551 7.554-3.383 3.384c-.019.021-.038.043-.059.063l-.063.058-.007.006-.008.006a1.022 1.022 0 01-1.325-.027l-.009-.008a1.19 1.19 0 01-.073-.073l-.007-.009-3.404-3.403-.737-.738a1.855 1.855 0 00-2.627 0 1.852 1.852 0 00-.042 2.58l.087.088 6.7 6.7.056.057.019.018c.383.344.962.352 1.351.021l.12-.121 1.84-1.839-.001-.001.535-.534 4.7-4.699.042-.045.046-.042.678-.68.006.005L22.347 3.3l.291-.292a1.852 1.852 0 00-.137-2.466z'/%3E%3C/svg%3E");-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:top;content:"";transform:translateY(-50%)}.dropdown-link.is-alert{color:var(--alert-color)}.dropdown-link.is-alert:hover{background-color:var(--alert-color-tint5);color:var(--alert-color)}.dropdown-link.has-new:before{display:inline-block;margin-right:.25rem;width:var(--new-badge-size);height:var(--new-badge-size);border-radius:50%;background:var(--unread-color);content:""}.dropdown-link .icon{display:inline-block;margin-right:6px;vertical-align:middle;width:20px;height:20px}.dropdown-link:hover{background-color:var(--dropdown-hover-color)}.dropdown-form>:last-child{margin-bottom:0}.dropdown-primary{margin:-1.25rem -1.25rem 0 -1.25rem;padding:1.25rem;border-radius:var(--global-radius) var(--global-radius) 0 0;background:var(--dropdown-accent-bg)}.dropdown-primary:last-child{margin-bottom:-1.25rem;border-radius:var(--global-radius)}.dropdown .button{margin:.5rem 0;width:100%;font-size:var(--dropdown-button-size, .75rem)}.dropdown .button:last-child{margin-bottom:0}.dropdown-actions{margin:0 -1.25rem -1.25rem}.dropdown-section-heading{font-size:.625rem;text-transform:uppercase;opacity:.8}.dropdown-main-heading{margin:.25rem 0;font-size:1.25rem}.dropdown-details{font-size:var(--font-size-small)}.dropdown-action-list{--link-color:var(--text-color);list-style:none;margin:0;padding:0}.dropdown-action-link{display:flex;align-items:center;padding:.625rem 1.25rem;text-decoration:none}.dropdown-action-link .icon{--icon-size:1.25rem;margin-right:.25rem}.dropdown-action-link:hover{background:var(--dropdown-hover-bg,--card-bg-shade)}.dropdown-action-link.is-rp-link{font-weight:var(--global-weight-semibold)}.dropdown .tag-list{margin-top:.5rem}.dropdown .game-label{margin-bottom:.25rem}:root{--icon-color:"currentColor";--icon-size:36px;--icon-pile-icon-size:1.5rem}.icon{max-width:100%;color:var(--icon-color);flex:0 0 auto;width:var(--icon-size);height:var(--icon-size)}.icon.icon-xsmall{--icon-size:16px}.icon.icon-small{--icon-size:24px}.icon.icon-large{--icon-size:80px}.icon[class*=theme-]{--icon-color:var(--theme-color)}.icon-border-circle,.icon-knockout-circle,.icon-knockout-square{width:var(--icon-size);height:var(--icon-size);display:flex;justify-content:center;align-items:center;border-radius:50%}.icon-border-circle .icon,.icon-knockout-circle .icon,.icon-knockout-square .icon{width:calc(var(--icon-size) * .5);height:calc(var(--icon-size) * .5)}.icon-knockout-circle,.icon-knockout-square{--icon-color:var(--theme-text-color, var(--tint));background-color:var(--theme-color,currentColor)}.icon-knockout-square{border-radius:0}.icon-border-circle{--icon-color:var(--theme-color, currentColor);border:4px solid var(--theme-color,currentColor)}.icon-pile{--icon-size:var(--icon-pile-icon-size);display:flex}.icon-pile>*{font-size:var(--icon-pile-icon-size)}.icon-pile>:not(:first-child){margin-left:calc(var(--icon-pile-icon-size) * -.4)}.icon-count{--icon-size:1.875rem;display:flex;justify-content:space-between;margin:0;padding:0;list-style:none}.icon-count-item{display:flex;flex-direction:column;margin:0 5px;text-align:center}.icon-count .emoji,.icon-count .icon{display:block;margin-bottom:.625rem;width:var(--icon-size);height:var(--icon-size);font-size:var(--icon-size)}.icon-link{--icon-size:1.5rem;--icon-color:var(--theme-color, var(--brand-color));display:flex;align-self:flex-start}a.icon-link:hover{--icon-color:var(--theme-color-shade, var(--brand-color-shade))}.center-icon{display:inline-flex;align-items:center}.center-icon .icon{margin-right:.625rem}.time-alert{--icon-size:28px;--icon-color:var(--time-alert-icon-color, var(--text-color));display:flex;align-items:center}.time-alert .icon{margin:0 .5rem 0 0}.time-alert-desc,.time-alert-text{color:var(--text-color-highlight2,var(--text-color));line-height:1}.time-alert-text{font-size:1rem;line-height:1.2;white-space:nowrap}.time-alert-desc{display:block;font-size:.625rem;font-weight:var(--global-weight-semibold);text-transform:uppercase}:root{--layout-option-icon-size:2.125rem}.sort-filter{display:grid;grid-gap:10px;grid-template-columns:100%;grid-template-areas:"secondary" "primary";grid-template-rows:1fr;align-items:center;margin:.625rem 0;padding:0}.sort-filter-primary{grid-area:primary;display:flex;align-items:center;flex-wrap:wrap}.sort-filter-primary .field.sort-by{flex:1 1 100%;justify-content:flex-end;margin-bottom:.625rem}.sort-filter-secondary{grid-area:secondary;display:flex;gap:.5rem}.sort-filter-heading{margin-right:1.25rem;font-size:1.25rem}.sort-filter .page-subheading{margin:0}.sort-filter .number-selected{width:5.3125rem;font-size:.875rem;white-space:nowrap}.sort-filter .field{display:flex;flex:1 1 auto;margin:0;width:100%;max-width:100%}.sort-filter .field.select-all{order:3;flex:0 0 auto;margin-top:1.25rem;margin-right:1.25rem;padding:0 0 0 .4375rem;width:auto;line-height:1.1}.sort-filter .field .has-dropdown{flex:1 1 auto;margin-bottom:0}.sort-filter .field .has-dropdown .button{width:100%}.sort-filter .search-wrap{flex:1 1 auto}.sort-filter label{margin:0}.sort-filter.well{padding:.625rem}.sort-filter .button+*{margin-left:.625rem}@media (min-width:570px){.sort-filter{grid-template-areas:"secondary" "primary"}.sort-filter.auto-collapse{grid-template-areas:"primary secondary";grid-template-columns:1fr 1fr}.sort-filter.extra-pad{padding-top:2.5rem;padding-bottom:.625rem}.sort-filter-primary{grid-area:primary;justify-content:flex-start}.sort-filter-primary>:last-child:not(:only-child){margin:0 0 0 auto}.sort-filter-primary>:last-child:not(:only-child).filter-button{font-weight:var(--global-weight-semibold);margin-bottom:-4px}.sort-filter-primary .field.select-all{order:1;margin-top:0}.sort-filter-primary .field.sort-by{order:3;flex:1 1 auto;margin:0 0 0 1.875rem}.sort-filter-primary .field.sort-by .has-dropdown{flex:0 0 auto}.sort-filter-primary .field.select-action{order:2}.sort-filter-secondary{grid-area:secondary;display:flex;justify-content:flex-end;align-items:center;margin-bottom:0}.sort-filter .search-wrap{width:100%;min-width:170px}.sort-filter .field{flex:0 0 auto;width:auto}.sort-filter .field .has-dropdown .button{width:auto}.sort-filter .push-right{margin-left:auto}}@media (min-width:1200px){.sort-filter{grid-template-columns:-webkit-max-content;grid-template-columns:max-content;grid-template-areas:"primary secondary";grid-gap:0 10px}.sort-filter .search-wrap{max-width:350px}.sort-filter .search-wrap:last-child{margin-right:0}}.sort-filter.add-row{display:flex;flex-direction:row;justify-content:flex-start;align-items:flex-start;flex-wrap:wrap;grid-gap:0}.sort-filter.add-row .button{margin:0 0 .625rem auto}.sort-filter.add-row .toggle-expandables{order:2}@media (min-width:570px){.sort-filter.add-row{align-items:center}.sort-filter.add-row .sort-filter-heading{order:1}.sort-filter.add-row .button{order:3;margin:0 0 0 auto}.sort-filter.add-row .field{order:2;width:auto}}.game-stage-list{display:flex;list-style:none;margin:1rem 0;padding:0;background:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 509 43' preserveAspectRatio='none'%3E%3Cpath d='M.582 4.083C-.18 2.117 1.27 0 3.379 0h493.774c1.17 0 2.233.68 2.723 1.742l8.543 18.5a2.996 2.996 0 0 1 0 2.516l-8.543 18.5A2.998 2.998 0 0 1 497.153 43H3.379C1.271 43-.18 40.882.582 38.916l6.325-16.333a3 3 0 0 0 0-2.166L.582 4.082Z' fill='%23fff'/%3E%3C/svg%3E");background-size:100% 100%;filter:drop-shadow(0 1px 2px rgba(0, 0, 0, .15))}.game-stage-item{flex:1 1 100%}.game-stage-link{display:flex;gap:8px;justify-content:center;align-items:center;padding:.75rem 1.25rem;width:100%;height:100%;color:var(--text-color);font-size:1rem;white-space:nowrap;font-weight:var(--global-weight-semibold);text-decoration:none;line-height:1.2}.game-stage-link.is-this-step{margin:-4px 0;height:calc(100% + 8px);color:var(--tint);background-image:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' preserveAspectRatio='none' viewBox='0 0 8 43'%3E%3Cpath d='M3.5 0A3.5 3.5 0 0 0 .232 4.753l5.803 15.136a4.5 4.5 0 0 1 0 3.222L.232 38.247A3.5 3.5 0 0 0 3.5 43h3.738V0H3.5Z' fill='%2300D86B'/%3E%3C/svg%3E"),url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' preserveAspectRatio='none' viewBox='0 0 16 11'%3E%3Cpath fill='%2300D86B' d='M0 0h16v11H0z'/%3E%3C/svg%3E"),url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' preserveAspectRatio='none' viewBox='0 0 12 43'%3E%3Cpath d='m11.467 20.045-8.228-18A3.494 3.494 0 0 0 .238.013v42.974a3.494 3.494 0 0 0 3-2.032l8.23-18a3.5 3.5 0 0 0 0-2.91Z' fill='%2300D86B'/%3E%3C/svg%3E");background-size:8px 100%,calc(100% - 18px) 100%,12px 100%;background-position:top left,top left 7px,top right;background-repeat:no-repeat,no-repeat,no-repeat;filter:drop-shadow(0 1px 2px rgba(0, 0, 0, .15))}:root{--modal-width:37.5rem;--modal-max-height:100vh;--modal-border-width:1px;--modal-border-color:var(--theme-color, var(--card-border-color-default));--modal-border-radius:var(--global-radius);--modal-header-border-radius:var(--modal-border-radius) var(--modal-border-radius) 0 0;--modal-footer-border-radius:0 var(--global-radius) var(--global-radius) 0;--modal-bg-opacity:0.4;--footer-height:5rem}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:8;display:block;margin:auto;padding:0;width:100%;max-width:var(--modal-width);height:100%;max-height:var(--modal-max-height);border:0 none;border-radius:0;background:var(--modal-bg);color:var(--text-color)}.modal::-webkit-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;background:rgba(43,102,178,.4)}.modal::backdrop{position:fixed;top:0;right:0;bottom:0;left:0;background:rgba(43,102,178,.4)}.modal+.backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:7;background:var(--theme-color,var(--brand-color));opacity:var(--modal-bg-opacity)}.modal:not([open]){display:none}.modal .scroll-wrap{padding:2.5rem 3.125rem;height:100%;max-height:calc(var(--modal-max-height) - (var(--modal-border-width) * 2));overflow:auto;-webkit-overflow-scrolling:touch;scrollbar-width:thin}.modal .close-button{position:fixed;top:1.125rem;right:1.125rem;z-index:8}.modal .modal-heading{justify-content:center;margin-bottom:2rem;font-size:1.5rem;color:var(--primary-heading-color)}.modal .button-wrap{padding-bottom:0}.modal .has-edit-icon{position:relative}.modal .has-edit-icon .icon-button{position:absolute;right:0;bottom:0;z-index:2}.modal .has-edit-icon:hover .icon-button{--icon-color:var(--knockout-color);background-color:var(--success-color)}.modal.small .modal-heading{font-size:1.125rem}.modal table{--avatar-size:2.5rem}.modal-header{display:flex;justify-content:center;flex-wrap:wrap;margin:-2.5rem -2.5rem 1.25rem -2.5rem;padding-top:3.75rem;padding-bottom:1.25rem;background:var(--modal-header-bg)}.modal-header .help-text{width:100%;text-align:center}.modal-header .field{margin-bottom:0}.modal .page-heading,.modal-heading{--icon-size:1.25rem;font-family:var(--modal-heading-font-family, var(--global-font-family));display:flex;align-items:center}.modal .page-heading .icon,.modal-heading .icon{margin-right:8px}.modal-header-small{display:flex;justify-content:space-between;align-items:flex-end;padding:0 0 var(--global-margin) 0}.modal-header-small .page-heading,.modal-header-small .page-subheading,.modal-header-small .page-subheading-2{margin:0}.modal-header-small .icon-wrap{margin-right:.625rem}.modal-header-small .time-alert{margin-left:auto}.modal-header-small.stack-content{flex-direction:column;align-items:flex-start;padding-bottom:0}.modal .scroll-wrap,.modal-footer,.modal-header{padding-right:2.5rem;padding-left:1.25rem}.modal .page-subheading{margin:1em 0 0 0;font-size:1.375rem}@media (min-width:570px){.modal{--modal-max-height:94vh;top:50%;bottom:auto;height:-moz-fit-content;height:-webkit-fit-content;height:fit-content;border:var(--modal-border-width) solid var(--modal-border-color);border-radius:var(--modal-border-radius);transform:translateY(-50%)}.modal .scroll-wrap{height:auto}.modal-header{border-radius:var(--modal-header-border-radius)}.modal-footer{border-radius:var(--modal-footer-border-radius)}}@media (min-width:768px){.modal .scroll-wrap,.modal-footer,.modal-header{padding-left:2.5rem}.modal .page-heading,.modal-heading{--icon-size:2rem}.modal.large{--modal-width:56.25rem}.modal.large-pad .scroll-wrap{padding:3.75rem}.modal.small{--modal-width:25rem}.modal.player-profile{--avatar-size:8.75rem}}.note{--icon-color:var(--theme-color, var(--text-color));--icon-size:1.625rem;display:flex;align-items:center;margin-bottom:.625rem;padding:.625rem;border:1px solid var(--theme-color,var(--note-default-border-color,var(--card-border-color-default)));border-radius:var(--global-radius);background:var(--theme-color-alpha,var(--theme-color-tint5,var(--note-default-bg-color,var(--card-bg))));font-size:var(--font-size-small);color:var(--note-default-color,var(--text-color))}.note-content>:last-child{margin-bottom:0}.note .icon,.note .icon-wrap{margin-right:.625rem}.note .icon-wrap .icon{margin-right:0}.note .close-button .icon{margin:0}.note .note-content{align-self:center;margin-right:10px}.note .action-callout{margin-left:.625rem}.note .button{--icon-color:currentColor;margin-left:auto;min-width:104px}.note a:not(.button){color:var(--note-default-color,var(--text-color))}.note.knockout{--icon-color:var(--theme-text-color, var(--knockout-color));background:var(--theme-color,var(--brand-color));color:var(--theme-text-color,var(--knockout-color))}.note.knockout a:not(.button){color:var(--theme-text-color,var(--knockout-color))}.note.knockout,.note.knockout li,.note.knockout p{color:var(--theme-text-color,var(--knockout-color))}.note.has-close-button{padding-right:1.875rem}.note.is-flex .note-content{display:flex;justify-content:space-between;align-items:center;width:100%;gap:1rem;margin-right:0}.note.is-flex .note-content>*{margin:0}.note.is-flex .note-content .action-link{flex:1 1 auto}.note.is-feature{font-size:1.25rem}.note.is-feature p{margin-bottom:.5em}.note.is-feature .feature-details{font-size:var(--font-size-small)}.note.has-large-icon{--icon-size:2.625rem;padding:1rem}.note.has-large-icon .button{white-space:nowrap}.note.border-theme{border:1px solid var(--card-border-color-default);border-left:4px solid var(--theme-color,var(--note-default-border-color,var(--card-border-color-default)));background:var(--card-bg)}.note.is-thin{padding:.125rem .625rem}.note.is-sticky{position:sticky;top:0;z-index:2}.note.is-sticky.is-at-bottom{top:auto;bottom:0}.note+.note{margin-bottom:.625rem}.note-heading{font-size:1rem}.note.button-and-time .note-content{display:grid;grid-template-columns:1fr minmax(5rem,-webkit-min-content);grid-template-columns:1fr minmax(5rem,min-content);grid-template-areas:"text text" "time button";width:100%}.note.button-and-time .note-text{grid-area:text}.note.button-and-time .feature-details{grid-area:time}.note.button-and-time .button-wrap{grid-area:button}.note.button-and-time .button{white-space:nowrap}@media (min-width:570px){.note.button-and-time .note-content{grid-template-areas:"text button" "time button"}}[data-notification-badge]{position:relative}[data-notification-badge]:after{position:absolute;top:0;right:0;padding:3px 5px;min-width:var(--notification-badge-high-priority-min-width,10px);height:12px;border-radius:var(--badge-border-radius,12px);background:var(--badge-color,var(--unread-color));font-family:var(--global-font-family);font-weight:var(--badge-font-weight,normal);font-size:.75rem;line-height:12px;text-align:center;color:var(--badge-text-color,var(--knockout-color));content:attr(data-notification-badge);transform:translate(20%,-20%);letter-spacing:0}[data-notification-badge].site-toggle:after{top:10px}.site-header.nav-open [data-notification-badge].site-toggle:after{content:none}[data-notification-badge="*"]:after,[data-notification-badge=high-priority]:after{padding:var(--notification-badge-high-priority-padding,0);min-width:var(--notification-badge-high-priority-min-width,6px);height:var(--notification-badge-high-priority-height,6px);border:var(--notification-badge-high-priority-border,6px solid var(--badge-color,var(--unread-color)));font-size:var(--notification-badge-high-priority-font-size, 1.25rem);line-height:var(--notification-badge-high-priority-line-height, 12px);background:var(--badge-color,var(--knockout-color));content:var(--notification-badge-high-priority-content, "")}[data-notification-badge=""]:after{content:none}.site-header [data-notification-badge]:after{content:var(--notification-badge-high-priority-content, " ");border:0 none;padding:var(--notification-badge-high-priority-padding,0);height:var(--notification-badge-high-priority-height,6px);width:var(--notification-badge-high-priority-height,6px);min-width:var(--notification-badge-high-priority-height,6px);line-height:var(--notification-badge-high-priority-line-height, 12px);font-size:var(--notification-badge-high-priority-font-size, 1.25rem);border:var(--notification-badge-high-priority-border,6px solid var(--badge-color,var(--unread-color)));background:var(--notification-badge-high-priority-bg,var(--knockout-color))}@-webkit-keyframes pulse-white{0%{box-shadow:0 0 0 0 rgba(255,255,255,.4)}70%{box-shadow:0 0 0 12px rgba(255,255,255,0)}100%{box-shadow:0 0 0 0 rgba(255,255,255,0)}}@keyframes pulse-white{0%{box-shadow:0 0 0 0 rgba(255,255,255,.4)}70%{box-shadow:0 0 0 12px rgba(255,255,255,0)}100%{box-shadow:0 0 0 0 rgba(255,255,255,0)}}@-webkit-keyframes pulse-info-color{0%{box-shadow:0 0 0 0 rgba(43,102,178,.4)}70%{box-shadow:0 0 0 12px rgba(43,102,178,0)}100%{box-shadow:0 0 0 0 rgba(43,102,178,0)}}@keyframes pulse-info-color{0%{box-shadow:0 0 0 0 rgba(43,102,178,.4)}70%{box-shadow:0 0 0 12px rgba(43,102,178,0)}100%{box-shadow:0 0 0 0 rgba(43,102,178,0)}}[data-notification-badge=high-priority]:after{box-shadow:0 0 0 0 rgba(43,102,178,.4);-webkit-animation:pulse-info-color 2s infinite;animation:pulse-info-color 2s infinite}.site-header [data-notification-badge=high-priority]:after{box-shadow:0 0 0 0 rgba(255,255,255,.4);-webkit-animation:pulse-white 2s infinite;animation:pulse-white 2s infinite}:root{--team-heading-w:230px;--header-label-w:60px;--period-w:42px;--period-h:50px}.progress-grid{width:calc(100% + 20px);overflow:auto}@media (min-width:980px){.progress-grid{width:auto;max-width:100%}}.pg-header{display:flex;padding-left:var(--team-heading-w);font-size:.75rem}.pg-header-label{flex:0 0 auto;width:var(--header-label-w);text-transform:uppercase}.pg-period{flex:0 0 auto;text-align:center;width:var(--period-w)}.pg-team{display:flex;align-items:center;margin-bottom:.5rem}.pg-team-heading{flex:0 0 auto;font-size:1rem;width:var(--team-heading-w);padding-right:.5rem;background:var(--body-bg-color)}.pg-team-progress-list{display:flex;list-style:none;margin:0;padding:0 0 0 var(--header-label-w);background:var(--tint)}.pg-team-progress-item{width:var(--period-w);height:var(--period-h);position:relative;display:flex;align-items:center;justify-content:center}.pg-team-progress-item:after{width:12px;height:12px;border-radius:50%;background-color:var(--info-color);opacity:.1;content:""}.pg-team-progress-item.task-timeout svg{fill:var(--text-color)}.pg-team-progress-item.task-timeout:after{content:none}.pg-team-progress-item.is-complete:after{opacity:1;width:16px;height:16px}.pg-team-progress-item.is-current{background:var(--info-color-tint5);border-bottom:2px solid var(--info-color)}.pg-team-progress-item.is-current:after{opacity:1;width:16px;height:16px}.pg-team-progress-item.is-current:before{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);opacity:1;width:10px;height:10px;border-radius:50%;border:2px solid var(--tint);background:var(--info-color);content:""}.pg-team-progress-item.task-bad:after,.pg-team-progress-item.task-done_fail:after,.pg-team-progress-item.task-done_well:after,.pg-team-progress-item.task-good:after{opacity:1;width:16px;height:16px;background:var(--info-color);content:"+";line-height:14px;color:var(--tint);font-weight:var(--global-weight-semibold)}.pg-team-progress-item.task-done_fail:after{content:"-"}.pg-team-progress-item.task-good:after{background:var(--success-color)}.pg-team-progress-item.task-bad:after{background:var(--alert-color-tint1)}.pg-team-count{font-size:.875rem;font-weight:400;margin:4px 0 0 0;display:block}.table-scroll.is-progress{max-width:calc(100vw - 2.5rem)}@media (min-width:980px){.table-scroll.is-progress{max-width:100%}}.progress-filters{--tab-wrap-border:0 none;--tab-margin:0;--tab-item-padding:0;display:flex;flex-direction:column-reverse;align-items:flex-start;gap:1rem;border-bottom:2px solid var(--info-color);margin-bottom:2rem}@media (min-width:980px){.progress-filters{--tab-item-padding:0 1.25rem 0 0;flex-direction:row;justify-content:space-between;align-items:flex-end}}.progress-epic-table-wrap{max-width:100%;width:calc(100vw - 1.25rem);max-height:calc(100vh - 293px);overflow:auto;background:var(--body-bg-color);border:1px solid var(--card-border-color-default);border-radius:var(--global-radius)}.progress-epic-table{border-spacing:6px 0;width:auto;font-size:1em;margin:0;border-collapse:inherit;table-layout:fixed}.progress-epic-table thead th{padding:1rem 0 .5rem 0;background:var(--body-bg-color);position:sticky;top:0;z-index:1}.progress-epic-table thead th:first-child{position:sticky;left:0;z-index:2}.progress-epic-table tbody th{position:sticky;left:0;z-index:1}.progress-epic-table td{padding:0}.progress-epic-table tbody table,.progress-epic-table tbody>tr{height:48px;margin-bottom:6px}.progress-epic-table tbody table{background:#fff}.progress-epic-table tr table tr{height:100%}.progress-epic-table tr table{border-spacing:0}.progress-epic-table tr table td{min-width:30px;text-align:center;padding:0 3px}.epic-label{background:#fff;padding:.25em .5em}.progress-key{--period-w:28px;--period-h:28px;display:flex;align-items:center;gap:1rem;margin:0 0 .5rem 0;padding:0;list-style:none}.progress-key-wrap{display:flex;align-items:center}.progress-key-title{font-size:var(--font-size-base);margin-right:2rem}.progress-key-item{display:flex;flex-direction:column;align-items:center;gap:6px}.task-label{font-size:.75rem}.progress-loader{position:absolute;right:0;background:var(--text-color-subdued);color:#fff;letter-spacing:1px;font-size:.7em;padding:.2em .7em;margin:0 1.25rem 0 0;border-radius:.3em}.progress-loader.listening{background:var(--success-color);opacity:0}.progress-loader.disconnected{background:var(--alert-color)}@media (min-width:980px){.progress-loader{margin-right:2.5rem}}.search-wrap{position:relative}.search-wrap input:not([type=submit]):not([type=checkbox]):not([type=radio]).search-input{padding-right:30px}.search-wrap input:not([type=submit]):not([type=checkbox]):not([type=radio]).search-input::-webkit-search-cancel-button{position:relative;right:10px}.search-wrap input:not([type=submit]):not([type=checkbox]):not([type=radio]).search-input::-moz-placeholder{font-family:var(--search-placeholder-font-family, var(--global-font-family));letter-spacing:var(--search-placeholder-letter-spacing, normal)}.search-wrap input:not([type=submit]):not([type=checkbox]):not([type=radio]).search-input:-ms-input-placeholder{font-family:var(--search-placeholder-font-family, var(--global-font-family));letter-spacing:var(--search-placeholder-letter-spacing, normal)}.search-wrap input:not([type=submit]):not([type=checkbox]):not([type=radio]).search-input::placeholder{font-family:var(--search-placeholder-font-family, var(--global-font-family));letter-spacing:var(--search-placeholder-letter-spacing, normal)}.search-wrap.w-400{width:400px;max-width:100%}.search-wrap .search-button{width:24px;height:24px;-webkit-appearance:none;-moz-appearance:none;appearance:none;position:absolute;top:8px;right:8px;margin:0;padding:0;border:none;background:0 0;color:var(--text-color)}.search-wrap .search-button .icon{width:24px;height:24px}.search-wrap .search-button:not(:disabled):hover{color:var(--brand-color-tint1)}.search-wrap .search-button:focus{box-shadow:var(--focus-shadow);outline:0}.site-header.is-simpl{display:flex;align-items:center;gap:1rem;padding-right:1rem;padding-left:1rem;min-height:var(--site-nav-height)}.site-header.is-simpl p{margin:0}.site-header.is-simpl .wharton-shield-icon{width:28px}.site-header.is-simpl .nav-items{flex:1 1 auto}.site-header.is-simpl.nav-open{display:grid}.site-header.is-simpl.nav-open .simpl-header-title-wrap{display:none}.site-header.is-simpl.nav-open .simpl-header-link{margin-top:40px;font-size:1.25rem}.simpl-header-title{font-weight:var(--global-weight-semibold);margin:0}.simpl-header-title .mode-flag{font-style:italic;background:rgba(255,255,255,.15);border-radius:3px;padding:0 6px}.simpl-header-subtitle{font-size:.75rem}.simpl-header-title-wrap{display:flex;align-items:center;gap:8px}.simpl-header-info{font-size:.75rem}.simpl-header-link{text-decoration:none;color:var(--site-nav-link-color);font-size:.75rem;display:block;white-space:nowrap}.simpl-subheader{background:var(--body-bg-shade);padding:.625rem;font-size:var(--font-size-small);display:flex;justify-content:space-between;align-items:center;gap:1rem}.simpl-subheader p{margin:0}.simpl-subheader-back.button.small{font-weight:var(--global-weight-semibold);font-size:.875rem;min-height:1.75rem;text-decoration:none;margin:-6px 0;padding:0 16px 0 10px}.simpl-subheader-status{font-size:var(--font-size-base);font-weight:var(--global-weight-semibold);margin:-4px 0;padding:2px 20px;height:calc(100% + 8px);color:var(--tint);background-image:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' preserveAspectRatio='none' viewBox='0 0 8 43'%3E%3Cpath d='M3.5 0A3.5 3.5 0 0 0 .232 4.753l5.803 15.136a4.5 4.5 0 0 1 0 3.222L.232 38.247A3.5 3.5 0 0 0 3.5 43h3.738V0H3.5Z' fill='%2300D86B'/%3E%3C/svg%3E"),url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' preserveAspectRatio='none' viewBox='0 0 16 11'%3E%3Cpath fill='%2300D86B' d='M0 0h16v11H0z'/%3E%3C/svg%3E"),url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' preserveAspectRatio='none' viewBox='0 0 12 43'%3E%3Cpath d='m11.467 20.045-8.228-18A3.494 3.494 0 0 0 .238.013v42.974a3.494 3.494 0 0 0 3-2.032l8.23-18a3.5 3.5 0 0 0 0-2.91Z' fill='%2300D86B'/%3E%3C/svg%3E");background-size:8px 100%,calc(100% - 18px) 100%,12px 100%;background-position:top left,top left 7px,top right;background-repeat:no-repeat,no-repeat,no-repeat;filter:drop-shadow(0 1px 2px rgba(0, 0, 0, .15))}@media (min-width:980px){.site-header.is-simpl{gap:2rem}.simpl-header.has-todos{padding-right:calc(var(--todo-aside-width) + 20px)}.simpl-header-subtitle{font-size:1rem}.simpl-header-info{font-size:var(--font-size-small)}.simpl-header-link{font-size:var(--font-size-small);display:inline}.simpl-header-mini-nav .simpl-header-link+.simpl-header-link:before{display:inline-flex;padding:0 8px 0 4px;opacity:.7;content:"/"}.simpl-subheader{padding:.625rem 1.25rem}}.has-fixed-nav{padding-top:var(--site-nav-height)}.has-fixed-nav .site-header.is-fixed{position:fixed;top:0;right:0;left:0;z-index:5}.has-fixed-nav .site-header.is-fixed.nav-open{z-index:7}.site-header{--link-color:var(--site-nav-link-color);--avatar-font-size:0.6875rem;display:grid;grid-gap:var(--site-header-gap,0 4px);grid-template-columns:3.75rem 1fr auto;grid-template-rows:var(--site-nav-height);grid-template-areas:"toggle title profile";align-items:center;background-color:var(--site-nav-background);background-image:var(--site-nav-bg-image,none);background-size:var(--site-nav-bg-size,auto);background-repeat:var(--site-nav-bg-repeat,no-repeat);background-position:var(--site-nav-bg-position,top left);position:relative;border-bottom:var(--site-nav-border-bottom,none);box-shadow:var(--site-nav-box-shadow,none);-webkit-mask-image:var(--site-nav-mask-image,none);mask-image:var(--site-nav-mask-image,none);-webkit-mask-size:var(--site-nav-mask-size,100% 100%);mask-size:var(--site-nav-mask-size,100% 100%);-webkit-mask-repeat:var(--site-nav-mask-repeat,no-repeat);mask-repeat:var(--site-nav-mask-repeat,no-repeat)}.site-header:after{position:absolute;height:100%;width:100%;top:0;left:0;background:var(--site-header-bg,none transparent);background-size:var(--site-header-bg-size,auto);filter:var(--site-header-bg-filter, none);z-index:1;content:var(--site-header-after-content,unset)}.header-dropdown-is-open .site-header{-webkit-mask-image:none;mask-image:none}.site-header>*{z-index:2}.site-header>.profile{z-index:3}.site-header-title{font-weight:var(--global-weight-semibold);text-align:center;text-overflow:ellipsis;white-space:nowrap;color:var(--site-nav-link-color);overflow:hidden;grid-area:title}.thin .site-header-title{color:var(--site-nav-thin-text-color,var(--site-nav-link-color))}.site-header.force-toggle-nav{grid-template-columns:3.75rem auto;grid-template-areas:"toggle title"}.site-header.force-toggle-nav .site-logo{justify-self:start;padding:0}.site-header.force-toggle-nav.nav-open .site-logo{grid-column-end:span 2}.site-header.nav-open{background:var(--site-header-mobile-is-open-bg-color,var(--site-nav-background))}.site-header.nav-open:after{content:none}.site-header.nav-open .secondary-nav{margin-left:var(--site-header-mobile-secondary-margin-left,0)}.site-header .avatar-label{display:var(--site-header-avatar-label-display,block)}.site-header .button:not(.icon-button):not(.site-back) .icon{display:var(--site-header-icons-display,block)}.site-toggle{position:relative;padding:.75rem;height:var(--site-nav-height);border:none;font:0/0 a;line-height:1rem;color:transparent;cursor:pointer}.site-toggle:before{position:absolute;top:50%;left:50%;width:1rem;height:1rem;background-color:var(--site-toggle-color,var(--site-nav-link-color));-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 613 478.29' fill='currentColor' id='hamburger' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1 0h612v70.64H1V0zm0 407.65h612v70.64H1v-70.64zM0 203h612v70.64H0V203z'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 613 478.29' fill='currentColor' id='hamburger' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1 0h612v70.64H1V0zm0 407.65h612v70.64H1v-70.64zM0 203h612v70.64H0V203z'/%3E%3C/svg%3E");-webkit-mask-position:center center;mask-position:center center;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;content:"";transform:translate(-50%,-50%)}.site-logo{display:none;align-items:center;align-self:center;line-height:1;text-decoration:none;justify-self:center}.site-logo,.site-logo:hover{color:var(--site-nav-logo-color)}.site-logo img{width:100%}.main-nav-list{display:flex;justify-content:space-around;align-items:center;margin:0;padding:0;color:var(--site-nav-link-color);list-style:none;background-color:var(--site-nav-list-bg-color,transparent)}.main-nav-link{position:relative;display:var(--site-header-link-display,inline-flex);flex-direction:var(--site-nav-link-flex-direction,row);align-items:center;border-radius:var(--site-nav-link-radius,var(--global-radius));font-family:var(--alt-font-family, var(--global-font-family));font-size:var(--site-nav-font-size, .8125rem);font-weight:var(--site-nav-font-weight,var(--global-weight-normal));text-decoration:none;text-transform:var(--site-nav-text-transform,uppercase);letter-spacing:var(--site-nav-letter-spacing, .1rem);background-image:var(--site-nav-text-bg-image,none);will-change:color;transition:color .25s ease-out}.main-nav-link:not(:disabled):hover{background-color:var(--site-nav-link-hover-bg-color);color:var(--site-nav-link-color-hover,var(--site-nav-link-color))}.main-nav-link[aria-current=page],.main-nav-link[aria-current=page]:not(:disabled):hover{background-color:var(--site-nav-link-current-bg);color:var(--site-nav-link-current-color);border:var(--site-nav-border-current,0 none);border-width:var(--site-nav-border-current-width,0);border-color:var(--site-nav-border-current-color,transparent)}.main-nav-link .icon{width:20px;height:20px;flex:0 0 auto;min-width:20px}.main-nav-link .icon+*{margin-left:.375rem}.profile{display:flex;grid-area:profile;justify-content:flex-end;align-items:center;padding-right:1.25rem;padding-left:.375rem;height:var(--site-nav-height)}.profile-img-link{width:40px;height:40px;display:block;border-radius:50%}.profile-img-link img{display:block;border-radius:50%}.profile .avatar-label{display:none}.profile .avatar-group .avatar{box-shadow:var(--site-nav-avatar-box-shadow,0 0 0 2px var(--site-nav-background))}.profile .avatar-link:hover .avatar{box-shadow:var(--site-nav-avatar-box-shadow-hover,0 0 0 2px var(--site-nav-link-hover-color))}.main-nav-link{background-image:var(--site-nav-text-bg-image,none);-webkit-text-fill-color:var(--site-nav-text-fill-color,unset)}.main-nav-link:not(:disabled):hover{background-image:var(--site-nav-text-bg-image-hover,none);-webkit-text-fill-color:var(--site-nav-text-fill-color,unset)}.main-nav-link[data-notification-badge]::after{-webkit-text-fill-color:var(--site-header-mobile-is-open-bg-color,unset);transform:var(--site-nav-notification-badge-transform,translate(20%,-20%))}.main-nav-link[aria-current=page]:before{position:var(--site-nav-active-pip-position,static);left:var(--site-nav-active-pip-left,unset);bottom:var(--site-nav-active-pip-bottom,unset);width:var(--site-nav-active-pip-width,unset);height:var(--site-nav-active-pip-height,unset);background-image:var(--site-nav-active-pip-img,none);transform:var(--site-nav-active-pip-before-transform-sm,none);content:var(--site-nav-active-pip-before-content,unset)}.main-nav-link.Dashboard:before,.main-nav-link.Files:before,.main-nav-link.Inbox:before,.main-nav-link.Insights:before,.main-nav-link.Meetings:before{width:var(--site-nav-icon-size,1.5rem);height:var(--site-nav-icon-size,1.5rem);background-color:var(--brand-color);-webkit-mask-image:var(--site-nav-link-icon-inbox,none);mask-image:var(--site-nav-link-icon-inbox,none);-webkit-mask-size:100% 100%;mask-size:100% 100%;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;content:var(--site-nav-link-icon-content,none)}.main-nav-link.Dashboard:before{-webkit-mask-image:var(--site-nav-link-icon-dashboard,none);mask-image:var(--site-nav-link-icon-dashboard,none)}.main-nav-link.Meetings:before{-webkit-mask-image:var(--site-nav-link-icon-meetings,none);mask-image:var(--site-nav-link-icon-meetings,none)}.main-nav-link.Files:before,.main-nav-link.Insights:before{-webkit-mask-image:var(--site-nav-link-icon-files,none);mask-image:var(--site-nav-link-icon-files,none)}.profile,.secondary-nav{border:var(--secondary-nav-border,none);border-width:var(--secondary-nav-border-width,0);box-shadow:var(--secondary-nav-border-width-shadow,none)}.secondary-nav{display:flex;align-items:center}.secondary-nav .button{position:relative;border:var(--site-nav-button-border,1px solid rgba(255,255,255,.2));border-bottom-width:var(--button-border-bottom-width,1px);background-color:transparent;color:var(--site-nav-link-color);font-size:var(--site-nav-font-size, .8125rem);font-family:var(--alt-font-family, var(--global-font-family));text-transform:var(--site-nav-button-text-transform,none);font-weight:var(--site-nav-button-font-weight,inherit);line-height:var(--site-nav-button-line-height, inherit);text-shadow:none}.secondary-nav .button:not(:disabled):focus,.secondary-nav .button:not(:disabled):hover{background-color:var(--site-nav-link-hover-bg-color);color:var(--site-nav-link-color-hover,var(--site-nav-link-color));border:var(--site-nav-button-border,1px solid rgba(255,255,255,.3));border-bottom-width:var(--button-border-bottom-width,1px)}.secondary-nav .button[aria-current=page],.secondary-nav .button[aria-current=page]:not(:disabled):focus,.secondary-nav .button[aria-current=page]:not(:disabled):hover{border-color:transparent;background-color:var(--site-nav-link-current-bg);color:var(--site-nav-link-current-color)}.nav-items{display:none}.site-header.nav-open{position:fixed;top:0;right:0;left:0;z-index:7;height:100vh;display:grid;grid-template-rows:var(--site-nav-height) 1fr;grid-template-columns:3.75rem -webkit-min-content 1fr auto;grid-template-columns:3.75rem min-content 1fr auto;grid-template-areas:"toggle logo .. profile" "...    menu menu menu";overflow:auto;-webkit-overflow-scrolling:touch;-webkit-mask-image:none;mask-image:none}.site-header.nav-open .site-header-title{display:none}.site-header.nav-open .site-logo{display:flex;white-space:nowrap}.site-header.nav-open .nav-items{grid-area:menu;display:block;margin:0 0 calc(var(--site-nav-height) * 2);text-align:left}.site-header.nav-open .main-nav-list{display:flex;flex-direction:column;justify-content:flex-start;align-items:flex-start;margin-left:-1.25rem;padding:1rem 0;width:100%}.site-header.nav-open .button,.site-header.nav-open .main-nav-link{display:inline-flex;justify-content:flex-start;margin:.25rem 0;padding:.625rem 1.15rem;width:auto;font-size:1.25rem;font-weight:var(--global-weight-normal);text-transform:none;letter-spacing:0}.site-header.nav-open .button.Dashboard:before,.site-header.nav-open .button.Files:before,.site-header.nav-open .button.Inbox:before,.site-header.nav-open .button.Insights:before,.site-header.nav-open .button.Meetings:before,.site-header.nav-open .main-nav-link.Dashboard:before,.site-header.nav-open .main-nav-link.Files:before,.site-header.nav-open .main-nav-link.Inbox:before,.site-header.nav-open .main-nav-link.Insights:before,.site-header.nav-open .main-nav-link.Meetings:before{content:none}.site-header.nav-open .profile,.site-header.nav-open .secondary-nav{box-shadow:none;border:0 none}.site-header.nav-open .secondary-nav{flex-direction:column;align-items:flex-start}.site-header.nav-open .site-toggle{padding-left:1.25rem;grid-area:toggle}.site-header.nav-open .site-toggle:before{background-color:var(--site-toggle-close-color,var(--site-toggle-color,var(--site-nav-link-color)));-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 16.59 16.59' id='close' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M11.38 7.75L16 3.14a1.86 1.86 0 00.25-2.38 1.79 1.79 0 00-2.74-.23L8.83 5.2a.76.76 0 01-1.08 0L3.14.6A1.86 1.86 0 00.76.33a1.79 1.79 0 00-.23 2.74L5.2 7.75a.76.76 0 010 1.08L.6 13.44a1.88 1.88 0 00-.27 2.39 1.81 1.81 0 002.74.23l4.68-4.68a.76.76 0 011.08 0L13.44 16a1.87 1.87 0 002.39.26 1.81 1.81 0 00.23-2.74l-4.68-4.69a.76.76 0 010-1.08z'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 16.59 16.59' id='close' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='currentColor' d='M11.38 7.75L16 3.14a1.86 1.86 0 00.25-2.38 1.79 1.79 0 00-2.74-.23L8.83 5.2a.76.76 0 01-1.08 0L3.14.6A1.86 1.86 0 00.76.33a1.79 1.79 0 00-.23 2.74L5.2 7.75a.76.76 0 010 1.08L.6 13.44a1.88 1.88 0 00-.27 2.39 1.81 1.81 0 002.74.23l4.68-4.68a.76.76 0 011.08 0L13.44 16a1.87 1.87 0 002.39.26 1.81 1.81 0 00.23-2.74l-4.68-4.69a.76.76 0 010-1.08z'/%3E%3C/svg%3E")}@media (min-width:980px){.site-header{padding:0;padding-bottom:var(--site-header-padding-bottom-lg,0);grid-template-columns:var(--site-header-grid-cols-lg,10rem 1fr auto);grid-template-areas:"logo nav-items profile";align-items:var(--site-header-align-items-lg,center)}.site-header-title{display:none}.site-header.nav-open{overflow:visible}.site-header:not(.nav-open):not(.force-toggle-nav) .site-toggle{display:none}.site-header.force-toggle-nav:not(.nav-open) .nav-items{display:none}.has-fixed-subnav .site-header{grid-template-rows:var(--site-nav-height) var(--subnav-height);grid-template-areas:"logo nav-items profile" "subnav subnav subnav";background-color:var(--site-header-has-fixed-subnav-bg,var(--site-nav-background));padding-bottom:var(--subnav-bg-padding-bottom)}.has-fixed-subnav .site-header:after{background-position:bottom 60px center}.main-nav{margin:var(--main-nav-margin-lg,0)}.main-nav-list li+li{margin-left:var(--site-nav-li-margin-left-lg,.5rem)}.main-nav-link,.secondary-nav .button{font-size:var(--site-nav-font-size-lg, var(--site-nav-font-size, .8125rem));white-space:nowrap}.main-nav-link[data-notification-badge]::after,.secondary-nav .button[data-notification-badge]::after{top:var(--site-nav-notification-badge-top-lg,0);right:var(--site-nav-notification-badge-right-lg,0);transform:var(--site-nav-notification-badge-transform-lg,translate(20%,-20%))}.main-nav-link[aria-current=page]:before,.secondary-nav .button[aria-current=page]:before{left:var(--site-nav-active-pip-before-left-lg,unset);bottom:var(--site-nav-active-pip-before-bottom-lg,unset);right:var(--site-nav-active-pip-before-right-lg,unset);transform:var(--site-nav-active-pip-before-transform-lg,none)}.main-nav-link{padding:var(--site-nav-link-padding-lg,.625rem)}.site-logo{display:flex;align-self:stretch;padding-right:1.25rem;padding-left:1.25rem}.site-logo.has-brand{padding:0;height:var(--site-logo-height,auto);width:var(--site-logo-width,auto);background-image:var(--site-logo-url,none);background-size:var(--site-logo-bg-size-sm,auto);background-position:var(--site-logo-bg-position-sm,auto);background-repeat:no-repeat;transform:var(--site-logo-transform,none)}.site-logo.has-brand img{height:1.625rem;display:var(--site-logo-img-display,block)}}@media (min-width:980px) and (min-width:980px){.site-logo.has-brand{background-position:var(--site-logo-bg-position-lg,auto);background-size:var(--site-logo-bg-size-lg,auto);transform:none}}@media (min-width:980px){.nav-items{grid-area:nav-items;display:flex;justify-content:space-between;align-self:var(--nav-items-align-self,center)}}@media (min-width:980px){.secondary-nav{grid-area:secondary-nav}.secondary-nav .button{margin-left:.625rem}}@media (min-width:980px){.profile .avatar-label{display:var(--site-header-avatar-label-display,block)}}@media (min-width:980px){.site-back-text{display:block;white-space:nowrap;font-size:13px;font-weight:var(--global-weight-semibold);margin-left:.375rem}}@media (min-width:1050px){.site-header{grid-template-columns:var(--site-header-grid-cols-xl,10rem 1fr auto)}.main-nav-link,.secondary-nav .button{font-size:var(--site-nav-font-size-xl, .8125rem)}.main-nav-link{padding:var(--site-nav-link-padding-xl,.625rem)}}@media (min-width:1280px){.site-header{grid-template-columns:var(--site-header-grid-cols-xl,10rem 1fr auto)}.main-nav-link,.secondary-nav .button{font-size:var(--site-nav-font-size-xxl, .8125rem)}.main-nav-link{padding:var(--site-nav-link-padding-xxl,.625rem)}.main-nav-list li+li{margin-left:var(--site-nav-li-margin-left-xxl,.625rem)}}.has-thin-nav{--site-nav-height:var(--site-nav-mobile-nav-thin-height)}.site-header.thin{--site-nav-height:var(--site-nav-mobile-nav-thin-height);grid-template-rows:var(--site-nav-height);grid-template-columns:2.5rem 1fr 3.75rem;grid-template-areas:"back title ..";padding:0;align-items:center;-webkit-mask-image:none;mask-image:none;background-color:var(--site-nav-background-thin,var(--site-nav-background));background-image:var(--site-nav-background-image-thin,none)}.site-header.thin:after{background:0 0}.site-header.thin .secondary-nav,.site-header.thin .site-back{--icon-size:1rem;--icon-color:var(--site-nav-thin-text-color, var(--site-nav-link-color));display:flex;margin:auto;align-items:center;text-decoration:none}.site-header.thin .secondary-nav{margin:0 4px 0 auto}.site-header.thin .nav-right-button{--icon-color:var(--site-nav-link-color);display:flex;justify-content:center;align-items:center;width:1.875rem;height:var(--site-nav-height);border:none;background:0 0}.site-header.thin .nav-right-button.dropdown-button:after{display:none}@media (min-width:980px){.site-header.thin{grid-template-columns:8.75rem 1fr 8.75rem}.site-header.thin .site-header-title{display:block}}.site-header.thin .has-dropdown{margin-bottom:0}.site-header.show-title-on-scroll .site-header-title{opacity:0;transition:opacity .3s linear}.site-header.show-title-on-scroll.headroom--not-top .site-header-title{opacity:1}@media (min-width:980px){.site-header.thin .secondary-nav{grid-area:auto}.site-header.thin .site-header-title{display:block;font-size:var(--font-size-base)}}.site-header.is-doc-builder{--site-nav-background:var(--ivideo-header-bg, var(--text-color));--site-nav-link-color:var(--tint);height:var(--doc-builder-site-nav-height,var(--site-nav-height));display:flex;align-items:center;padding:0;-webkit-mask-image:none;mask-image:none;background-image:none}.site-header.is-doc-builder .site-header-title{overflow:visible}.site-header.is-doc-builder .site-back{--icon-size:1rem;--icon-color:var(--site-nav-link-color);--button-icon-opacity:1;display:flex;margin:0 .625rem;align-items:center;text-decoration:none;flex:0 0 auto;color:var(--site-nav-thin-text-color,var(--link-color))}.site-header.is-doc-builder .site-header-title{display:block;font-size:var(--font-size-base);flex:1 1 auto;margin:0 auto}@media (min-width:980px){.site-header.is-doc-builder .site-back{margin-right:289px}.site-header.is-doc-builder .secondary-nav{justify-content:flex-end;min-width:315px}}.floating-ghost-modal{position:fixed;bottom:6px;right:6px;border:1px solid var(--caution-color-shade);border-radius:4px;padding:16px 24px 10px;background:var(--ghost-modal-bg,rgba(255,255,255,.95));z-index:100;box-shadow:var(--heavy-shadow);color:var(--ghost-modal-text-color,var(--text-color))}@supports ((-webkit-backdrop-filter:blur(4px)) or (backdrop-filter:blur(4px))){.floating-ghost-modal{-webkit-backdrop-filter:blur(4px);backdrop-filter:blur(4px);background:var(--ghost-modal-bg-blurred,rgba(255,255,255,.6))}}.floating-ghost-modal .button.button{margin:1rem 0 0 0;min-height:1.5rem;white-space:nowrap;color:var(--global-modal-button-color,var(--button-hollow-color,var(--info-color-shade)));text-shadow:none}.floating-ghost-modal .avatar-detail-meta{white-space:nowrap}.floating-ghost-modal:after{position:absolute;top:28px;left:4px;display:block;width:16px;height:16px;background-image:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' viewBox='0 0 16 17' id='drag_handle' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M14 4a2 2 0 100-4 2 2 0 000 4zm0 6.03a2 2 0 100-4 2 2 0 000 4zm0 6.03a2 2 0 100-4 2 2 0 000 4zM2 4a2 2 0 100-4 2 2 0 000 4zm0 6.03a2 2 0 100-4 2 2 0 000 4zm0 6.03a2 2 0 100-4 2 2 0 000 4zM8 4a2 2 0 100-4 2 2 0 000 4zm0 6.03a2 2 0 100-4 2 2 0 000 4zm0 6.03a2 2 0 100-4 2 2 0 000 4z' fill='currentColor'/%3E%3C/svg%3E");background-position:center center;background-size:16px 16px;opacity:.4;content:"";z-index:120}.floating-ghost-modal:before{position:absolute;top:0;left:0;display:block;width:100%;height:6px;content:"";background-color:var(--caution-color);border-radius:3px 3px 0 0;background-image:repeating-linear-gradient(45deg,var(--caution-color-shade),var(--caution-color-shade) 10px,transparent 10px,transparent 20px)}:root{--bg-multiplier:1}@media (min-width:768px){:root{--bg-multiplier:2}}@media (min-width:1200px){:root{--bg-multiplier:2.5}}#reply:target{height:calc(var(--site-nav-height) + 30px);width:1px;display:block;position:absolute;margin-top:calc((var(--site-nav-height) + 30px) * -1)}.tabs{--icon-size:1.25rem;margin-bottom:0}.tabs.dropdown-is-open .tab-button:after{transform:rotate(180deg)}.tabs.dropdown-is-open .tab-dropdown{display:block}.tabs.step-tabs{--tab-font-weight:var(--global-weight-semibold);--tab-link-border-width:0 0 6px 0;--tab-link-padding:0 12px 4px;--tab-link-current-border-color:var(--info-color);--tab-link-bg-color:transparent;--tab-bg-color-current:var(--tab-link-bg-color);--tab-link-color:var(--text-color);--tab-link-color-current:var(--tab-link-color);--tab-link-color-hover:var(--tab-link-color)}.tabs.step-tabs .tab-item{flex:1 1 100%;padding-right:0}.tabs.step-tabs .tab-link{flex-direction:column;align-items:center;font-size:1.5rem;height:100%;width:100%;opacity:.6;line-height:1.2}.tabs.step-tabs .tab-link.current{opacity:1}.tabs.step-tabs .tab-sm-label{font-size:.875rem;font-weight:var(--global-weight-normal)}.tab{list-style:none;display:flex;flex-direction:row;justify-content:var(--tab-justify-content,flex-start);margin:var(--tab-margin,3.75rem 0 1.25rem);padding:0;width:100%;border:var(--tab-wrap-border,1px solid var(--info-color));border-width:var(--tab-wrap-border-width,0 0 2px 0);border-radius:var(--tab-wrap-border-radius,var(--global-radius-tl) var(--global-radius-tr) 0 0);background-color:var(--tab-bg-color,transparent)}.page-header .tab{margin:var(--tab-margin-feedback,1.25rem 0 0 0);border-width:var(--tab-wrap-border-width-feedback,0);background:0 0}.page-header .tab .tab-link.current,.page-header .tab .tab-link.current:hover,.page-header .tab .tab-link[aria-current=page],.page-header .tab .tab-link[aria-current=page]:hover,.page-header .tab .tab-link[aria-selected=true],.page-header .tab .tab-link[aria-selected=true]:hover{border-radius:var(--tab-first-border-radius,var(--tab-link-border-radius,var(--global-radius-tl) var(--global-radius-tr) 0 0))}.tab::-webkit-scrollbar{display:none}.tab.secondary{margin-bottom:var(--global-margin);border-bottom:1px solid var(--body-bg-shade2)}.tab-item{flex:var(--tab-item-flex,0 0 auto);margin:0 0 -1px 0;padding:var(--tab-item-padding,0 1.25rem 0 0)}.tab-item:last-of-type{padding-right:var(--tab-item-padding-right-last,0)}.tab-item-more.is-hidden,.tab-item.is-hidden{display:none}.tab-item-more{position:relative;border-radius:var(--tab-last-border-radius,0);border-width:var(--tab-last-border-width,0);margin-left:auto}.tab-link{position:relative;display:flex;padding:var(--tab-link-padding,10px 16px);background-color:var(--tab-link-bg-color,transparent);border:1px solid var(--tab-bg-color-current,var(--info-color));border-width:var(--tab-link-border-width,0);text-decoration:none;border-radius:var(--tab-link-border-radius,var(--global-radius-tl) var(--global-radius-tr) 0 0);font-family:var(--tab-font-family, var(--global-font-family));font-weight:var(--tab-font-weight,normal);color:var(--tab-link-color,var(--link-color))}.tab-link .icon{margin-right:.5rem}.tab-link:focus,.tab-link:hover{background-color:var(--tab-bg-color-hover,transparent);border-bottom:3px solid var(--link-color-tint);border-width:var(--tab-link-border-width,0 0 0 0);color:var(--tab-link-color-hover,var(--info-color));box-shadow:none}.knockout .tab-link:focus,.knockout .tab-link:hover{color:var(--tab-link-color-current,var(--knockout-color))}.tab-link.current,.tab-link.current:hover,.tab-link.selected,.tab-link.selected:hover,.tab-link[aria-current=page],.tab-link[aria-current=page]:hover,.tab-link[aria-selected=true],.tab-link[aria-selected=true]:hover{border-bottom:3px solid var(--tab-link-current-border-color,var(--link-color));border-width:var(--tab-link-border-width,0);color:var(--tab-link-color-current,var(--knockout-color));background-color:var(--tab-bg-color-current,var(--info-color));background-image:var(--tab-bg-image-current,none);background-size:var(--tab-bg-image-size,100% 100%);background-repeat:var(--tab-bg-image-repeat,no-repeat);background-position:var(--tab-bg-image-position,top left)}.tab-link.current:before,.tab-link.current:hover:before,.tab-link.selected:before,.tab-link.selected:hover:before,.tab-link[aria-current=page]:before,.tab-link[aria-current=page]:hover:before,.tab-link[aria-selected=true]:before,.tab-link[aria-selected=true]:hover:before{position:absolute;width:6px;height:6px;bottom:0;left:-6px;background-image:var(--tab-active-after-image,none);content:""}.tab-link[data-notification-badge]:after{top:var(--tab-notification-position-top,-.125rem);right:var(--tab-notification-position-right,-.375rem);z-index:2}.tab-item:first-child .tab-link:before{content:none}.tab-button{height:100%;padding:0 10px;margin:0;display:flex;align-items:center;-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent;border:1px solid var(--tab-link-border-color,transparent);border-width:var(--tab-last-border-width,0);color:var(--tab-link-color,var(--link-color));font-family:var(--tab-font-family, var(--global-font-family));font-weight:var(--tab-font-weight,normal);line-height:1.5;cursor:pointer;border-radius:var(--tab-last-border-radius,var(--tab-link-border-radius,var(--global-radius-tl) var(--global-radius-tr) 0 0))}.tab-button:after{display:inline-flex;width:12px;height:12px;margin-left:8px;-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 18 10'%3E%3Cpath fill='none' vector-effect='non-scaling-stroke' stroke='%2342435A' stroke-width='2' stroke-linecap='round' stroke-linejoin='round' stroke-miterlimit='10' d='M1 1l8 8 8-8'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 18 10'%3E%3Cpath fill='none' vector-effect='non-scaling-stroke' stroke='%2342435A' stroke-width='2' stroke-linecap='round' stroke-linejoin='round' stroke-miterlimit='10' d='M1 1l8 8 8-8'/%3E%3C/svg%3E");-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:12px 12px;mask-size:12px 12px;background-color:var(--tab-link-color,var(--link-color));transition:transform .2s;content:""}.tab-button:focus,.tab-button:hover{border-bottom:3px solid var(--link-color-tint);border-width:var(--tab-last-border-width,0);box-shadow:none}.tab-button.current,.tab-button[aria-current=page],.tab-button[aria-selected=true]{color:var(--tab-link-color-current,var(--link-color));background-color:var(--tab-bg-color-current,transparent);background-image:var(--tab-more-button-bg-image-current,none)}.tab-button.current:after,.tab-button[aria-current=page]:after,.tab-button[aria-selected=true]:after{background-color:var(--tab-link-color-current,var(--link-color))}.tab-dropdown{display:none;position:absolute;top:100%;right:0;border-radius:var(--global-radius);z-index:3;padding:.75rem 0;width:80vh;max-width:15rem;box-shadow:var(--heavy-shadow);border-radius:var(--global-radius);background:var(--tab-dropdown-bg-color,var(--dropdown-bg));font-size:1rem}.tab-dropdown .tab-item{padding:0}.tab-dropdown .tab-item:last-of-type .tab-link{border-radius:0}.tab-dropdown .tab-link{padding:.5rem .75rem;background:0 0;border:0 none;border-color:var(--tab-bg-color-current,transparent);border-radius:0;color:var(--tab-dropdown-text-color,var(--link-color));flex:1 1 100%;display:flex}.tab-dropdown .tab-link:hover{background-color:var(--tab-dropdown-bg-color-hover,var(--dropdown-hover-color));color:var(--tab-dropdown-text-color-hover,var(--link-color))}.tab-dropdown .tab-link.current,.tab-dropdown .tab-link[aria-current=page],.tab-dropdown .tab-link[aria-selected=true]{background-color:var(--tab-dropdown-bg-color-current,var(--dropdown-hover-color));color:var(--tab-link-color-current,var(--link-color));background-color:var(--tab-bg-color-current,transparent);background-image:var(--tab-more-dropdown-bg-image-current,var(--tab-bg-image-current,none))}.tab-dropdown .tab-link[data-notification-badge]:after{z-index:3;top:.875rem;right:.625rem}.page-header.has-tabs{border-bottom:var(--tab-wrap-border,2px solid var(--info-color))}.sub-nav-with-tabs{background:var(--site-header-has-fixed-subnav-bg,var(--subnav-background-lg,var(--subnav-background)));padding:var(--sub-nav-with-tabs-padding,20px 0 0 0);margin-top:var(--sub-nav-with-tabs-margin-top,0);margin-bottom:var(--sub-nav-with-tabs-margin-bottom,40px);border-bottom:var(--tab-wrap-border,2px solid var(--info-color))}.sub-nav-with-tabs .tab{margin:0;border-width:0;background:0 0}.sub-nav-with-tabs .tab-link[data-notification-badge]:not([data-notification-badge="*"])::after{border:2px solid --site-header-has-fixed-subnav-bg,var(--subnav-background-lg,var(--subnav-background))}.tab-pane[hidden]{display:none}:root{--tag-bg:var(--card-bg-shade);--tag-bg-hover:var(--card-bg-shade2)}.tag-list{display:flex;flex-wrap:wrap;margin:var(--global-margin) 0;padding:0;list-style:none;font-size:.875rem}.tag-list-label{margin-right:.25rem}.tag-list.has-hash .tag:not(.is-leader):before{opacity:.5;content:"#"}.tag-list li:first-child .tag{margin-left:0}.tag-list .tag{margin:0 .5rem .25rem 0}.tag{display:inline-block;margin:0;padding:0 .375rem;border-radius:var(--global-radius);background:var(--tag-bg-color,var(--theme-color-tint4,var(--tag-bg)));text-decoration:none;color:var(--tag-color,var(--text-color));font-family:var(--global-font-family)}.tag-link{color:var(--tag-link-color,var(--text-color))}.tag.is-leader{background-color:var(--leader-color);color:var(--knockout-color);display:var(--tag-is-leader-display,inline-block)}.tag.is-leader:before{display:inline-block;margin-right:.25rem;width:.625rem;height:.625rem;background-color:var(--knockout-color);-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 17.602 15.749' id='asterisk'%3E%3Cpath fill='currentColor' d='M16.252 6.239h-3.519a.613.613 0 01-.331-.083.62.62 0 01-.208-.882l.002-.006 1.532-2.653.216-.374a1.562 1.562 0 00-.668-1.943L13.127.21a1.565 1.565 0 00-2.014.389l-.223.385-1.527 2.645a.4.4 0 01-.04.07l-.002.003a.622.622 0 01-1.059-.032l-.003-.005L6.711.983 6.489.599A1.564 1.564 0 004.477.21l-.15.087a1.564 1.564 0 00-.669 1.943l.217.374 1.531 2.652v.001a.622.622 0 01.106.349.623.623 0 01-.624.623H1.35A1.565 1.565 0 000 7.789v.173c0 .789.584 1.442 1.344 1.549h3.499a.62.62 0 01.359.082c.294.17.397.544.234.841l-.006.011-.01.015-1.542 2.67-.222.385a1.563 1.563 0 00.67 1.938l.15.087a1.562 1.562 0 002.016-.394l.217-.375 1.531-2.65v-.001c.014-.027.027-.054.045-.079a.624.624 0 011.033.003l.006.009a.419.419 0 00.017.028l.011.021 1.542 2.67.216.375a1.567 1.567 0 002.018.394l.148-.086a1.564 1.564 0 00.67-1.938l-.221-.385-1.536-2.66a.62.62 0 01-.098-.337c0-.33.258-.602.583-.622l.04-.001.039.001h3.506a1.564 1.564 0 001.344-1.549v-.175a1.567 1.567 0 00-1.351-1.55z'/%3E%3C/svg%3E");mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 17.602 15.749' id='asterisk'%3E%3Cpath fill='currentColor' d='M16.252 6.239h-3.519a.613.613 0 01-.331-.083.62.62 0 01-.208-.882l.002-.006 1.532-2.653.216-.374a1.562 1.562 0 00-.668-1.943L13.127.21a1.565 1.565 0 00-2.014.389l-.223.385-1.527 2.645a.4.4 0 01-.04.07l-.002.003a.622.622 0 01-1.059-.032l-.003-.005L6.711.983 6.489.599A1.564 1.564 0 004.477.21l-.15.087a1.564 1.564 0 00-.669 1.943l.217.374 1.531 2.652v.001a.622.622 0 01.106.349.623.623 0 01-.624.623H1.35A1.565 1.565 0 000 7.789v.173c0 .789.584 1.442 1.344 1.549h3.499a.62.62 0 01.359.082c.294.17.397.544.234.841l-.006.011-.01.015-1.542 2.67-.222.385a1.563 1.563 0 00.67 1.938l.15.087a1.562 1.562 0 002.016-.394l.217-.375 1.531-2.65v-.001c.014-.027.027-.054.045-.079a.624.624 0 011.033.003l.006.009a.419.419 0 00.017.028l.011.021 1.542 2.67.216.375a1.567 1.567 0 002.018.394l.148-.086a1.564 1.564 0 00.67-1.938l-.221-.385-1.536-2.66a.62.62 0 01-.098-.337c0-.33.258-.602.583-.622l.04-.001.039.001h3.506a1.564 1.564 0 001.344-1.549v-.175a1.567 1.567 0 00-1.351-1.55z'/%3E%3C/svg%3E");-webkit-mask-position:center center;mask-position:center center;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;content:""}a.tag:hover{background:var(--tag-link-hover-bg,var(--theme-color-tint3,var(--tag-bg-hover)));text-decoration:underline}.tag-description{--tag-bg:var(--info-color-tint4);list-style:none;margin:0;padding:0}.tag-description-desc{margin-bottom:0}.tag-description-item{margin-bottom:var(--global-margin)}@media (min-width:768px){.tag-description-item{display:flex}.tag-description-tags{width:20%}}:root{--switch-size:48px;--toggle-bg-color:#abafb2;--toggle-value-color:var(--text-color);--toggle-value-font-size:14px;--v-toggle-adjust:6px;--v-toggle-value-width:80px}.field-row{--v-toggle-adjust:1px}.toggle{position:relative}.toggle label{position:relative;display:block;margin:0;padding:0;padding-right:calc(var(--switch-size) + var(--v-toggle-value-width) + 8px);cursor:pointer;font-weight:var(--global-weight-semibold)}.toggle label:before{position:absolute;top:var(--v-toggle-adjust);right:var(--v-toggle-value-width);display:block;width:var(--switch-size);height:calc(var(--switch-size)/ 2);border-radius:calc(var(--switch-size)/ 2);background:var(--toggle-bg-color);font-size:var(--toggle-value-font-size);line-height:calc(var(--switch-size) / 2);text-align:right;content:attr(data-unchecked)}.toggle label:after{position:absolute;top:calc(var(--v-toggle-adjust) + 2px);right:calc(var(--v-toggle-value-width) + 2px + (var(--switch-size)/ 2));width:calc(var(--switch-size)/ 2 - 4px);height:calc(var(--switch-size)/ 2 - 4px);box-shadow:1px 1px 1px rgba(0,0,0,.4);border-radius:calc(var(--switch-size)/ 2 - 4px);background:#fff;content:"";transition:.1s}.toggle label:active:after{width:calc(var(--switch-size)/ 2);transform:translateX(4px)}.toggle [type=checkbox],.toggle [type=radio]{position:absolute;left:-9999px}.toggle [type=checkbox]:checked+label:before,.toggle [type=radio]:checked+label:before{background:var(--theme-color,var(--success-color))}.toggle [type=checkbox]+label .values:before,.toggle [type=radio]+label .values:before{position:absolute;top:var(--v-toggle-adjust);width:calc(var(--v-toggle-value-width) - 10px);right:0;line-height:calc(var(--switch-size) / 2);font-size:var(--toggle-value-font-size);font-weight:var(--global-weight-semibold);text-transform:none;color:var(--toggle-value-color);content:attr(data-unchecked)}.toggle [type=checkbox]:checked+label .values:before,.toggle [type=radio]:checked+label .values:before{content:attr(data-checked)}.toggle [type=checkbox]:checked+label:after,.toggle [type=radio]:checked+label:after{right:calc(var(--v-toggle-value-width) + 2px)}.toggle [type=checkbox]:checked+label:active:after,.toggle [type=radio]:checked+label:active:after{transform:translateX(0)}.toggle [type=checkbox]:disabled+label:after,.toggle [type=checkbox]:disabled+label:before,.toggle [type=radio]:disabled+label:after,.toggle [type=radio]:disabled+label:before{opacity:.3}.toggle.disabled .help-text,.toggle.disabled label{opacity:1}.toggle.no-value-label{--v-toggle-value-width:0.01px}.toggle.no-value-label label:before{right:0}.toggle.no-value-label label:after{right:calc((var(--switch-size)/ 2 - 4px) + 6px)}.toggle.no-value-label [type=checkbox]:checked+label:after,.toggle.no-value-label [type=radio]:checked+label:after{right:2px}.toggle.no-value-label .values{display:none}.toggle.inline-block label{display:inline-block}.toggle.align-with-input label{margin-top:2.3125rem}.toggle.short-label{--max-field-width:none}.toggle.short-label label{display:inline-block;width:11.25rem}.toggle.priority-label{--v-toggle-adjust:6px}.toggle.priority-label label{min-width:16.25rem;font-size:1.125rem;color:var(--primary-heading-color);font-weight:var(--global-weight-semibold)}.toggle.large-toggle{--switch-size:46px}.toggle .help-text{font-style:normal;display:inline-block;margin:var(--v-toggle-adjust) 0 0 0;vertical-align:top;padding-right:calc(var(--switch-size) + var(--v-toggle-value-width) + 8px)}.inline-toggles{--v-toggle-adjust:1px;display:flex;gap:0 3rem}.inline-toggles .toggle [type=checkbox]+label .values:before,.inline-toggles .toggle [type=radio]+label .values:before{top:auto;bottom:2px;right:auto;left:calc(var(--switch-size) + 10px);font-weight:var(--global-weight-normal)}.inline-toggles .toggle [type=checkbox]:checked+label:after,.inline-toggles .toggle [type=radio]:checked+label:after{right:auto;left:calc(var(--switch-size)/ 2 + 1px)}.inline-toggles .toggle [type=checkbox]+label:active:after,.inline-toggles .toggle [type=radio]+label:active:after{transform:translateX(0)}.inline-toggles .toggle [type=checkbox]:checked+label:active:after,.inline-toggles .toggle [type=radio]:checked+label:active:after{transform:translateX(-4px)}.inline-toggles .toggle.priority-label label{padding-right:0;padding-bottom:calc((var(--switch-size)/ 2) + .5rem);min-width:0}.inline-toggles .toggle.priority-label label:before{top:auto;bottom:0;left:0;height:calc(var(--switch-size)/ 2)}.inline-toggles .toggle.priority-label label:after{top:auto;left:2px;bottom:2px}.well{margin-bottom:var(--global-margin);padding:var(--global-margin);border-radius:var(--global-radius);background:var(--well-bg)}.well>:last-child{margin-bottom:0}.well+.well{margin-top:calc(var(--global-margin)/ 2)}.well.page-bg{--well-bg:var(--body-bg-color);border:1px solid var(--card-border-color-default)}.well.is-smaller{padding:.5rem;font-size:.8em}.well.is-smaller .page-subheading-2{font-size:.8em}.well.has-overflow{max-height:150px;overflow:auto}.well-headline{margin-bottom:var(--global-margin);font-size:1.25rem;font-weight:var(--global-weight-bold);color:var(--primary-heading-color)}.page{margin-top:var(--page-margin-top-mobile,0)}.page-header{margin-bottom:1.25rem;padding:var(--page-header-padding-sm,1.875rem 0 0);background:var(--header-bg,transparent);border-bottom:var(--header-border-bottom,1px solid var(--card-border-color-default))}.page-header-description{max-width:74ch;padding-right:2.5rem}.page-header-description:empty{display:none}.page-heading{margin:.5em 0 .75em;color:var(--primary-heading-color);font-family:var(--heading-font-family)}.page-heading.has-field{display:flex;flex-wrap:wrap;gap:2rem;margin-bottom:3rem}.page-subheading{margin:.5em 0 .75em;font-size:1.75rem;color:var(--primary-heading-color)}.page-subheading-2{margin:.5em 0 .75em;font-size:var(--font-size-small);text-transform:uppercase;color:var(--primary-heading-color)}.page-section+.page-section{padding-top:36px}@media (min-width:980px){.page{margin-top:var(--page-margin-top-desktop,0)}.page-header{padding:var(--page-header-padding-lg,1.875rem 0 0 0)}.page-header-flex-wrap{display:flex;flex-wrap:wrap;justify-content:space-between;align-items:center;gap:2rem}.page-header-flex-wrap.h-pad{padding:0 1rem}.page-heading{margin:.15em 0 .25em}.page-actions{margin-top:2.5rem}.page-actions.has-metadata-at-top{margin-top:1.25rem}.page-actions.has-metadata-at-top .page-metadata{padding-top:0;padding-bottom:1.25rem}.page-actions.has-metadata-at-top .notification-flag{margin-top:.5rem}.page-section+.page-section{padding-top:56px}}:root{--edu-header-height:var(--site-nav-height);--game-header-bg:var(--brand-color)}.edu-header{position:fixed;top:0;right:0;left:80px;height:var(--edu-header-height);background:var(--body-bg-color);z-index:5;border-bottom:1px solid var(--brand-color-tint4)}.edu-header-aside-text,.edu-header-subtitle,.edu-header-title{margin:0}.edu-header-title{font-size:var(--font-size-small);color:var(--text-color-subdued);font-weight:var(--global-weight-semibold)}.edu-header-aside-text{text-transform:uppercase;font-weight:var(--global-weight-semibold)}.edu-header .walkthrough-grid{height:100%}.is-below-edu-header{min-height:100vh;display:flex;flex-direction:column}.v-nav-page-layout{height:calc(100vh - var(--site-nav-height) - var(--site-subheader-height));display:grid;grid-gap:0;grid-template-rows:-webkit-min-content minmax(0,1fr) -webkit-min-content;grid-template-rows:min-content minmax(0,1fr) min-content}.v-nav-flex-layout{padding-bottom:100px;display:flex;flex-direction:column;min-height:calc(100vh - var(--site-nav-height) - var(--site-subheader-height))}@media (min-width:980px){.v-nav-flex-layout{padding-bottom:0}}.edu-pad-bleed-right{margin-right:-1.25rem}.edu-pad-bleed-right.table-scroll{max-width:none}.edu-h-pad,.edu-l-pad,.edu-r-pad{padding-right:1.25rem;padding-left:1.25rem}.edu-has-v-nav{position:relative;padding-right:1.25rem;padding-left:1.25rem}@media (min-width:980px){.edu-h-pad{padding-right:2.5rem;padding-left:2.5rem}.edu-h-pad.clamp-w-large{max-width:1100px}.edu-h-pad.has-todo-aside{padding-right:calc(var(--todo-aside-width) + 2.5rem)}.edu-has-v-nav{padding-right:2.5rem;padding-left:120px}.edu-pad-bleed-right{margin-right:-2.5rem}.edu-r-pad{padding-right:2.5rem;padding-left:0}.edu-l-pad{padding-left:2.5rem;padding-right:0}}.walkthrough-grid{display:flex;flex-direction:column-reverse}.walkthrough-grid .card>:last-child{margin-bottom:0}.walkthrough-main{grid-area:main;display:flex;flex-direction:column;justify-content:center;padding-bottom:var(--global-margin)}.walkthrough-main.half-pb{padding-bottom:calc(var(--global-margin)/ 2)}.walkthrough-aside{grid-area:aside}.walkthrough-aside.is-shade{background:var(--brand-color-tint4)}.walkthrough-heading{font-weight:var(--global-weight-semibold);margin-bottom:0;font-size:1.25rem}.walkthrough-help-heading,.walkthrough-help-text{--icon-size:1.25rem;display:flex;align-items:flex-start;font-weight:var(--global-weight-semibold);margin-bottom:.5rem}.walkthrough-help-heading .icon,.walkthrough-help-text .icon{margin-top:.25rem;margin-right:.375rem}.walkthrough-help-text,.walkthrough-subheading{font-size:var(--font-size-small)}.walkthrough-help-text.is-large,.walkthrough-subheading.is-large{font-size:var(--font-size-normal)}.walkthrough-help-heading,.walkthrough-help-text{max-width:480px}.walkthrough-help-text{font-weight:var(--global-weight-normal)}.walkthrough-fieldset{margin-bottom:3.75rem}.walkthrough-subdued-heading{font-weight:var(--global-weight-semibold);font-size:.875rem;color:var(--text-color-subdued)}.walkthrough-chapter-heading{display:flex;gap:8px;align-items:center;font-weight:var(--global-weight-semibold);margin-bottom:1rem;font-size:1.25rem}.walkthrough .is-v-centered{display:flex;flex-direction:column;justify-content:center}.walkthrough .is-h-centered{display:flex;flex-direction:column;align-items:center}@media (min-width:980px){.walkthrough-grid{display:grid;grid-gap:0 1.875rem;grid-template-columns:5fr 4fr;grid-template-areas:"main aside"}}.event-triggers{display:flex;justify-content:space-between;align-items:center;width:100%;max-width:340px}.event-triggers>*{margin:0}.synchronized-chapter-card{padding:0}.synchronized-chapter-card .walkthrough-aside,.synchronized-chapter-card .walkthrough-main{padding:1.25rem}.synchronized-chapter-card .walkthrough-aside.pb-0,.synchronized-chapter-card .walkthrough-main.pb-0{padding-bottom:0}.synchronized-chapter-item.is-selected{margin-left:-10px;margin-right:-10px;box-shadow:var(--base-shadow);background:var(--card-bg);border-radius:var(--global-radius);border:1px solid var(--card-border-color-default)}.synchronized-chapter-item .walkthrough-aside{background:var(--info-color-alpha-7)}.edu-header-actions{display:flex;justify-content:space-between;flex-wrap:wrap}.edu-header-actions input{min-width:240px}.edu-header-actions .button-wrap{flex:0 0 auto;flex-wrap:nowrap}.team-grid-wrap{display:flex;flex-direction:column;gap:2rem 3.75rem}@media (min-width:980px){.team-grid-wrap{display:grid;grid-template-columns:1fr 1fr}}.player-col{padding-bottom:1.25rem}.player-col .status-flag{display:inline-flex;padding:2px 8px;background:rgba(255,255,255,.2);border-radius:var(--global-radius);font-size:.875rem;font-weight:var(--global-weight-normal)}.player-col .status-flag.is-finished{background:var(--success-color-shade);color:var(--tint)}.player-col .status-flag.is-player{color:var(--text-color);background:var(--info-color-alpha)}.player-header{display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;min-height:40px}.player-header.is-nested{padding-left:0;padding-right:0}.player-header.pad-top{padding-top:3rem}.player-header p{margin:0}.player-header .button{margin-right:6px}.player-header a{text-decoration:none;font-size:var(--font-size-small);font-weight:var(--global-weight-semibold)}.player-header a:hover{text-decoration:underline}.player-card{padding:0}.player-card>:not(dialog){position:static}.player-card .card{box-shadow:none}.player-card.is-inactive-player .avatar-detail{opacity:.5}.player-card-heading{flex:1 1 100%;display:flex;align-items:baseline;flex-wrap:wrap;gap:8px;color:var(--theme-text-color,var(--knockout-color));font-size:1.125rem;margin:0}.player-card-summary{display:flex;gap:4px;justify-content:space-between;align-items:center;margin:0 0 0 auto;white-space:nowrap}.player-card-summary,.player-email{font-size:var(--font-size-small)}.player-item{--avatar-size:2.25rem;display:flex;justify-content:space-between;gap:.5rem;align-items:center;padding:.5rem;border-bottom:1px solid var(--card-border-color-default)}.player-item:last-child{border-bottom:0 none}.player-item .field{margin:0}.player-item .has-dropdown{flex:0 0 auto}.player-item .dropdown-button.button.hollow{--theme-text-color:var(--info-color);border-color:var(--info-color);color:var(--info-color)}.player-item .dropdown-button.button.hollow:focus,.player-item .dropdown-button.button.hollow:hover{background-color:var(--tint)}.player-item .dropdown-button.button.hollow:before{right:9px}.player-item .dropdown-link{font-size:var(--font-size-small)}.player-item .dropdown-link small{flex-shrink:0;margin-left:auto}.player-item.no-checkbox,.player-item.no-checkbox:not(.is-selected):not(.is-header):hover{background-color:transparent}.player-item.no-checkbox .avatar:before,.player-item.no-checkbox:not(.is-selected):not(.is-header):hover .avatar:before{content:none}.player-item.is-selected{background-color:var(--info-color-tint5)}.player-item.is-selected .avatar:before{position:absolute;top:-1px;right:-1px;bottom:-1px;left:-1px;background-image:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 36 36'%3E%3Ccircle cx='18' cy='18' r='18' fill='%239EC2E3' /%3E%3Cpath fill='%23fff' d='M11.5 11.5h13v13.772h-13z'/%3E%3Cpath d='M13 18.555l4.118 3.5 5.882-9' stroke='%232e373f' stroke-width='3' stroke-linejoin='round'/%3E%3C/svg%3E");content:""}.player-item:not(.is-selected):not(.is-header):hover{background-color:var(--info-color-tint5)}.player-item:not(.is-selected):not(.is-header):hover .avatar:before{position:absolute;top:-1px;right:-1px;bottom:-1px;left:-1px;background-image:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 36 36'%3E%3Ccircle cx='18' cy='18' r='18' fill='%239EC2E3'/%3E%3Cpath fill='%23fff' d='M11.5 11.5h13v13.772h-13z'/%3E%3C/svg%3E");content:""}.player-item .avatar-detail-meta{font-weight:var(--global-weight-semibold);font-size:var(--font-size-small)}.player-item .avatar-detail-meta .tag-list{font-weight:var(--global-weight-normal)}.player-item.is-header{color:var(--theme-text-color,var(--knockout-color));background-color:var(--theme-color,var(--game-header-bg));border-radius:var(--global-radius-tl) var(--global-radius-tr) 0 0;display:flex;gap:1rem;min-height:64px}.player-item.is-header .button{flex:1 0 auto;white-space:nowrap;color:var(--theme-text-color,var(--knockout-color))}.player-item.is-header .button:focus,.player-item.is-header .button:hover{color:var(--theme-text-color,var(--knockout-color));background:var(--theme-color-shade,var(--info-color-tint2))}.player-item.is-header .start-button{background:var(--tint);color:var(--game-header-bg);min-height:34px}.player-item.is-header .start-button:not([disabled]):hover{color:var(--tint);border-color:var(--tint);background:trans}.player-list .player-item{grid-template-columns:1fr 3fr 6rem}.player-card-actions{display:flex;justify-content:flex-end;align-items:center;flex:1 0 auto;gap:4px}@media (min-width:980px){.player-grid{display:grid;grid-gap:0 3.75rem;grid-template-columns:minmax(0,1fr) minmax(0,1fr)}.page-header .player-grid{height:auto}.player-col{padding-bottom:0}.player-item{padding-right:1rem}.player-item.is-header{padding:1rem}}@media (max-width:569px){.player-item .button{padding-left:.25rem;padding-right:.25rem;margin-left:.5rem}}.pill-list{display:flex;flex-direction:column;list-style:none;gap:.25rem;padding:0;margin:0 0 .5rem 0;font-size:var(--font-size-small)}.pill-list.is-horizontal{flex-direction:row;gap:1rem}.pill-list.is-large{font-size:var(--font-size-base)}.pill-item{display:flex;align-items:center;gap:.5rem}.pill-var{display:flex;align-items:center;justify-content:center;min-width:32px;min-height:32px;padding:4px;font-size:var(--font-size-base);font-weight:var(--global-weight-semibold);background:var(--tint);border-radius:var(--global-radius);border:1px solid var(--card-border-color-default)}.team-status-box{position:relative}.team-status-box .download-button{position:absolute;top:.5rem;right:1rem}.player-help-header{font-size:1.125rem;margin:1rem 0 .5rem}.player-help-img{width:200px;border:4px solid var(--tint);float:right;margin:0 0 1rem 1rem;box-shadow:var(--base-shadow);opacity:.5}.button.inline-help-button{display:inline-flex;align-items:center;margin:-7px 8px 0}.settings-button,.toggle-button{--icon-size:1.25rem;-webkit-appearance:none;-moz-appearance:none;appearance:none;border:0 none;background:0 0;color:var(--knockout-color);padding:0;margin:0;border-right:1px solid var(--tint-alpha-30);display:flex;align-items:center}.settings-button{padding:0}.settings-button:before{right:2px}.settings-button:after{content:none}.toggle-button{--icon-size:1.25rem;border-right:0 none}.toggle-button.is-expanded{transform:rotate(180deg)}.player-toggle{list-style:none;margin:0;padding:0;display:flex}.player-toggle li:not(:last-child):after{color:var(--text-color-subdued);content:"/";display:inline-block;margin:0 8px}.player-toggle a{display:inline-block;border-radius:var(--global-radius)}.player-toggle a[aria-selected=true]{background:var(--info-color-shade);color:var(--knockout-color);padding:0 8px}.all-players-managed{--icon-color:var(--info-color-tint2);--icon-size:64px;background-color:var(--tint);padding:3.75rem 1.25rem;border-radius:var(--global-radius);display:flex;flex-direction:column;justify-content:center;align-items:center;margin-top:.75rem}.all-players-managed .icon{margin-bottom:1rem}.chart-filters{max-width:600px}.filtered-charts{margin:2rem 0}@media (min-width:980px){.filtered-charts{display:grid;grid-gap:3rem;grid-template-columns:1fr 1fr}}.reports-max-width{max-width:1170px}:-webkit-full-screen .reports-max-width{max-width:none;height:100%}:-ms-fullscreen .reports-max-width{max-width:none;height:100%}:fullscreen .reports-max-width{max-width:none;height:100%}:-webkit-full-screen{background:var(--body-bg-color);padding:100px;overflow:auto}:-ms-fullscreen{background:var(--body-bg-color);padding:100px;overflow:auto}:fullscreen{background:var(--body-bg-color);padding:100px;overflow:auto}.report-header-wrap{display:flex;justify-content:space-between;align-items:flex-end}body,html{box-sizing:border-box;height:100%;min-height:100%}.main-container{margin:0 auto;padding-right:10px;padding-left:10px;width:100%;max-width:var(--main-container-width,1200px)}.main-container .main-container{padding-right:0;padding-left:0}.main-container.two-thirds{max-width:800px}.main-container.half{max-width:600px}.main-container.one-third{max-width:400px}.main-container.extra-wide{max-width:1600px}.main-container.v-pad{padding-top:1.25rem;padding-bottom:1.25rem}.main-container.v-pad-half{padding-top:.625rem;padding-bottom:.625rem}.main-container.v-pad-page-bottom{padding-bottom:2.5rem}@media (min-width:768px){.main-container{padding-right:20px;padding-left:20px}.main-container.v-pad{padding-top:2.5rem;padding-bottom:2.5rem}.main-container.v-pad-half{padding-top:1.25rem;padding-bottom:1.25rem}.main-container.v-pad-page-bottom{padding-bottom:25rem}}.avatar-content{display:grid;grid-gap:0 0.625rem;grid-template-columns:var(--avatar-size) 1fr;grid-template-areas:"avatar content";align-items:start;padding:.625rem 0}.avatar-content.v-center{align-items:center}.avatar-content .avatar-wrap{grid-area:avatar}.avatar-content .content-wrap{grid-area:content}.avatar-content .content-wrap>:last-child{margin-bottom:0}@media (max-width:569px){.avatar-content.hide-avatar-on-mobile{display:block}.avatar-content.hide-avatar-on-mobile .avatar-wrap{display:none}}.grid{display:grid;grid-gap:var(--global-margin)}.grid.variable-column{grid-template-columns:repeat(auto-fit,minmax(200px,1fr))}.grid.align-center{align-items:center}.grid .well+.well,.grid>*{margin:0}@media (min-width:570px){.grid>.well{margin:0}.grid.two-column{grid-template-columns:minmax(0,1fr) minmax(0,1fr)}.grid.three-column{grid-template-columns:minmax(0,1fr) minmax(0,1fr) minmax(0,1fr)}.grid.four-column{grid-template-columns:minmax(0,1fr) minmax(0,1fr) minmax(0,1fr) minmax(0,1fr)}.grid .span-two{grid-column-end:span 2}.grid .span-three{grid-column-end:span 3}.grid .full-width{grid-column-start:1;grid-column-end:-1}}.todo-list{display:flex;flex-direction:column;gap:.5rem;list-style:none;margin:0;padding:0}.todo-list li{counter-increment:this-counter}.todo-link{position:relative;font-size:1rem;font-weight:var(--global-weight-semibold);text-decoration:none;display:flex;align-items:center;gap:.75rem;padding:1rem;color:var(--text-color);border:1px solid var(--brand-color);border-radius:var(--global-radius);background-image:linear-gradient(340.18deg,rgba(36,56,87,.5) -75.52%,rgba(255,255,255,.4) 50.7%);background-size:130% 180%;transition:background-position .3s linear}.todo-link:not(.is-disabled):hover{background-position:bottom right}.todo-link:before{content:counter(this-counter);flex:0 0 auto;display:flex;justify-content:center;align-items:center;line-height:1;width:24px;height:24px;border-radius:50%;-webkit-mask-position:center left;mask-position:center left;-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;background-color:var(--body-bg-shade2);color:var(--tint)}.todo-link.is-complete:before{content:"";mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 22 22'%3E%3Cpath d='M11 0C4.926 0 0 4.926 0 11c0 6.078 4.926 11 11 11 6.076 0 11-4.924 11-11 0-6.074-4.924-11-11-11zm4.934 9.357c-.014.016-.025.03-.04.044l-2.261 2.258a.293.293 0 01-.04.035l-.219.219-.018.018-.015.018-1.97 1.966a.092.092 0 01-.018.019l-.743.743a.93.93 0 01-1.289-.016l-.02-.02-2.588-2.588a1.242 1.242 0 01.029-1.736 1.246 1.246 0 011.766 0l1.478 1.479 4.13-4.13c.23-.214.532-.333.846-.333a1.242 1.242 0 01.972 2.024z' fill='%23144984'/%3E%3C/svg%3E");-webkit-mask-image:url("data:image/svg+xml;charset=utf8,%3Csvg fill='none' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 22 22'%3E%3Cpath d='M11 0C4.926 0 0 4.926 0 11c0 6.078 4.926 11 11 11 6.076 0 11-4.924 11-11 0-6.074-4.924-11-11-11zm4.934 9.357c-.014.016-.025.03-.04.044l-2.261 2.258a.293.293 0 01-.04.035l-.219.219-.018.018-.015.018-1.97 1.966a.092.092 0 01-.018.019l-.743.743a.93.93 0 01-1.289-.016l-.02-.02-2.588-2.588a1.242 1.242 0 01.029-1.736 1.246 1.246 0 011.766 0l1.478 1.479 4.13-4.13c.23-.214.532-.333.846-.333a1.242 1.242 0 01.972 2.024z' fill='%23144984'/%3E%3C/svg%3E");background-color:var(--success-color);border-color:var(--success-color)}.todo-link.is-alert{border-color:var(--caution-color)}.todo-link.is-alert:before{background-color:var(--caution-color)}.todo-link.is-disabled{cursor:not-allowed}.todo-link.no-dot:before{content:none}.todo-link.is-centered{justify-content:center}.todo-link.is-button-style{background-color:var(--info-color);background-image:none;color:var(--knockout-color);transition:var(--button-transition, none)}.todo-link.is-button-style:not(:disabled):focus,.todo-link.is-button-style:not(:disabled):hover{color:var(--info-color);background-color:var(--knockout-color);background-image:none}.todo-count{background:var(--info-color-tint4);border-radius:var(--global-radius);padding:0 6px;margin-right:4px}.todo-help-text{display:flex;align-items:center;font-size:var(--font-size-small);font-weight:var(--global-weight-normal);color:var(--text-color)}.simpl-push-footer{display:flex;flex-direction:column;min-height:calc(100vh - var(--site-nav-height))}.copyright-text{display:none}@media (min-width:980px){.copyright-text{display:block;margin-top:auto;font-size:13px;padding-top:20px;padding-left:20px}}.tab-link.outline.svelte-1jc2hdr{border-width:1px;border-style:solid;border-bottom:0 none}.player-item.svelte-hxuor6:hover input.svelte-hxuor6{transform:scale(1.1)}h3.svelte-gwov2v{font-size:1rem}.progress-loader.svelte-jxbktk{position:absolute;right:0;background:grey;color:#fff;letter-spacing:1px;font-size:.7em;padding:.2em .7em;margin:0 1em 0 0;border-radius:.3em}.progress-loader.listening.svelte-jxbktk{background:#006400;opacity:.4}.progress-loader.disconnected.svelte-jxbktk{background:#8b0000}
```

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/base.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/base.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/form_debrief.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/form_debrief.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/form_end.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/form_end.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/form_prepare.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/form_prepare.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/page-header.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/page-header.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/players_list/instructions.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/players_list/instructions.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/search_form.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/search_form.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/site-header.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/site-header.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/site-subheader.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/site-subheader.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/includes/status-arrows.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/includes/status-arrows.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/run_players.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/run_players.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/run_status.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/run_status.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templates/simpl/run_team.html` & `simpl-cloud-1.3.0/simpl/templates/simpl/run_team.html`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templatetags/includecontents.py` & `simpl-cloud-1.3.0/simpl/templatetags/includecontents.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/templatetags/simpl.py` & `simpl-cloud-1.3.0/simpl/templatetags/simpl.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/tests/settings.py` & `simpl-cloud-1.3.0/simpl/tests/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 SECRET_KEY = "-"
 
 INSTALLED_APPS = [
+    "simpl.testapp",
     "simpl.apps.SimplConfig",
     "django.contrib.sites",
     "django.contrib.contenttypes",
     "django.contrib.auth",
     "allauth",
     "allauth.account",
     "allauth.socialaccount",
```

### Comparing `simpl-cloud-1.2.4/simpl/tests/test_models.py` & `simpl-cloud-1.3.0/simpl/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,28 +199,28 @@
         user.refresh_from_db()
         self.assertEqual(user.first_name, "Bob")
         self.assertEqual(user.last_name, "Jones")
 
     def test_updates_user_without_extra_data(self):
         user = baker.make(get_user_model())
         SocialAccount.objects.create(extra_data={}, user=user)
-        user_refreshed = get_user_model().objects.get()
+        user_refreshed = get_user_model().objects.get(pk=user.pk)
         self.assertEqual(user.first_name, user_refreshed.first_name)
         self.assertEqual(user.last_name, user_refreshed.last_name)
 
     def test_sets_user_email_if_empty(self):
         user = baker.make(get_user_model(), email="")
         SocialAccount.objects.create(extra_data={"email": "new@example.com"}, user=user)
         user.refresh_from_db()
         self.assertEqual(user.email, "new@example.com")
 
     def test_dont_update_user_email(self):
         user = baker.make(get_user_model(), email="old@example.com")
         SocialAccount.objects.create(extra_data={"email": "new@example.com"}, user=user)
-        user_refreshed = get_user_model().objects.get()
+        user_refreshed = get_user_model().objects.get(pk=user.pk)
         self.assertEqual(user.email, user_refreshed.email)
 
 
 class CharacterTestCase(TestCase):
     def setUp(self):
         self.character = baker.make(Character)
```

### Comparing `simpl-cloud-1.2.4/simpl/tests/test_simpl.py` & `simpl-cloud-1.3.0/simpl/tests/test_simpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from unittest import mock
 import uuid
 
 from allauth.socialaccount.models import SocialAccount
 from django.contrib.auth import get_user_model
-from django.test import TestCase
+from django.test import TestCase, TransactionTestCase
 from django.urls import reverse
 from django.utils import timezone
 from model_bakery import baker
 
 from simpl import (
     get_run_model,
     get_player_model,
@@ -27,15 +27,15 @@
 GameExperience = get_game_experience_model()
 
 
 class FakeContext:
     pass
 
 
-class AuthTestCase(TestCase):
+class AuthTestCase(TransactionTestCase):
     def setUp(self):
         self.api_url = reverse("simpl-api")
 
     def test_anon(self):
         request = self.client.post(
             self.api_url, '{"query": "{runs{id}}"}', content_type="application/json"
         )
```

### Comparing `simpl-cloud-1.2.4/simpl/urls.py` & `simpl-cloud-1.3.0/simpl/urls.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/utils/models.py` & `simpl-cloud-1.3.0/simpl/utils/models.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/utils/name_faker.py` & `simpl-cloud-1.3.0/simpl/utils/name_faker.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl/views.py` & `simpl-cloud-1.3.0/simpl/views.py`

 * *Files identical despite different names*

### Comparing `simpl-cloud-1.2.4/simpl_cloud.egg-info/PKG-INFO` & `simpl-cloud-1.3.0/simpl_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: simpl-cloud
-Version: 1.2.4
+Version: 1.3.0
 Summary: Base models and API for Django-based simulations.
 Home-page: https://github.com/Wharton-Interactive/simpl-cloud
 Author: Chris Beaven
 Author-email: smileychris@gmail.com
 License: GPL2
 Keywords: api simulation administration
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -200,7 +201,9 @@
 
 If using Auth0 for social authentication, add the following Django settings to
 make sure users are correctly logged out of Auth0 and (optionally) redirected after logout::
 
 
   ACCOUNT_ADAPTER = "simpl.auth0.Auth0LogoutAdapter"
   AUTH0_LOGOUT_RETURN_TO = "some.url"
+
+
```

### Comparing `simpl-cloud-1.2.4/simpl_cloud.egg-info/SOURCES.txt` & `simpl-cloud-1.3.0/simpl_cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,18 @@
 simpl/templates/simpl/includes/players_list/multiplayer_in_setup.html
 simpl/templates/simpl/includes/players_list/singleplayer_in_play.html
 simpl/templatetags/__init__.py
 simpl/templatetags/includecontents.py
 simpl/templatetags/simpl.py
 simpl/tests/__init__.py
 simpl/tests/settings.py
+simpl/tests/test_external_schema.py
 simpl/tests/test_models.py
 simpl/tests/test_simpl.py
+simpl/tests/test_utils.py
 simpl/utils/__init__.py
 simpl/utils/models.py
 simpl/utils/name_faker.py
 simpl_cloud.egg-info/PKG-INFO
 simpl_cloud.egg-info/SOURCES.txt
 simpl_cloud.egg-info/dependency_links.txt
 simpl_cloud.egg-info/not-zip-safe
```

### Comparing `simpl-cloud-1.2.4/tox.ini` & `simpl-cloud-1.3.0/tox.ini`

 * *Files identical despite different names*
