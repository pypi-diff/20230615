# Comparing `tmp/ora2-5.0.2.tar.gz` & `tmp/ora2-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ora2-5.0.2.tar", last modified: Wed May 31 13:11:01 2023, max compression
+gzip compressed data, was "ora2-5.0.3.tar", last modified: Wed Jun 14 23:39:51 2023, max compression
```

## Comparing `ora2-5.0.2.tar` & `ora2-5.0.3.tar`

### file list

```diff
@@ -1,551 +1,551 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.215283 ora2-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-05-31 13:10:52.000000 ora2-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-31 13:10:52.000000 ora2-5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-05-31 13:11:01.215283 ora2-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-05-31 13:10:52.000000 ora2-5.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/assessment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/assessment/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39052 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/api/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/api/self.py
--rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/api/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/api/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/api/teams.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/data_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/assessment/errors/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/errors/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/errors/self.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/errors/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/errors/student_training.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/assessment/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/0002_staffworkflow.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/0003_expand_course_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/0006_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/0007_staff_workflow_blank.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/assessment/models/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/models/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/models/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/models/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/models/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/score_type_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/assessment/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/serializers/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/serializers/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/assessment/views.py
--rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/fileupload/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/fileupload/backends/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/backends/django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/backends/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/backends/swift.py
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/views_django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/fileupload/views_filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.131277 ora2-5.0.2/openassessment/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.135277 ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82260 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   137572 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/ar_SA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.135277 ora2-5.0.2/openassessment/locale/ar_SA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.135277 ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.135277 ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.135277 ora2-5.0.2/openassessment/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    94672 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23724 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.135277 ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)   145495 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   195906 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    21982 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    38500 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.135277 ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.139278 ora2-5.0.2/openassessment/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.139278 ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.139278 ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.139278 ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.139278 ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.139278 ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.143278 ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.143278 ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.143278 ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    40204 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   112010 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.143278 ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.143278 ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.143278 ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.143278 ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.147278 ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/messages.mo
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.147278 ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.147278 ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.147278 ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.147278 ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.147278 ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81743 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   132378 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29200 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.147278 ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.151278 ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.151278 ora2-5.0.2/openassessment/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.151278 ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/sw_KE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.151278 ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.151278 ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.151278 ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    49577 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   116193 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.151278 ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.123276 ora2-5.0.2/openassessment/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/management/commands/collect_ora2_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/management/commands/create_oa_submissions.py
--rw-r--r--   0 runner    (1001) docker     (122)    17900 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/management/commands/create_oa_submissions_from_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/management/commands/upload_oa_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/runtime_imports/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/runtime_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/runtime_imports/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/runtime_imports/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/staffgrader/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/staffgrader/errors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/errors/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/staffgrader/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/staffgrader/models/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/models/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.155279 ora2-5.0.2/openassessment/staffgrader/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      474 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/serializers/assessments.py
--rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/serializers/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/serializers/submission_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/staffgrader/staff_grader_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.159279 ora2-5.0.2/openassessment/templates/openassessmentblock/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.159279 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit.html
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
--rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
--rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_training_example.html
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.159279 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/
--rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.159279 ora2-5.0.2/openassessment/templates/openassessmentblock/icons/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/icons/warning_filled.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.159279 ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.163279 ora2-5.0.2/openassessment/templates/openassessmentblock/leaderboard/
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.163279 ora2-5.0.2/openassessment/templates/openassessmentblock/message/
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_open.html
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/oa_base.html
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/oa_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/oa_latex_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/oa_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/oa_submission_answer.html
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
--rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/oa_uploaded_file.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.163279 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/
--rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.163279 ora2-5.0.2/openassessment/templates/openassessmentblock/response/
--rw-r--r--   0 runner    (1001) docker     (122)    21833 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response.html
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_graded.html
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.163279 ora2-5.0.2/openassessment/templates/openassessmentblock/self/
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.163279 ora2-5.0.2/openassessment/templates/openassessmentblock/staff/
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.167280 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/
--rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
--rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.167280 ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/
--rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.167280 ora2-5.0.2/openassessment/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/templatetags/oa_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.167280 ora2-5.0.2/openassessment/workflow/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    19932 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.167280 ora2-5.0.2/openassessment/workflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/migrations/0002_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/migrations/0003_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44741 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     8350 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/workflow/team_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.171280 ora2-5.0.2/openassessment/xblock/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/config_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      914 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/course_items_listing_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/editor_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30777 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/grade_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/leaderboard_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/lms_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/load_static.py
--rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/message_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/mobile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/openassesment_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    51017 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/openassessmentblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/peer_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/resolve_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/rubric_reuse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/self_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    34259 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/staff_area_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/staff_assessment_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/xblock/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/xblock/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/xblock/static/css/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.171280 ora2-5.0.2/openassessment/xblock/static/css/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/css/lib/backgrid/backgrid.css
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.207283 ora2-5.0.2/openassessment/xblock/static/dist/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js
--rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js
--rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-lms.css
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.css
--rw-r--r--   0 runner    (1001) docker     (122)  1350596 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js
--rw-r--r--   0 runner    (1001) docker     (122) 28868716 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-lms.js
--rw-r--r--   0 runner    (1001) docker     (122)   757135 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js
--rw-r--r--   0 runner    (1001) docker     (122)   851349 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.css
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.js
--rw-r--r--   0 runner    (1001) docker     (122)   757164 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js
--rw-r--r--   0 runner    (1001) docker     (122)   851378 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.css
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.js
--rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js
--rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/dist/openassessment-studio.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/xblock/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.127277 ora2-5.0.2/openassessment/xblock/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.211283 ora2-5.0.2/openassessment/xblock/static/js/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/lib/backgrid/backgrid.js
--rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.211283 ora2-5.0.2/openassessment/xblock/static/js/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.215283 ora2-5.0.2/openassessment/xblock/static/js/src/lms/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.215283 ora2-5.0.2/openassessment/xblock/static/js/src/lms/api/
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.215283 ora2-5.0.2/openassessment/xblock/static/js/src/lms/editors/
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_base.js
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_datefactory.js
--rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_file_upload.js
--rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_grade.js
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_message.js
--rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_peer.js
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    32835 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_response.js
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_response_editor.js
--rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_self.js
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_staff.js
--rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_staff_area.js
--rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_training.js
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/lms_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    26166 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/oa_server.js
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/oa_shared.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.215283 ora2-5.0.2/openassessment/xblock/static/js/src/studio/
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_container.js
--rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_container_item.js
--rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
--rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
--rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
--rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/static/js/src/studio_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/student_training_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/studio_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    42012 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/submission_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/team_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/team_workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/user_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     8409 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-05-31 13:10:52.000000 ora2-5.0.2/openassessment/xblock/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.215283 ora2-5.0.2/ora2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-05-31 13:11:01.000000 ora2-5.0.2/ora2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23039 2023-05-31 13:11:01.000000 ora2-5.0.2/ora2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 13:11:01.000000 ora2-5.0.2/ora2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-31 13:11:01.000000 ora2-5.0.2/ora2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-31 13:11:01.000000 ora2-5.0.2/ora2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-31 13:11:01.000000 ora2-5.0.2/ora2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:11:01.215283 ora2-5.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/quality.in
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/test-acceptance.in
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-31 13:10:52.000000 ora2-5.0.2/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-31 13:11:01.215283 ora2-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-05-31 13:10:52.000000 ora2-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.417129 ora2-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-06-14 23:39:45.000000 ora2-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-14 23:39:45.000000 ora2-5.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-14 23:39:51.417129 ora2-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-06-14 23:39:45.000000 ora2-5.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.313123 ora2-5.0.3/openassessment/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.313123 ora2-5.0.3/openassessment/assessment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.313123 ora2-5.0.3/openassessment/assessment/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39052 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/api/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/api/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/api/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/api/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/api/teams.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.313123 ora2-5.0.3/openassessment/assessment/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/errors/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/errors/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/errors/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/errors/student_training.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.313123 ora2-5.0.3/openassessment/assessment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/0002_staffworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/0003_expand_course_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/0006_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/0007_staff_workflow_blank.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.317124 ora2-5.0.3/openassessment/assessment/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/models/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/models/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/models/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/models/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/score_type_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.317124 ora2-5.0.3/openassessment/assessment/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/serializers/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/serializers/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/assessment/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.317124 ora2-5.0.3/openassessment/fileupload/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.317124 ora2-5.0.3/openassessment/fileupload/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/backends/django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/backends/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/backends/swift.py
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/views_django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/fileupload/views_filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.317124 ora2-5.0.3/openassessment/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.321124 ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82260 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   137572 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/ar_SA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.321124 ora2-5.0.3/openassessment/locale/ar_SA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.321124 ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.321124 ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.321124 ora2-5.0.3/openassessment/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    94672 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23724 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.321124 ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)   145495 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   195906 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    21982 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    38500 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.325124 ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.301123 ora2-5.0.3/openassessment/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.325124 ora2-5.0.3/openassessment/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.325124 ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.325124 ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.325124 ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.329124 ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.329124 ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.329124 ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.329124 ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.329124 ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    40204 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112010 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.333124 ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.333124 ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.333124 ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.333124 ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.333124 ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/messages.mo
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.337124 ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.337124 ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.337124 ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.337124 ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.337124 ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81743 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132378 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29200 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.337124 ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.341125 ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.305123 ora2-5.0.3/openassessment/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.341125 ora2-5.0.3/openassessment/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.341125 ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/sw_KE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.341125 ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.341125 ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.345125 ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    49577 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116193 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.345125 ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.345125 ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.345125 ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.345125 ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.345125 ora2-5.0.3/openassessment/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.345125 ora2-5.0.3/openassessment/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/management/commands/collect_ora2_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/management/commands/create_oa_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17900 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/management/commands/create_oa_submissions_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/management/commands/upload_oa_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.349125 ora2-5.0.3/openassessment/runtime_imports/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/runtime_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/runtime_imports/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/runtime_imports/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.349125 ora2-5.0.3/openassessment/staffgrader/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.349125 ora2-5.0.3/openassessment/staffgrader/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/errors/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.349125 ora2-5.0.3/openassessment/staffgrader/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.349125 ora2-5.0.3/openassessment/staffgrader/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/models/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.349125 ora2-5.0.3/openassessment/staffgrader/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/serializers/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/serializers/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/serializers/submission_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/staffgrader/staff_grader_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.349125 ora2-5.0.3/openassessment/templates/openassessmentblock/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.353125 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
+-rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_training_example.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.353125 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/
+-rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.353125 ora2-5.0.3/openassessment/templates/openassessmentblock/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/icons/warning_filled.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.357126 ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.357126 ora2-5.0.3/openassessment/templates/openassessmentblock/leaderboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.357126 ora2-5.0.3/openassessment/templates/openassessmentblock/message/
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_open.html
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/oa_base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/oa_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/oa_latex_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/oa_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/oa_submission_answer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/oa_uploaded_file.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.357126 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/
+-rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.357126 ora2-5.0.3/openassessment/templates/openassessmentblock/response/
+-rw-r--r--   0 runner    (1001) docker     (122)    21833 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_graded.html
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.361126 ora2-5.0.3/openassessment/templates/openassessmentblock/self/
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.361126 ora2-5.0.3/openassessment/templates/openassessmentblock/staff/
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.361126 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/
+-rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.361126 ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/
+-rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.361126 ora2-5.0.3/openassessment/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/templatetags/oa_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.361126 ora2-5.0.3/openassessment/workflow/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19932 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.365126 ora2-5.0.3/openassessment/workflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/migrations/0002_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/migrations/0003_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44741 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8350 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/workflow/team_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.369126 ora2-5.0.3/openassessment/xblock/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/config_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      914 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/course_items_listing_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/editor_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30777 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/grade_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/leaderboard_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/lms_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/load_static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/message_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/openassesment_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50871 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/openassessmentblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/peer_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/resolve_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/rubric_reuse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/self_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34259 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/staff_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/staff_assessment_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/xblock/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/xblock/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/xblock/static/css/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.369126 ora2-5.0.3/openassessment/xblock/static/css/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/css/lib/backgrid/backgrid.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.409128 ora2-5.0.3/openassessment/xblock/static/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js
+-rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js
+-rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-lms.css
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.css
+-rw-r--r--   0 runner    (1001) docker     (122)  1350596 2023-06-14 23:39:45.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js
+-rw-r--r--   0 runner    (1001) docker     (122) 28868716 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-lms.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757135 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js
+-rw-r--r--   0 runner    (1001) docker     (122)   851349 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.css
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757164 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js
+-rw-r--r--   0 runner    (1001) docker     (122)   851378 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.css
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.js
+-rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/dist/openassessment-studio.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/xblock/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.309123 ora2-5.0.3/openassessment/xblock/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.409128 ora2-5.0.3/openassessment/xblock/static/js/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/lib/backgrid/backgrid.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.413128 ora2-5.0.3/openassessment/xblock/static/js/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.413128 ora2-5.0.3/openassessment/xblock/static/js/src/lms/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.413128 ora2-5.0.3/openassessment/xblock/static/js/src/lms/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.413128 ora2-5.0.3/openassessment/xblock/static/js/src/lms/editors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_base.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_datefactory.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_file_upload.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_grade.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_message.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_peer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    32835 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_response.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_response_editor.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_self.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_staff.js
+-rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_staff_area.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_training.js
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/lms_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26166 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/oa_server.js
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/oa_shared.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.417129 ora2-5.0.3/openassessment/xblock/static/js/src/studio/
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_container.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_container_item.js
+-rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/static/js/src/studio_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/student_training_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/studio_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42012 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/submission_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/team_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/team_workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8409 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-06-14 23:39:46.000000 ora2-5.0.3/openassessment/xblock/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.417129 ora2-5.0.3/ora2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-14 23:39:51.000000 ora2-5.0.3/ora2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23039 2023-06-14 23:39:51.000000 ora2-5.0.3/ora2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 23:39:51.000000 ora2-5.0.3/ora2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-14 23:39:51.000000 ora2-5.0.3/ora2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-14 23:39:51.000000 ora2-5.0.3/ora2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-14 23:39:51.000000 ora2-5.0.3/ora2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 23:39:51.417129 ora2-5.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/quality.in
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/test-acceptance.in
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-14 23:39:46.000000 ora2-5.0.3/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-14 23:39:51.417129 ora2-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-06-14 23:39:46.000000 ora2-5.0.3/setup.py
```

### Comparing `ora2-5.0.2/LICENSE` & `ora2-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/MANIFEST.in` & `ora2-5.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/PKG-INFO` & `ora2-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.0.2
+Version: 5.0.3
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.0.2/README.rst` & `ora2-5.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/admin.py` & `ora2-5.0.3/openassessment/assessment/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/api/peer.py` & `ora2-5.0.3/openassessment/assessment/api/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/api/self.py` & `ora2-5.0.3/openassessment/assessment/api/self.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/api/staff.py` & `ora2-5.0.3/openassessment/assessment/api/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/api/student_training.py` & `ora2-5.0.3/openassessment/assessment/api/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/api/teams.py` & `ora2-5.0.3/openassessment/assessment/api/teams.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/errors/peer.py` & `ora2-5.0.3/openassessment/assessment/errors/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/errors/self.py` & `ora2-5.0.3/openassessment/assessment/errors/self.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/errors/staff.py` & `ora2-5.0.3/openassessment/assessment/errors/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/migrations/0001_initial.py` & `ora2-5.0.3/openassessment/assessment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/migrations/0002_staffworkflow.py` & `ora2-5.0.3/openassessment/assessment/migrations/0002_staffworkflow.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/migrations/0003_expand_course_id.py` & `ora2-5.0.3/openassessment/assessment/migrations/0003_expand_course_id.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py` & `ora2-5.0.3/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py` & `ora2-5.0.3/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/migrations/0006_TeamWorkflows.py` & `ora2-5.0.3/openassessment/assessment/migrations/0006_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/migrations/0007_staff_workflow_blank.py` & `ora2-5.0.3/openassessment/assessment/migrations/0007_staff_workflow_blank.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/models/base.py` & `ora2-5.0.3/openassessment/assessment/models/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/models/peer.py` & `ora2-5.0.3/openassessment/assessment/models/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/models/staff.py` & `ora2-5.0.3/openassessment/assessment/models/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/models/student_training.py` & `ora2-5.0.3/openassessment/assessment/models/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/models/training.py` & `ora2-5.0.3/openassessment/assessment/models/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/serializers/base.py` & `ora2-5.0.3/openassessment/assessment/serializers/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/serializers/peer.py` & `ora2-5.0.3/openassessment/assessment/serializers/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/serializers/training.py` & `ora2-5.0.3/openassessment/assessment/serializers/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/assessment/views.py` & `ora2-5.0.3/openassessment/assessment/views.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/data.py` & `ora2-5.0.3/openassessment/data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/api.py` & `ora2-5.0.3/openassessment/fileupload/api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/backends/__init__.py` & `ora2-5.0.3/openassessment/fileupload/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/backends/base.py` & `ora2-5.0.3/openassessment/fileupload/backends/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/backends/django_storage.py` & `ora2-5.0.3/openassessment/fileupload/backends/django_storage.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/backends/filesystem.py` & `ora2-5.0.3/openassessment/fileupload/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/backends/s3.py` & `ora2-5.0.3/openassessment/fileupload/backends/s3.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/backends/swift.py` & `ora2-5.0.3/openassessment/fileupload/backends/swift.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/exceptions.py` & `ora2-5.0.3/openassessment/fileupload/exceptions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/fileupload/views_filesystem.py` & `ora2-5.0.3/openassessment/fileupload/views_filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ar/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/el/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/en/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/en/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eo/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_419/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/es_419/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/he/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/hi/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/hi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/id/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ka/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/ka/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/lv/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/messages.mo` & `ora2-5.0.3/openassessment/locale/messages.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/mn/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/nb/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pl/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ro/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/ru/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sk/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sk/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sq/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/sq/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/th/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/th/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/uk/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/vi/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/vi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/django.mo` & `ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/django.po` & `ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo` & `ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po` & `ora2-5.0.3/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/management/commands/collect_ora2_data.py` & `ora2-5.0.3/openassessment/management/commands/collect_ora2_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/management/commands/create_oa_submissions.py` & `ora2-5.0.3/openassessment/management/commands/create_oa_submissions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/management/commands/create_oa_submissions_from_file.py` & `ora2-5.0.3/openassessment/management/commands/create_oa_submissions_from_file.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/management/commands/upload_oa_data.py` & `ora2-5.0.3/openassessment/management/commands/upload_oa_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/runtime_imports/classes.py` & `ora2-5.0.3/openassessment/runtime_imports/classes.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/runtime_imports/functions.py` & `ora2-5.0.3/openassessment/runtime_imports/functions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/staffgrader/admin.py` & `ora2-5.0.3/openassessment/staffgrader/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/staffgrader/migrations/0001_initial.py` & `ora2-5.0.3/openassessment/staffgrader/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/staffgrader/models/submission_lock.py` & `ora2-5.0.3/openassessment/staffgrader/models/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/staffgrader/serializers/assessments.py` & `ora2-5.0.3/openassessment/staffgrader/serializers/assessments.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/staffgrader/serializers/submission_list.py` & `ora2-5.0.3/openassessment/staffgrader/serializers/submission_list.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/staffgrader/serializers/submission_lock.py` & `ora2-5.0.3/openassessment/staffgrader/serializers/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/staffgrader/staff_grader_mixin.py` & `ora2-5.0.3/openassessment/staffgrader/staff_grader_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_option.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_option.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_training_example.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_training_example.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_closed.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_complete.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_no_team.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_no_team.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/message/oa_message_open.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/message/oa_message_open.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/oa_base.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/oa_base.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/oa_latex_preview.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/oa_latex_preview.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/oa_rubric.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/oa_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/oa_submission_answer.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/oa_submission_answer.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/oa_uploaded_file.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/oa_uploaded_file.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_closed.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_graded.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_graded.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_submitted.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_assessment.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_closed.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_complete.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_closed.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_complete.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_error.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_error.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html` & `ora2-5.0.3/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/templatetags/oa_extras.py` & `ora2-5.0.3/openassessment/templatetags/oa_extras.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/test_utils.py` & `ora2-5.0.3/openassessment/test_utils.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/admin.py` & `ora2-5.0.3/openassessment/workflow/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/api.py` & `ora2-5.0.3/openassessment/workflow/api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/errors.py` & `ora2-5.0.3/openassessment/workflow/errors.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/migrations/0001_initial.py` & `ora2-5.0.3/openassessment/workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/migrations/0003_TeamWorkflows.py` & `ora2-5.0.3/openassessment/workflow/migrations/0003_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/models.py` & `ora2-5.0.3/openassessment/workflow/models.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/serializers.py` & `ora2-5.0.3/openassessment/workflow/serializers.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/workflow/team_api.py` & `ora2-5.0.3/openassessment/workflow/team_api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/config_mixin.py` & `ora2-5.0.3/openassessment/xblock/config_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/course_items_listing_mixin.py` & `ora2-5.0.3/openassessment/xblock/course_items_listing_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/data_conversion.py` & `ora2-5.0.3/openassessment/xblock/data_conversion.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/defaults.py` & `ora2-5.0.3/openassessment/xblock/defaults.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/editor_config.py` & `ora2-5.0.3/openassessment/xblock/editor_config.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/grade_mixin.py` & `ora2-5.0.3/openassessment/xblock/grade_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/leaderboard_mixin.py` & `ora2-5.0.3/openassessment/xblock/leaderboard_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/lms_mixin.py` & `ora2-5.0.3/openassessment/xblock/lms_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/load_static.py` & `ora2-5.0.3/openassessment/xblock/load_static.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/message_mixin.py` & `ora2-5.0.3/openassessment/xblock/message_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/mobile.py` & `ora2-5.0.3/openassessment/xblock/mobile.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/openassesment_template_mixin.py` & `ora2-5.0.3/openassessment/xblock/openassesment_template_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/openassessmentblock.py` & `ora2-5.0.3/openassessment/xblock/openassessmentblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1335,20 +1335,18 @@
             return user.username
         return None
 
     def _adjust_start_date_for_beta_testers(self, start):
         """
         Returns the start date for a Beta tester.
         """
