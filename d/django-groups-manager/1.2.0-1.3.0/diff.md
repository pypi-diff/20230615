# Comparing `tmp/django-groups-manager-1.2.0.tar.gz` & `tmp/django-groups-manager-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-groups-manager-1.2.0.tar", last modified: Sat Jan 29 09:46:23 2022, max compression
+gzip compressed data, was "django-groups-manager-1.3.0.tar", last modified: Thu Jun 15 09:51:53 2023, max compression
```

## Comparing `django-groups-manager-1.2.0.tar` & `django-groups-manager-1.3.0.tar`

### file list

```diff
@@ -1,106 +1,109 @@
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.021574 django-groups-manager-1.2.0/
--rw-r--r--   0 vittorio   (502) staff       (20)       30 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/AUTHORS
--rw-r--r--   0 vittorio   (502) staff       (20)     1084 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/LICENSE
--rw-r--r--   0 vittorio   (502) staff       (20)      217 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/MANIFEST.in
--rw-r--r--   0 vittorio   (502) staff       (20)     5250 2022-01-29 09:46:23.021445 django-groups-manager-1.2.0/PKG-INFO
--rw-r--r--   0 vittorio   (502) staff       (20)     4287 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/README.md
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.008736 django-groups-manager-1.2.0/django_groups_manager.egg-info/
--rw-r--r--   0 vittorio   (502) staff       (20)     5250 2022-01-29 09:46:22.000000 django-groups-manager-1.2.0/django_groups_manager.egg-info/PKG-INFO
--rw-r--r--   0 vittorio   (502) staff       (20)     4398 2022-01-29 09:46:23.000000 django-groups-manager-1.2.0/django_groups_manager.egg-info/SOURCES.txt
--rw-r--r--   0 vittorio   (502) staff       (20)        1 2022-01-29 09:46:22.000000 django-groups-manager-1.2.0/django_groups_manager.egg-info/dependency_links.txt
--rw-r--r--   0 vittorio   (502) staff       (20)       22 2022-01-29 09:46:22.000000 django-groups-manager-1.2.0/django_groups_manager.egg-info/requires.txt
--rw-r--r--   0 vittorio   (502) staff       (20)       15 2022-01-29 09:46:22.000000 django-groups-manager-1.2.0/django_groups_manager.egg-info/top_level.txt
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.008844 django-groups-manager-1.2.0/docs/
--rw-r--r--   0 vittorio   (502) staff       (20)     6823 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/Makefile
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.012358 django-groups-manager-1.2.0/docs/source/
--rw-r--r--   0 vittorio   (502) staff       (20)       57 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/API.rst
--rw-r--r--   0 vittorio   (502) staff       (20)      779 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/auth_integration.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     2287 2022-01-29 09:46:16.000000 django-groups-manager-1.2.0/docs/source/changelog.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     8961 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/conf.py
--rw-r--r--   0 vittorio   (502) staff       (20)     1269 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/custom_member.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     3016 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/custom_signals.rst
--rw-r--r--   0 vittorio   (502) staff       (20)      743 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/expiring_memberships.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     1190 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/index.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     2664 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/intro.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     5681 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/model_mixins.rst
--rw-r--r--   0 vittorio   (502) staff       (20)      478 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/models.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     2362 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/permissions_by_group_type.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     2315 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/permissions_by_role.rst
--rw-r--r--   0 vittorio   (502) staff       (20)      116 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/perms.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     3901 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/proxy_models.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     4575 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/settings.rst
--rw-r--r--   0 vittorio   (502) staff       (20)     1708 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/templates.rst
--rw-r--r--   0 vittorio   (502) staff       (20)      476 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/tests.rst
--rw-r--r--   0 vittorio   (502) staff       (20)       26 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/todo.rst
--rw-r--r--   0 vittorio   (502) staff       (20)      268 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/docs/source/use_cases.rst
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.014268 django-groups-manager-1.2.0/groups_manager/
--rw-r--r--   0 vittorio   (502) staff       (20)       18 2022-01-29 09:46:16.000000 django-groups-manager-1.2.0/groups_manager/__init__.py
--rwxr-xr-x   0 vittorio   (502) staff       (20)      301 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/admin.py
--rw-r--r--   0 vittorio   (502) staff       (20)      803 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/exceptions_gm.py
--rw-r--r--   0 vittorio   (502) staff       (20)     1309 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/forms.py
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.015301 django-groups-manager-1.2.0/groups_manager/migrations/
--rw-r--r--   0 vittorio   (502) staff       (20)     6381 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/migrations/0001_initial.py
--rw-r--r--   0 vittorio   (502) staff       (20)      731 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/migrations/0002_0_4_3_remove_m2m_null.py
--rw-r--r--   0 vittorio   (502) staff       (20)     1858 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/migrations/0003_0_5_0_rename_reverse_relations_with_vars.py
--rw-r--r--   0 vittorio   (502) staff       (20)      503 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/migrations/0004_0_6_0_groupmember_expiration_date.py
--rw-r--r--   0 vittorio   (502) staff       (20)     6590 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/migrations/0005_0_6_2_verbose_name_expiration_date.py
--rw-r--r--   0 vittorio   (502) staff       (20)     1433 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/migrations/0006_1_0_0_default.py
--rw-r--r--   0 vittorio   (502) staff       (20)        0 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/migrations/__init__.py
--rw-r--r--   0 vittorio   (502) staff       (20)    26882 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/models.py
--rw-r--r--   0 vittorio   (502) staff       (20)     4782 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/perms.py
--rw-r--r--   0 vittorio   (502) staff       (20)     1552 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/settings.py
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.006976 django-groups-manager-1.2.0/groups_manager/static/
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.007179 django-groups-manager-1.2.0/groups_manager/static/groups_manager/
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.015380 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/
--rw-r--r--   0 vittorio   (502) staff       (20)      125 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/groups_manager.css
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.016385 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/
--rw-r--r--   0 vittorio   (502) staff       (20)     1695 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.css
--rw-r--r--   0 vittorio   (502) staff       (20)     7128 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.eot
--rw-r--r--   0 vittorio   (502) staff       (20)    39359 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.svg
--rw-r--r--   0 vittorio   (502) staff       (20)     6928 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.ttf
--rw-r--r--   0 vittorio   (502) staff       (20)     3824 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.woff
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.016508 django-groups-manager-1.2.0/groups_manager/static/groups_manager/js/
--rw-r--r--   0 vittorio   (502) staff       (20)        0 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/static/groups_manager/js/groups_manager.js
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.007301 django-groups-manager-1.2.0/groups_manager/templates/
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.007354 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.020977 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/
--rw-r--r--   0 vittorio   (502) staff       (20)       69 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/form_template.html
--rw-r--r--   0 vittorio   (502) staff       (20)      549 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group.html
--rw-r--r--   0 vittorio   (502) staff       (20)      853 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_confirm_delete.html
--rw-r--r--   0 vittorio   (502) staff       (20)     5026 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_detail.html
--rw-r--r--   0 vittorio   (502) staff       (20)      729 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity.html
--rw-r--r--   0 vittorio   (502) staff       (20)      852 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_confirm_delete.html
--rw-r--r--   0 vittorio   (502) staff       (20)     2332 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_detail.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1250 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1244 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_list.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1179 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1502 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_list.html
--rw-r--r--   0 vittorio   (502) staff       (20)      837 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_group_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)      831 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_member_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)      835 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_confirm_delete.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1090 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)      735 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1038 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_confirm_delete.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1847 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_detail.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1389 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1306 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_list.html
--rw-r--r--   0 vittorio   (502) staff       (20)      713 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type.html
--rw-r--r--   0 vittorio   (502) staff       (20)      828 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_confirm_delete.html
--rw-r--r--   0 vittorio   (502) staff       (20)     2291 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_detail.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1285 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1215 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_list.html
--rw-r--r--   0 vittorio   (502) staff       (20)      749 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1755 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager_home.html
--rw-r--r--   0 vittorio   (502) staff       (20)      552 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member.html
--rw-r--r--   0 vittorio   (502) staff       (20)      856 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_confirm_delete.html
--rw-r--r--   0 vittorio   (502) staff       (20)     2939 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_detail.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1220 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_form.html
--rw-r--r--   0 vittorio   (502) staff       (20)     1307 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_list.html
-drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2022-01-29 09:46:23.021263 django-groups-manager-1.2.0/groups_manager/templatetags/
--rw-r--r--   0 vittorio   (502) staff       (20)        0 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templatetags/__init__.py
--rw-r--r--   0 vittorio   (502) staff       (20)     2967 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/templatetags/groups_manager_filters.py
--rw-r--r--   0 vittorio   (502) staff       (20)     4203 2022-01-29 09:21:05.000000 django-groups-manager-1.2.0/groups_manager/urls.py
--rw-r--r--   0 vittorio   (502) staff       (20)      225 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/utils.py
--rw-r--r--   0 vittorio   (502) staff       (20)     8957 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/groups_manager/views.py
--rw-r--r--   0 vittorio   (502) staff       (20)       38 2022-01-29 09:46:23.021623 django-groups-manager-1.2.0/setup.cfg
--rw-r--r--   0 vittorio   (502) staff       (20)     1694 2022-01-29 08:57:29.000000 django-groups-manager-1.2.0/setup.py
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.558282 django-groups-manager-1.3.0/
+-rw-r--r--   0 vittorio   (502) staff       (20)       43 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/AUTHORS
+-rw-r--r--   0 vittorio   (502) staff       (20)     1084 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/LICENSE
+-rw-r--r--   0 vittorio   (502) staff       (20)      217 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/MANIFEST.in
+-rw-r--r--   0 vittorio   (502) staff       (20)     5319 2023-06-15 09:51:53.558131 django-groups-manager-1.3.0/PKG-INFO
+-rw-r--r--   0 vittorio   (502) staff       (20)     4354 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/README.md
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.544007 django-groups-manager-1.3.0/django_groups_manager.egg-info/
+-rw-r--r--   0 vittorio   (502) staff       (20)     5319 2023-06-15 09:51:53.000000 django-groups-manager-1.3.0/django_groups_manager.egg-info/PKG-INFO
+-rw-r--r--   0 vittorio   (502) staff       (20)     4589 2023-06-15 09:51:53.000000 django-groups-manager-1.3.0/django_groups_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 vittorio   (502) staff       (20)        1 2023-06-15 09:51:53.000000 django-groups-manager-1.3.0/django_groups_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 vittorio   (502) staff       (20)       24 2023-06-15 09:51:53.000000 django-groups-manager-1.3.0/django_groups_manager.egg-info/requires.txt
+-rw-r--r--   0 vittorio   (502) staff       (20)       15 2023-06-15 09:51:53.000000 django-groups-manager-1.3.0/django_groups_manager.egg-info/top_level.txt
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.544349 django-groups-manager-1.3.0/docs/
+-rw-r--r--   0 vittorio   (502) staff       (20)     6823 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/Makefile
+-rw-r--r--   0 vittorio   (502) staff       (20)       46 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/requirements_docs.txt
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.548047 django-groups-manager-1.3.0/docs/source/
+-rw-r--r--   0 vittorio   (502) staff       (20)       57 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/API.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)      778 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/auth_integration.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     2623 2023-06-15 09:50:56.000000 django-groups-manager-1.3.0/docs/source/changelog.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     9555 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/conf.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     1243 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/custom_member.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     2995 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/custom_signals.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)      743 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/expiring_memberships.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     1264 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/index.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     2666 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/intro.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     5669 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/model_mixins.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)      478 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/models.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     2328 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/permissions_by_group_type.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     2282 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/permissions_by_role.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)      116 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/perms.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     3901 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/proxy_models.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     4570 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/docs/source/settings.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)     1708 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/templates.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)      476 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/tests.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)       26 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/todo.rst
+-rw-r--r--   0 vittorio   (502) staff       (20)      268 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/docs/source/use_cases.rst
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.549907 django-groups-manager-1.3.0/groups_manager/
+-rw-r--r--   0 vittorio   (502) staff       (20)       18 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/groups_manager/__init__.py
+-rwxr-xr-x   0 vittorio   (502) staff       (20)      301 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/admin.py
+-rw-r--r--   0 vittorio   (502) staff       (20)      803 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/exceptions_gm.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     1309 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/forms.py
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.551320 django-groups-manager-1.3.0/groups_manager/migrations/
+-rw-r--r--   0 vittorio   (502) staff       (20)     6381 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/migrations/0001_initial.py
+-rw-r--r--   0 vittorio   (502) staff       (20)      731 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/migrations/0002_0_4_3_remove_m2m_null.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     1858 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/migrations/0003_0_5_0_rename_reverse_relations_with_vars.py
+-rw-r--r--   0 vittorio   (502) staff       (20)      503 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/migrations/0004_0_6_0_groupmember_expiration_date.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     6590 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/migrations/0005_0_6_2_verbose_name_expiration_date.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     1433 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/migrations/0006_1_0_0_default.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     2405 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/groups_manager/migrations/0007_1_2_0_alter_group_group_entities_alter_group_group_members_and_more.py
+-rw-r--r--   0 vittorio   (502) staff       (20)      517 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/groups_manager/migrations/0008_1_3_0_jsonfield_from_django.py
+-rw-r--r--   0 vittorio   (502) staff       (20)        0 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/migrations/__init__.py
+-rw-r--r--   0 vittorio   (502) staff       (20)    26994 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/groups_manager/models.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     4782 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/perms.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     1552 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/settings.py
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.542350 django-groups-manager-1.3.0/groups_manager/static/
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.542505 django-groups-manager-1.3.0/groups_manager/static/groups_manager/
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.551418 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/
+-rw-r--r--   0 vittorio   (502) staff       (20)      125 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/groups_manager.css
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.552245 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/
+-rw-r--r--   0 vittorio   (502) staff       (20)     1695 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.css
+-rw-r--r--   0 vittorio   (502) staff       (20)     7128 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.eot
+-rw-r--r--   0 vittorio   (502) staff       (20)    39359 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.svg
+-rw-r--r--   0 vittorio   (502) staff       (20)     6928 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.ttf
+-rw-r--r--   0 vittorio   (502) staff       (20)     3824 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.woff
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.552397 django-groups-manager-1.3.0/groups_manager/static/groups_manager/js/
+-rw-r--r--   0 vittorio   (502) staff       (20)        0 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/static/groups_manager/js/groups_manager.js
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.542604 django-groups-manager-1.3.0/groups_manager/templates/
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.542643 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.557649 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/
+-rw-r--r--   0 vittorio   (502) staff       (20)       69 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/form_template.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      549 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      853 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_confirm_delete.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     5026 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_detail.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      729 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      852 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_confirm_delete.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     2332 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_detail.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1250 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1244 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_list.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1179 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1502 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_list.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      837 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_group_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      831 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_member_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      835 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_confirm_delete.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1090 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      735 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1038 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_confirm_delete.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1847 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_detail.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1389 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1306 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_list.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      713 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      828 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_confirm_delete.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     2291 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_detail.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1285 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1215 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_list.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      749 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1755 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager_home.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      552 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member.html
+-rw-r--r--   0 vittorio   (502) staff       (20)      856 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_confirm_delete.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     2939 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_detail.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1220 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_form.html
+-rw-r--r--   0 vittorio   (502) staff       (20)     1307 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_list.html
+drwxr-xr-x   0 vittorio   (502) staff       (20)        0 2023-06-15 09:51:53.557871 django-groups-manager-1.3.0/groups_manager/templatetags/
+-rw-r--r--   0 vittorio   (502) staff       (20)        0 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templatetags/__init__.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     2967 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/templatetags/groups_manager_filters.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     4203 2022-01-29 09:21:05.000000 django-groups-manager-1.3.0/groups_manager/urls.py
+-rw-r--r--   0 vittorio   (502) staff       (20)      225 2022-01-29 08:57:29.000000 django-groups-manager-1.3.0/groups_manager/utils.py
+-rw-r--r--   0 vittorio   (502) staff       (20)     8944 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/groups_manager/views.py
+-rw-r--r--   0 vittorio   (502) staff       (20)       38 2023-06-15 09:51:53.558334 django-groups-manager-1.3.0/setup.cfg
+-rw-r--r--   0 vittorio   (502) staff       (20)     1698 2023-06-15 08:59:37.000000 django-groups-manager-1.3.0/setup.py
```

### Comparing `django-groups-manager-1.2.0/LICENSE` & `django-groups-manager-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/PKG-INFO` & `django-groups-manager-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-groups-manager
-Version: 1.2.0
+Version: 1.3.0
 Summary: Django groups manager through django-mptt.
 Home-page: https://github.com/vittoriozamboni/django-groups-manager
 Author: Vittorio Zamboni
 Author-email: vittorio.zamboni@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # Django groups manager
 
