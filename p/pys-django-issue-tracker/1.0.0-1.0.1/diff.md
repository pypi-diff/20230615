# Comparing `tmp/pys-django-issue-tracker-1.0.0.tar.gz` & `tmp/pys-django-issue-tracker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pys-django-issue-tracker-1.0.0.tar", last modified: Wed Jun 14 13:10:52 2023, max compression
+gzip compressed data, was "pys-django-issue-tracker-1.0.1.tar", last modified: Thu Jun 15 05:48:22 2023, max compression
```

## Comparing `pys-django-issue-tracker-1.0.0.tar` & `pys-django-issue-tracker-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.813185 pys-django-issue-tracker-1.0.0/
--rw-rw-r--   0 pys       (1000) pys       (1000)     1063 2023-06-14 07:02:14.000000 pys-django-issue-tracker-1.0.0/LICENSE.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)     5812 2023-06-14 13:10:52.813185 pys-django-issue-tracker-1.0.0/PKG-INFO
--rw-rw-r--   0 pys       (1000) pys       (1000)     4490 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/README.md
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.805184 pys-django-issue-tracker-1.0.0/issue_tracker/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      117 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/admin.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      207 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/app_settings.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      157 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/apps.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.805184 pys-django-issue-tracker-1.0.0/issue_tracker/channels/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/__init__.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.809185 pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1931 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/db.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1809 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/discord.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1644 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/email.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1327 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/slack.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2288 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/teams.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      634 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/channel.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2830 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/channels/channels_factory.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2621 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/middleware.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.809185 pys-django-issue-tracker-1.0.0/issue_tracker/migrations/
--rw-rw-r--   0 pys       (1000) pys       (1000)     1525 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/migrations/0001_initial.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      428 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/migrations/0002_remove_issue_content_type_remove_issue_user.py
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/migrations/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      784 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/models.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.809185 pys-django-issue-tracker-1.0.0/issue_tracker/tests/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/__init__.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.809185 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/__init__.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.813185 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/backends/
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/backends/__init__.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     2512 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/backends/test_discord.py
--rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/backends/test_teams.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     1685 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/test_app_settings.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      881 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/test_channel.py
--rw-rw-r--   0 pys       (1000) pys       (1000)     3415 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/test_middleware.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      984 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/conftest.py
--rw-rw-r--   0 pys       (1000) pys       (1000)      460 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.0/issue_tracker/tests/test_channels_factory.py
-drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-14 13:10:52.813185 pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/
--rw-rw-r--   0 pys       (1000) pys       (1000)     5812 2023-06-14 13:10:52.000000 pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 pys       (1000) pys       (1000)     1396 2023-06-14 13:10:52.000000 pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)        1 2023-06-14 13:10:52.000000 pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)       12 2023-06-14 13:10:52.000000 pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/requires.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)       14 2023-06-14 13:10:52.000000 pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/top_level.txt
--rw-rw-r--   0 pys       (1000) pys       (1000)       78 2023-06-14 13:10:52.813185 pys-django-issue-tracker-1.0.0/setup.cfg
--rw-rw-r--   0 pys       (1000) pys       (1000)     1690 2023-06-14 13:10:40.000000 pys-django-issue-tracker-1.0.0/setup.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1063 2023-06-14 13:33:04.000000 pys-django-issue-tracker-1.0.1/LICENSE.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)     5848 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/PKG-INFO
+-rw-rw-r--   0 pys       (1000) pys       (1000)     4490 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/README.md
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      117 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/admin.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      207 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/app_settings.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      157 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/apps.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/channels/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/__init__.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1931 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/db.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1809 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/discord.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1644 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/email.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1327 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/slack.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2288 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/teams.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      634 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/channel.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2830 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/channels/channels_factory.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2621 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/middleware.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.219771 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1525 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/0001_initial.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      428 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/0002_remove_issue_content_type_remove_issue_user.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/migrations/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      784 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/models.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/issue_tracker/tests/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/__init__.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/__init__.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/__init__.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     2512 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/test_discord.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)        0 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/test_teams.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1685 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_app_settings.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      881 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_channel.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)     3415 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_middleware.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      984 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/conftest.py
+-rw-rw-r--   0 pys       (1000) pys       (1000)      460 2023-06-14 05:29:45.000000 pys-django-issue-tracker-1.0.1/issue_tracker/tests/test_channels_factory.py
+drwxrwxr-x   0 pys       (1000) pys       (1000)        0 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/
+-rw-rw-r--   0 pys       (1000) pys       (1000)     5848 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1396 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)        1 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)      538 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/requires.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)       14 2023-06-15 05:48:22.000000 pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 pys       (1000) pys       (1000)       78 2023-06-15 05:48:22.223771 pys-django-issue-tracker-1.0.1/setup.cfg
+-rw-rw-r--   0 pys       (1000) pys       (1000)     1712 2023-06-15 05:45:00.000000 pys-django-issue-tracker-1.0.1/setup.py
```

### Comparing `pys-django-issue-tracker-1.0.0/LICENSE.txt` & `pys-django-issue-tracker-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/PKG-INFO` & `pys-django-issue-tracker-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pys-django-issue-tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Issue tracker
 Home-page: https://github.com/pys-info/pys-issue-tracker
 Author: Pysquad
 Author-email: vh@pysquad.com
