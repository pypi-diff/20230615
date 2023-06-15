# Comparing `tmp/nobinobi-daily-follow-up-0.1.2.3.tar.gz` & `tmp/nobinobi-daily-follow-up-0.1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobinobi-daily-follow-up-0.1.2.3.tar", last modified: Wed Feb  1 12:58:13 2023, max compression
+gzip compressed data, was "nobinobi-daily-follow-up-0.1.2.5.tar", last modified: Thu Jun 15 13:22:02 2023, max compression
```

## Comparing `nobinobi-daily-follow-up-0.1.2.3.tar` & `nobinobi-daily-follow-up-0.1.2.5.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.059291 nobinobi-daily-follow-up-0.1.2.3/
--rw-rw-rw-   0        0        0      153 2020-09-16 11:53:19.000000 nobinobi-daily-follow-up-0.1.2.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3379 2020-09-16 11:58:16.000000 nobinobi-daily-follow-up-0.1.2.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     4238 2023-02-01 12:57:42.000000 nobinobi-daily-follow-up-0.1.2.3/HISTORY.rst
--rw-rw-rw-   0        0        0    31809 2020-09-16 11:57:37.000000 nobinobi-daily-follow-up-0.1.2.3/LICENSE
--rw-rw-rw-   0        0        0      508 2020-10-12 14:04:53.000000 nobinobi-daily-follow-up-0.1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8037 2023-02-01 12:58:13.060290 nobinobi-daily-follow-up-0.1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3016 2020-09-17 09:48:24.000000 nobinobi-daily-follow-up-0.1.2.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.444007 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/
--rw-rw-rw-   0        0        0      901 2023-02-01 12:57:42.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/__init__.py
--rw-rw-rw-   0        0        0     6644 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/admin.py
--rw-rw-rw-   0        0        0     2132 2021-05-28 08:59:39.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/apps.py
--rw-rw-rw-   0        0        0    24928 2023-01-24 14:19:44.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/forms.py
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.335730 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.334717 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/en/
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.450954 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0    36220 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.335730 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.452983 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    17584 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    43173 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     3840 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/menus.py
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.466957 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/
--rw-rw-rw-   0        0        0    21335 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0001_initial.py
--rw-rw-rw-   0        0        0    29811 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py
--rw-rw-rw-   0        0        0     1251 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py
--rw-rw-rw-   0        0        0      902 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py
--rw-rw-rw-   0        0        0     2218 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py
--rw-rw-rw-   0        0        0    18214 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py
--rw-rw-rw-   0        0        0     3355 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py
--rw-rw-rw-   0        0        0     1288 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0006_medication_child.py
--rw-rw-rw-   0        0        0     1313 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py
--rw-rw-rw-   0        0        0     1966 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py
--rw-rw-rw-   0        0        0     1357 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py
--rw-rw-rw-   0        0        0     1577 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py
--rw-rw-rw-   0        0        0     1368 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py
--rw-rw-rw-   0        0        0      794 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/__init__.py
--rw-rw-rw-   0        0        0    18845 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/models.py
--rw-rw-rw-   0        0        0     6365 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/serializers.py
--rw-rw-rw-   0        0        0    13848 2022-01-28 08:50:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/signals.py
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.338725 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.506738 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/css/
--rw-rw-rw-   0        0        0     2723 2022-01-28 08:50:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css
--rw-rw-rw-   0        0        0     1132 2020-05-11 12:40:13.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map
--rw-rw-rw-   0        0        0     2984 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.524555 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/
--rw-rw-rw-   0        0        0        0 2019-05-07 09:02:52.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/.gitignore
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.953575 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/
--rw-rw-rw-   0        0        0    26606 2020-05-11 12:40:13.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/anger.png
--rw-rw-rw-   0        0        0    26912 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/burn.png
--rw-rw-rw-   0        0        0    25533 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/caca.png
--rw-rw-rw-   0        0        0    23167 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/confused.png
--rw-rw-rw-   0        0        0    24827 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/cool.png
--rw-rw-rw-   0        0        0    24276 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/cry.png
--rw-rw-rw-   0        0        0    30248 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/fire.png
--rw-rw-rw-   0        0        0    30457 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/grimace.png
--rw-rw-rw-   0        0        0    27131 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/love.png
--rw-rw-rw-   0        0        0    23405 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/miao.png
--rw-rw-rw-   0        0        0    38098 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/nothing.png
--rw-rw-rw-   0        0        0   191276 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/nothing.psd
--rw-rw-rw-   0        0        0    31987 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/prettiness.png
--rw-rw-rw-   0        0        0    26621 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/question.png
--rw-rw-rw-   0        0        0    23059 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/shout.png
--rw-rw-rw-   0        0        0    26669 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/slobber.png
--rw-rw-rw-   0        0        0    27523 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/smile.png
--rw-rw-rw-   0        0        0    22780 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/spook.png
--rw-rw-rw-   0        0        0    26432 2020-05-11 12:40:14.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/startle.png
--rw-rw-rw-   0        0        0    31314 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/surprise.png
--rw-rw-rw-   0        0        0    24973 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/sweat.png
--rw-rw-rw-   0        0        0    24280 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/thirst.png
--rw-rw-rw-   0        0        0    27373 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/vomit.png
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.966579 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/
--rw-rw-rw-   0        0        0      805 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.967539 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/notifications/
--rw-rw-rw-   0        0        0     2602 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/notifications/notify.js
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.978513 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/vendor/
--rw-rw-rw-   0        0        0    38511 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.341723 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.980510 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_child/
--rw-rw-rw-   0        0        0     4633 2022-01-13 14:13:29.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_child/base.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.982548 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.987539 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/
--rw-rw-rw-   0        0        0     1196 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html
--rw-rw-rw-   0        0        0      650 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html
--rw-rw-rw-   0        0        0     1535 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html
--rw-rw-rw-   0        0        0     1535 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html
--rw-rw-rw-   0        0        0     1598 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.988514 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/
--rw-rw-rw-   0        0        0      301 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.995518 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/
--rw-rw-rw-   0        0        0     1542 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html
--rw-rw-rw-   0        0        0     1418 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html
--rw-rw-rw-   0        0        0     1718 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html
--rw-rw-rw-   0        0        0    45469 2021-09-30 13:15:29.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html
--rw-rw-rw-   0        0        0     1407 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.999513 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/
--rw-rw-rw-   0        0        0      660 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html
--rw-rw-rw-   0        0        0     1565 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html
--rw-rw-rw-   0        0        0     1567 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.002512 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/
--rw-rw-rw-   0        0        0      655 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html
--rw-rw-rw-   0        0        0     1416 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html
--rw-rw-rw-   0        0        0     1416 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.009566 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/
--rw-rw-rw-   0        0        0      782 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html
--rw-rw-rw-   0        0        0     1551 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html
--rw-rw-rw-   0        0        0      968 2020-05-11 12:40:15.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html
--rw-rw-rw-   0        0        0     6663 2021-09-30 13:15:29.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html
--rw-rw-rw-   0        0        0     1551 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.344718 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.013521 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/
--rw-rw-rw-   0        0        0       49 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/checkbox.html
--rw-rw-rw-   0        0        0      400 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio-input.html
--rw-rw-rw-   0        0        0      717 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html
--rw-rw-rw-   0        0        0      490 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_option.html
--rw-rw-rw-   0        0        0      717 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.017521 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/
--rw-rw-rw-   0        0        0      726 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html
--rw-rw-rw-   0        0        0     1540 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html
--rw-rw-rw-   0        0        0     1664 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html
--rw-rw-rw-   0        0        0     1542 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.023044 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/
--rw-rw-rw-   0        0        0     2228 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html
--rw-rw-rw-   0        0        0     1647 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html
--rw-rw-rw-   0        0        0     2209 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html
--rw-rw-rw-   0        0        0     1689 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.027038 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/
--rw-rw-rw-   0        0        0      691 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html
--rw-rw-rw-   0        0        0     1536 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html
--rw-rw-rw-   0        0        0     1549 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.029040 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/
--rw-rw-rw-   0        0        0     2235 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html
--rw-rw-rw-   0        0        0     1535 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.033039 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/
--rw-rw-rw-   0        0        0      660 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html
--rw-rw-rw-   0        0        0     1565 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html
--rw-rw-rw-   0        0        0     1259 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html
--rw-rw-rw-   0        0        0     1567 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.036042 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/
--rw-rw-rw-   0        0        0      626 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html
--rw-rw-rw-   0        0        0     1533 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html
--rw-rw-rw-   0        0        0     1533 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.044045 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/
--rw-rw-rw-   0        0        0    32358 2020-10-12 14:04:53.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html
--rw-rw-rw-   0        0        0     1196 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html
--rw-rw-rw-   0        0        0     1538 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html
--rw-rw-rw-   0        0        0     1535 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html
--rw-rw-rw-   0        0        0    21134 2021-06-18 08:56:48.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html
--rw-rw-rw-   0        0        0    10664 2022-01-28 08:50:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html
--rw-rw-rw-   0        0        0     1158 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html
--rw-rw-rw-   0        0        0    52404 2023-01-24 14:19:44.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.045050 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/
--rw-rw-rw-   0        0        0     1539 2021-07-22 11:48:42.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.048040 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/
--rw-rw-rw-   0        0        0     1196 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html
--rw-rw-rw-   0        0        0     1797 2020-05-11 12:40:16.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.050772 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templatetags/
--rw-rw-rw-   0        0        0     1498 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3742 2022-01-13 13:10:42.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py
--rw-rw-rw-   0        0        0      978 2022-01-28 08:50:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.051778 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/
--rw-rw-rw-   0        0        0      794 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.058328 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/
--rw-rw-rw-   0        0        0      794 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/__init__.py
--rw-rw-rw-   0        0        0      867 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/admin.py
--rw-rw-rw-   0        0        0      889 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/apps.py
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:13.059291 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/migrations/
--rw-rw-rw-   0        0        0      794 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py
--rw-rw-rw-   0        0        0      855 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/models.py
--rw-rw-rw-   0        0        0    25536 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/urls.py
--rw-rw-rw-   0        0        0     3866 2021-01-22 13:43:09.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/utils.py
--rw-rw-rw-   0        0        0   130245 2022-10-25 13:46:06.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/views.py
--rw-rw-rw-   0        0        0     1964 2020-09-17 09:48:22.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/widgets.py
-drwxrwxrwx   0        0        0        0 2023-02-01 12:58:12.449955 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/
--rw-rw-rw-   0        0        0     8037 2023-02-01 12:58:12.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10027 2023-02-01 12:58:12.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 12:58:12.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-01 12:56:30.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      659 2023-02-01 12:58:12.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-02-01 12:58:12.000000 nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      710 2023-02-01 12:57:41.000000 nobinobi-daily-follow-up-0.1.2.3/requirements.txt
--rw-rw-rw-   0        0        0      185 2023-01-24 14:19:44.000000 nobinobi-daily-follow-up-0.1.2.3/requirements_dev.txt
--rw-rw-rw-   0        0        0      205 2023-01-24 14:19:44.000000 nobinobi-daily-follow-up-0.1.2.3/requirements_test.txt
--rw-rw-rw-   0        0        0      301 2023-02-01 12:58:13.061319 nobinobi-daily-follow-up-0.1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2357 2021-01-22 13:43:10.000000 nobinobi-daily-follow-up-0.1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.153694 nobinobi-daily-follow-up-0.1.2.5/
+-rw-rw-rw-   0        0        0      166 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3491 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     4589 2023-06-15 13:21:22.000000 nobinobi-daily-follow-up-0.1.2.5/HISTORY.rst
+-rw-rw-rw-   0        0        0    31999 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/LICENSE
+-rw-rw-rw-   0        0        0      508 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8347 2023-06-15 13:22:02.154726 nobinobi-daily-follow-up-0.1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3016 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.848267 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/
+-rw-rw-rw-   0        0        0      901 2023-06-15 13:21:22.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/__init__.py
+-rw-rw-rw-   0        0        0     6644 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/admin.py
+-rw-rw-rw-   0        0        0     2132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/apps.py
+-rw-rw-rw-   0        0        0    24928 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.758274 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.757757 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.855425 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    36220 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.758274 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.890345 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    17584 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    43173 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     3840 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/menus.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.912077 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/
+-rw-rw-rw-   0        0        0    21335 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0    29811 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py
+-rw-rw-rw-   0        0        0     1251 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py
+-rw-rw-rw-   0        0        0      902 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py
+-rw-rw-rw-   0        0        0     2218 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py
+-rw-rw-rw-   0        0        0    18214 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py
+-rw-rw-rw-   0        0        0     3355 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py
+-rw-rw-rw-   0        0        0     1288 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0006_medication_child.py
+-rw-rw-rw-   0        0        0     1313 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py
+-rw-rw-rw-   0        0        0     1966 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py
+-rw-rw-rw-   0        0        0     1357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py
+-rw-rw-rw-   0        0        0     1577 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py
+-rw-rw-rw-   0        0        0     1368 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/__init__.py
+-rw-rw-rw-   0        0        0    18845 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/models.py
+-rw-rw-rw-   0        0        0     6365 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/serializers.py
+-rw-rw-rw-   0        0        0    13848 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.759807 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.914127 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/
+-rw-rw-rw-   0        0        0     2723 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css
+-rw-rw-rw-   0        0        0     1132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map
+-rw-rw-rw-   0        0        0     2984 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.915141 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/
+-rw-rw-rw-   0        0        0        0 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.028237 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/
+-rw-rw-rw-   0        0        0    26606 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/anger.png
+-rw-rw-rw-   0        0        0    26912 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/burn.png
+-rw-rw-rw-   0        0        0    25533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/caca.png
+-rw-rw-rw-   0        0        0    23167 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/confused.png
+-rw-rw-rw-   0        0        0    24827 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cool.png
+-rw-rw-rw-   0        0        0    24276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cry.png
+-rw-rw-rw-   0        0        0    30248 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/fire.png
+-rw-rw-rw-   0        0        0    30457 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/grimace.png
+-rw-rw-rw-   0        0        0    27131 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/love.png
+-rw-rw-rw-   0        0        0    23405 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/miao.png
+-rw-rw-rw-   0        0        0    38098 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.png
+-rw-rw-rw-   0        0        0   191276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.psd
+-rw-rw-rw-   0        0        0    31987 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/prettiness.png
+-rw-rw-rw-   0        0        0    26621 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/question.png
+-rw-rw-rw-   0        0        0    23059 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/shout.png
+-rw-rw-rw-   0        0        0    26669 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/slobber.png
+-rw-rw-rw-   0        0        0    27523 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/smile.png
+-rw-rw-rw-   0        0        0    22780 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/spook.png
+-rw-rw-rw-   0        0        0    26432 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/startle.png
+-rw-rw-rw-   0        0        0    31314 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/surprise.png
+-rw-rw-rw-   0        0        0    24973 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/sweat.png
+-rw-rw-rw-   0        0        0    24280 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/thirst.png
+-rw-rw-rw-   0        0        0    27373 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/vomit.png
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.029258 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/
+-rw-rw-rw-   0        0        0      805 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.031287 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/notifications/
+-rw-rw-rw-   0        0        0     2602 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/notifications/notify.js
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.031287 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/vendor/
+-rw-rw-rw-   0        0        0    38511 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.760827 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.032458 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_child/
+-rw-rw-rw-   0        0        0     4633 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_child/base.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.033480 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.039768 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html
+-rw-rw-rw-   0        0        0      650 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html
+-rw-rw-rw-   0        0        0     1598 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.041391 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/
+-rw-rw-rw-   0        0        0      301 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.049141 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/
+-rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html
+-rw-rw-rw-   0        0        0     1418 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html
+-rw-rw-rw-   0        0        0     1718 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html
+-rw-rw-rw-   0        0        0    45469 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html
+-rw-rw-rw-   0        0        0     1407 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.054309 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/
+-rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html
+-rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.057494 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/
+-rw-rw-rw-   0        0        0      655 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html
+-rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html
+-rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.084154 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/
+-rw-rw-rw-   0        0        0      782 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html
+-rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html
+-rw-rw-rw-   0        0        0      968 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html
+-rw-rw-rw-   0        0        0     6663 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html
+-rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.764146 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.089389 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/
+-rw-rw-rw-   0        0        0       49 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/checkbox.html
+-rw-rw-rw-   0        0        0      400 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio-input.html
+-rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html
+-rw-rw-rw-   0        0        0      490 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_option.html
+-rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.094494 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/
+-rw-rw-rw-   0        0        0      726 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1540 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html
+-rw-rw-rw-   0        0        0     1664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html
+-rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.100710 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/
+-rw-rw-rw-   0        0        0     2228 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html
+-rw-rw-rw-   0        0        0     1647 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html
+-rw-rw-rw-   0        0        0     2209 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html
+-rw-rw-rw-   0        0        0     1689 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.103909 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/
+-rw-rw-rw-   0        0        0      691 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html
+-rw-rw-rw-   0        0        0     1536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html
+-rw-rw-rw-   0        0        0     1549 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.105949 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/
+-rw-rw-rw-   0        0        0     2235 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.111191 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/
+-rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html
+-rw-rw-rw-   0        0        0     1259 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html
+-rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.113858 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/
+-rw-rw-rw-   0        0        0      626 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html
+-rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html
+-rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.135144 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/
+-rw-rw-rw-   0        0        0    32358 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html
+-rw-rw-rw-   0        0        0     1538 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html
+-rw-rw-rw-   0        0        0    21134 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html
+-rw-rw-rw-   0        0        0    10664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html
+-rw-rw-rw-   0        0        0     1158 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html
+-rw-rw-rw-   0        0        0    52404 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.137186 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/
+-rw-rw-rw-   0        0        0     1539 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.141269 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html
+-rw-rw-rw-   0        0        0     1797 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.143829 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/
+-rw-rw-rw-   0        0        0     1498 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3742 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py
+-rw-rw-rw-   0        0        0      978 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.145871 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.151466 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/__init__.py
+-rw-rw-rw-   0        0        0      867 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/admin.py
+-rw-rw-rw-   0        0        0      889 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.152474 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/migrations/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py
+-rw-rw-rw-   0        0        0      855 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/models.py
+-rw-rw-rw-   0        0        0    25536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/urls.py
+-rw-rw-rw-   0        0        0     3866 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/utils.py
+-rw-rw-rw-   0        0        0   127708 2023-06-15 13:11:13.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/views.py
+-rw-rw-rw-   0        0        0     1964 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.854410 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/
+-rw-rw-rw-   0        0        0     8347 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10027 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      169 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      195 2023-06-14 13:30:37.000000 nobinobi-daily-follow-up-0.1.2.5/requirements.txt
+-rw-rw-rw-   0        0        0      125 2023-06-15 10:29:37.000000 nobinobi-daily-follow-up-0.1.2.5/requirements_dev.txt
+-rw-rw-rw-   0        0        0      192 2023-06-14 13:33:20.000000 nobinobi-daily-follow-up-0.1.2.5/requirements_test.txt
+-rw-rw-rw-   0        0        0      301 2023-06-15 13:22:02.155748 nobinobi-daily-follow-up-0.1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/setup.py
```

### Comparing `nobinobi-daily-follow-up-0.1.2.3/CONTRIBUTING.rst` & `nobinobi-daily-follow-up-0.1.2.5/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every
-little bit helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/prolibre-ch/nobinobi-daily-follow-up/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug"
-is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "feature"
-is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-Nobinobi Daily Follow-Up could always use more documentation, whether as part of the
-official Nobinobi Daily Follow-Up docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/prolibre-ch/nobinobi-daily-follow-up/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `nobinobi-daily-follow-up` for local development.
-
-1. Fork the `nobinobi-daily-follow-up` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/nobinobi-daily-follow-up.git
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv nobinobi-daily-follow-up
-    $ cd nobinobi-daily-follow-up/
-    $ python setup.py develop
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-        $ flake8 nobinobi_daily_follow_up tests
-        $ python setup.py test
-        $ tox
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-6. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 2.6, 2.7, and 3.3, and for PyPy. Check
-   https://travis-ci.org/prolibre-ch/nobinobi-daily-follow-up/pull_requests
-   and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-    $ python -m unittest tests.test_nobinobi_daily_follow_up
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every
+little bit helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/prolibre-ch/nobinobi-daily-follow-up/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug"
+is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "feature"
+is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+Nobinobi Daily Follow-Up could always use more documentation, whether as part of the
+official Nobinobi Daily Follow-Up docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/prolibre-ch/nobinobi-daily-follow-up/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `nobinobi-daily-follow-up` for local development.
+
+1. Fork the `nobinobi-daily-follow-up` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/nobinobi-daily-follow-up.git
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv nobinobi-daily-follow-up
+    $ cd nobinobi-daily-follow-up/
+    $ python setup.py develop
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+        $ flake8 nobinobi_daily_follow_up tests
+        $ python setup.py test
+        $ tox
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+6. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 2.6, 2.7, and 3.3, and for PyPy. Check
+   https://travis-ci.org/prolibre-ch/nobinobi-daily-follow-up/pull_requests
+   and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+    $ python -m unittest tests.test_nobinobi_daily_follow_up
```

### Comparing `nobinobi-daily-follow-up-0.1.2.3/HISTORY.rst` & `nobinobi-daily-follow-up-0.1.2.5/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 .. :changelog:
 
 History
 -------
 
