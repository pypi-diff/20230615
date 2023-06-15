# Comparing `tmp/django-content-blocks-1.3.3.tar.gz` & `tmp/django-content-blocks-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-content-blocks-1.3.3.tar", last modified: Mon Jun  5 17:04:46 2023, max compression
+gzip compressed data, was "django-content-blocks-1.3.4.tar", last modified: Wed Jun 14 16:43:11 2023, max compression
```

## Comparing `django-content-blocks-1.3.3.tar` & `django-content-blocks-1.3.4.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.821662 django-content-blocks-1.3.3/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     4662 2023-06-05 17:04:46.821797 django-content-blocks-1.3.3/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     3166 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.795332 django-content-blocks-1.3.3/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.3/content_blocks/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/abstract_models.py
--rw-r--r--   0 quantra    (501) staff       (20)    11872 2023-06-04 21:01:31.000000 django-content-blocks-1.3.3/content_blocks/admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     5070 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/admin_forms.py
--rw-r--r--   0 quantra    (501) staff       (20)      952 2023-06-04 20:53:17.000000 django-content-blocks-1.3.3/content_blocks/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     1591 2023-06-03 20:41:24.000000 django-content-blocks-1.3.3/content_blocks/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.3/content_blocks/fields.py
--rw-r--r--   0 quantra    (501) staff       (20)     8031 2023-05-24 23:15:33.000000 django-content-blocks-1.3.3/content_blocks/forms.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.795839 django-content-blocks-1.3.3/content_blocks/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.3/content_blocks/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.797384 django-content-blocks-1.3.3/content_blocks/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.3/content_blocks/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/management/commands/clear_content_blocks_cache.py
--rw-r--r--   0 quantra    (501) staff       (20)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/management/commands/export_content_block_templates.py
--rw-r--r--   0 quantra    (501) staff       (20)     1461 2023-05-24 11:55:23.000000 django-content-blocks-1.3.3/content_blocks/management/commands/import_content_block_templates.py
--rw-r--r--   0 quantra    (501) staff       (20)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/management/commands/set_content_blocks_cache.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.798514 django-content-blocks-1.3.3/content_blocks/migrations/
--rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.3/content_blocks/migrations/0001_initial.py
--rw-r--r--   0 quantra    (501) staff       (20)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.3/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
--rw-r--r--   0 quantra    (501) staff       (20)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.3/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.3/content_blocks/migrations/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    23959 2023-06-04 20:37:37.000000 django-content-blocks-1.3.3/content_blocks/models.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.800017 django-content-blocks-1.3.3/content_blocks/services/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-05-23 18:56:52.000000 django-content-blocks-1.3.3/content_blocks/services/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    12032 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/services/content_block.py
--rw-r--r--   0 quantra    (501) staff       (20)     1141 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/services/content_block_parent.py
--rw-r--r--   0 quantra    (501) staff       (20)     5283 2023-05-24 11:55:40.000000 django-content-blocks-1.3.3/content_blocks/services/content_block_template.py
--rw-r--r--   0 quantra    (501) staff       (20)     3312 2023-06-04 21:01:31.000000 django-content-blocks-1.3.3/content_blocks/signals.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.787085 django-content-blocks-1.3.3/content_blocks/static/
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.800302 django-content-blocks-1.3.3/content_blocks/static/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.801746 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      709 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/content_block_template_admin.css
--rw-r--r--   0 quantra    (501) staff       (20)    10043 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/content_blocks.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.788454 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.803184 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/
--rw-r--r--   0 quantra    (501) staff       (20)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/light.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
--rw-r--r--   0 quantra    (501) staff       (20)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.804221 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/
--rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.805432 django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/
--rw-r--r--   0 quantra    (501) staff       (20)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
--rw-r--r--   0 quantra    (501) staff       (20)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.806108 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/
--rw-r--r--   0 quantra    (501) staff       (20)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
--rw-r--r--   0 quantra    (501) staff       (20)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.806747 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/
--rw-r--r--   0 quantra    (501) staff       (20)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
--rw-r--r--   0 quantra    (501) staff       (20)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.808529 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/
--rw-r--r--   0 quantra    (501) staff       (20)     1894 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/admin_choices_widget.js
--rw-r--r--   0 quantra    (501) staff       (20)      980 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/ajax_setup.js
--rw-r--r--   0 quantra    (501) staff       (20)    19428 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_editor.js
--rw-r--r--   0 quantra    (501) staff       (20)     2015 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_template_admin.js
--rw-r--r--   0 quantra    (501) staff       (20)     2201 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/popup.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.809154 django-content-blocks-1.3.3/content_blocks/templates/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.3/content_blocks/templates/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/base.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.810157 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.810989 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/
--rw-r--r--   0 quantra    (501) staff       (20)      317 2023-06-04 15:21:52.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
--rw-r--r--   0 quantra    (501) staff       (20)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
--rw-r--r--   0 quantra    (501) staff       (20)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/content_block_collection.html
--rw-r--r--   0 quantra    (501) staff       (20)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/content_block_preview.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.812599 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/
--rw-r--r--   0 quantra    (501) staff       (20)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/base.html
--rw-r--r--   0 quantra    (501) staff       (20)     2656 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form.html
--rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
--rw-r--r--   0 quantra    (501) staff       (20)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_forms.html
--rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/editor.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.813684 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/
--rw-r--r--   0 quantra    (501) staff       (20)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/delete_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.814268 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/
--rw-r--r--   0 quantra    (501) staff       (20)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/checkbox.html
--rw-r--r--   0 quantra    (501) staff       (20)      497 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/default.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.815251 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/
--rw-r--r--   0 quantra    (501) staff       (20)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/base.html
--rw-r--r--   0 quantra    (501) staff       (20)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
--rw-r--r--   0 quantra    (501) staff       (20)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/image.html
--rw-r--r--   0 quantra    (501) staff       (20)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/video.html
--rw-r--r--   0 quantra    (501) staff       (20)      442 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/loader.html
--rw-r--r--   0 quantra    (501) staff       (20)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/popup.html
--rw-r--r--   0 quantra    (501) staff       (20)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/reset_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.816106 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/
--rw-r--r--   0 quantra    (501) staff       (20)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/choices.html
--rw-r--r--   0 quantra    (501) staff       (20)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/clearable_file.html
--rw-r--r--   0 quantra    (501) staff       (20)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.817441 django-content-blocks-1.3.3/content_blocks/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.3/content_blocks/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.3/content_blocks/templatetags/content_block_admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/templatetags/content_blocks.py
--rw-r--r--   0 quantra    (501) staff       (20)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.3/content_blocks/urls.py
--rw-r--r--   0 quantra    (501) staff       (20)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/views.py
--rw-r--r--   0 quantra    (501) staff       (20)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.3.3/content_blocks/widgets.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.821517 django-content-blocks-1.3.3/django_content_blocks.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     4662 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     4653 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       55 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       23 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/top_level.txt
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1945 2023-06-05 17:04:46.825328 django-content-blocks-1.3.3/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.3/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.340798 django-content-blocks-1.3.4/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     7611 2023-06-14 16:43:11.340938 django-content-blocks-1.3.4/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     6072 2023-06-10 15:19:48.000000 django-content-blocks-1.3.4/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.305933 django-content-blocks-1.3.4/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.4/content_blocks/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/abstract_models.py
+-rw-r--r--   0 quantra    (501) staff       (20)    11969 2023-06-06 15:28:11.000000 django-content-blocks-1.3.4/content_blocks/admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     5301 2023-06-06 15:28:11.000000 django-content-blocks-1.3.4/content_blocks/admin_forms.py
+-rw-r--r--   0 quantra    (501) staff       (20)      952 2023-06-04 20:53:17.000000 django-content-blocks-1.3.4/content_blocks/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1591 2023-06-03 20:41:24.000000 django-content-blocks-1.3.4/content_blocks/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.4/content_blocks/fields.py
+-rw-r--r--   0 quantra    (501) staff       (20)     8031 2023-05-24 23:15:33.000000 django-content-blocks-1.3.4/content_blocks/forms.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.306728 django-content-blocks-1.3.4/content_blocks/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.4/content_blocks/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.308931 django-content-blocks-1.3.4/content_blocks/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.4/content_blocks/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/management/commands/clear_content_blocks_cache.py
+-rw-r--r--   0 quantra    (501) staff       (20)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/management/commands/export_content_block_templates.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1461 2023-05-24 11:55:23.000000 django-content-blocks-1.3.4/content_blocks/management/commands/import_content_block_templates.py
+-rw-r--r--   0 quantra    (501) staff       (20)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/management/commands/set_content_blocks_cache.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.310628 django-content-blocks-1.3.4/content_blocks/migrations/
+-rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.4/content_blocks/migrations/0001_initial.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.4/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.4/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.4/content_blocks/migrations/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    23959 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/models.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.312838 django-content-blocks-1.3.4/content_blocks/services/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-05-23 18:56:52.000000 django-content-blocks-1.3.4/content_blocks/services/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12059 2023-06-14 16:14:38.000000 django-content-blocks-1.3.4/content_blocks/services/content_block.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1141 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/services/content_block_parent.py
+-rw-r--r--   0 quantra    (501) staff       (20)     5283 2023-05-24 11:55:40.000000 django-content-blocks-1.3.4/content_blocks/services/content_block_template.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3312 2023-06-04 21:01:31.000000 django-content-blocks-1.3.4/content_blocks/signals.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.295842 django-content-blocks-1.3.4/content_blocks/static/
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.313476 django-content-blocks-1.3.4/content_blocks/static/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.314875 django-content-blocks-1.3.4/content_blocks/static/content_blocks/css/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/css/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)     1114 2023-06-06 15:28:11.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/css/content_block_template_admin.css
+-rw-r--r--   0 quantra    (501) staff       (20)    10043 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/css/content_blocks.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.297239 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.316673 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/
+-rw-r--r--   0 quantra    (501) staff       (20)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/light.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
+-rw-r--r--   0 quantra    (501) staff       (20)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.318292 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/webfonts/
+-rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.319500 django-content-blocks-1.3.4/content_blocks/static/content_blocks/iframeresizer/
+-rw-r--r--   0 quantra    (501) staff       (20)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
+-rw-r--r--   0 quantra    (501) staff       (20)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.320060 django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryform/
+-rw-r--r--   0 quantra    (501) staff       (20)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
+-rw-r--r--   0 quantra    (501) staff       (20)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.320621 django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryui/
+-rw-r--r--   0 quantra    (501) staff       (20)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.322708 django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/
+-rw-r--r--   0 quantra    (501) staff       (20)     1894 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/admin_choices_widget.js
+-rw-r--r--   0 quantra    (501) staff       (20)      980 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/ajax_setup.js
+-rw-r--r--   0 quantra    (501) staff       (20)    19428 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/content_block_editor.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2015 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/content_block_template_admin.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2201 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/popup.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.323312 django-content-blocks-1.3.4/content_blocks/templates/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.4/content_blocks/templates/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/base.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.324161 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.325264 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/admin/
+-rw-r--r--   0 quantra    (501) staff       (20)      317 2023-06-04 15:21:52.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
+-rw-r--r--   0 quantra    (501) staff       (20)      197 2023-06-06 15:28:11.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/admin/content_block_template_field_delete_checkbox.html
+-rw-r--r--   0 quantra    (501) staff       (20)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
+-rw-r--r--   0 quantra    (501) staff       (20)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/content_block_collection.html
+-rw-r--r--   0 quantra    (501) staff       (20)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/content_block_preview.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.327357 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/
+-rw-r--r--   0 quantra    (501) staff       (20)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)     2656 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/content_block_form.html
+-rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
+-rw-r--r--   0 quantra    (501) staff       (20)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/content_block_forms.html
+-rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/editor.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.328697 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/
+-rw-r--r--   0 quantra    (501) staff       (20)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/delete_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.329211 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/
+-rw-r--r--   0 quantra    (501) staff       (20)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/checkbox.html
+-rw-r--r--   0 quantra    (501) staff       (20)      497 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/default.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.330200 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/previews/
+-rw-r--r--   0 quantra    (501) staff       (20)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/previews/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/previews/image.html
+-rw-r--r--   0 quantra    (501) staff       (20)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/fields/previews/video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      442 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/loader.html
+-rw-r--r--   0 quantra    (501) staff       (20)      499 2023-06-14 16:14:32.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/popup.html
+-rw-r--r--   0 quantra    (501) staff       (20)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/partials/reset_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.330876 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/widgets/
+-rw-r--r--   0 quantra    (501) staff       (20)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/widgets/choices.html
+-rw-r--r--   0 quantra    (501) staff       (20)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/widgets/clearable_file.html
+-rw-r--r--   0 quantra    (501) staff       (20)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.333610 django-content-blocks-1.3.4/content_blocks/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.4/content_blocks/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.4/content_blocks/templatetags/content_block_admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/templatetags/content_blocks.py
+-rw-r--r--   0 quantra    (501) staff       (20)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.4/content_blocks/urls.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.4/content_blocks/views.py
+-rw-r--r--   0 quantra    (501) staff       (20)     2078 2023-06-06 15:28:11.000000 django-content-blocks-1.3.4/content_blocks/widgets.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-14 16:43:11.340650 django-content-blocks-1.3.4/django_content_blocks.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     7611 2023-06-14 16:43:11.000000 django-content-blocks-1.3.4/django_content_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     4749 2023-06-14 16:43:11.000000 django-content-blocks-1.3.4/django_content_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-14 16:43:11.000000 django-content-blocks-1.3.4/django_content_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       55 2023-06-14 16:43:11.000000 django-content-blocks-1.3.4/django_content_blocks.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       23 2023-06-14 16:43:11.000000 django-content-blocks-1.3.4/django_content_blocks.egg-info/top_level.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.4/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1977 2023-06-14 16:43:11.346675 django-content-blocks-1.3.4/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.4/setup.py
```

### Comparing `django-content-blocks-1.3.3/LICENSE` & `django-content-blocks-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/PKG-INFO` & `django-content-blocks-1.3.4/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,64 @@
-Metadata-Version: 2.1
-Name: django-content-blocks
-Version: 1.3.3
-Summary: HTML content blocks for Django.
-Home-page: https://github.com/Quantra/django-content-blocks
-Author: Vince Coleman
-Author-email: vince@shystudios.co.uk
-License: MIT
-Project-URL: Documentation, https://django-content-blocks.readthedocs.io
-Project-URL: Source, https://github.com/Quantra/django-content-blocks
-Keywords: django,django-content-blocks,django content blocks,django content,django dynamic content,django content manager,django cms
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Requires-Python: >=3.7
-License-File: LICENSE
-
-|coverage|
 |package version|
