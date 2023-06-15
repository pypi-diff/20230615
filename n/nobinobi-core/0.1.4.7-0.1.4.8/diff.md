# Comparing `tmp/nobinobi-core-0.1.4.7.tar.gz` & `tmp/nobinobi-core-0.1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobinobi-core-0.1.4.7.tar", last modified: Tue Jun 13 10:54:12 2023, max compression
+gzip compressed data, was "nobinobi-core-0.1.4.8.tar", last modified: Thu Jun 15 13:28:20 2023, max compression
```

## Comparing `nobinobi-core-0.1.4.7.tar` & `nobinobi-core-0.1.4.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.981832 nobinobi-core-0.1.4.7/
--rw-rw-rw-   0        0        0      166 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/AUTHORS.rst
--rw-rw-rw-   0        0        0     3363 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1389 2023-06-12 09:30:30.000000 nobinobi-core-0.1.4.7/HISTORY.rst
--rw-rw-rw-   0        0        0    31960 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/LICENSE
--rw-rw-rw-   0        0        0      247 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4132 2023-06-13 10:54:12.982832 nobinobi-core-0.1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2032 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.765581 nobinobi-core-0.1.4.7/nobinobi_core/
--rw-rw-rw-   0        0        0      819 2023-06-12 09:30:30.000000 nobinobi-core-0.1.4.7/nobinobi_core/__init__.py
--rw-rw-rw-   0        0        0     4699 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/admin.py
--rw-rw-rw-   0        0        0     1100 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/apps.py
--rw-rw-rw-   0        0        0     1775 2023-06-12 09:19:34.000000 nobinobi-core-0.1.4.7/nobinobi_core/forms.py
--rw-rw-rw-   0        0        0    13512 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.648265 nobinobi-core-0.1.4.7/nobinobi_core/locale/
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.647757 nobinobi-core-0.1.4.7/nobinobi_core/locale/en/
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.823835 nobinobi-core-0.1.4.7/nobinobi_core/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      421 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/locale/en/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.648265 nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.824834 nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2138 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.828214 nobinobi-core-0.1.4.7/nobinobi_core/migrations/
--rw-rw-rw-   0        0        0     2001 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     2473 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/0002_organisation_organisationclosure.py
--rw-rw-rw-   0        0        0      442 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/0003_alter_holiday_date.py
--rw-rw-rw-   0        0        0     1231 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/__init__.py
--rw-rw-rw-   0        0        0     2719 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/models.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.661849 nobinobi-core-0.1.4.7/nobinobi_core/static/
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.855718 nobinobi-core-0.1.4.7/nobinobi_core/static/css/
--rw-rw-rw-   0        0        0     3222 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css
--rw-rw-rw-   0        0        0    10217 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.css
--rw-rw-rw-   0        0        0     7789 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.min.css
--rw-rw-rw-   0        0        0      805 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/nobinobi_core.css
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.952538 nobinobi-core-0.1.4.7/nobinobi_core/static/js/
--rw-rw-rw-   0        0        0    38511 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/js/bootstrap-datetimepicker.min.js
--rw-rw-rw-   0        0        0   336451 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/js/moment-with-locales.min.js
--rw-rw-rw-   0        0        0      805 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/js/nobinobi_core.js
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.663863 nobinobi-core-0.1.4.7/nobinobi_core/templates/
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.956537 nobinobi-core-0.1.4.7/nobinobi_core/templates/includes/
--rw-rw-rw-   0        0        0      521 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/includes/messages.html
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.968024 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/
--rw-rw-rw-   0        0        0     2248 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_act.html
--rw-rw-rw-   0        0        0     2251 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_image.html
--rw-rw-rw-   0        0        0     1627 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html
--rw-rw-rw-   0        0        0     1620 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html
--rw-rw-rw-   0        0        0     1622 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html
--rw-rw-rw-   0        0        0     1187 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/field_errors_block.html
--rw-rw-rw-   0        0        0     1251 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/help_text.html
--rw-rw-rw-   0        0        0     1817 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect.html
--rw-rw-rw-   0        0        0     2076 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_image.html
--rw-rw-rw-   0        0        0     1658 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline.html
--rw-rw-rw-   0        0        0     1664 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline_image.html
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.969054 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/sj/
--rw-rw-rw-   0        0        0     1354 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/sj/collation_general.html
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.971003 nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/
--rw-rw-rw-   0        0        0      520 2023-06-12 09:16:28.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/add_official_holiday.html
--rw-rw-rw-   0        0        0      682 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/base.html
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.979315 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/
--rw-rw-rw-   0        0        0     1231 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1837 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_dict_value.py
--rw-rw-rw-   0        0        0      989 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_user_method.py
--rw-rw-rw-   0        0        0     1685 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/math.py
--rw-rw-rw-   0        0        0     3512 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/notifications_tags_custom.py
--rw-rw-rw-   0        0        0      989 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_date_sem.py
--rw-rw-rw-   0        0        0     1056 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_tags_html.py
--rw-rw-rw-   0        0        0     1276 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/startwith.py
--rw-rw-rw-   0        0        0     1153 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/urls.py
--rw-rw-rw-   0        0        0     3113 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/views.py
--rw-rw-rw-   0        0        0    23107 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.822835 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/
--rw-rw-rw-   0        0        0     4132 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      102 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2023-06-13 10:53:58.000000 nobinobi-core-0.1.4.7/requirements.txt
--rw-rw-rw-   0        0        0       63 2023-06-09 08:47:26.000000 nobinobi-core-0.1.4.7/requirements_dev.txt
--rw-rw-rw-   0        0        0      119 2023-06-13 10:48:31.000000 nobinobi-core-0.1.4.7/requirements_test.txt
--rw-rw-rw-   0        0        0      427 2023-06-13 10:54:12.983831 nobinobi-core-0.1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     2303 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.981832 nobinobi-core-0.1.4.7/tests/
--rw-rw-rw-   0        0        0     2695 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/tests/test_admin.py
--rw-rw-rw-   0        0        0     1399 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/tests/test_models.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.897096 nobinobi-core-0.1.4.8/
+-rw-rw-rw-   0        0        0      166 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3363 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1497 2023-06-15 13:28:00.000000 nobinobi-core-0.1.4.8/HISTORY.rst
+-rw-rw-rw-   0        0        0    31960 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/LICENSE
+-rw-rw-rw-   0        0        0      247 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4240 2023-06-15 13:28:20.898098 nobinobi-core-0.1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2032 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.819294 nobinobi-core-0.1.4.8/nobinobi_core/
+-rw-rw-rw-   0        0        0      819 2023-06-15 13:28:00.000000 nobinobi-core-0.1.4.8/nobinobi_core/__init__.py
+-rw-rw-rw-   0        0        0     4699 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/admin.py
+-rw-rw-rw-   0        0        0     1100 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/apps.py
+-rw-rw-rw-   0        0        0     1775 2023-06-12 09:19:34.000000 nobinobi-core-0.1.4.8/nobinobi_core/forms.py
+-rw-rw-rw-   0        0        0    13512 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.792959 nobinobi-core-0.1.4.8/nobinobi_core/locale/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.791803 nobinobi-core-0.1.4.8/nobinobi_core/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.825813 nobinobi-core-0.1.4.8/nobinobi_core/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      421 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/locale/en/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.792959 nobinobi-core-0.1.4.8/nobinobi_core/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.826812 nobinobi-core-0.1.4.8/nobinobi_core/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2138 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/locale/fr/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.839186 nobinobi-core-0.1.4.8/nobinobi_core/migrations/
+-rw-rw-rw-   0        0        0     2001 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     2473 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/migrations/0002_organisation_organisationclosure.py
+-rw-rw-rw-   0        0        0      442 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/migrations/0003_alter_holiday_date.py
+-rw-rw-rw-   0        0        0     1231 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2719 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/models.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.793960 nobinobi-core-0.1.4.8/nobinobi_core/static/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.852870 nobinobi-core-0.1.4.8/nobinobi_core/static/css/
+-rw-rw-rw-   0        0        0     3222 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css
+-rw-rw-rw-   0        0        0    10217 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/static/css/bootstrap-datetimepicker.css
+-rw-rw-rw-   0        0        0     7789 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/static/css/bootstrap-datetimepicker.min.css
+-rw-rw-rw-   0        0        0      805 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/static/css/nobinobi_core.css
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.860948 nobinobi-core-0.1.4.8/nobinobi_core/static/js/
+-rw-rw-rw-   0        0        0    38511 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/static/js/bootstrap-datetimepicker.min.js
+-rw-rw-rw-   0        0        0   336451 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/static/js/moment-with-locales.min.js
+-rw-rw-rw-   0        0        0      805 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/static/js/nobinobi_core.js
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.795960 nobinobi-core-0.1.4.8/nobinobi_core/templates/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.862473 nobinobi-core-0.1.4.8/nobinobi_core/templates/includes/
+-rw-rw-rw-   0        0        0      521 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/includes/messages.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.871007 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/
+-rw-rw-rw-   0        0        0     2248 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_act.html
+-rw-rw-rw-   0        0        0     2251 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_image.html
+-rw-rw-rw-   0        0        0     1627 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html
+-rw-rw-rw-   0        0        0     1620 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html
+-rw-rw-rw-   0        0        0     1622 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html
+-rw-rw-rw-   0        0        0     1187 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/field_errors_block.html
+-rw-rw-rw-   0        0        0     1251 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/help_text.html
+-rw-rw-rw-   0        0        0     1817 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect.html
+-rw-rw-rw-   0        0        0     2076 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect_image.html
+-rw-rw-rw-   0        0        0     1658 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect_inline.html
+-rw-rw-rw-   0        0        0     1664 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect_inline_image.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.871007 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/sj/
+-rw-rw-rw-   0        0        0     1354 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/sj/collation_general.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.883068 nobinobi-core-0.1.4.8/nobinobi_core/templates/nobinobi_core/
+-rw-rw-rw-   0        0        0      520 2023-06-12 09:16:28.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/nobinobi_core/add_official_holiday.html
+-rw-rw-rw-   0        0        0      682 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templates/nobinobi_core/base.html
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.893093 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/
+-rw-rw-rw-   0        0        0     1231 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1837 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/get_dict_value.py
+-rw-rw-rw-   0        0        0      989 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/get_user_method.py
+-rw-rw-rw-   0        0        0     1685 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/math.py
+-rw-rw-rw-   0        0        0     3512 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/notifications_tags_custom.py
+-rw-rw-rw-   0        0        0      989 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/remove_date_sem.py
+-rw-rw-rw-   0        0        0     1056 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/remove_tags_html.py
+-rw-rw-rw-   0        0        0     1276 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/templatetags/startwith.py
+-rw-rw-rw-   0        0        0     1153 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/urls.py
+-rw-rw-rw-   0        0        0     3113 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/views.py
+-rw-rw-rw-   0        0        0    23107 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/nobinobi_core/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.824820 nobinobi-core-0.1.4.8/nobinobi_core.egg-info/
+-rw-rw-rw-   0        0        0     4240 2023-06-15 13:28:20.000000 nobinobi-core-0.1.4.8/nobinobi_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-06-15 13:28:20.000000 nobinobi-core-0.1.4.8/nobinobi_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:28:20.000000 nobinobi-core-0.1.4.8/nobinobi_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 13:27:07.000000 nobinobi-core-0.1.4.8/nobinobi_core.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      102 2023-06-15 13:28:20.000000 nobinobi-core-0.1.4.8/nobinobi_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-15 13:28:20.000000 nobinobi-core-0.1.4.8/nobinobi_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      107 2023-06-15 13:28:00.000000 nobinobi-core-0.1.4.8/requirements.txt
+-rw-rw-rw-   0        0        0       63 2023-06-09 08:47:26.000000 nobinobi-core-0.1.4.8/requirements_dev.txt
+-rw-rw-rw-   0        0        0      118 2023-06-15 13:28:00.000000 nobinobi-core-0.1.4.8/requirements_test.txt
+-rw-rw-rw-   0        0        0      427 2023-06-15 13:28:20.899095 nobinobi-core-0.1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     2303 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:28:20.896094 nobinobi-core-0.1.4.8/tests/
+-rw-rw-rw-   0        0        0     2695 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/tests/test_admin.py
+-rw-rw-rw-   0        0        0     1399 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.8/tests/test_models.py
```

### Comparing `nobinobi-core-0.1.4.7/CONTRIBUTING.rst` & `nobinobi-core-0.1.4.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/HISTORY.rst` & `nobinobi-core-0.1.4.8/HISTORY.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+0.1.4.8 (2023-06-15)
+++++++++++++++++++++++
+
+* 0e0b9c2 - Fix requirements
+* 5d60e13 - Remove pipfile
+
 0.1.4.7 (2023-06-12)
 ++++++++++++++++++++++
 
 * 5c74e84 - Update for new cripsy form version
 * Update requirements
 
 0.1.4.6 (2021-09-16)
