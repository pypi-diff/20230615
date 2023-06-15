# Comparing `tmp/python-iso639-2023.4.13.tar.gz` & `tmp/python-iso639-2023.6.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iso639-2023.4.13.tar", last modified: Thu Apr 13 23:11:57 2023, max compression
+gzip compressed data, was "python-iso639-2023.6.15.tar", last modified: Thu Jun 15 12:50:34 2023, max compression
```

## Comparing `python-iso639-2023.4.13.tar` & `python-iso639-2023.6.15.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.942475 python-iso639-2023.4.13/
--rw-r--r--   0 jacksonlee   (501) staff       (20)    10759 2022-08-28 17:23:57.000000 python-iso639-2023.4.13/LICENSE.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)    13262 2023-04-13 23:11:57.942257 python-iso639-2023.4.13/PKG-INFO
--rw-r--r--   0 jacksonlee   (501) staff       (20)    11919 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/README.md
--rw-r--r--   0 jacksonlee   (501) staff       (20)     1778 2023-04-13 23:10:38.000000 python-iso639-2023.4.13/pyproject.toml
--rw-r--r--   0 jacksonlee   (501) staff       (20)       38 2023-04-13 23:11:57.942509 python-iso639-2023.4.13/setup.cfg
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.938351 python-iso639-2023.4.13/src/
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.939445 python-iso639-2023.4.13/src/iso639/
--rw-r--r--   0 jacksonlee   (501) staff       (20)      525 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/src/iso639/__init__.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)     7722 2023-04-13 23:04:34.000000 python-iso639-2023.4.13/src/iso639/language.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)   540672 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/src/iso639/languages.db
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.941526 python-iso639-2023.4.13/src/python_iso639.egg-info/
--rw-r--r--   0 jacksonlee   (501) staff       (20)    13262 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/PKG-INFO
--rw-r--r--   0 jacksonlee   (501) staff       (20)      402 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/SOURCES.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/dependency_links.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2022-08-28 17:28:05.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/not-zip-safe
--rw-r--r--   0 jacksonlee   (501) staff       (20)       76 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/requires.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        7 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/top_level.txt
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.941910 python-iso639-2023.4.13/tests/
--rw-r--r--   0 jacksonlee   (501) staff       (20)     2435 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/tests/test_language.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)     1295 2022-08-28 17:23:57.000000 python-iso639-2023.4.13/tests/test_version_number.py
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-06-15 12:50:34.755966 python-iso639-2023.6.15/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    10759 2022-08-28 17:23:57.000000 python-iso639-2023.6.15/LICENSE.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    13401 2023-06-15 12:50:34.755773 python-iso639-2023.6.15/PKG-INFO
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    12058 2023-06-15 12:49:43.000000 python-iso639-2023.6.15/README.md
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     1778 2023-06-15 12:49:43.000000 python-iso639-2023.6.15/pyproject.toml
+-rw-r--r--   0 jacksonlee   (501) staff       (20)       38 2023-06-15 12:50:34.756013 python-iso639-2023.6.15/setup.cfg
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-06-15 12:50:34.751675 python-iso639-2023.6.15/src/
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-06-15 12:50:34.753076 python-iso639-2023.6.15/src/iso639/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)      525 2023-02-04 19:16:58.000000 python-iso639-2023.6.15/src/iso639/__init__.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     7897 2023-06-15 12:49:43.000000 python-iso639-2023.6.15/src/iso639/language.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)   540672 2023-02-04 19:16:58.000000 python-iso639-2023.6.15/src/iso639/languages.db
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-06-15 12:50:34.754874 python-iso639-2023.6.15/src/python_iso639.egg-info/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    13401 2023-06-15 12:50:34.000000 python-iso639-2023.6.15/src/python_iso639.egg-info/PKG-INFO
+-rw-r--r--   0 jacksonlee   (501) staff       (20)      402 2023-06-15 12:50:34.000000 python-iso639-2023.6.15/src/python_iso639.egg-info/SOURCES.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2023-06-15 12:50:34.000000 python-iso639-2023.6.15/src/python_iso639.egg-info/dependency_links.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2022-08-28 17:28:05.000000 python-iso639-2023.6.15/src/python_iso639.egg-info/not-zip-safe
+-rw-r--r--   0 jacksonlee   (501) staff       (20)       76 2023-06-15 12:50:34.000000 python-iso639-2023.6.15/src/python_iso639.egg-info/requires.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        7 2023-06-15 12:50:34.000000 python-iso639-2023.6.15/src/python_iso639.egg-info/top_level.txt
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-06-15 12:50:34.755381 python-iso639-2023.6.15/tests/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     3046 2023-06-15 12:49:43.000000 python-iso639-2023.6.15/tests/test_language.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     1295 2022-08-28 17:23:57.000000 python-iso639-2023.6.15/tests/test_version_number.py
```

### Comparing `python-iso639-2023.4.13/LICENSE.txt` & `python-iso639-2023.6.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-iso639-2023.4.13/PKG-INFO` & `python-iso639-2023.6.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iso639
-Version: 2023.4.13
+Version: 2023.6.15
 Summary: Look-up utilities for ISO 639 language codes and names
 Author-email: "Jackson L. Lee" <jacksonlunlee@gmail.com>
 License: Apache 2.0
 Project-URL: source, https://github.com/jacksonllee/iso639
 Project-URL: tracker, https://github.com/jacksonllee/iso639/issues
 Keywords: ISO 639,language codes,languages,linguistics
 Classifier: Development Status :: 5 - Production/Stable
