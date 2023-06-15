# Comparing `tmp/django-delayed-notifications-0.6.18.tar.gz` & `tmp/django-delayed-notifications-0.6.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-delayed-notifications-0.6.18.tar", last modified: Mon Feb 13 10:57:18 2023, max compression
+gzip compressed data, was "django-delayed-notifications-0.6.19.tar", last modified: Thu Jun 15 07:43:31 2023, max compression
```

## Comparing `django-delayed-notifications-0.6.18.tar` & `django-delayed-notifications-0.6.19.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.336356 django-delayed-notifications-0.6.18/
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4150 2023-02-13 10:57:18.336356 django-delayed-notifications-0.6.18/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2757 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.304363 django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4150 2023-02-13 10:57:18.000000 django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1981 2023-02-13 10:57:18.000000 django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-13 10:57:18.000000 django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      155 2023-02-13 10:57:18.000000 django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-13 10:57:18.000000 django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.308362 django-delayed-notifications-0.6.18/django_notifications/
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-02-13 10:56:41.000000 django-delayed-notifications-0.6.18/django_notifications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.312361 django-delayed-notifications-0.6.18/django_notifications/admin/
--rw-rw-rw-   0 root         (0) root         (0)     9933 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/admin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2675 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/admin/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/admin/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/admin/inlines.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.272369 django-delayed-notifications-0.6.18/django_notifications/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.272369 django-delayed-notifications-0.6.18/django_notifications/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.316360 django-delayed-notifications-0.6.18/django_notifications/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     6401 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.316360 django-delayed-notifications-0.6.18/django_notifications/management/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.320360 django-delayed-notifications-0.6.18/django_notifications/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/management/commands/send_notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.324359 django-delayed-notifications-0.6.18/django_notifications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3661 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/migrations/0002_notificationconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/migrations/0003_auto_20220207_1157.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/migrations/0004_notification_from_email.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/migrations/0005_debugging.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.324359 django-delayed-notifications-0.6.18/django_notifications/models/
--rw-rw-rw-   0 root         (0) root         (0)    15295 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2338 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/models/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1825 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/models/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.276368 django-delayed-notifications-0.6.18/django_notifications/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.328358 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.280368 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.332357 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/dates.html
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/recipients.html
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/related_object.html
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/states.html
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/subject.html
--rw-rw-rw-   0 root         (0) root         (0)     5716 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/base_email.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/base_email.txt.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.332357 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/debug/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/debug/body.txt.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.332357 django-delayed-notifications-0.6.18/django_notifications/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/templatetags/notifications_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 10:57:18.332357 django-delayed-notifications-0.6.18/django_notifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/django_notifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3252 2023-02-13 10:52:43.000000 django-delayed-notifications-0.6.18/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-13 10:57:18.336356 django-delayed-notifications-0.6.18/setup.cfg
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.080773 django-delayed-notifications-0.6.19/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     1105 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/LICENSE
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      126 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/MANIFEST.in
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     4150 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/PKG-INFO
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     2757 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/README.md
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     4150 2023-06-15 07:43:31.000000 django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     1981 2023-06-15 07:43:31.000000 django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)        1 2023-06-15 07:43:31.000000 django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      155 2023-06-15 07:43:31.000000 django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/requires.txt
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)       21 2023-06-15 07:43:31.000000 django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      295 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/__init__.py
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/admin/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     9933 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/admin/__init__.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     2675 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/admin/filters.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      649 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/admin/forms.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      524 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/admin/inlines.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      523 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/apps.py
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.072773 django-delayed-notifications-0.6.19/django_notifications/locale/
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.072773 django-delayed-notifications-0.6.19/django_notifications/locale/fr/
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     4348 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     6401 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/management/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      183 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/management/__init__.py
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/management/commands/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      201 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/management/commands/__init__.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      945 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/management/commands/send_notifications.py
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/migrations/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     3661 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/migrations/0001_initial.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     4207 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/migrations/0002_notificationconfig.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     1056 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/migrations/0003_auto_20220207_1157.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      599 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/migrations/0004_notification_from_email.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     1024 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/migrations/0005_debugging.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/migrations/__init__.py
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/models/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)    15295 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/models/__init__.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     2338 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/models/config.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     1825 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/models/helpers.py
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.072773 django-delayed-notifications-0.6.19/django_notifications/templates/
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.072773 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      606 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/dates.html
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      641 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/recipients.html
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      172 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/related_object.html
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      474 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/states.html
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      613 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/subject.html
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     5716 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/base_email.html
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      183 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/base_email.txt.tpl
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/debug/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)       46 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/debug/body.txt.tpl
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/templatetags/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      191 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/templatetags/__init__.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     1049 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/templatetags/notifications_tags.py
+drwxr-xr-x   0 fguerin   (1000) fguerin   (1000)        0 2023-06-15 07:43:31.076773 django-delayed-notifications-0.6.19/django_notifications/tests/
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)      960 2023-06-15 07:28:02.000000 django-delayed-notifications-0.6.19/django_notifications/tests/__init__.py
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)     3252 2023-06-15 07:42:11.000000 django-delayed-notifications-0.6.19/pyproject.toml
+-rw-r--r--   0 fguerin   (1000) fguerin   (1000)       38 2023-06-15 07:43:31.080773 django-delayed-notifications-0.6.19/setup.cfg
```

### Comparing `django-delayed-notifications-0.6.18/LICENSE` & `django-delayed-notifications-0.6.19/LICENSE`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/PKG-INFO` & `django-delayed-notifications-0.6.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-delayed-notifications
-Version: 0.6.18
+Version: 0.6.19
 Summary: django-delayed-notifications provides tracking of notifications, and delayed sending.
 Author-email: François GUÉRIN <frague59@gmail.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/frague59/django-delayed-notifications
 Project-URL: Source, https://gitlab.com/frague59/django-delayed-notifications
 Keywords: django,notifications,delayed sending
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-delayed-notifications-0.6.18/README.md` & `django-delayed-notifications-0.6.19/README.md`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/PKG-INFO` & `django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-delayed-notifications
-Version: 0.6.18
+Version: 0.6.19
 Summary: django-delayed-notifications provides tracking of notifications, and delayed sending.
 Author-email: François GUÉRIN <frague59@gmail.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/frague59/django-delayed-notifications
 Project-URL: Source, https://gitlab.com/frague59/django-delayed-notifications
 Keywords: django,notifications,delayed sending
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-delayed-notifications-0.6.18/django_delayed_notifications.egg-info/SOURCES.txt` & `django-delayed-notifications-0.6.19/django_delayed_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/admin/__init__.py` & `django-delayed-notifications-0.6.19/django_notifications/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/admin/filters.py` & `django-delayed-notifications-0.6.19/django_notifications/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/admin/forms.py` & `django-delayed-notifications-0.6.19/django_notifications/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/admin/inlines.py` & `django-delayed-notifications-0.6.19/django_notifications/admin/inlines.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/apps.py` & `django-delayed-notifications-0.6.19/django_notifications/apps.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/locale/fr/LC_MESSAGES/django.mo` & `django-delayed-notifications-0.6.19/django_notifications/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/locale/fr/LC_MESSAGES/django.po` & `django-delayed-notifications-0.6.19/django_notifications/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/management/commands/send_notifications.py` & `django-delayed-notifications-0.6.19/django_notifications/management/commands/send_notifications.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/migrations/0001_initial.py` & `django-delayed-notifications-0.6.19/django_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/migrations/0002_notificationconfig.py` & `django-delayed-notifications-0.6.19/django_notifications/migrations/0002_notificationconfig.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/migrations/0003_auto_20220207_1157.py` & `django-delayed-notifications-0.6.19/django_notifications/migrations/0003_auto_20220207_1157.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/migrations/0004_notification_from_email.py` & `django-delayed-notifications-0.6.19/django_notifications/migrations/0004_notification_from_email.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/migrations/0005_debugging.py` & `django-delayed-notifications-0.6.19/django_notifications/migrations/0005_debugging.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/models/__init__.py` & `django-delayed-notifications-0.6.19/django_notifications/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/models/config.py` & `django-delayed-notifications-0.6.19/django_notifications/models/config.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/models/helpers.py` & `django-delayed-notifications-0.6.19/django_notifications/models/helpers.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/dates.html` & `django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/dates.html`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/recipients.html` & `django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/recipients.html`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/admin/snippets/subject.html` & `django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/admin/snippets/subject.html`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/templates/django_notifications/base_email.html` & `django-delayed-notifications-0.6.19/django_notifications/templates/django_notifications/base_email.html`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/templatetags/notifications_tags.py` & `django-delayed-notifications-0.6.19/django_notifications/templatetags/notifications_tags.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/django_notifications/tests/__init__.py` & `django-delayed-notifications-0.6.19/django_notifications/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-delayed-notifications-0.6.18/pyproject.toml` & `django-delayed-notifications-0.6.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "Django>=3.2,<4.0",
     "django-ckeditor>=6.4.0,<7.0",
     "django-currentuser~=0.5.0",
-    "django-solo>=1.1.5,<2.1",
+    "django-solo>=1.1.5,<2.2",
     "beautifulsoup4~=4.10",
 ]
 dynamic = ["version", "readme"]
 keywords = [
     "django",
     "notifications",
     "delayed sending"
```