+0.1.2.5 (2023-06-15)
++++++++++++++++++++++++++
+
+* 4e6cee2 - FIX: when create in presence day in table naps, lotion,medication, etc
+* 5e04f16 - Fix new version of crispy forms
+* Update requirements
+
+0.1.2.4 (2023-05-23)
++++++++++++++++++++++++++
+
+* 6d7582f - Fix: local variable 'hour0' referenced before assignment
+* Update requirements
+
 0.1.2.3 (2023-02-01)
 +++++++++++++++++++++++++
 
 * 4f14684 - Add check to display default menu
 * 79c6438 - fix test exemple
 * c51d34e - Add settings models
```

### Comparing `nobinobi-daily-follow-up-0.1.2.3/LICENSE` & `nobinobi-daily-follow-up-0.1.2.5/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-Copyright (c) 2020, Florian Alu
-GNU AFFERO GENERAL PUBLIC LICENSE
-
-Version 3, 19 November 2007
-
-Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
-Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
-Preamble
-
-The GNU Affero General Public License is a free, copyleft license for software and other kinds of works, specifically designed to ensure cooperation with the community in the case of network server software.
-
-The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, our General Public Licenses are intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users.
-
-When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
-
-Developers that use our General Public Licenses protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License which gives you legal permission to copy, distribute and/or modify the software.
-
-A secondary benefit of defending all users' freedom is that improvements made in alternate versions of the program, if they receive widespread use, become available for other developers to incorporate. Many developers of free software are heartened and encouraged by the resulting cooperation. However, in the case of software used on network servers, this result may fail to come about. The GNU General Public License permits making a modified version and letting the public access it on a server without ever releasing its source code to the public.
-
-The GNU Affero General Public License is designed specifically to ensure that, in such cases, the modified source code becomes available to the community. It requires the operator of a network server to provide the source code of the modified version running there to the users of that server. Therefore, public use of a modified version, on a publicly accessible server, gives the public access to the source code of the modified version.
-
-An older license, called the Affero General Public License and published by Affero, was designed to accomplish similar goals. This is a different license, not a version of the Affero GPL, but Affero has released a new version of the Affero GPL which permits relicensing under this license.
-
-The precise terms and conditions for copying, distribution and modification follow.
-TERMS AND CONDITIONS
-0. Definitions.
-
-"This License" refers to version 3 of the GNU Affero General Public License.
-
-"Copyright" also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
-
-"The Program" refers to any copyrightable work licensed under this License. Each licensee is addressed as "you". "Licensees" and "recipients" may be individuals or organizations.
-
-To "modify" a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a "modified version" of the earlier work or a work "based on" the earlier work.
-
-A "covered work" means either the unmodified Program or a work based on the Program.
-
-To "propagate" a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
-
-To "convey" a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
-
-An interactive user interface displays "Appropriate Legal Notices" to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
-1. Source Code.
-
-The "source code" for a work means the preferred form of the work for making modifications to it. "Object code" means any non-source form of a work.
-
-A "Standard Interface" means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
-
-The "System Libraries" of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A "Major Component", in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same work.
-2. Basic Permissions.
-
-All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
-
-When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
-4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
-5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
-    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to "keep intact all notices".
-    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
-    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
-
-A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an "aggregate" if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
-6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
-    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
-    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
-    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
-    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
-
-A "User Product" is either (1) a "consumer product", which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, "normally used" refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
-
-"Installation Information" for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
-
-The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
-7. Additional Terms.
-
-"Additional permissions" are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
-    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
-    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
-    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
-    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
-    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
-
-All other non-permissive additional terms are considered "further restrictions" within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
-8. Termination.
-
-You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
-
-However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
-
-Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
-9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
-10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
-
-An "entity transaction" is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
-11. Patents.
-
-A "contributor" is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's "contributor version".
-
-A contributor's "essential patent claims" are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, "control" includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
-
-In the following three paragraphs, a "patent license" is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To "grant" such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. "Knowingly relying" means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
-
-A patent license is "discriminatory" if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
-12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
-13. Remote Network Interaction; Use with the GNU General Public License.
-
-Notwithstanding any other provision of this License, if you modify the Program, your modified version must prominently offer all users interacting with it remotely through a computer network (if your version supports such interaction) an opportunity to receive the Corresponding Source of your version by providing access to the Corresponding Source from a network server at no charge, through some standard or customary means of facilitating copying of software. This Corresponding Source shall include the Corresponding Source for any work covered by version 3 of the GNU General Public License that is incorporated pursuant to the following paragraph.
-
-Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the work with which it is combined will remain governed by version 3 of the GNU General Public License.
-14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions of the GNU Affero General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU Affero General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU Affero General Public License, you may choose any version ever published by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions of the GNU Affero General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
-
-Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
-15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
-
-
-
+Copyright (c) 2020, Florian Alu
+GNU AFFERO GENERAL PUBLIC LICENSE
+
+Version 3, 19 November 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+Preamble
+
+The GNU Affero General Public License is a free, copyleft license for software and other kinds of works, specifically designed to ensure cooperation with the community in the case of network server software.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, our General Public Licenses are intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+Developers that use our General Public Licenses protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License which gives you legal permission to copy, distribute and/or modify the software.
+
+A secondary benefit of defending all users' freedom is that improvements made in alternate versions of the program, if they receive widespread use, become available for other developers to incorporate. Many developers of free software are heartened and encouraged by the resulting cooperation. However, in the case of software used on network servers, this result may fail to come about. The GNU General Public License permits making a modified version and letting the public access it on a server without ever releasing its source code to the public.
+
+The GNU Affero General Public License is designed specifically to ensure that, in such cases, the modified source code becomes available to the community. It requires the operator of a network server to provide the source code of the modified version running there to the users of that server. Therefore, public use of a modified version, on a publicly accessible server, gives the public access to the source code of the modified version.
+
+An older license, called the Affero General Public License and published by Affero, was designed to accomplish similar goals. This is a different license, not a version of the Affero GPL, but Affero has released a new version of the Affero GPL which permits relicensing under this license.
+
+The precise terms and conditions for copying, distribution and modification follow.
+TERMS AND CONDITIONS
+0. Definitions.
+
+"This License" refers to version 3 of the GNU Affero General Public License.
+
+"Copyright" also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this License. Each licensee is addressed as "you". "Licensees" and "recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a "modified version" of the earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based on the Program.
+
+To "propagate" a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays "Appropriate Legal Notices" to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+1. Source Code.
+
+The "source code" for a work means the preferred form of the work for making modifications to it. "Object code" means any non-source form of a work.
+
+A "Standard Interface" means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A "Major Component", in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+2. Basic Permissions.
+
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to "keep intact all notices".
+    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an "aggregate" if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, "normally used" refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+"Installation Information" for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered "further restrictions" within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+8. Termination.
+
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, "control" includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To "grant" such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. "Knowingly relying" means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is "discriminatory" if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+13. Remote Network Interaction; Use with the GNU General Public License.
+
+Notwithstanding any other provision of this License, if you modify the Program, your modified version must prominently offer all users interacting with it remotely through a computer network (if your version supports such interaction) an opportunity to receive the Corresponding Source of your version by providing access to the Corresponding Source from a network server at no charge, through some standard or customary means of facilitating copying of software. This Corresponding Source shall include the Corresponding Source for any work covered by version 3 of the GNU General Public License that is incorporated pursuant to the following paragraph.
+
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the work with which it is combined will remain governed by version 3 of the GNU General Public License.
+14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions of the GNU Affero General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU Affero General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU Affero General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU Affero General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+
+
```

### Comparing `nobinobi-daily-follow-up-0.1.2.3/PKG-INFO` & `nobinobi-daily-follow-up-0.1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: nobinobi-daily-follow-up
-Version: 0.1.2.3
+Version: 0.1.2.5
 Summary: Application Daily follow-up for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-daily-follow-up
 Author: Florian Alu
 Author-email: alu@prolibre.com