+|license|
+|pypi status|
+
 |python versions supported|
 |django versions supported|
+
+|coverage|
+|docs build|
+
 |code style black|
-|license|
+|pypi downloads|
+|github stars|
 
-=====================
 Django Content Blocks
 =====================
 
-Django Content Blocks is a reusable Django app that allows users to create and manage custom content blocks for their website. Via the django admin site it provides an easy-to-use interface for creating content blocks that can be inserted into any page, as well as a powerful template system for customizing the appearance of those blocks.
+Django Content Blocks is a reusable Django app that allows users to create and manage custom content blocks for their website. Via the django admin site it provides an easy-to-use interface for creating content blocks that can be related to any other object. This allows you to provide rich, dynamic, editable content for your existing models such as pages, products, projects or whatever your project has.
+
+The templates used to render content blocks are made in the same way as any other template in your project, giving you access to the full power of your chosen template engine.
 
-Content blocks can contain any type of content, including text, images, videos, and more, and can be arranged in any order on a page. Additionally, Django Content Blocks includes support for drafts and previews, allowing users to see how their changes will look before publishing them.
+Content blocks can contain any type of content, including text, images, videos, and more, and can be arranged in any order. Additionally, Django Content Blocks includes support for drafts and previews, allowing users to see how their changes will look before publishing them.
 