@@ -48,20 +48,20 @@
     'SLUGIFY_FUNCTION': lambda s: slugify(s, to_lower=True),
     'SLUGIFY_USERNAME_FUNCTION': lambda s: slugify(s, to_lower=True, separator="_")
 }
 ```
 
 ## Requirements
 
-    - Python >= 3.5
-    - Django >= 2
+    - Python >= 3.8
+    - Django >= 3.2
     - django-guardian for user permissions
     - jsonfield == 3.1.0
 
-For older versions of Python or Django, please look at 0.6.2 version.
+For older versions of Python or Django, please look at 1.2.0 (Django <3.2, Python < 3.8>) or 0.6.2 version (Django 1.x, Python < 3.5).
 
 ## Installation
 
 Use pip to install `django-groups-manager`:
 
 ```bash
 pip install django-groups-manager
```

### Comparing `django-groups-manager-1.2.0/README.md` & `django-groups-manager-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,20 @@
     'SLUGIFY_FUNCTION': lambda s: slugify(s, to_lower=True),
     'SLUGIFY_USERNAME_FUNCTION': lambda s: slugify(s, to_lower=True, separator="_")
 }
 ```
 
 ## Requirements
 
-    - Python >= 3.5
-    - Django >= 2
+    - Python >= 3.8
+    - Django >= 3.2
     - django-guardian for user permissions
     - jsonfield == 3.1.0
 
-For older versions of Python or Django, please look at 0.6.2 version.
+For older versions of Python or Django, please look at 1.2.0 (Django <3.2, Python < 3.8>) or 0.6.2 version (Django 1.x, Python < 3.5).
 
 ## Installation
 
 Use pip to install `django-groups-manager`:
 
 ```bash
 pip install django-groups-manager