-        if hasattr(self, "xmodule_runtime"):
-            days_early_for_beta = getattr(self.xmodule_runtime, 'days_early_for_beta', 0)  # pylint: disable=no-member
-            if days_early_for_beta is not None:
-                delta = dt.timedelta(days_early_for_beta)
-                effective = start - delta
-                return effective
+        if days_early_for_beta := getattr(self, 'days_early_for_beta', None):
+            delta = dt.timedelta(days_early_for_beta)
+            effective = start - delta
+            return effective
 
         return start
 
     def get_xblock_id(self):
         """
         Returns the xblock id
         """
```

### Comparing `ora2-5.0.2/openassessment/xblock/peer_assessment_mixin.py` & `ora2-5.0.3/openassessment/xblock/peer_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/resolve_dates.py` & `ora2-5.0.3/openassessment/xblock/resolve_dates.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/rubric_reuse_mixin.py` & `ora2-5.0.3/openassessment/xblock/rubric_reuse_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/schema.py` & `ora2-5.0.3/openassessment/xblock/schema.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/self_assessment_mixin.py` & `ora2-5.0.3/openassessment/xblock/self_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/staff_area_mixin.py` & `ora2-5.0.3/openassessment/xblock/staff_area_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/staff_assessment_mixin.py` & `ora2-5.0.3/openassessment/xblock/staff_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/css/lib/backgrid/backgrid.css` & `ora2-5.0.3/openassessment/xblock/static/css/lib/backgrid/backgrid.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css` & `ora2-5.0.3/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/manifest.json` & `ora2-5.0.3/openassessment/xblock/static/dist/manifest.json`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-textarea.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-editor-tinymce.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-editor-tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-lms.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-lms.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.css` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-ltr.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-ltr.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.css` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-rtl.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-rtl.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/dist/openassessment-studio.js` & `ora2-5.0.3/openassessment/xblock/static/dist/openassessment-studio.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/lib/backgrid/backgrid.js` & `ora2-5.0.3/openassessment/xblock/static/js/lib/backgrid/backgrid.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js` & `ora2-5.0.3/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_base.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_base.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_datefactory.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_datefactory.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_file_upload.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_file_upload.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_grade.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_grade.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_leaderboard.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_leaderboard.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_message.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_message.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_peer.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_peer.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_prompts.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_response.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_response.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_response_editor.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_response_editor.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_rubric.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_self.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_self.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_staff.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_staff.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_staff_area.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_staff_area.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/lms/oa_training.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/lms/oa_training.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/oa_server.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/oa_server.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/oa_shared.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/oa_shared.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_container.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_container.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_container_item.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_container_item.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_fields.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_fields.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_settings.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_settings.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js` & `ora2-5.0.3/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/student_training_mixin.py` & `ora2-5.0.3/openassessment/xblock/student_training_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/studio_mixin.py` & `ora2-5.0.3/openassessment/xblock/studio_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/submission_mixin.py` & `ora2-5.0.3/openassessment/xblock/submission_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/team_mixin.py` & `ora2-5.0.3/openassessment/xblock/team_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/team_workflow_mixin.py` & `ora2-5.0.3/openassessment/xblock/team_workflow_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/user_data.py` & `ora2-5.0.3/openassessment/xblock/user_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/validation.py` & `ora2-5.0.3/openassessment/xblock/validation.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/workflow_mixin.py` & `ora2-5.0.3/openassessment/xblock/workflow_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/openassessment/xblock/xml.py` & `ora2-5.0.3/openassessment/xblock/xml.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/ora2.egg-info/PKG-INFO` & `ora2-5.0.3/ora2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.0.2
+Version: 5.0.3
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.0.2/ora2.egg-info/SOURCES.txt` & `ora2-5.0.3/ora2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/requirements/test.in` & `ora2-5.0.3/requirements/test.in`

 * *Files identical despite different names*

### Comparing `ora2-5.0.2/setup.py` & `ora2-5.0.3/setup.py`

 * *Files identical despite different names*