-.. image:: https://github.com/Quantra/django-content-blocks/raw/master/docs/images/content_block_editor_dark.png
+.. figure:: https://github.com/Quantra/django-content-blocks/raw/master/docs/images/content_block_editor_dark.png
+    :alt: The content block editor in the Django admin site.
+
+    The content block editor in the Django admin site.
 
 Installation instructions and detailed documentation can be found on `ReadTheDocs <https://django-content-blocks.readthedocs.io>`_.
 
-Supported Django & Python Versions
-----------------------------------
+Development Status & Roadmap
+----------------------------
 
-* Python >= 3.7
-* Django >= 3.2
+Django content blocks is already in use in a number of production websites however it is still considered to be in beta as active development continues.
+
+Major development plans/ideas include:
+
+* Rework the cacheing system to make it a lot simpler
+    * Currently content blocks are pre cached on publish. This becomes complex when sites are considered. The intention is to remove pre-cacheing and only cache on render, greatly simplifying the cacheing system.
+* Content block editor HTML, CSS and JS rework.
+    * This all needs updating to use modern HTML and CSS (flex, grid etc) and vanilla JS.
+    * Currently using jQuery which isn't the end of the world as it comes with django.contrib.admin so not an extra dependency.
+* Option for vertical layout for nested forms in the content block editor
+    * Sometimes nested blocks can represent columns within a content block. It would be nice to give the option to have these shown side by side in the content block editor.
+* django-content-blocks 2.0
+    * This will be a major rewrite which will move the representation of content blocks out of the database and into a ``JSONField``. This will greatly improve performance as the whole representation of an object's content blocks can be returned at once and any subsequent queries required can be made in a prefetch fashion.
+    * The ``ContentBlockField`` will become pluggable allowing developers to add/remove available fields from within their project.
+* Django content blocks suite of apps providing additional functionality and basic apps powered by content blocks:
+    * CMS
+    * Blog
+    * Contact forms
 
 Dependencies (and Thank You)
 ----------------------------
 
 * https://github.com/jrief/django-admin-sortable2