```

### Comparing `django-groups-manager-1.2.0/django_groups_manager.egg-info/PKG-INFO` & `django-groups-manager-1.3.0/django_groups_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-groups-manager
-Version: 1.2.0
+Version: 1.3.0
 Summary: Django groups manager through django-mptt.
 Home-page: https://github.com/vittoriozamboni/django-groups-manager
 Author: Vittorio Zamboni
 Author-email: vittorio.zamboni@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # Django groups manager
 
@@ -48,20 +48,20 @@
     'SLUGIFY_FUNCTION': lambda s: slugify(s, to_lower=True),
     'SLUGIFY_USERNAME_FUNCTION': lambda s: slugify(s, to_lower=True, separator="_")
 }
 ```
 
 ## Requirements
 
-    - Python >= 3.5
-    - Django >= 2
+    - Python >= 3.8
+    - Django >= 3.2
     - django-guardian for user permissions
     - jsonfield == 3.1.0
 
-For older versions of Python or Django, please look at 0.6.2 version.
+For older versions of Python or Django, please look at 1.2.0 (Django <3.2, Python < 3.8>) or 0.6.2 version (Django 1.x, Python < 3.5).
 
 ## Installation
 
 Use pip to install `django-groups-manager`:
 
 ```bash
 pip install django-groups-manager