-License: UNKNOWN
 Keywords: nobinobi-daily-follow-up
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -137,14 +135,27 @@
 
 
 
 
 History
 -------
 
+0.1.2.5 (2023-06-15)
++++++++++++++++++++++++++
+
+* 4e6cee2 - FIX: when create in presence day in table naps, lotion,medication, etc
+* 5e04f16 - Fix new version of crispy forms
+* Update requirements
+
+0.1.2.4 (2023-05-23)
++++++++++++++++++++++++++
+
+* 6d7582f - Fix: local variable 'hour0' referenced before assignment
+* Update requirements
+
 0.1.2.3 (2023-02-01)
 +++++++++++++++++++++++++
 
 * 4f14684 - Add check to display default menu
 * 79c6438 - fix test exemple
 * c51d34e - Add settings models
 
@@ -295,9 +306,7 @@
 * Update requirements
 * Add Holiday and Organisation Closure in Presence Week
 
 0.1.0 (2020-09-16)
 ++++++++++++++++++
 
 * First release on PyPI.
-
-
```

### Comparing `nobinobi-daily-follow-up-0.1.2.3/README.rst` & `nobinobi-daily-follow-up-0.1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/__init__.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.1.2.3'
+__version__ = '0.1.2.5'
 default_app_config = 'nobinobi_daily_follow_up.apps.NobinobiDailyFollowUpConfig'