+License: UNKNOWN
 Project-URL: Source, https://github.com/pys-info/pys-issue-tracker
 Keywords: django,issue,tracker,development
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
@@ -110,7 +112,8 @@
 -  Release version related information you can get inside the release-notes documents.See details information inside `docs/release-notes.rst`
 
 ## License
 *MIT License:* <https://choosealicense.com/licenses/mit/>
 
 ## Contact
 For any inquiries or feedback, you can reach us at xyz@example.com or join our community channel.
+
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.1 Summary:
 Django Issue tracker Home-page: https://github.com/pys-info/pys-issue-tracker
-Author: Pysquad Author-email: vh@pysquad.com Project-URL: Source, https://
-github.com/pys-info/pys-issue-tracker Keywords:
-django,issue,tracker,development Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
-:: Software Development :: Build Tools Classifier: License :: OSI Approved ::
-MIT License Classifier: Environment :: Web Environment Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Framework :: Django Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5 Description-
-Content-Type: text/markdown License-File: LICENSE.txt
+Author: Pysquad Author-email: vh@pysquad.com License: UNKNOWN Project-URL:
+Source, https://github.com/pys-info/pys-issue-tracker Keywords:
+django,issue,tracker,development Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
+OSI Approved :: MIT License Classifier: Environment :: Web Environment
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Framework :: Django Classifier: Framework ::
+Django :: 3.0 Classifier: Framework :: Django :: 3.1 Classifier: Framework ::
+Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
+Django :: 4.1 Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5
+Description-Content-Type: text/markdown License-File: LICENSE.txt
 ****** django-issue-tracker ******
 **[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/)** [Made_with_Django.] ## Project
 description Django Issue Tracker is a robust package designed to streamline
 issue tracking within Django web applications.The package supports various
 notification channels, allowing teams to receive updates through their
 preferred communication methods.By integrating this package, teams can
```

### Comparing `pys-django-issue-tracker-1.0.0/README.md` & `pys-django-issue-tracker-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/db.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/db.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/discord.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/discord.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/email.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/email.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/slack.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/slack.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/channels/backends/teams.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/channels/backends/teams.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/channels/channel.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/channels/channel.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/channels/channels_factory.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/channels/channels_factory.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/middleware.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/middleware.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/migrations/0001_initial.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/models.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/models.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/backends/test_discord.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/backends/test_discord.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/test_app_settings.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/test_channel.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_channel.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/tests/channels/test_middleware.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/tests/channels/test_middleware.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/issue_tracker/tests/conftest.py` & `pys-django-issue-tracker-1.0.1/issue_tracker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/PKG-INFO` & `pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pys-django-issue-tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Issue tracker
 Home-page: https://github.com/pys-info/pys-issue-tracker
 Author: Pysquad
 Author-email: vh@pysquad.com
+License: UNKNOWN
 Project-URL: Source, https://github.com/pys-info/pys-issue-tracker
 Keywords: django,issue,tracker,development
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
@@ -110,7 +112,8 @@
 -  Release version related information you can get inside the release-notes documents.See details information inside `docs/release-notes.rst`
 
 ## License
 *MIT License:* <https://choosealicense.com/licenses/mit/>
 
 ## Contact
 For any inquiries or feedback, you can reach us at xyz@example.com or join our community channel.
+
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: pys-django-issue-tracker Version: 1.0.1 Summary:
 Django Issue tracker Home-page: https://github.com/pys-info/pys-issue-tracker
-Author: Pysquad Author-email: vh@pysquad.com Project-URL: Source, https://
-github.com/pys-info/pys-issue-tracker Keywords:
-django,issue,tracker,development Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
-:: Software Development :: Build Tools Classifier: License :: OSI Approved ::
-MIT License Classifier: Environment :: Web Environment Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Framework :: Django Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5 Description-
-Content-Type: text/markdown License-File: LICENSE.txt
+Author: Pysquad Author-email: vh@pysquad.com License: UNKNOWN Project-URL:
+Source, https://github.com/pys-info/pys-issue-tracker Keywords:
+django,issue,tracker,development Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
+OSI Approved :: MIT License Classifier: Environment :: Web Environment
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Framework :: Django Classifier: Framework ::
+Django :: 3.0 Classifier: Framework :: Django :: 3.1 Classifier: Framework ::
+Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
+Django :: 4.1 Classifier: Framework :: Django :: 4.2 Requires-Python: >=3.5
+Description-Content-Type: text/markdown License-File: LICENSE.txt
 ****** django-issue-tracker ******
 **[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/)** [Made_with_Django.] ## Project
 description Django Issue Tracker is a robust package designed to streamline
 issue tracking within Django web applications.The package supports various
 notification channels, allowing teams to receive updates through their
 preferred communication methods.By integrating this package, teams can
```

### Comparing `pys-django-issue-tracker-1.0.0/pys_django_issue_tracker.egg-info/SOURCES.txt` & `pys-django-issue-tracker-1.0.1/pys_django_issue_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pys-django-issue-tracker-1.0.0/setup.py` & `pys-django-issue-tracker-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from setuptools import setup, find_packages
 import pathlib
 
+from setuptools import find_packages, setup
+
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pys-django-issue-tracker",
-    version="1.0.0",
+    version="1.0.1",
     author="Pysquad",
     author_email="vh@pysquad.com",
     description="Django Issue tracker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pys-info/pys-issue-tracker",
-    install_requires=[
-        'Django>=3.0',
-    ],
+    install_requires=[line.strip() for line in open("requirements.txt")],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Environment :: Web Environment",
         "Operating System :: OS Independent",
```

