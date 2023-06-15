# Comparing `tmp/superspreader-0.2.5.tar.gz` & `tmp/superspreader-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.2.5.tar", last modified: Thu Jun 15 07:01:59 2023, max compression
+gzip compressed data, was "superspreader-0.2.6.tar", last modified: Thu Jun 15 07:34:20 2023, max compression
```

## Comparing `superspreader-0.2.5.tar` & `superspreader-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 07:01:47.000000 superspreader-0.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:01:59.265650 superspreader-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 07:01:47.000000 superspreader-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 07:01:47.000000 superspreader-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 07:01:59.265650 superspreader-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-15 07:01:47.000000 superspreader-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-15 07:01:47.000000 superspreader-0.2.5/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 07:01:59.000000 superspreader-0.2.5/src/superspreader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:01:59.265650 superspreader-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 07:01:47.000000 superspreader-0.2.5/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 07:01:47.000000 superspreader-0.2.5/tests/test_full_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-15 07:01:47.000000 superspreader-0.2.5/tests/test_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 07:34:11.000000 superspreader-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:34:20.975258 superspreader-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 07:34:11.000000 superspreader-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 07:34:11.000000 superspreader-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 07:34:20.975258 superspreader-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-15 07:34:11.000000 superspreader-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.971258 superspreader-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 07:34:11.000000 superspreader-0.2.6/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-15 07:34:11.000000 superspreader-0.2.6/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-15 07:34:11.000000 superspreader-0.2.6/tests/test_sheet.py
```

### Comparing `superspreader-0.2.5/LICENSE.txt` & `superspreader-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.5/PKG-INFO` & `superspreader-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.5
+Version: 0.2.6
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Intended Audience :: Developers
```

### Comparing `superspreader-0.2.5/README.md` & `superspreader-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.5/setup.py` & `superspreader-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.2.5",
+    version="0.2.6",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
```

### Comparing `superspreader-0.2.5/src/superspreader/fields.py` & `superspreader-0.2.6/src/superspreader/fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.5/src/superspreader/i18n.py` & `superspreader-0.2.6/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.5/src/superspreader/messages.py` & `superspreader-0.2.6/src/superspreader/messages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from .i18n import DE, EN
 
 messages = {
     EN: {
         "field.wrong_type": (
-            "Field %(field)s should be of type %(target_type)s, but it’s of type %(actual_type)s",
+            "“%(field)s” should be of type %(target_type)s, but it’s of type %(actual_type)s",
             None,
         ),
-        "field.is_required": ("Field %(field)s is required", None),
+        "field.is_required": ("“%(field)s” is required", None),
         "field.timecode_parse_error": (
-            "Field %(field)s has an invalid format: %(_timecode)s",
+            "“%(field)s” has an invalid format: %(_timecode)s",
             None,
         ),
         "field.related_does_not_exist": (
-            "Related object identified by %(value)s on field %(field)s does not exist",
+            "Related object identified by %(value)s on “%(field)s” does not exist",
             None,
         ),
         "field.related_multiple_objects_returned": (
-            "More than one related object identified by %(value)s on field %(field)s",
+            "More than one related object identified by %(value)s on “%(field)s”",
             None,
         ),
-        "sheet.row_info": ("Sheet %(sheet)s, row %(row)s: %(message)s", None),
-        "sheet.column_missing": ("Column %(column)s not present in sheet", None),
-        "sheet.sheet_missing": ("Sheet %(sheet)s not present in document", None),
+        "sheet.row_info": ("Row %(row)s: %(message)s", None),
+        "sheet.column_missing": ("Column “%(column)s” not present in sheet", None),
+        "sheet.sheet_missing": ("Sheet “%(sheet)s” not present in document", None),
     },
     DE: {
         "field.wrong_type": (
-            "Das Feld %(field)s sollte den Typ %(target_type)s haben, aber der"
+            "„%(field)s“ sollte den Typ %(target_type)s haben, aber der"
             "Typ ist %(actual_type)s",
             None,
         ),
-        "field.is_required": ("Das Feld %(field)s muss ausgefüllt sein", None),
+        "field.is_required": ("„%(field)s“ muss ausgefüllt sein", None),
         "field.timecode_parse_error": (
-            "Das Feld %(field)s hat ein ungültiges Format: %(_timecode)s",
+            "„%(field)s“ hat ein ungültiges Format: %(_timecode)s",
             None,
         ),
         "field.related_does_not_exist": (
-            "Ein Objekt mit %(value)s beim Feld %(field)s existiert nicht",
+            "Ein Objekt mit %(value)s bei „%(field)s“ existiert nicht",
             None,
         ),
         "field.related_multiple_objects_returned": (
-            "Mehr als ein Objekt mit %(value)s beim Feld %(field)s gefunden",
+            "Mehr als ein Objekt mit %(value)s beim „%(field)s“ gefunden",
             None,
         ),
-        "sheet.row_info": ("Blatt %(sheet)s, Zeile %(row)s: %(message)s", None),
-        "sheet.column_missing": ("Die Spalte %(column)s fehlt im Blatt", None),
-        "sheet.sheet_missing": ("Das Blatt %(sheet)s ist nicht vorhanden", None),
+        "sheet.row_info": ("Zeile %(row)s: %(message)s", None),
+        "sheet.column_missing": ("Die Spalte „%(column)s“ fehlt im Blatt", None),
+        "sheet.sheet_missing": ("Das Blatt „%(sheet)s“ ist nicht vorhanden", None),
     },
 }