```

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/admin.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/apps.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/forms.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/forms.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/menus.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/menus.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0001_initial.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0006_medication_child.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0006_medication_child.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/migrations/__init__.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/models.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/serializers.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/serializers.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/signals.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/signals.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/anger.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/anger.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/burn.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/burn.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/caca.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/caca.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/confused.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/confused.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/cool.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cool.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/cry.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cry.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/fire.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/fire.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/grimace.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/grimace.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/love.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/love.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/miao.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/miao.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/nothing.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/nothing.psd` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.psd`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/prettiness.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/prettiness.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/question.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/question.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/shout.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/shout.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/slobber.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/slobber.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/smile.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/smile.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/spook.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/spook.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/startle.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/startle.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/surprise.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/surprise.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/sweat.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/sweat.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/thirst.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/thirst.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/img/smiley/vomit.png` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/vomit.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/notifications/notify.js` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/notifications/notify.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_child/base.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_child/base.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templatetags/__init__.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/__init__.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/__init__.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/admin.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/apps.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/test_utils/test_app/models.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/urls.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/urls.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/utils.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/utils.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up/widgets.py` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/widgets.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/PKG-INFO` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: nobinobi-daily-follow-up
-Version: 0.1.2.3
+Version: 0.1.2.5
 Summary: Application Daily follow-up for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-daily-follow-up
 Author: Florian Alu
 Author-email: alu@prolibre.com
-License: UNKNOWN
 Keywords: nobinobi-daily-follow-up
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -137,14 +135,27 @@
 
 
 
 
 History
 -------
 
+0.1.2.5 (2023-06-15)
++++++++++++++++++++++++++
+
+* 4e6cee2 - FIX: when create in presence day in table naps, lotion,medication, etc
+* 5e04f16 - Fix new version of crispy forms
+* Update requirements
+
+0.1.2.4 (2023-05-23)
++++++++++++++++++++++++++
+
+* 6d7582f - Fix: local variable 'hour0' referenced before assignment
+* Update requirements
+
 0.1.2.3 (2023-02-01)
 +++++++++++++++++++++++++
 
 * 4f14684 - Add check to display default menu
 * 79c6438 - fix test exemple
 * c51d34e - Add settings models
 
@@ -295,9 +306,7 @@
 * Update requirements
 * Add Holiday and Organisation Closure in Presence Week
 
 0.1.0 (2020-09-16)
 ++++++++++++++++++
 
 * First release on PyPI.
-
-
```

### Comparing `nobinobi-daily-follow-up-0.1.2.3/nobinobi_daily_follow_up.egg-info/SOURCES.txt` & `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.3/setup.py` & `nobinobi-daily-follow-up-0.1.2.5/setup.py`

 * *Files identical despite different names*

