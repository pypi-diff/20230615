# Comparing `tmp/federated-content-connector-1.0.2.tar.gz` & `tmp/federated-content-connector-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-1.0.2.tar", last modified: Thu Jun 15 10:24:23 2023, max compression
+gzip compressed data, was "federated-content-connector-1.0.3.tar", last modified: Thu Jun 15 13:46:12 2023, max compression
```

## Comparing `federated-content-connector-1.0.2.tar` & `federated-content-connector-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8506 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.209461 federated-content-connector-1.0.2/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     9983 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/course_metadata_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/management/commands/import_course_runs_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.205461 federated-content-connector-1.0.2/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8506 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8567 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9586 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/course_metadata_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/management/commands/import_course_runs_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.193713 federated-content-connector-1.0.3/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.197713 federated-content-connector-1.0.3/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8567 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-15 13:46:12.000000 federated-content-connector-1.0.3/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 13:46:12.201713 federated-content-connector-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-15 13:46:03.000000 federated-content-connector-1.0.3/tests/test_signals.py
```

### Comparing `federated-content-connector-1.0.2/CHANGELOG.rst` & `federated-content-connector-1.0.3/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.3 – 2023-06-15
+------------------
+* backfill all data
+
 1.0.2 – 2023-06-15
 ------------------
 * Handle empty courserun seats.
 * Add limit query param in api call
 
 1.0.1 – 2023-06-14
 ------------------
```

### Comparing `federated-content-connector-1.0.2/LICENSE.txt` & `federated-content-connector-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/PKG-INFO` & `federated-content-connector-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.2
+Version: 1.0.3
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.3 – 2023-06-15
+------------------
+* backfill all data
+
 1.0.2 – 2023-06-15
 ------------------
 * Handle empty courserun seats.
 * Add limit query param in api call
 
 1.0.1 – 2023-06-14
 ------------------
```

### Comparing `federated-content-connector-1.0.2/README.rst` & `federated-content-connector-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector/apps.py` & `federated-content-connector-1.0.3/federated_content_connector/apps.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector/course_metadata_importer.py` & `federated-content-connector-1.0.3/federated_content_connector/course_metadata_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,32 +103,23 @@
 
         logger.info('[COURSE_METADATA_IMPORTER] Course metadata import completed for all courses.')
 
     @classmethod
     def courserun_locators_to_import(cls):
         """
         Construct list of active course locators for which we want to import data.
-
-        We will exclude the courseruns which are already imported.
         """
-        course_overviews = CourseOverview.get_all_courses()
-        course_details_ids = list(CourseDetails.objects.all().values_list('id', flat=True))
-
-        logger.info(
-            f'[COURSE_METADATA_IMPORTER] Already imported courseruns will be excluded. Keys: {course_details_ids}'
-        )
-
         now = datetime.datetime.now(pytz.UTC)
-        return list(course_overviews.filter(
+        return list(CourseOverview.objects.filter(
             Q(end__gt=now) &
             (
                 Q(enrollment_end__gt=now) |
                 Q(enrollment_end__isnull=True)
             )
-        ).exclude(id__in=course_details_ids).values_list(
+        ).values_list(
             'id',
             flat=True
         ))
 
     @classmethod
     def fetch_courses_details(cls, client, courserun_locators, api_base_url):
         """
```

### Comparing `federated-content-connector-1.0.2/federated_content_connector/filters/pipeline.py` & `federated-content-connector-1.0.3/federated_content_connector/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector/migrations/0001_initial.py` & `federated-content-connector-1.0.3/federated_content_connector/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector/models.py` & `federated-content-connector-1.0.3/federated_content_connector/models.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector/signals.py` & `federated-content-connector-1.0.3/federated_content_connector/signals.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector/tasks.py` & `federated-content-connector-1.0.3/federated_content_connector/tasks.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-1.0.3/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-1.0.3/federated_content_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.2
+Version: 1.0.3
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.3 – 2023-06-15
+------------------
+* backfill all data
+
 1.0.2 – 2023-06-15
 ------------------
 * Handle empty courserun seats.
 * Add limit query param in api call
 
 1.0.1 – 2023-06-14
 ------------------
```

### Comparing `federated-content-connector-1.0.2/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-1.0.3/federated_content_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/requirements/constraints.txt` & `federated-content-connector-1.0.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/setup.py` & `federated-content-connector-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.2/tests/test_signals.py` & `federated-content-connector-1.0.3/tests/test_signals.py`

 * *Files identical despite different names*