-* https://github.com/tj-django/django-clone - Additional thanks for tox.ini setup
+* https://github.com/tj-django/django-clone
 * https://github.com/python-pillow/Pillow
 
 Thank You
 ---------
 
 * https://shystudios.co.uk - For the monies I need to eat
 * https://opalstack.com/?lmref=A2GlhA - For great value hosting and superb support over the years (affiliate link)
@@ -80,22 +73,45 @@
 
 Contributions, advice and guidance are welcome. Please make contact **before** writing any code!
 
 
 .. shields.io badges
 
 .. |package version| image:: https://img.shields.io/pypi/v/django-content-blocks
-   :target: https://pypi.python.org/pypi/django-content-blocks/
+    :alt: PyPI Package Version
+    :target: https://pypi.python.org/pypi/django-content-blocks/
 
 .. |python versions supported| image:: https://img.shields.io/pypi/pyversions/django-content-blocks
-   :target: https://pypi.python.org/pypi/django-content-blocks/
+    :alt: Python Versions Supported
+    :target: https://pypi.python.org/pypi/django-content-blocks/
 
 .. |django versions supported| image:: https://img.shields.io/pypi/frameworkversions/django/django-content-blocks
-   :target: https://pypi.python.org/pypi/django-content-blocks/
+    :alt: Django Versions Supported
+    :target: https://pypi.python.org/pypi/django-content-blocks/
 
 .. |coverage| image:: https://img.shields.io/badge/dynamic/xml?color=success&label=coverage&query=round%28%2F%2Fcoverage%2F%40line-rate%20%2A%20100%29&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2FQuantra%2Fdjango-content-blocks%2Fmaster%2Fcoverage.xml