```

### Comparing `django-groups-manager-1.2.0/django_groups_manager.egg-info/SOURCES.txt` & `django-groups-manager-1.3.0/django_groups_manager.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 django_groups_manager.egg-info/PKG-INFO
 django_groups_manager.egg-info/SOURCES.txt
 django_groups_manager.egg-info/dependency_links.txt
 django_groups_manager.egg-info/requires.txt
 django_groups_manager.egg-info/top_level.txt
 docs/Makefile
+docs/requirements_docs.txt
 docs/source/API.rst
 docs/source/auth_integration.rst
 docs/source/changelog.rst
 docs/source/conf.py
 docs/source/custom_member.rst
 docs/source/custom_signals.rst
 docs/source/expiring_memberships.rst
@@ -41,14 +42,16 @@
 groups_manager/views.py
 groups_manager/migrations/0001_initial.py
 groups_manager/migrations/0002_0_4_3_remove_m2m_null.py
 groups_manager/migrations/0003_0_5_0_rename_reverse_relations_with_vars.py
 groups_manager/migrations/0004_0_6_0_groupmember_expiration_date.py
 groups_manager/migrations/0005_0_6_2_verbose_name_expiration_date.py
 groups_manager/migrations/0006_1_0_0_default.py
+groups_manager/migrations/0007_1_2_0_alter_group_group_entities_alter_group_group_members_and_more.py
+groups_manager/migrations/0008_1_3_0_jsonfield_from_django.py
 groups_manager/migrations/__init__.py
 groups_manager/static/groups_manager/css/groups_manager.css
 groups_manager/static/groups_manager/css/icons/groups_manager.css
 groups_manager/static/groups_manager/css/icons/groups_manager.eot
 groups_manager/static/groups_manager/css/icons/groups_manager.svg
 groups_manager/static/groups_manager/css/icons/groups_manager.ttf
 groups_manager/static/groups_manager/css/icons/groups_manager.woff
```

### Comparing `django-groups-manager-1.2.0/docs/Makefile` & `django-groups-manager-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/docs/source/auth_integration.rst` & `django-groups-manager-1.3.0/docs/source/auth_integration.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Django auth models integration
 ==============================
 