```

### Comparing `nobinobi-core-0.1.4.7/LICENSE` & `nobinobi-core-0.1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/PKG-INFO` & `nobinobi-core-0.1.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobinobi-core
-Version: 0.1.4.7
+Version: 0.1.4.8
 Summary: Core for application Nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-core
 Author: Florian Alu
 Author-email: alu@prolibre.com
 Keywords: nobinobi-core
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.1
@@ -114,14 +114,20 @@
 
 
 
 
 History
 -------
 
+0.1.4.8 (2023-06-15)
+++++++++++++++++++++++
+
+* 0e0b9c2 - Fix requirements
+* 5d60e13 - Remove pipfile
+
 0.1.4.7 (2023-06-12)
 ++++++++++++++++++++++
 
 * 5c74e84 - Update for new cripsy form version
 * Update requirements
 
 0.1.4.6 (2021-09-16)
```

### Comparing `nobinobi-core-0.1.4.7/README.rst` & `nobinobi-core-0.1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/__init__.py` & `nobinobi-core-0.1.4.8/nobinobi_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.1.4.7'
+__version__ = '0.1.4.8'
```

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/admin.py` & `nobinobi-core-0.1.4.8/nobinobi_core/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/apps.py` & `nobinobi-core-0.1.4.8/nobinobi_core/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/forms.py` & `nobinobi-core-0.1.4.8/nobinobi_core/forms.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/functions.py` & `nobinobi-core-0.1.4.8/nobinobi_core/functions.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-core-0.1.4.8/nobinobi_core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/migrations/0001_initial.py` & `nobinobi-core-0.1.4.8/nobinobi_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/migrations/0002_organisation_organisationclosure.py` & `nobinobi-core-0.1.4.8/nobinobi_core/migrations/0002_organisation_organisationclosure.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/migrations/__init__.py` & `nobinobi-core-0.1.4.8/nobinobi_core/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/models.py` & `nobinobi-core-0.1.4.8/nobinobi_core/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css` & `nobinobi-core-0.1.4.8/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.css` & `nobinobi-core-0.1.4.8/nobinobi_core/static/css/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.min.css` & `nobinobi-core-0.1.4.8/nobinobi_core/static/css/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/static/css/nobinobi_core.css` & `nobinobi-core-0.1.4.8/nobinobi_core/static/css/nobinobi_core.css`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/static/js/bootstrap-datetimepicker.min.js` & `nobinobi-core-0.1.4.8/nobinobi_core/static/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/static/js/moment-with-locales.min.js` & `nobinobi-core-0.1.4.8/nobinobi_core/static/js/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/static/js/nobinobi_core.js` & `nobinobi-core-0.1.4.8/nobinobi_core/static/js/nobinobi_core.js`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/includes/messages.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/includes/messages.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_act.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_act.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_image.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/field_errors_block.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/field_errors_block.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/help_text.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/help_text.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_image.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect_inline.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline_image.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/radioselect_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/sj/collation_general.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/layout/sj/collation_general.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/add_official_holiday.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/nobinobi_core/add_official_holiday.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/base.html` & `nobinobi-core-0.1.4.8/nobinobi_core/templates/nobinobi_core/base.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/__init__.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_dict_value.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/get_dict_value.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_user_method.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/get_user_method.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/math.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/math.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/notifications_tags_custom.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/notifications_tags_custom.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_date_sem.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/remove_date_sem.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_tags_html.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/remove_tags_html.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/startwith.py` & `nobinobi-core-0.1.4.8/nobinobi_core/templatetags/startwith.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/urls.py` & `nobinobi-core-0.1.4.8/nobinobi_core/urls.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/views.py` & `nobinobi-core-0.1.4.8/nobinobi_core/views.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core/widgets.py` & `nobinobi-core-0.1.4.8/nobinobi_core/widgets.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core.egg-info/PKG-INFO` & `nobinobi-core-0.1.4.8/nobinobi_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobinobi-core
-Version: 0.1.4.7
+Version: 0.1.4.8
 Summary: Core for application Nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-core
 Author: Florian Alu
 Author-email: alu@prolibre.com
 Keywords: nobinobi-core
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.1
@@ -114,14 +114,20 @@
 
 
 
 
 History
 -------
 
+0.1.4.8 (2023-06-15)
+++++++++++++++++++++++
+
+* 0e0b9c2 - Fix requirements
+* 5d60e13 - Remove pipfile
+
 0.1.4.7 (2023-06-12)
 ++++++++++++++++++++++
 
 * 5c74e84 - Update for new cripsy form version
 * Update requirements
 
 0.1.4.6 (2021-09-16)
```

### Comparing `nobinobi-core-0.1.4.7/nobinobi_core.egg-info/SOURCES.txt` & `nobinobi-core-0.1.4.8/nobinobi_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/setup.py` & `nobinobi-core-0.1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/tests/test_admin.py` & `nobinobi-core-0.1.4.8/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.7/tests/test_models.py` & `nobinobi-core-0.1.4.8/tests/test_models.py`

 * *Files identical despite different names*