+    :alt: Test Coverage
+    :target: https://github.com/Quantra/django-content-blocks/blob/master/coverage.xml
 
 .. |code style black| image:: https://img.shields.io/badge/code%20style-black-black
+    :alt: Code Style Black
     :target: https://github.com/psf/black
 
 .. |license| image:: https://img.shields.io/github/license/Quantra/django-content-blocks
+    :alt: MIT License
     :target: https://github.com/Quantra/django-content-blocks/blob/master/LICENSE
+
+.. |docs build| image:: https://img.shields.io/readthedocs/django-content-blocks
+    :alt: Read the Docs
+    :target: https://django-content-blocks.readthedocs.io/
+
+.. |github stars| image:: https://img.shields.io/github/stars/Quantra/django-content-blocks?style=social
+    :alt: GitHub Repo Stars
+    :target: https://github.com/Quantra/django-content-blocks/stargazers
+
+.. |pypi downloads| image:: https://img.shields.io/pypi/dm/django-content-blocks
+    :alt: PyPI Downloads
+    :target: https://pypi.python.org/pypi/django-content-blocks/
+
+.. |pypi status| image:: https://img.shields.io/pypi/status/django-content-blocks
+    :alt: PyPI Status
+    :target: https://pypi.python.org/pypi/django-content-blocks/
```

### Comparing `django-content-blocks-1.3.3/content_blocks/abstract_models.py` & `django-content-blocks-1.3.4/content_blocks/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/admin.py` & `django-content-blocks-1.3.4/content_blocks/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from django.template.loader import get_template
 from django.urls import path, reverse
 from django.utils.safestring import mark_safe
 
 from content_blocks.admin_forms import (
     ContentBlockTemplateAdminForm,
     ContentBlockTemplateFieldAdminForm,
+    ContentBlockTemplateFieldInlineFormSet,
 )
 from content_blocks.models import (
     ContentBlockAvailability,
     ContentBlockCollection,
     ContentBlockTemplate,
     ContentBlockTemplateField,
 )