@@ -294,14 +294,16 @@
 The `python-iso639` code is released under an Apache 2.0 license.
 Please see [LICENSE.txt](https://github.com/jacksonllee/iso639/blob/main/LICENSE.txt)
 for details.
 
 The data source that backs this package is the
 [language code tables published by SIL](https://iso639-3.sil.org/code_tables/download_tables).
 Note that SIL resources have their [terms of use](https://www.sil.org/terms-use).
+For exactly how the data is included in the package,
+see the script at [`scripts/create_languages_db.py`](scripts/create_languages_db.py).
 
 ## Why Another ISO 639 Package?
 
 Both packages [iso639](https://pypi.org/project/iso639/)
 and [iso-639](https://pypi.org/project/iso-639/) exist on PyPI.
 However, as of this writing (May 2022), they were last updated in 2016 and don't seem to be maintained anymore
 for updating the language codes.
```

### Comparing `python-iso639-2023.4.13/README.md` & `python-iso639-2023.6.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,16 @@
 The `python-iso639` code is released under an Apache 2.0 license.
 Please see [LICENSE.txt](https://github.com/jacksonllee/iso639/blob/main/LICENSE.txt)
 for details.
 
 The data source that backs this package is the
 [language code tables published by SIL](https://iso639-3.sil.org/code_tables/download_tables).
 Note that SIL resources have their [terms of use](https://www.sil.org/terms-use).
+For exactly how the data is included in the package,
+see the script at [`scripts/create_languages_db.py`](scripts/create_languages_db.py).
 
 ## Why Another ISO 639 Package?
 
 Both packages [iso639](https://pypi.org/project/iso639/)
 and [iso-639](https://pypi.org/project/iso-639/) exist on PyPI.
 However, as of this writing (May 2022), they were last updated in 2016 and don't seem to be maintained anymore
 for updating the language codes.
```

### Comparing `python-iso639-2023.4.13/pyproject.toml` & `python-iso639-2023.6.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.3.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-iso639"
-version = "2023.4.13"
+version = "2023.6.15"
 description = "Look-up utilities for ISO 639 language codes and names"
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { text = "Apache 2.0" }
 authors = [ { name = "Jackson L. Lee", email = "jacksonlunlee@gmail.com" } ]
 keywords = ["ISO 639", "language codes", "languages", "linguistics"]
 classifiers = [
```

### Comparing `python-iso639-2023.4.13/src/iso639/__init__.py` & `python-iso639-2023.6.15/src/iso639/__init__.py`

 * *Files identical despite different names*

### Comparing `python-iso639-2023.4.13/src/iso639/language.py` & `python-iso639-2023.6.15/src/iso639/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,20 @@
 
     # From the "retirements" table
     retire_reason: str
     retire_change_to: str
     retire_remedy: str
     retire_date: datetime.date
 
+    def __hash__(self) -> int:
+        return hash(self.part3)
+
+    def __eq__(self, other) -> bool:
+        return isinstance(other, Language) and self.part3 == other.part3
+
     @classmethod
     def match(cls, user_input) -> "Language":
         """Return a ``Language`` instance by matching on the user input.
 
         Parameters
         ----------
         user_input : str
```

### Comparing `python-iso639-2023.4.13/src/iso639/languages.db` & `python-iso639-2023.6.15/src/iso639/languages.db`

 * *Files identical despite different names*

### Comparing `python-iso639-2023.4.13/src/python_iso639.egg-info/PKG-INFO` & `python-iso639-2023.6.15/src/python_iso639.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iso639
-Version: 2023.4.13
+Version: 2023.6.15
 Summary: Look-up utilities for ISO 639 language codes and names
 Author-email: "Jackson L. Lee" <jacksonlunlee@gmail.com>
 License: Apache 2.0
 Project-URL: source, https://github.com/jacksonllee/iso639
 Project-URL: tracker, https://github.com/jacksonllee/iso639/issues
 Keywords: ISO 639,language codes,languages,linguistics
 Classifier: Development Status :: 5 - Production/Stable
@@ -294,14 +294,16 @@
 The `python-iso639` code is released under an Apache 2.0 license.
 Please see [LICENSE.txt](https://github.com/jacksonllee/iso639/blob/main/LICENSE.txt)
 for details.
 
 The data source that backs this package is the
 [language code tables published by SIL](https://iso639-3.sil.org/code_tables/download_tables).
 Note that SIL resources have their [terms of use](https://www.sil.org/terms-use).
+For exactly how the data is included in the package,
+see the script at [`scripts/create_languages_db.py`](scripts/create_languages_db.py).
 
 ## Why Another ISO 639 Package?
 
 Both packages [iso639](https://pypi.org/project/iso639/)
 and [iso-639](https://pypi.org/project/iso-639/) exist on PyPI.
 However, as of this writing (May 2022), they were last updated in 2016 and don't seem to be maintained anymore
 for updating the language codes.
```

### Comparing `python-iso639-2023.4.13/tests/test_language.py` & `python-iso639-2023.6.15/tests/test_language.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,7 +75,29 @@
     assert type(ALL_LANGUAGES) == list
     assert type(ALL_LANGUAGES[0]) == Language
     assert len(ALL_LANGUAGES) == 7916, "Need to update README.md"
 
     lang = ALL_LANGUAGES[0]
     assert lang.part3 == "aaa", "Need to update README.md"
     assert lang.name == "Ghotuo", "Need to update README.md"
+
+
+def test_eq():
+    yue1 = Language.match("yue")
+    yue2 = Language.match("yue")
+    fra = Language.match("fra")
+
+    assert yue1.part3 == yue2.part3 == "yue"
+    assert fra.part3 == "fra"
+    assert yue1 == yue2
+    assert yue1 != fra
+
+
+def test_hashable():
+    """Language class instances are hashable, e.g., can be in a set.
+    See https://github.com/jacksonllee/iso639/issues/3
+    """
+    cat = Language.match("cat")
+    assert cat.part3 == "cat"
+    assert type(cat.other_names) == list  # Need a list attr for the hashing test...
+    hash(cat)  # Shouldn't error!
+    assert len({cat, cat, cat}) == 1
```

### Comparing `python-iso639-2023.4.13/tests/test_version_number.py` & `python-iso639-2023.6.15/tests/test_version_number.py`

 * *Files identical despite different names*

