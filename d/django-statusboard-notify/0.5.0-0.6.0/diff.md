# Comparing `tmp/django-statusboard-notify-0.5.0.tar.gz` & `tmp/django-statusboard-notify-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-statusboard-notify-0.5.0.tar", last modified: Mon Sep  5 15:57:38 2022, max compression
+gzip compressed data, was "django-statusboard-notify-0.6.0.tar", last modified: Thu Jun 15 09:16:38 2023, max compression
```

## Comparing `django-statusboard-notify-0.5.0.tar` & `django-statusboard-notify-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-09-05 15:57:38.000000 django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-09-05 15:57:38.000000 django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 15:57:38.000000 django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-05 15:57:38.000000 django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-05 15:57:38.000000 django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/statusboard_notify/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.143849 django-statusboard-notify-0.5.0/statusboard_notify/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.143849 django-statusboard-notify-0.5.0/statusboard_notify/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/statusboard_notify/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/statusboard_notify/management/
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/statusboard_notify/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/management/commands/send_notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/statusboard_notify/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.143849 django-statusboard-notify-0.5.0/statusboard_notify/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:57:38.147849 django-statusboard-notify-0.5.0/statusboard_notify/templates/statusboard_notify/
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/templates/statusboard_notify/email.html
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-09-05 15:57:30.000000 django-statusboard-notify-0.5.0/statusboard_notify/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.435597 django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-15 09:16:38.000000 django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-15 09:16:38.000000 django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:16:38.000000 django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 09:16:38.000000 django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 09:16:38.000000 django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/statusboard_notify/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.435597 django-statusboard-notify-0.6.0/statusboard_notify/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.435597 django-statusboard-notify-0.6.0/statusboard_notify/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/statusboard_notify/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/statusboard_notify/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/statusboard_notify/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/management/commands/send_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/statusboard_notify/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.435597 django-statusboard-notify-0.6.0/statusboard_notify/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:16:38.439597 django-statusboard-notify-0.6.0/statusboard_notify/templates/statusboard_notify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/templates/statusboard_notify/email.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 09:16:26.000000 django-statusboard-notify-0.6.0/statusboard_notify/views.py
```

### Comparing `django-statusboard-notify-0.5.0/LICENSE` & `django-statusboard-notify-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/PKG-INFO` & `django-statusboard-notify-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: django-statusboard-notify
-Version: 0.5.0
+Version: 0.6.0
 Summary: Utility for django-statusboard to notify status changes
 Home-page: http://github.com/edigiacomo/django-statusboard-notify
 Author: Emanuele Di Giacomo
 Author-email: emanuele@digiacomo.cc
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: with_telegram
 Provides-Extra: with_matrix
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: django-statusboard-notify Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: django-statusboard-notify Version: 0.6.0 Summary:
 Utility for django-statusboard to notify status changes Home-page: http://
 github.com/edigiacomo/django-statusboard-notify Author: Emanuele Di Giacomo
 Author-email: emanuele@digiacomo.cc License: GPLv2+ Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Web Environment Classifier:
 License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Framework :: Django Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python:
->=3.6 Description-Content-Type: text/markdown Provides-Extra: with_telegram
-Provides-Extra: with_matrix License-File: LICENSE # statusboard-notify [!
-[Build](https://github.com/edigiacomo/django-statusboard-notify/actions/
-workflows/build.yml/badge.svg)](https://github.com/edigiacomo/django-
-statusboard-notify/actions/workflows/build.yml) [![Pypi](https://
-img.shields.io/pypi/v/django-statusboard-notify.svg)](https://pypi.python.org/
-pypi/django-statusboard-notify/) [![codecov](https://codecov.io/gh/edigiacomo/
-django-statusboard-notify/branch/main/graph/badge.svg)](https://codecov.io/gh/
-edigiacomo/django-statusboard-notify) Utility for [django-statusboard][1] that
-notifies users about service status changes. The notification are sent via
-email or published in a Telegram channel. This app periodically notifies about
-service status changes - except for changes from "Operational" to "Performance
-issues" (and viceversa). ![screenshot of a Telegram channel](telegram-
-screenshot.png) ## Installation Install the package: ```sh pip install django-
-statusboard-notify[with_telegram] ``` If you don't need Telegram notifications,
-you can install the package without the `with_telegram` extra. ## Configure the
-application Add the following applications to your Django projects: ```python #
-settings.py INSTALLED_APPS += [ 'statusboard', 'statusboard-notify', ] ``` ###
-Email notification In order to enable the email notifications, you have to set
-the sender: ```python # settings.py STATUSBOARD_NOTIFY_EMAIL_SENDER =
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
+Dynamic Content Requires-Python: >=3.6 Description-Content-Type: text/markdown
+Provides-Extra: with_telegram Provides-Extra: with_matrix License-File: LICENSE
+# statusboard-notify [![Build](https://github.com/edigiacomo/django-
+statusboard-notify/actions/workflows/build.yml/badge.svg)](https://github.com/
+edigiacomo/django-statusboard-notify/actions/workflows/build.yml) [![Pypi]
+(https://img.shields.io/pypi/v/django-statusboard-notify.svg)](https://
+pypi.python.org/pypi/django-statusboard-notify/) [![codecov](https://
+codecov.io/gh/edigiacomo/django-statusboard-notify/branch/main/graph/
+badge.svg)](https://codecov.io/gh/edigiacomo/django-statusboard-notify) Utility
+for [django-statusboard][1] that notifies users about service status changes.
+The notification are sent via email or published in a Telegram channel. This
+app periodically notifies about service status changes - except for changes
+from "Operational" to "Performance issues" (and viceversa). ![screenshot of a
+Telegram channel](telegram-screenshot.png) ## Installation Install the package:
+```sh pip install django-statusboard-notify[with_telegram] ``` If you don't
+need Telegram notifications, you can install the package without the
+`with_telegram` extra. ## Configure the application Add the following
+applications to your Django projects: ```python # settings.py INSTALLED_APPS +=
+[ 'statusboard', 'statusboard-notify', ] ``` ### Email notification In order to
+enable the email notifications, you have to set the sender: ```python #
+settings.py STATUSBOARD_NOTIFY_EMAIL_SENDER =
 "statusboard@localhost.localdomain ``` You can edit the subject: ```python #
 settings.py STATUSBOARD_NOTIFY_EMAIL_SUBJECT = "Mysubject" ``` You can add a
 list of recipients that will receive the notifications about all the services:
 ```python # settings.py STATUSBOARD_NOTIFY_EMAIL_RECIPIENTS =
 [ "admin@localhost.localdomain", "anotheradmin@localhost.localdomain", ] ```
 From the admin page you can associate an existing user to one or more services:
 ![screenshot of the admin page](admin-screenshot.png) The email is sent in two
```

### Comparing `django-statusboard-notify-0.5.0/README.md` & `django-statusboard-notify-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/PKG-INFO` & `django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: django-statusboard-notify
-Version: 0.5.0
+Version: 0.6.0
 Summary: Utility for django-statusboard to notify status changes
 Home-page: http://github.com/edigiacomo/django-statusboard-notify
 Author: Emanuele Di Giacomo
 Author-email: emanuele@digiacomo.cc
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: with_telegram
 Provides-Extra: with_matrix
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: django-statusboard-notify Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: django-statusboard-notify Version: 0.6.0 Summary:
 Utility for django-statusboard to notify status changes Home-page: http://
 github.com/edigiacomo/django-statusboard-notify Author: Emanuele Di Giacomo
 Author-email: emanuele@digiacomo.cc License: GPLv2+ Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Web Environment Classifier:
 License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Framework :: Django Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python:
->=3.6 Description-Content-Type: text/markdown Provides-Extra: with_telegram
-Provides-Extra: with_matrix License-File: LICENSE # statusboard-notify [!
-[Build](https://github.com/edigiacomo/django-statusboard-notify/actions/
-workflows/build.yml/badge.svg)](https://github.com/edigiacomo/django-
-statusboard-notify/actions/workflows/build.yml) [![Pypi](https://
-img.shields.io/pypi/v/django-statusboard-notify.svg)](https://pypi.python.org/
-pypi/django-statusboard-notify/) [![codecov](https://codecov.io/gh/edigiacomo/
-django-statusboard-notify/branch/main/graph/badge.svg)](https://codecov.io/gh/
-edigiacomo/django-statusboard-notify) Utility for [django-statusboard][1] that
-notifies users about service status changes. The notification are sent via
-email or published in a Telegram channel. This app periodically notifies about
-service status changes - except for changes from "Operational" to "Performance
-issues" (and viceversa). ![screenshot of a Telegram channel](telegram-
-screenshot.png) ## Installation Install the package: ```sh pip install django-
-statusboard-notify[with_telegram] ``` If you don't need Telegram notifications,
-you can install the package without the `with_telegram` extra. ## Configure the
-application Add the following applications to your Django projects: ```python #
-settings.py INSTALLED_APPS += [ 'statusboard', 'statusboard-notify', ] ``` ###
-Email notification In order to enable the email notifications, you have to set
-the sender: ```python # settings.py STATUSBOARD_NOTIFY_EMAIL_SENDER =
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
+Dynamic Content Requires-Python: >=3.6 Description-Content-Type: text/markdown
+Provides-Extra: with_telegram Provides-Extra: with_matrix License-File: LICENSE
+# statusboard-notify [![Build](https://github.com/edigiacomo/django-
+statusboard-notify/actions/workflows/build.yml/badge.svg)](https://github.com/
+edigiacomo/django-statusboard-notify/actions/workflows/build.yml) [![Pypi]
+(https://img.shields.io/pypi/v/django-statusboard-notify.svg)](https://
+pypi.python.org/pypi/django-statusboard-notify/) [![codecov](https://
+codecov.io/gh/edigiacomo/django-statusboard-notify/branch/main/graph/
+badge.svg)](https://codecov.io/gh/edigiacomo/django-statusboard-notify) Utility
+for [django-statusboard][1] that notifies users about service status changes.
+The notification are sent via email or published in a Telegram channel. This
+app periodically notifies about service status changes - except for changes
+from "Operational" to "Performance issues" (and viceversa). ![screenshot of a
+Telegram channel](telegram-screenshot.png) ## Installation Install the package:
+```sh pip install django-statusboard-notify[with_telegram] ``` If you don't
+need Telegram notifications, you can install the package without the
+`with_telegram` extra. ## Configure the application Add the following
+applications to your Django projects: ```python # settings.py INSTALLED_APPS +=
+[ 'statusboard', 'statusboard-notify', ] ``` ### Email notification In order to
+enable the email notifications, you have to set the sender: ```python #
+settings.py STATUSBOARD_NOTIFY_EMAIL_SENDER =
 "statusboard@localhost.localdomain ``` You can edit the subject: ```python #
 settings.py STATUSBOARD_NOTIFY_EMAIL_SUBJECT = "Mysubject" ``` You can add a
 list of recipients that will receive the notifications about all the services:
 ```python # settings.py STATUSBOARD_NOTIFY_EMAIL_RECIPIENTS =
 [ "admin@localhost.localdomain", "anotheradmin@localhost.localdomain", ] ```
 From the admin page you can associate an existing user to one or more services:
 ![screenshot of the admin page](admin-screenshot.png) The email is sent in two
```

### Comparing `django-statusboard-notify-0.5.0/django_statusboard_notify.egg-info/SOURCES.txt` & `django-statusboard-notify-0.6.0/django_statusboard_notify.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 django_statusboard_notify.egg-info/PKG-INFO
 django_statusboard_notify.egg-info/SOURCES.txt
 django_statusboard_notify.egg-info/dependency_links.txt
 django_statusboard_notify.egg-info/requires.txt
 django_statusboard_notify.egg-info/top_level.txt
 statusboard_notify/__init__.py
```

### Comparing `django-statusboard-notify-0.5.0/setup.py` & `django-statusboard-notify-0.6.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 import os
 import re
 
 from setuptools import find_packages, setup
 
 
-def get_version(package):
-    # Thanks to Tom Christie
-    init_py = open(os.path.join(package, '__init__.py')).read()
-    return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
-
-
-version = get_version('statusboard_notify')
-
 setup(
     name="django-statusboard-notify",
-    version=version,
     packages=find_packages(include=["statusboard_notify", "statusboard_notify.*"]),
     include_package_data=True,
     license='GPLv2+',
     description='Utility for django-statusboard to notify status changes',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='http://github.com/edigiacomo/django-statusboard-notify',
@@ -34,21 +25,23 @@
     },
     test_suite="runtests.runtests",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
 )
```

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/__init__.py` & `django-statusboard-notify-0.6.0/statusboard_notify/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-__version__ = '0.5.0'
+__version__ = "0.6.0"
 __author__ = "Emanuele Di Giacomo <emanuele@digiacomo.cc>"
 __copyright__ = "Copyright (C) 2021 Emanuele Di Giacomo"
 __license__ = "GPLv2+"
 
-default_app_config = 'statusboard_notify.apps.StatusboardNotifyConfig'
+default_app_config = "statusboard_notify.apps.StatusboardNotifyConfig"
```

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/admin.py` & `django-statusboard-notify-0.6.0/statusboard_notify/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from django.contrib import admin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from .models import Recipient
 
 
 class RecipientAdmin(admin.ModelAdmin):
-    list_display = ('email', 'service_list')
+    list_display = ("email", "service_list")
 
     def service_list(self, o):
         return ", ".join(s.name for s in o.services.all())
-    service_list.short_description = _('service list')
+
+    service_list.short_description = _("service list")
 
 
 admin.site.register(Recipient, RecipientAdmin)
```

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/apps.py` & `django-statusboard-notify-0.6.0/statusboard_notify/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from django.apps import AppConfig
 from django.utils.translation import gettext_lazy as _
 
 
 class StatusboardNotifyConfig(AppConfig):
-    name = 'statusboard_notify'
-    verbose_name = _('statusboard notifier')
-    default_auto_field = 'django.db.models.AutoField'
+    name = "statusboard_notify"
+    verbose_name = _("statusboard notifier")
+    default_auto_field = "django.db.models.AutoField"
```

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/locale/it/LC_MESSAGES/django.mo` & `django-statusboard-notify-0.6.0/statusboard_notify/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/locale/it/LC_MESSAGES/django.po` & `django-statusboard-notify-0.6.0/statusboard_notify/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/management/__init__.py` & `django-statusboard-notify-0.6.0/statusboard_notify/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/management/commands/__init__.py` & `django-statusboard-notify-0.6.0/statusboard_notify/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/management/commands/send_notifications.py` & `django-statusboard-notify-0.6.0/statusboard_notify/management/commands/send_notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,37 +19,37 @@
 from statusboard_notify.utils import send_notification_telegram
 
 
 class Command(BaseCommand):
     help = "Send statusbord notifications"
 
     def add_arguments(self, parser):
-        parser.add_argument('-n', '--dry-run', action="store_true")
+        parser.add_argument("-n", "--dry-run", action="store_true")
 
     def handle(self, *args, **kwargs):
         notifications = Notification.objects.all()
         if not notifications.exists():
             self.stdout.write("Notification queue is empty")
             return
 
         for dest, func in (
             ("telegram", send_notification_telegram),
             ("email", send_notification_mail),
         ):
-            self.stdout.write("Sending {} notifications via {}".format(
-                notifications.count(),
-                dest,
-            ))
+            self.stdout.write(
+                "Sending {} notifications via {}".format(
+                    notifications.count(),
+                    dest,
+                )
+            )
             if not kwargs["dry_run"]:
                 try:
                     func(notifications)
                 except Exception as e:
                     self.stderr.write(e)
 
-        self.stdout.write("Removing {} notifications from the queue".format(
-            notifications.count()
-        ))
+        self.stdout.write("Removing {} notifications from the queue".format(notifications.count()))
         if not kwargs["dry_run"]:
             try:
                 notifications.delete()
             except Exception as e:
                 self.stderr.write(e)
```

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/migrations/0001_initial.py` & `django-statusboard-notify-0.6.0/statusboard_notify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/models.py` & `django-statusboard-notify-0.6.0/statusboard_notify/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,52 +19,51 @@
 
 from statusboard.models import Service, SERVICE_STATUSES
 
 
 class Recipient(models.Model):
     """Recipient for the notifications. Each recipient can receive
     notifications for a subset of services."""
+
     email = models.EmailField(unique=True, verbose_name="email")
     services = models.ManyToManyField(Service, verbose_name=_("services"))
 
     def notifications(self, qs=None):
         if qs is None:
             qs = Notification.objects.all()
 
         return qs.filter(service__in=self.services.all())
 
     class Meta:
-        verbose_name = _('recipient')
-        verbose_name_plural = _('recipients')
+        verbose_name = _("recipient")
+        verbose_name_plural = _("recipients")
 
 
 class Notification(models.Model):
     """Pending notifications."""
+
     service = models.OneToOneField(Service, on_delete=models.deletion.CASCADE)
     from_status = models.IntegerField(choices=SERVICE_STATUSES, null=True, blank=True)
     to_status = models.IntegerField(choices=SERVICE_STATUSES)
 
     class Meta:
-        verbose_name = _('notification')
-        verbose_name_plural = _('notifications')
+        verbose_name = _("notification")
+        verbose_name_plural = _("notifications")
 
 
 @receiver(post_save, sender=Service)
 def update_notification(sender, instance, **kwargs):
     """Update the state of a pending notification. A status change from
     "operational" to "performance issues" (or viceversa) is ignored.
     The notification is removed when a service status changes to operational or
     "performance issues". The pending notification keeps track of the first and
     last status: if the service status changes again before the notification is
     sent, this function overwrites the final status.
     """
-    if any([
-        instance._status == instance.status,
-        (instance._status, instance.status) in ((0, 1), (1, 0))
-    ]):
+    if any([instance._status == instance.status, (instance._status, instance.status) in ((0, 1), (1, 0))]):
         # Ignore if the status is unchanged or the change is between 0
         # (operational) and 1 (performance issues).
         return
     else:
         try:
             n = Notification.objects.get(service=instance)
             if n.from_status == instance.status:
@@ -73,10 +72,9 @@
                 n.delete()
             else:
                 # Else, update the final status.
                 n.to_status = instance.status
                 n.save()
         except Notification.DoesNotExist:
             # Create the notification if it doesn't exist.
-            n = Notification(service=instance, from_status=instance._status,
-                             to_status=instance.status)
+            n = Notification(service=instance, from_status=instance._status, to_status=instance.status)
             n.save()
```

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/templates/statusboard_notify/email.html` & `django-statusboard-notify-0.6.0/statusboard_notify/templates/statusboard_notify/email.html`

 * *Files identical despite different names*

### Comparing `django-statusboard-notify-0.5.0/statusboard_notify/utils.py` & `django-statusboard-notify-0.6.0/statusboard_notify/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from django.conf import settings
 from django.core.mail import send_mail
 from django.template.loader import render_to_string
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 import pypandoc
 
 try:
     telegram = None
     import telegram
 except ImportError:
@@ -39,20 +39,19 @@
     except AttributeError:
         return
 
     html_msg, plain_msg = render_notification_message(notifications)
 
     try:
         subject = settings.STATUSBOARD_NOTIFY_EMAIL_SUBJECT
-    except:
+    except AttributeError:
         subject = _("[statusboard] Service status updates")
 
     for recipient in recipients:
-        send_mail(subject, plain_msg, sender, [recipient],
-                  fail_silently=False, html_message=html_msg)
+        send_mail(subject, plain_msg, sender, [recipient], fail_silently=False, html_message=html_msg)
 
 
 def send_notification_mail(notifications):
     try:
         send_notification_mail_for_recipients(
             settings.STATUSBOARD_NOTIFY_EMAIL_RECIPIENTS,
             notifications,
@@ -64,19 +63,21 @@
         send_notification_mail_for_recipients(
             [recipient.email],
             recipient.notifications(notifications),
         )
 
 
 def render_notification_message(notifications):
-    html_msg = render_to_string('statusboard_notify/email.html', {
-        'notifications': notifications,
-    })
-    plain_msg = pypandoc.convert_text(html_msg, "markdown_strict",
-                                      format="html")
+    html_msg = render_to_string(
+        "statusboard_notify/email.html",
+        {
+            "notifications": notifications,
+        },
+    )
+    plain_msg = pypandoc.convert_text(html_msg, "markdown_strict", format="html")
     return html_msg, plain_msg
 
 
 def send_notification_telegram(notifications):
     if not telegram:
         pass
 
@@ -84,40 +85,34 @@
         token = settings.STATUSBOARD_NOTIFY_TELEGRAM_TOKEN
         chat_id = settings.STATUSBOARD_NOTIFY_TELEGRAM_CHAT_ID
     except AttributeError:
         return
 
     bot = telegram.Bot(token=token)
     for notification in notifications:
-        bot.send_message(chat_id=chat_id,
-                         text=render_notification_telegram(notification),
-                         parse_mode=telegram.ParseMode.MARKDOWN)
+        bot.send_message(
+            chat_id=chat_id, text=render_notification_telegram(notification), parse_mode=telegram.ParseMode.MARKDOWN
+        )
 
 
 def render_notification_telegram(notification):
     status_emoji = {
         "0": "\U0001F7E2",  # 🟢
         "1": "\U0001F535",  # 🔵
         "2": "\U0001F7E0",  # 🟠
         "3": "\U0001F534",  # 🔴
     }
     if notification.from_status is not None:
-        end_msg = _(
-            "changed from __%(fromst)s__ to __%(tost)s__"
-        ) % {
-            'fromst': notification.get_from_status_display(),
-            'tost': notification.get_to_status_display(),
+        end_msg = _("changed from __%(fromst)s__ to __%(tost)s__") % {
+            "fromst": notification.get_from_status_display(),
+            "tost": notification.get_to_status_display(),
         }
     else:
-        end_msg = _(
-            "created with status __%(tost)s__"
-        ) % {
-            'tost': notification.get_to_status_display(),
+        end_msg = _("created with status __%(tost)s__") % {
+            "tost": notification.get_to_status_display(),
         }
 
     msg = "{emoji} **{name}** {end_msg}".format(
-        emoji=status_emoji.get(str(notification.to_status)),
-        name=notification.service.name,
-        end_msg=end_msg
+        emoji=status_emoji.get(str(notification.to_status)), name=notification.service.name, end_msg=end_msg
     )
 
     return msg
```