-It is possibile to auto-map ``Group`` and ``Member`` instances with ``django.contrib.auth.models`` ``Group`` and ``User``.
+It is possible to auto-map ``Group`` and ``Member`` instances with ``django.contrib.auth.models`` ``Group`` and ``User``.
 To enable mapping, ``"AUTH_MODELS_SYNC"`` setting must be set to ``True`` (default: ``False``), and also ``Group`` and ``Member`` instances attribute ``django_auth_sync`` (that is ``True`` by default).
 
 Add to your ``settings`` file::
 
 	
 	GROUPS_MANAGER = {
 	    'AUTH_MODELS_SYNC': True,
```

### Comparing `django-groups-manager-1.2.0/docs/source/changelog.rst` & `django-groups-manager-1.3.0/docs/source/changelog.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 Changelog
 =========
-- 22-01-29 (1.2.0):
+
+- 2023-06-15 (1.3.0):
+    - Verified compatibility with Django up to 4.2 and Python up to 3.11.
+    - Dropped compatibility guarantees with anything older than Django 3.2 and Python 3.8.
+    - Use Django's build in models.JSONField instead of the one from the jsonfield package.
+    - Minor documentation changes
+
+- 2022-01-29 (1.2.0):
     - Support Django 4: uses correct url parser function `re_path` (see issue #60, thank you Lukas Hennies!)
     - Updated intro.rst, fixed wrong example (see issue #57, thank you Areski Belaid!)
 
-- 21-04-11 (1.1.0):
+- 2021-04-11 (1.1.0):
     - Removed `awesome-slugify` from requirements. It needs to be installed separately due to his licence (see issue #54, thank you BoPeng!);
     - Added a new settings to customize the slugify functions for username and other cases.
 
-- 20-06-17 (1.0.2):
+- 2020-06-17 (1.0.2):
     - Changed jsonfield2 to jsonfield in requirements and tests (see issue #49, thank you ioio!);
 
-- 20-03-07 (1.0.1):
+- 2020-03-07 (1.0.1):
     - Amended Django 3 deprecations
     - Documentation changes
 
-- 19-12-10 (1.0.0):
+- 2019-12-10 (1.0.0):
     - Dropped support for Django < 2 and Python 2.*
 
-- 19-01-11 (0.6.2):
+- 2019-01-11 (0.6.2):
     - Added migrations for expiration_date and verbose names
 
-- 18-01-18 (0.6.1):
+- 2018-01-18 (0.6.1):
     - Added support for Django 2
 
-- 17-12-09 (0.6.0) (thank you Oskar Persson!):
+- 2017-12-09 (0.6.0) (thank you Oskar Persson!):
     - Added group type permission handling
     - Added ``expiration_date`` attribute
     - Added support to django-jsonfield
 
-- 16-11-08 (0.5.0):
+- 2016-11-08 (0.5.0):
     - Added models mixins
     - Removed compatibility for Django < 1.7
 
-- 16-10-10 (0.4.2):
+- 2016-10-10 (0.4.2):
     - Added initial migration
     - Removed null attributes from m2m relations
 
-- 16-04-19 (0.4.1):
+- 2016-04-19 (0.4.1):
     - Removed unique to group name (this cause issues when subclassing, since it does not allows to have same names for different models)
     - Fixed issue with python 3 compatibility in templatetags (thank you Josh Manning!)
 
-- 16-03-01 (0.4.0):
+- 2016-03-01 (0.4.0):
     - Added kwargs to signals for override settings parameters
     - Added remove_member to group as a method (previously must be done manually)
 
-- 16-02-25 (0.3.0):
+- 2016-02-25 (0.3.0):
     - Added permissions assignment to groups
     - Added support for Django 1.8 and 1.9
 
-- 15-05-05 (0.2.1):
+- 2015-05-05 (0.2.1):
     - Added 'add' to default permissions
 
-- 15-05-05 (0.2.0):
+- 2015-05-05 (0.2.0):
     - Changed retrieval of permission's name: 'view', 'change' and 'delete' will be translated to '<name>_<model_name>', the others are left untouched (see :ref:`permission name policy <permission-name-policy>`)
-    - Added GroupsManagerMeta class to Group that allows to specify the member model to use for members list (see :ref:`custom Member model <custom-member-model>`)
+    - Added GroupsManagerMeta class to Group that allows to specify the member model to use for members list (see `custom Member model <custom_member>`)
 
-- 14-10-29 (0.1.0): Initial version
+- 2014-10-29 (0.1.0): Initial version
```

### Comparing `django-groups-manager-1.2.0/docs/source/conf.py` & `django-groups-manager-1.3.0/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import sys
 import os
 from datetime import datetime
 
+
 base_path = os.path.abspath(os.path.join(os.path.dirname(__file__), '../../'))
 sys.path.insert(1, base_path)
 sys.path.insert(1, os.path.join(base_path, 'testproject'))
-os.environ['DJANGO_SETTINGS_MODULE'] = 'testproject.settings'
+
 
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 
@@ -33,17 +34,19 @@
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
+    "sphinx.ext.autosectionlabel",
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
     'sphinx.ext.viewcode',
+    'sphinxcontrib_django2',
 ]
 
 todo_include_todos = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
@@ -59,23 +62,27 @@
 # General information about the project.
 project = u'Django Groups Manager'
 copyright = u'2014-%s, Vittorio Zamboni' % datetime.today().year
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
-#
-# The short X.Y version.
-version = '1.0'
+
 # The full version, including alpha/beta/rc tags.
-release = '1.0.0'
+try:
+    from groups_manager import VERSION
+    release = VERSION
+except ImportError:
+    release = "0.0.0"
+# The short X.Y.Z version. (will be shown in docs header)
+version = '.'.join(release.split('.')[:3])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
 
@@ -273,7 +280,20 @@
 #texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
+
+# -- Options for sphinx.ext.autosectionlabel ------------------------------
+
+# Make sure the ref targets created by are unique
+autosectionlabel_prefix_document = True
+
+# -- Options for sphinxcontrib-django2 ------------------------------------
+
+# Configure the path to the Django settings module
+django_settings = 'testproject.settings'
+autodoc_default_options = {
+    "exclude-members": "__weakref__,DoesNotExist,MultipleObjectsReturned"
+}
```

### Comparing `django-groups-manager-1.2.0/docs/source/custom_member.rst` & `django-groups-manager-1.3.0/docs/source/custom_member.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-.. _custom-member-model:
-
 Custom member model
 -------------------
 
 By default, ``Group``'s attribute ``members`` returns a list of ``Member`` instances.
 If you want to create also a custom Member model in addition to custom Group, maybe you
 want to obtain a list of custom Member model instances with ``members`` attribute.
 This can be obtained with ``GroupsManagerMeta``'s ``member_model`` attribute. This class
```

### Comparing `django-groups-manager-1.2.0/docs/source/custom_signals.rst` & `django-groups-manager-1.3.0/docs/source/custom_signals.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-.. _custom-signals:
-
 Custom signals
 --------------
 
 If you redefine models via proxy or subclass and you need to manage sync permissions with
 a different setting (like ``MY_APP['AUTH_MODELS_SYNC']`` you need to use different signals functions
 when saving objects and relations.
 Signals functions accept kwargs:
```

### Comparing `django-groups-manager-1.2.0/docs/source/expiring_memberships.rst` & `django-groups-manager-1.3.0/docs/source/expiring_memberships.rst`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/docs/source/index.rst` & `django-groups-manager-1.3.0/docs/source/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
    sphinx-quickstart on Tue Oct 28 13:53:01 2014.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Django Groups Manager
 =====================
 
-Django Groups Manager allows to manage groups based on `django-mptt <https://github.com/django-mptt/django-mptt>`_.
-
-The application offers three main classes: `Group`, `Member` and `GroupMember`.
-It's possible to *map* groups and members with Django's auth models, in order to use external applcations such `django-guardian <https://github.com/lukaszb/django-guardian>`_ to handle permissions.
+Django Groups Manager allows to manage groups, group membership and members. 
+It's possible to *map* groups and members with Django's auth models, in order to use external applications such `django-guardian <https://github.com/lukaszb/django-guardian>`_ to handle permissions.
+Groups can have a hierarchical structure based on `django-mptt <https://github.com/django-mptt/django-mptt>`_.
 
+The application offers three main classes: `Group`, `Member` and `GroupMember`. 
 The basic idea of Groups is that each `Group` instance could have a `Group` instance as parent (this relation is managed via django-mptt).
 
 The code is hosted on `github <https://github.com/vittoriozamboni/django-groups-manager>`_.
 
 Documentation
 =============
```

### Comparing `django-groups-manager-1.2.0/docs/source/intro.rst` & `django-groups-manager-1.3.0/docs/source/intro.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Installation
 ============
 
 Requirements
-    - Python >= 3.5
-    - Django >= 2
+    - Python >= 3.8
+    - Django >= 3.2
 
 First of all, install the latest build with ``pip``::
 
    pip install django-groups-manager
    # and, in case you want per-object permissions related features
    pip install django-guardian
```

### Comparing `django-groups-manager-1.2.0/docs/source/model_mixins.rst` & `django-groups-manager-1.3.0/docs/source/model_mixins.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
  - all fields are in the same table (with subclassed models, only extra fields are stored in the subclass table);
  - better for shared applications (the "original" django-groups-manager tables don't share entries from different models).
 
 Cons:
  - all external foreign keys must be declared in the concrete model;
  - all signals must be declared with concrete models.
 
-Model mixins example
---------------------
+Mixins Example
+^^^^^^^^^^^^^^
 
 The following models allow to manage a set of Organizations with related members (from ``organization`` app).
 In this example, a ``last_edit_date`` is added to models, and member display name has the user email (if defined).
 
 **1) Define models in models.py**::
 
     from groups_manager.models import GroupMixin, MemberMixin, GroupMemberMixin, GroupMemberRoleMixin, \
```

### Comparing `django-groups-manager-1.2.0/docs/source/permissions_by_group_type.rst` & `django-groups-manager-1.3.0/docs/source/permissions_by_group_type.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-.. _custom-permissions-by-group-type:
-
 Resource assignment via group type permissions
-----------------------------------------
+----------------------------------------------
 
 Permissions can also be applied to related groups filtered by group types.
 Instead of simply using a list to specify permissions one can use a ``dict`` to
 specify which group types get which permissions.
 
 
 Example
-#######
-
+^^^^^^^
 
 John Money is the commercial referent of the company; Patrick Html is the web
 developer. John and Patrick can view the site, but only Patrick can change and
 delete it.
 
 **1) Define models in models.py**::
```

### Comparing `django-groups-manager-1.2.0/docs/source/permissions_by_role.rst` & `django-groups-manager-1.3.0/docs/source/permissions_by_role.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-.. _custom-permissions-by-role:
-
 Resource assignment via role permissions
 ----------------------------------------
 
 John Money is the commercial referent of the company; Patrick Html is the web
 developer. The company has only one group, but different roles.
 John can view and sell the site, and Patrick can view, change and delete the site.
```

### Comparing `django-groups-manager-1.2.0/docs/source/proxy_models.rst` & `django-groups-manager-1.3.0/docs/source/proxy_models.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Projects management with Proxy Models
 -------------------------------------
 
 John Boss is the project leader. Marcus Worker and Julius Backend are the
 django backend guys; Teresa Html is the front-end developer and Jack College is the
 student that has to learn to write good backends.
-The Celery pipeline is owned by Marcus, and Jack must see it without intercations.
+The Celery pipeline is owned by Marcus, and Jack must see it without interactions.
 Teresa can't see the pipeline, but John has full permissions as project leader.
 As part of the backend group, Julius has the right of viewing and editing, but not to
 stop (delete) the pipeline.
 
 **1) Define models in models.py**::
 
     from groups_manager.models import Group, GroupType
```

### Comparing `django-groups-manager-1.2.0/docs/source/settings.rst` & `django-groups-manager-1.3.0/docs/source/settings.rst`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 	- ``"groups_downstream"``: a string. This object-permissions are assigned to the descendants groups (default: ``[]``)
 	- ``"groups_siblings"``: a string. This object-permissions are assigned to the siblings groups (default: ``['view']``)
 
 .. _permission-name-policy:
 
 .. note::
    The four special permission names ``"add"``, ``"view"``, ``"change"``,  and ``"delete"`` are translated to ``<permission>_<model_name>`` string during permission's name lookup.
-   This allows to use a standard permission policy (*view*, *change*, *delete*) but also allows to use :ref:`custom permissions <custom-permissions-by-role>`.
+   This allows to use a standard permission policy (*view*, *change*, *delete*) but also allows to use `custom permissions <custom-permissions-by-role>`.
 
 An example of permissions assigned by role can be found on use cases.
 
 Templates
 ---------
 
 - ``TEMPLATE_STYLE``: name of the templates folder inside "groups_manager". By default is ``"bootstrap3"``, this means that templates are searched inside folder "groups_manager/bootstrap3"
```

### Comparing `django-groups-manager-1.2.0/docs/source/templates.rst` & `django-groups-manager-1.3.0/docs/source/templates.rst`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/exceptions_gm.py` & `django-groups-manager-1.3.0/groups_manager/exceptions_gm.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/forms.py` & `django-groups-manager-1.3.0/groups_manager/forms.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/migrations/0001_initial.py` & `django-groups-manager-1.3.0/groups_manager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/migrations/0002_0_4_3_remove_m2m_null.py` & `django-groups-manager-1.3.0/groups_manager/migrations/0002_0_4_3_remove_m2m_null.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/migrations/0003_0_5_0_rename_reverse_relations_with_vars.py` & `django-groups-manager-1.3.0/groups_manager/migrations/0003_0_5_0_rename_reverse_relations_with_vars.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/migrations/0005_0_6_2_verbose_name_expiration_date.py` & `django-groups-manager-1.3.0/groups_manager/migrations/0005_0_6_2_verbose_name_expiration_date.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/migrations/0006_1_0_0_default.py` & `django-groups-manager-1.3.0/groups_manager/migrations/0006_1_0_0_default.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/models.py` & `django-groups-manager-1.3.0/groups_manager/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from collections import OrderedDict
-from importlib import import_module
 from uuid import uuid4
 import warnings
 
 from django.contrib.auth.models import Group as DjangoGroup
 from django.db import models
 from django.db.models.signals import post_save, post_delete
 from django.utils.translation import gettext_lazy as _
@@ -11,15 +10,14 @@
 from django.apps import apps
 django_get_model = apps.get_model
 
 from django.conf import settings as django_settings
 from django.contrib.auth.models import User as DefaultUser
 DjangoUser = getattr(django_settings, 'AUTH_USER_MODEL', DefaultUser)
 
-from jsonfield import JSONField
 from mptt.models import MPTTModel, TreeForeignKey
 
 from groups_manager import exceptions_gm
 from groups_manager.perms import assign_object_to_member, assign_object_to_group
 from groups_manager.settings import GROUPS_MANAGER
 
 slugify = GROUPS_MANAGER['SLUGIFY_FUNCTION']
@@ -67,17 +65,14 @@
 
     django_auth_sync = models.BooleanField(_('django auth sync'), default=True, blank=True)
 
     class Meta:
         abstract = True
         ordering = ('last_name', 'first_name')
 
-    def __unicode__(self):
-        return self.full_name
-
     def __str__(self):
         return self.full_name
 
     def save(self, *args, **kwargs):
         if not self.username:
             self.username = slugify_username(self.full_name)
         super(MemberMixin, self).save(*args, **kwargs)
@@ -127,14 +122,15 @@
 
 
 class Member(MemberMixin):
 
     django_user = models.ForeignKey(DjangoUser, null=True, blank=True, on_delete=models.SET_NULL,
                                     related_name='%(app_label)s_%(class)s_set', verbose_name=_('django user'))
 
+    # This class Meta is not necessary acc. to https://docs.djangoproject.com/en/4.2/topics/db/models/#meta-inheritance
     class Meta(MemberMixin.Meta):
         abstract = False
 
 
 def member_save(sender, instance, created, *args, **kwargs):
     """
     Add User to Django Users
@@ -178,15 +174,15 @@
             instance.django_user.last_name = instance.last_name
             instance.django_user.email = instance.email
             instance.django_user.save()
 
 
 def member_delete(sender, instance, *args, **kwargs):
     """
-    Remove the related Django Group
+    Remove the related Django User
     """
     get_auth_models_sync_func = kwargs.get('get_auth_models_sync_func',
                                            get_auth_models_sync_func_default)
     if get_auth_models_sync_func(instance) and instance.django_auth_sync:
         if instance.django_user:
             django_user = instance.django_user
             django_user.delete()
@@ -309,15 +305,15 @@
     :Parameters:
       - `name`: (required)
       - `codename`: NON unique codename; if not set, it's autogenerated by slugifying the label
         (lower case)
       - `description`: text field
       - `comment`: text field
       - `full_name`: auto generated full name starting from tree root
-      - `properties`: jsonfield properties
+      - `properties`: JSONField properties
       - `group_members`: m2m to Member, through GroupMember model (related name: `groups`)
       - `group_type`: foreign key to GroupType (related name: `groups`)
       - `group_entities`: m2m to GroupEntity (related name: `groups`)
       - `django_group`: django auth related group
       - `django_auth_sync`: synchronize or not the group (if setting DJANGO_AUTH_SYNC is True)
         (default: True)
       - `level`: ``django-mptt`` level attribute
@@ -332,18 +328,18 @@
     codename = models.SlugField(_('codename'), blank=True, max_length=255)
     description = models.TextField(_('description'), default='', blank=True)
     comment = models.TextField(_('comment'), default='', blank=True)
     parent = TreeForeignKey('self', null=True, blank=True, on_delete=models.CASCADE,
                             related_name='sub_%(app_label)s_%(class)s_set', verbose_name=_('parent'))
     full_name = models.CharField(_('full name'), max_length=255, default='', blank=True)
     try:
-        properties = JSONField(_('properties'), default={}, blank=True,
+        properties = models.JSONField(_('properties'), default=dict, blank=True,
                                 load_kwargs={'object_pairs_hook': OrderedDict})
     except TypeError:
-        properties = JSONField(_('properties'), default={}, blank=True)
+        properties = models.JSONField(_('properties'), default=dict, blank=True)
 
     django_auth_sync = models.BooleanField(default=True, blank=True)
 
     class Meta:
         abstract = True
         ordering = ('name', )
 
@@ -399,15 +395,15 @@
                 # subclassed
                 else:
                     members = list(member_model.objects.filter(
                         member_ptr__in=members_relation.all()))
         else:
             members = [gm.member for gm in group_member_model.objects.filter(group=self)]
         if subgroups:
-            for subgroup in self.subgroups.all():
+            for subgroup in self.sub_groups_manager_group_set.all():
                 members += subgroup.members
         members = list(set(members))
         return members
 
     @property
     def members(self):
         """Return group members. """
@@ -426,15 +422,15 @@
         """Return group entities.
 
         :Parameters:
           - `subgroups`: return also descendants entities (default: `False`)
         """
         entities = list(self.group_entities.all())
         if subgroups:
-            for subgroup in self.subgroups.all():
+            for subgroup in self.sub_groups_manager_group_set.all():
                 entities += subgroup.entities
             entities = list(set(entities))
         return entities
 
     @property
     def entities(self):
         """Return group entities."""
@@ -616,15 +612,16 @@
 
 
 class GroupMemberMixin(models.Model):
 
     class Meta:
         abstract = True
         ordering = ('group', 'member')
-        # BUG in Django: https://code.djangoproject.com/ticket/16732
+        # BUG in Django: "Unable to have abstract model with unique_together"
+        # https://code.djangoproject.com/ticket/16732
         # unique_together = (('group', 'member'), )
 
     def __unicode__(self):
         return '%s - %s' % (self.group.name, self.member.full_name)
 
     def __str__(self):
         return '%s - %s' % (self.group.name, self.member.full_name)
```

### Comparing `django-groups-manager-1.2.0/groups_manager/perms.py` & `django-groups-manager-1.3.0/groups_manager/perms.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/settings.py` & `django-groups-manager-1.3.0/groups_manager/settings.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.css` & `django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.css`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.eot` & `django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.eot`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.svg` & `django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.svg`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.ttf` & `django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.ttf`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/static/groups_manager/css/icons/groups_manager.woff` & `django-groups-manager-1.3.0/groups_manager/static/groups_manager/css/icons/groups_manager.woff`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_confirm_delete.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_detail.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_detail.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_confirm_delete.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_detail.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_detail.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_list.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_entity_list.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_list.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_list.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_group_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_group_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_member_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_add_member_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_confirm_delete.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_confirm_delete.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_detail.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_detail.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_list.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_member_role_list.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_confirm_delete.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_detail.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_detail.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/group_type_list.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/group_type_list.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager_home.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/groups_manager_home.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_confirm_delete.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_detail.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_detail.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_form.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_form.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templates/groups_manager/bootstrap3/member_list.html` & `django-groups-manager-1.3.0/groups_manager/templates/groups_manager/bootstrap3/member_list.html`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/templatetags/groups_manager_filters.py` & `django-groups-manager-1.3.0/groups_manager/templatetags/groups_manager_filters.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/urls.py` & `django-groups-manager-1.3.0/groups_manager/urls.py`

 * *Files identical despite different names*

### Comparing `django-groups-manager-1.2.0/groups_manager/views.py` & `django-groups-manager-1.3.0/groups_manager/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import json
-
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.http import HttpResponseRedirect
 from django.urls import reverse
 from django.views.generic import ListView, DetailView, CreateView, UpdateView, DeleteView
 from django.views.generic.base import TemplateView
 
 from groups_manager import models, forms, settings
```

### Comparing `django-groups-manager-1.2.0/setup.py` & `django-groups-manager-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 from groups_manager import VERSION
 
 install_requires=[
-    'django>=2',
+    'django>=3.2',
     'django-mptt',
 ]
 
 if not _HAD_JSONFIELD:
     install_requires.append('jsonfield')
 
 setup(
@@ -45,14 +45,14 @@
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Security',
     ],
 )
```