```

### Comparing `superspreader-0.2.5/src/superspreader/sheets.py` & `superspreader-0.2.6/src/superspreader/sheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,14 @@
     def _add_error(self, message, index=None) -> None:
         # Add to row index, if it’s related to a row.
         if isinstance(index, int):
             message = _(
                 "sheet.row_info",
                 self.language,
                 params={
-                    "sheet": self.get_sheet_name(),
                     "row": index + 1 + self.get_header_rows(),
                     "message": message,
                 },
             )
         self._errors.append(message)
 
     def _add_errors(self, errors) -> None:
@@ -221,15 +220,14 @@
     def _add_info(self, message, index=None) -> None:
         # Add to row index, if it’s related to a row.
         if isinstance(index, int):
             message = _(
                 "sheet.row_info",
                 self.language,
                 params={
-                    "sheet": self.get_sheet_name(),
                     "row": index + 1 + self.get_header_rows(),
                     "message": message,
                 },
             )
         self._infos.append(message)
 
     def _check(self) -> None:
```

### Comparing `superspreader-0.2.5/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.6/src/superspreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.5
+Version: 0.2.6
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Intended Audience :: Developers
```

### Comparing `superspreader-0.2.5/tests/test_fields.py` & `superspreader-0.2.6/tests/test_fields.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class BaseFieldTestCase(unittest.TestCase):
     def test_required(self):
         test_field = DummyField(source="test")
 
         with self.assertRaises(ValidationException) as cm:
             test_field(None, "en")
 
-        self.assertEqual(cm.exception.msg, "Field test is required")
+        self.assertEqual(cm.exception.msg, "“test” is required")
 
         test_field = DummyField(source="test", required=False)
         self.assertEqual(test_field(None, language="en"), None)
 
         # Reverse case.
         value = test_field(666, "en")
         self.assertEqual(value, 666)
@@ -27,22 +27,22 @@
     def test_wrong_type(self):
         test_field = DummyField(source="test")
 
         with self.assertRaises(ValidationException) as cm:
             test_field("I’m a string", "en")
 
         self.assertEqual(
-            cm.exception.msg, "Field test should be of type int, but it’s of type str"
+            cm.exception.msg, "“test” should be of type int, but it’s of type str"
         )
 
     def test_timecode_field(self):
         test_field = TimecodeField(source="test")
         timecode_str = "00:13:06,9"
         invalid_timecode_str = "asdf123"
 
         value = test_field(timecode_str, language="en")
         self.assertEqual(value, 786.9)
 
         with self.assertRaises(ValidationException) as cm:
             test_field(invalid_timecode_str, language="en")
 
-        self.assertEqual(cm.exception.msg, "Field test has an invalid format: asdf123")
+        self.assertEqual(cm.exception.msg, "“test” has an invalid format: asdf123")
```

### Comparing `superspreader-0.2.5/tests/test_full_import.py` & `superspreader-0.2.6/tests/test_full_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,25 +56,23 @@
         self.sheet.load()
         rows = self.sheet.rows(exclude=["album"])
         with self.assertRaises(KeyError):
             rows[0]["album"]
 
     def test_info(self):
         self.sheet.load()
-        self.assertEqual("Sheet Albums, row 6: Skipped row", self.sheet.infos[0])
+        self.assertEqual("Row 6: Skipped row", self.sheet.infos[0])
 
     def test_errors(self):
         path = self._file_path("albums_with_errors.xlsx")
         sheet_with_errors = AlbumSheet(path)
         sheet_with_errors.load()
 
         self.assertTrue(sheet_with_errors.has_errors)
-        self.assertEqual(
-            sheet_with_errors.errors[0], "Sheet Albums, row 7: Field Album is required"
-        )
+        self.assertEqual(sheet_with_errors.errors[0], "Row 7: “Album” is required")
 
     def test_empty_sheet_with_extra_data(self):
         """Tests whether empty rows are skipped, even when extra data is provided"""
         path = self._file_path("albums_empty.xlsx")
         sheet = AlbumSheet(path, extra_data={"status": "released"})
         self.assertFalse(sheet.has_errors)
         self.assertEqual(len(sheet), 0)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `superspreader-0.2.5/tests/test_sheet.py` & `superspreader-0.2.6/tests/test_sheet.py`

 * *Files identical despite different names*