@@ -48,14 +49,15 @@
 VISIBLE_FIELDS = ["visible"]
 VISIBLE_FIELDSET = ("Visibility", {"fields": VISIBLE_FIELDS})
 
 
 class ContentBlockTemplateFieldInline(SortableInlineAdminMixin, admin.StackedInline):
     model = ContentBlockTemplateField
     fk_name = "content_block_template"
+    formset = ContentBlockTemplateFieldInlineFormSet
     form = ContentBlockTemplateFieldAdminForm
     min_num = 0
     extra = 0
     autocomplete_fields = ["nested_templates"]
 
 
 @admin.register(ContentBlockTemplate)
```

### Comparing `django-content-blocks-1.3.3/content_blocks/admin_forms.py` & `django-content-blocks-1.3.4/content_blocks/admin_forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import json
 
+from adminsortable2.admin import CustomInlineFormSet
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.validators import FileExtensionValidator
 
 from content_blocks.models import (
     ContentBlock,
     ContentBlockField,
     ContentBlockFields,
     ContentBlockTemplate,
     ContentBlockTemplateField,
 )
 from content_blocks.services.content_block_template import ImportExportServices
-from content_blocks.widgets import ChoicesWidget, TemplateFilenameAutocompleteWidget
+from content_blocks.widgets import (
+    ChoicesWidget,
+    ContentBlockTemplateFieldDeleteWidget,
+    TemplateFilenameAutocompleteWidget,
+)
 
