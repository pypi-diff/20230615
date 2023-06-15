# Comparing `tmp/federated-content-connector-1.0.1.tar.gz` & `tmp/federated-content-connector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-1.0.1.tar", last modified: Wed Jun 14 13:20:24 2023, max compression
+gzip compressed data, was "federated-content-connector-1.0.2.tar", last modified: Thu Jun 15 10:24:23 2023, max compression
```

## Comparing `federated-content-connector-1.0.1.tar` & `federated-content-connector-1.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8397 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     9672 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/course_metadata_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/management/commands/import_course_runs_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.455163 federated-content-connector-1.0.1/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.459163 federated-content-connector-1.0.1/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8397 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-14 13:20:24.000000 federated-content-connector-1.0.1/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:20:24.463163 federated-content-connector-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-14 13:20:16.000000 federated-content-connector-1.0.1/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8506 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.209461 federated-content-connector-1.0.2/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9983 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/course_metadata_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/management/commands/import_course_runs_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.205461 federated-content-connector-1.0.2/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.213461 federated-content-connector-1.0.2/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8506 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-15 10:24:23.000000 federated-content-connector-1.0.2/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:24:23.217461 federated-content-connector-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-15 10:24:10.000000 federated-content-connector-1.0.2/tests/test_signals.py
```

### Comparing `federated-content-connector-1.0.1/CHANGELOG.rst` & `federated-content-connector-1.0.2/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.2 – 2023-06-15
+------------------
+* Handle empty courserun seats.
+* Add limit query param in api call
+
 1.0.1 – 2023-06-14
 ------------------
 * Update courserun seat sorting logic.
 
 1.0.0 – 2023-06-06
 ------------------
 * Fetch course metadata from discovery and store.
```

### Comparing `federated-content-connector-1.0.1/LICENSE.txt` & `federated-content-connector-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/PKG-INFO` & `federated-content-connector-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.2 – 2023-06-15
+------------------
+* Handle empty courserun seats.
+* Add limit query param in api call
+
 1.0.1 – 2023-06-14
 ------------------
 * Update courserun seat sorting logic.
 
 1.0.0 – 2023-06-06
 ------------------
 * Fetch course metadata from discovery and store.
```

### Comparing `federated-content-connector-1.0.1/README.rst` & `federated-content-connector-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector/apps.py` & `federated-content-connector-1.0.2/federated_content_connector/apps.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector/course_metadata_importer.py` & `federated-content-connector-1.0.2/federated_content_connector/course_metadata_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         """
         Fetch the course data from discovery using `/api/v1/courses` endpoint.
         """
         course_keys = [cls.construct_course_key(courserun_locator) for courserun_locator in courserun_locators]
         encoded_course_keys = ','.join(map(quote_plus, course_keys))
 
         logger.info(f'[COURSE_METADATA_IMPORTER] Fetching details from discovery. Courses {course_keys}.')
-        api_url = urljoin(f"{api_base_url}/", f"courses/?keys={encoded_course_keys}")
+        api_url = urljoin(f"{api_base_url}/", f"courses/?limit=50&keys={encoded_course_keys}")
         response = client.get(api_url)
         response.raise_for_status()
         courses_details = response.json()
         results = courses_details.get('results', [])
 
         # Find and log the course keys not found in course-discovery
         course_keys_in_response = [result.get('key') for result in results]
@@ -182,15 +182,20 @@
                     enroll_by = additional_metadata.get('registration_deadline')
                     start_date = additional_metadata.get('start_date')
                     end_date = additional_metadata.get('end_date')
             else:
                 course_run = cls.find_attr(course_metadata.get('course_runs'), 'key', courserun_key)
                 if course_run:
                     seat = cls.find_best_mode_seat(course_run.get('seats'))
-                    enroll_by = seat.get('upgrade_deadline')
+                    if seat:
+                        enroll_by = seat.get('upgrade_deadline')
+                    else:
+                        logger.info(
+                            f"[{log_prefix}] No Seat Found. Seats: {course_run.get('seats')}"
+                        )
                     start_date = course_run.get('start')
                     end_date = course_run.get('end')
                 else:
                     logger.info(
                         f'[{log_prefix}] Courserun not found. CourserunKey: {courserun_key}, CourseKey: {course_key}'
                     )
 
@@ -227,15 +232,19 @@
             """
             mode_type = mode['type']
             if mode_type in BEST_MODE_ORDER:
                 return len(BEST_MODE_ORDER) - BEST_MODE_ORDER.index(mode_type)
             else:
                 return 0
 
-        return sorted(seats, key=sort_key, reverse=True)[0]
+        sorted_seats = sorted(seats, key=sort_key, reverse=True)
+        if sorted_seats:
+            return sorted_seats[0]
+
+        return None
 
     @classmethod
     def chunks(cls, keys, chunk_size=50):
         """
         Yield chunks of size `chunk_size`.
         """
         for i in range(0, len(keys), chunk_size):
```

### Comparing `federated-content-connector-1.0.1/federated_content_connector/filters/pipeline.py` & `federated-content-connector-1.0.2/federated_content_connector/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector/migrations/0001_initial.py` & `federated-content-connector-1.0.2/federated_content_connector/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector/models.py` & `federated-content-connector-1.0.2/federated_content_connector/models.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector/signals.py` & `federated-content-connector-1.0.2/federated_content_connector/signals.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector/tasks.py` & `federated-content-connector-1.0.2/federated_content_connector/tasks.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-1.0.2/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-1.0.2/federated_content_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,19 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.0.2 – 2023-06-15
+------------------
+* Handle empty courserun seats.
+* Add limit query param in api call
+
 1.0.1 – 2023-06-14
 ------------------
 * Update courserun seat sorting logic.
 
 1.0.0 – 2023-06-06
 ------------------
 * Fetch course metadata from discovery and store.
```

### Comparing `federated-content-connector-1.0.1/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-1.0.2/federated_content_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/requirements/constraints.txt` & `federated-content-connector-1.0.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/setup.py` & `federated-content-connector-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.0.1/tests/test_signals.py` & `federated-content-connector-1.0.2/tests/test_signals.py`

 * *Files identical despite different names*

