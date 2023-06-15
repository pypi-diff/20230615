# Comparing `tmp/superspreader-0.2.4.tar.gz` & `tmp/superspreader-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.2.4.tar", last modified: Wed Jun 14 15:15:59 2023, max compression
+gzip compressed data, was "superspreader-0.2.5.tar", last modified: Thu Jun 15 07:01:59 2023, max compression
```

## Comparing `superspreader-0.2.4.tar` & `superspreader-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 15:15:50.000000 superspreader-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 15:15:59.955763 superspreader-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-14 15:15:50.000000 superspreader-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 15:15:50.000000 superspreader-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 15:15:59.959763 superspreader-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-14 15:15:50.000000 superspreader-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-14 15:15:50.000000 superspreader-0.2.4/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 15:15:59.000000 superspreader-0.2.4/src/superspreader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:15:59.955763 superspreader-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 15:15:50.000000 superspreader-0.2.4/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-14 15:15:50.000000 superspreader-0.2.4/tests/test_full_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-14 15:15:50.000000 superspreader-0.2.4/tests/test_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 07:01:47.000000 superspreader-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:01:59.265650 superspreader-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 07:01:47.000000 superspreader-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 07:01:47.000000 superspreader-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 07:01:59.265650 superspreader-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-15 07:01:47.000000 superspreader-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 07:01:47.000000 superspreader-0.2.5/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 07:01:47.000000 superspreader-0.2.5/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-15 07:01:47.000000 superspreader-0.2.5/tests/test_sheet.py
```

### Comparing `superspreader-0.2.4/LICENSE.txt` & `superspreader-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.4/PKG-INFO` & `superspreader-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.4
+Version: 0.2.5
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
@@ -80,44 +80,48 @@
 # {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
-## Adding non-spreadsheet fields
+## Adding static & dynamic data to rows
 
-To provide additional fields, use `extra_data`. Fields from the spreadsheet take precedence over extra data.
+To provide additional data, use `extra_data`. Data from the spreadsheet take precedence over extra data.
 
 ```
 extra_data = {
     "status": "released"
 }
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
 sheet.load()
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'status': 'released'}
 ```
 
 Use a callable for dynamic extra data:
 
 ```
 extra_data = {
-    "summary": lambda row: f"{row.get('album')} by {row.get('artist')}"
+    "summary": lambda row: f"“{row.get('album')}” by {row.get('artist')}"
 }
 
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
-# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': 'Toy by David Bowie'}
+# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': '“Toy” by David Bowie'}
 ```
 
 ## Changelog
 
 ### 0.2.3
 
 - Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
 ### 0.2.2
 
-- Adds support for callables in `extra_data``
+- Adds support for callables in `extra_data`
+
+### 0.2.1
+
+- Adds support for providing field defaults by setting the `default` attribute or providing an instance-label value: `fields.CharField(source="Album", default="not specified")`
 
 ---
 
 The API is inspired by [Django’s model API](https://docs.djangoproject.com/en/dev/ref/models/) and [ElasticSearch DSL](https://elasticsearch-dsl.readthedocs.io/en/latest/persistence.html#document).
```

### Comparing `superspreader-0.2.4/README.md` & `superspreader-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -56,44 +56,48 @@
 # {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
-## Adding non-spreadsheet fields
+## Adding static & dynamic data to rows
 
-To provide additional fields, use `extra_data`. Fields from the spreadsheet take precedence over extra data.
+To provide additional data, use `extra_data`. Data from the spreadsheet take precedence over extra data.
 
 ```
 extra_data = {
     "status": "released"
 }
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
 sheet.load()
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'status': 'released'}
 ```
 
 Use a callable for dynamic extra data:
 
 ```
 extra_data = {
-    "summary": lambda row: f"{row.get('album')} by {row.get('artist')}"
+    "summary": lambda row: f"“{row.get('album')}” by {row.get('artist')}"
 }
 
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
-# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': 'Toy by David Bowie'}
+# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': '“Toy” by David Bowie'}
 ```
 
 ## Changelog
 
 ### 0.2.3
 
 - Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
 ### 0.2.2
 
-- Adds support for callables in `extra_data``
+- Adds support for callables in `extra_data`
+
+### 0.2.1
+
+- Adds support for providing field defaults by setting the `default` attribute or providing an instance-label value: `fields.CharField(source="Album", default="not specified")`
 
 ---
 
 The API is inspired by [Django’s model API](https://docs.djangoproject.com/en/dev/ref/models/) and [ElasticSearch DSL](https://elasticsearch-dsl.readthedocs.io/en/latest/persistence.html#document).
```

### Comparing `superspreader-0.2.4/setup.py` & `superspreader-0.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.2.4",
+    version="0.2.5",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
-        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="excel, spreadsheets, import, csv, tsv, openpyxl",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.6, <4",
     install_requires=["openpyxl>=3"],
```

### Comparing `superspreader-0.2.4/src/superspreader/fields.py` & `superspreader-0.2.5/src/superspreader/fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.4/src/superspreader/i18n.py` & `superspreader-0.2.5/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.4/src/superspreader/messages.py` & `superspreader-0.2.5/src/superspreader/messages.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.4/src/superspreader/sheets.py` & `superspreader-0.2.5/src/superspreader/sheets.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.4/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.5/src/superspreader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.4
+Version: 0.2.5
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
@@ -80,44 +80,48 @@
 # {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
-## Adding non-spreadsheet fields
+## Adding static & dynamic data to rows
 