-REQUIRED_ERROR_MSG = "This field is required"
+REQUIRED_ERROR_MSG = "This field is required."
 
 
 class ContentBlockTemplateAdminForm(forms.ModelForm):
     class Meta:
         model = ContentBlockTemplate
         exclude = []
         widgets = {
@@ -43,14 +48,18 @@
 
         if not len(choice) == 2:
             return False
 
     return True
 
 
+class ContentBlockTemplateFieldInlineFormSet(CustomInlineFormSet):
+    deletion_widget = ContentBlockTemplateFieldDeleteWidget()
+
+
 class ContentBlockTemplateFieldAdminForm(forms.ModelForm):
     class Meta:
         model = ContentBlockTemplateField
         exclude = []
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -91,15 +100,15 @@
 
         elif field_type == ContentBlockFields.MODEL_CHOICE_FIELD:
             model_choice_content_type = cleaned_data.get("model_choice_content_type")
             if not model_choice_content_type:
                 self.add_error("model_choice_content_type", REQUIRED_ERROR_MSG)
 
         if self.instance.pk and "field_type" in self.changed_data:
-            self.add_error("field_type", "Field type cannot be changed after save")
+            self.add_error("field_type", "Field type cannot be changed.")
 
         return cleaned_data
 
     def save(self, commit=True):
         """
         Update content block fields based on this template field.
         """
```

### Comparing `django-content-blocks-1.3.3/content_blocks/apps.py` & `django-content-blocks-1.3.4/content_blocks/apps.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/conf.py` & `django-content-blocks-1.3.4/content_blocks/conf.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/fields.py` & `django-content-blocks-1.3.4/content_blocks/fields.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/forms.py` & `django-content-blocks-1.3.4/content_blocks/forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/management/commands/export_content_block_templates.py` & `django-content-blocks-1.3.4/content_blocks/management/commands/export_content_block_templates.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/management/commands/import_content_block_templates.py` & `django-content-blocks-1.3.4/content_blocks/management/commands/import_content_block_templates.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/migrations/0001_initial.py` & `django-content-blocks-1.3.4/content_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py` & `django-content-blocks-1.3.4/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py` & `django-content-blocks-1.3.4/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/models.py` & `django-content-blocks-1.3.4/content_blocks/models.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/services/content_block.py` & `django-content-blocks-1.3.4/content_blocks/services/content_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     class DummyRequest:
         """
         DummyRequest to hold a site attribute. In no other way similar to an actual request.
         """
 
         def __init__(self, site):
             self.site = site
+            self.META = {}
 
     @staticmethod
     def render_html(content_block, context=None, site=None):
         """
         Render the html for the given ContentBlock.
         :context: Dictionary of context to render the template with.
         :site: If a Site is supplied and there is no request context set it in the context under request.site
```

### Comparing `django-content-blocks-1.3.3/content_blocks/services/content_block_parent.py` & `django-content-blocks-1.3.4/content_blocks/services/content_block_parent.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/services/content_block_template.py` & `django-content-blocks-1.3.4/content_blocks/services/content_block_template.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/signals.py` & `django-content-blocks-1.3.4/content_blocks/signals.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/.DS_Store` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/.DS_Store` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/content_blocks.css` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/css/content_blocks.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/solid.min.css` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/admin_choices_widget.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/admin_choices_widget.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/ajax_setup.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/ajax_setup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_editor.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/content_block_editor.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_template_admin.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/content_block_template_admin.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/popup.js` & `django-content-blocks-1.3.4/content_blocks/static/content_blocks/js/popup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/.DS_Store` & `django-content-blocks-1.3.4/content_blocks/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/.DS_Store` & `django-content-blocks-1.3.4/content_blocks/templates/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html` & `django-content-blocks-1.3.4/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/base.html` & `django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/base.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form.html` & `django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/content_block_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html` & `django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/editor.html` & `django-content-blocks-1.3.4/content_blocks/templates/content_blocks/editor/editor.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/clearable_file.html` & `django-content-blocks-1.3.4/content_blocks/templates/content_blocks/widgets/clearable_file.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templatetags/content_block_admin.py` & `django-content-blocks-1.3.4/content_blocks/templatetags/content_block_admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/templatetags/content_blocks.py` & `django-content-blocks-1.3.4/content_blocks/templatetags/content_blocks.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/urls.py` & `django-content-blocks-1.3.4/content_blocks/urls.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/views.py` & `django-content-blocks-1.3.4/content_blocks/views.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.3/content_blocks/widgets.py` & `django-content-blocks-1.3.4/content_blocks/widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,7 +56,17 @@
 class ChoicesWidget(forms.HiddenInput):
     template_name = "content_blocks/widgets/choices.html"
 
     @property
     def is_hidden(self):
         # Show the label in the admin change page.
         return False
+
+
+class ContentBlockTemplateFieldDeleteWidget(forms.CheckboxInput):
+    """
+    Add a warning message to the delete checkbox.
+    """
+
+    template_name = (
+        "content_blocks/admin/content_block_template_field_delete_checkbox.html"
+    )
```

### Comparing `django-content-blocks-1.3.3/django_content_blocks.egg-info/SOURCES.txt` & `django-content-blocks-1.3.4/django_content_blocks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 content_blocks/static/content_blocks/js/popup.js
 content_blocks/templates/.DS_Store
 content_blocks/templates/base.html
 content_blocks/templates/content_blocks/.DS_Store
 content_blocks/templates/content_blocks/content_block_collection.html
 content_blocks/templates/content_blocks/content_block_preview.html
 content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
+content_blocks/templates/content_blocks/admin/content_block_template_field_delete_checkbox.html
 content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
 content_blocks/templates/content_blocks/editor/base.html
 content_blocks/templates/content_blocks/editor/content_block_form.html
 content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
 content_blocks/templates/content_blocks/editor/content_block_forms.html
 content_blocks/templates/content_blocks/editor/editor.html
 content_blocks/templates/content_blocks/partials/delete_popup.html
```

### Comparing `django-content-blocks-1.3.3/setup.cfg` & `django-content-blocks-1.3.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = django-content-blocks
-version = 1.3.3
+version = 1.3.4
 description = HTML content blocks for Django.
 long_description = file:README.rst
 url = https://github.com/Quantra/django-content-blocks
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
 	Intended Audience :: Developers
+	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