-To provide additional fields, use `extra_data`. Fields from the spreadsheet take precedence over extra data.
+To provide additional data, use `extra_data`. Data from the spreadsheet take precedence over extra data.
 
 ```
 extra_data = {
     "status": "released"
 }
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
 sheet.load()
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'status': 'released'}
 ```
 
 Use a callable for dynamic extra data:
 
 ```
 extra_data = {
-    "summary": lambda row: f"{row.get('album')} by {row.get('artist')}"
+    "summary": lambda row: f"“{row.get('album')}” by {row.get('artist')}"
 }
 
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
-# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': 'Toy by David Bowie'}
+# {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': '“Toy” by David Bowie'}
 ```
 
 ## Changelog
 
 ### 0.2.3
 
 - Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
 ### 0.2.2
 
-- Adds support for callables in `extra_data``
+- Adds support for callables in `extra_data`
+
+### 0.2.1
+
+- Adds support for providing field defaults by setting the `default` attribute or providing an instance-label value: `fields.CharField(source="Album", default="not specified")`
 
 ---
 
 The API is inspired by [Django’s model API](https://docs.djangoproject.com/en/dev/ref/models/) and [ElasticSearch DSL](https://elasticsearch-dsl.readthedocs.io/en/latest/persistence.html#document).
```

### Comparing `superspreader-0.2.4/tests/test_fields.py` & `superspreader-0.2.5/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.4/tests/test_full_import.py` & `superspreader-0.2.5/tests/test_full_import.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # testing in general, but rather to support the `find_packages` example in
 # setup.py that excludes installing the "tests" package
 
 import datetime
 import os
 import unittest
 from pathlib import Path
+from unittest.mock import MagicMock
 
 from superspreader import fields
 from superspreader.sheets import BaseSheet
 
 
 class AlbumSheet(BaseSheet):
     sheet_name = "Albums"
@@ -21,20 +22,20 @@
     release_date = fields.DateField(source="Release Date")
     average_review = fields.FloatField(source="Average Review")
     chart_position = fields.IntegerField(source="Chart Position")
 
 
 class TestFullImport(unittest.TestCase):
     """
-    Test the process of importing a whole spreadsheet
+    Test the process of importing a spreadsheet
     """
 
     def _file_path(self, file_name):
-        script_dir = Path(__file__).parent.absolute()
-        path = os.path.join(script_dir, "spreadsheets", file_name)
+        tests_dir = Path(__file__).parent.absolute()
+        path = os.path.join(tests_dir, "spreadsheets", file_name)
         return path
 
     def setUp(self) -> None:
         self.sheet = AlbumSheet(self._file_path("albums.xlsx"))
 
     def test_basics(self):
         self.sheet.load()
@@ -57,24 +58,48 @@
         with self.assertRaises(KeyError):
             rows[0]["album"]
 
     def test_info(self):
         self.sheet.load()
         self.assertEqual("Sheet Albums, row 6: Skipped row", self.sheet.infos[0])
 
-    def test_extra_data(self):
-        extra = {"test": "1-2-3"}
-        sheet = AlbumSheet(self._file_path("albums.xlsx"), extra_data=extra)
-        sheet.load()
-        first_record = sheet[0]
-
-        self.assertEqual(first_record.get("test"), "1-2-3")
-
     def test_errors(self):
         path = self._file_path("albums_with_errors.xlsx")
         sheet_with_errors = AlbumSheet(path)
         sheet_with_errors.load()
 
         self.assertTrue(sheet_with_errors.has_errors)
         self.assertEqual(
             sheet_with_errors.errors[0], "Sheet Albums, row 7: Field Album is required"
         )
+
+    def test_empty_sheet_with_extra_data(self):
+        """Tests whether empty rows are skipped, even when extra data is provided"""
+        path = self._file_path("albums_empty.xlsx")
+        sheet = AlbumSheet(path, extra_data={"status": "released"})
+        self.assertFalse(sheet.has_errors)
+        self.assertEqual(len(sheet), 0)
+
+    def test_extra_data_static(self):
+        """Tests whether extra data is returned in the resulting row"""
+        fp = self._file_path("albums.xlsx")
+        sheet = AlbumSheet(path=fp, extra_data={"status": "released"})
+        sheet.load()
+        self.assertEqual(sheet.rows()[0].get("status"), "released")
+
+    def test_extra_data_dynamic(self):
+        """Tests whether callables in extra data are called"""
+        fp = self._file_path("albums.xlsx")
+        test_fn = MagicMock()
+        sheet = AlbumSheet(path=fp, extra_data={"test_fn": test_fn})
+        sheet.load()
+        test_fn.assert_called()
+
+    def test_extra_data_dynamic_args(self):
+        """Tests whether callables in extra data are called with the row"""
+        fp = self._file_path("albums.xlsx")
+
+        def test_fn(row):
+            self.assertIsInstance(row, dict)
+
+        sheet = AlbumSheet(path=fp, extra_data={"test_fn": test_fn})
+        sheet.load()
```

### Comparing `superspreader-0.2.4/tests/test_sheet.py` & `superspreader-0.2.5/tests/test_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # the inclusion of the tests module is not meant to offer best practices for
 # testing in general, but rather to support the `find_packages` example in
 # setup.py that excludes installing the "tests" package
 
 import unittest
 
+from superspreader import fields
 from superspreader.exceptions import ImproperlyConfigured
 from superspreader.sheets import BaseSheet
-from superspreader import fields
 
 
 class TestSheet(unittest.TestCase):
     def test_sheet_name(self):
         class AlbumSheet(BaseSheet):
             pass
 
@@ -38,8 +38,8 @@
 
         class BSheet(ASheet):
             pass
 
         sheet = BSheet(path="test")
         sheet_fields = sheet._build_fields()
 
-        self.assertTrue('a_field' in sheet_fields)
+        self.assertTrue("a_field" in sheet_fields)
```

