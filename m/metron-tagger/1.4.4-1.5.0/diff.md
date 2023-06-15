# Comparing `tmp/metron_tagger-1.4.4.tar.gz` & `tmp/metron_tagger-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metron_tagger-1.4.4.tar", max compression
+gzip compressed data, was "metron_tagger-1.5.0.tar", max compression
```

## Comparing `metron_tagger-1.4.4.tar` & `metron_tagger-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/LICENSE
--rw-r--r--   0        0        0     2814 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/README.rst
--rw-r--r--   0        0        0       74 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/__init__.py
--rw-r--r--   0        0        0     1328 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/cli.py
--rw-r--r--   0        0        0     7090 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/filerenamer.py
--rw-r--r--   0        0        0     3270 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/filesorter.py
--rw-r--r--   0        0        0     2574 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/options.py
--rwxr-xr-x   0        0        0     8599 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/run.py
--rw-r--r--   0        0        0     4753 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/settings.py
--rw-r--r--   0        0        0      129 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/styles.py
--rw-r--r--   0        0        0     9460 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/talker.py
--rw-r--r--   0        0        0     1492 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/metrontagger/utils.py
--rw-r--r--   0        0        0     2039 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/__init__.py
--rw-r--r--   0        0        0     2029 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/conftest.py
--rw-r--r--   0        0        0     1212 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_filerenamer.py
--rw-r--r--   0        0        0     2600 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_filesorter.py
--rw-r--r--   0        0        0     6621 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_metron_tagger.py
--rw-r--r--   0        0        0     1158 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_options.py
--rw-r--r--   0        0        0     1279 2023-05-21 13:46:38.407701 metron_tagger-1.4.4/tests/test_settings.py
--rw-r--r--   0        0        0     9347 2023-05-21 13:46:38.411701 metron_tagger-1.4.4/tests/test_talker.py
--rw-r--r--   0        0        0     2094 2023-05-21 13:46:38.411701 metron_tagger-1.4.4/tests/test_utils.py
--rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 metron_tagger-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2734 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/README.rst
+-rw-r--r--   0        0        0       74 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/__init__.py
+-rw-r--r--   0        0        0     1391 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/cli.py
+-rw-r--r--   0        0        0     7090 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/filerenamer.py
+-rw-r--r--   0        0        0     3270 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/filesorter.py
+-rw-r--r--   0        0        0     2748 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/options.py
+-rwxr-xr-x   0        0        0     9809 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/run.py
+-rw-r--r--   0        0        0     5013 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/schema/v1/ComicInfo.xsd
+-rw-r--r--   0        0        0     7556 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/schema/v2/ComicInfo.xsd
+-rw-r--r--   0        0        0     4789 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/settings.py
+-rw-r--r--   0        0        0      129 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/styles.py
+-rw-r--r--   0        0        0     9460 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/talker.py
+-rw-r--r--   0        0        0     1492 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/utils.py
+-rw-r--r--   0        0        0     1637 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/metrontagger/validate_ci.py
+-rw-r--r--   0        0        0     2111 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     2029 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1212 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/test_filerenamer.py
+-rw-r--r--   0        0        0     2600 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/test_filesorter.py
+-rw-r--r--   0        0        0     6621 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/test_metron_tagger.py
+-rw-r--r--   0        0        0     1158 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/test_options.py
+-rw-r--r--   0        0        0     1279 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/test_settings.py
+-rw-r--r--   0        0        0     9347 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/test_talker.py
+-rw-r--r--   0        0        0     2094 2023-06-15 17:59:47.423135 metron_tagger-1.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 metron_tagger-1.5.0/PKG-INFO
```

### Comparing `metron_tagger-1.4.4/LICENSE` & `metron_tagger-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/README.rst` & `metron_tagger-1.5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/metron-tagger.svg
     :target: https://pypi.org/project/metron-tagger/
 
 .. image:: https://img.shields.io/github/license/bpepple/metron-tagger
     :target: https://opensource.org/licenses/GPL-3.0
 
-.. image:: https://codecov.io/gh/Metron-Project/metron-tagger/branch/master/graph/badge.svg?token=d8TyzWM2Uz 
-    :target: https://codecov.io/gh/Metron-Project/metron-tagger
-
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 Quick Description
 -----------------
 
 A command-line tool to tag comic archives with metadata from metron.cloud_.
@@ -63,14 +60,15 @@
     -d, --delete         Delete the metadata tags from the file. (default: False)
     --ignore-existing    Ignore files that have existing metadata tag. (default: False)
     -i, --interactive    Interactively query the user when there are matches for an online search. (default: False)
     --missing            List files without metadata. (default: False)
     -s, --sort           Sort files that contain metadata tags. (default: False)
     -e, --export-to-cb7  Export a CBZ (zip) or CBR (rar) archive to a CB7 (7zip) archive. (default: False)
     -z, --export-to-cbz  Export a CB7 (7zip) or CBR (rar) archive to a CBZ (zip) archive. (default: False)
+    --validate           Verify that comic archive has a valid ComicInfo.xml. (default: False)
     --delete-original    Delete the original archive after successful export to another format. (default: False)
     --version            Show the version number and exit
 
 
 Bugs/Requests
 -------------
```

### Comparing `metron_tagger-1.4.4/metrontagger/cli.py` & `metron_tagger-1.5.0/metrontagger/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 
     if opts.export_to_cbz:
         config.export_to_cbz = opts.export_to_cbz
 
     if opts.delete_original:
         config.delete_original = opts.delete_original
 
+    if opts.validate:
+        config.validate = opts.validate
+
     return config
 
 
 def main():
     args = get_args()
     config = get_configs(args)
```

### Comparing `metron_tagger-1.4.4/metrontagger/filerenamer.py` & `metron_tagger-1.5.0/metrontagger/filerenamer.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/metrontagger/filesorter.py` & `metron_tagger-1.5.0/metrontagger/filesorter.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/metrontagger/options.py` & `metron_tagger-1.5.0/metrontagger/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,20 @@
         "-z",
         "--export-to-cbz",
         help="Export a CB7 (7zip) or CBR (rar) archive to a CBZ (zip) archive.",
         action="store_true",
         default=False,
     )
     parser.add_argument(
+        "--validate",
+        help="Verify that comic archive has a valid ComicInfo.xml.",
+        action="store_true",
+        default=False,
+    )
+    parser.add_argument(
         "--delete-original",
         help="Delete the original archive after successful export to another format.",
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "--version",
```

### Comparing `metron_tagger-1.4.4/metrontagger/run.py` & `metron_tagger-1.5.0/metrontagger/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from darkseid.utils import get_recursive_filelist
 
 from metrontagger.filerenamer import FileRenamer
 from metrontagger.filesorter import FileSorter
 from metrontagger.settings import MetronTaggerSettings
 from metrontagger.styles import Styles
 from metrontagger.talker import Talker
+from metrontagger.validate_ci import SchemaVersion, ValidateComicInfo
 
 
 class Runner:
     """Main runner"""
 
     def __init__(self, config: MetronTaggerSettings) -> None:
         self.config = config
@@ -99,14 +100,37 @@
                     questionary.print(f"Failed to export '{comic.name}'", style=Styles.ERROR)
             else:
                 questionary.print(
                     f"'{comic.name}' is not a cbr or cb7 archive. skipping...",
                     style=Styles.WARNING,
                 )
 
+    def _validate_comic_info(self, file_list: List[Path]) -> None:
+        questionary.print("\nValidating ComicInfo:\n---------------------", style=Styles.TITLE)
+        for comic in file_list:
+            ca = Comic(comic)
+            if not ca.has_metadata():
+                questionary.print(
+                    f"'{ca.path.name}' doesn't have a ComicInfo.xml file.",
+                    style=Styles.WARNING,
+                )
+                continue
+            xml = ca.archiver.read_file("ComicInfo.xml")
+            result = ValidateComicInfo(xml).validate()
+            if result == SchemaVersion.v2:
+                questionary.print(
+                    f"'{ca.path.name}' is a valid ComicInfo Version 2", style=Styles.SUCCESS
+                )
+            elif result == SchemaVersion.v1:
+                questionary.print(
+                    f"'{ca.path.name}' is a valid ComicInfo Version 1", style=Styles.SUCCESS
+                )
+            else:
+                questionary.print(f"'{ca.path.name}' is not valid", style=Styles.ERROR)
+
     def _sort_comic_list(self, file_list: List[Path]) -> None:
         if not self.config.sort_dir:
             questionary.print(
                 "\nUnable to sort files. No destination directory was provided.",
                 style=Styles.ERROR,
             )
             return
@@ -172,15 +196,14 @@
             self.config.sort_dir = answers["dir"]
             if answers["save"]:
                 self.config.save()
             return True
         return False
 
     def run(self) -> None:
-
         if not (file_list := get_recursive_filelist(self.config.path)):
             print("No files to process. Exiting.")
             exit(0)
 
         if self.config.missing:
             self._comics_with_no_metadata(file_list)
 
@@ -215,7 +238,10 @@
             self._sort_comic_list(file_list)
 
         if self.config.export_to_cb7:
             self._export_to_cb7(file_list)
 
         if self.config.export_to_cbz:
             self._export_to_zip(file_list)
+
+        if self.config.validate:
+            self._validate_comic_info(file_list)
```

### Comparing `metron_tagger-1.4.4/metrontagger/settings.py` & `metron_tagger-1.5.0/metrontagger/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self.rename: bool = False
         self.sort: bool = False
         self.interactive: bool = False
         self.ignore_existing: bool = False
         self.export_to_cb7: bool = False
         self.export_to_cbz: bool = False
         self.delete_original: bool = False
+        self.validate: bool = False
 
         # Rename settings
         self.rename_template = "%series% v%volume% #%issue% (%year%)"
         self.rename_issue_number_padding = 3
         self.rename_use_smart_string_cleanup = True
 
         self.config = configparser.RawConfigParser()
```

### Comparing `metron_tagger-1.4.4/metrontagger/talker.py` & `metron_tagger-1.5.0/metrontagger/talker.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/metrontagger/utils.py` & `metron_tagger-1.5.0/metrontagger/utils.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/pyproject.toml` & `metron_tagger-1.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "metron-tagger"
-version = "1.4.4"
+version = "1.5.0"
 description = "A program to write metadata from metron.cloud to a comic archive"
-authors = ["Brian Pepple <bdpepple@gmail.com>"]
+authors = ["Brian Pepple <bpepple@metron.cloud>"]
 license = "GPL-3.0-or-later"
-maintainers = ["Brian Pepple <bdpepple@gmail.com>"]
+maintainers = ["Brian Pepple <bpepple@metron.cloud>"]
 readme = "README.rst"
 packages = [
 	{ include = "metrontagger" },
 ]
 include = [
     { path = "tests", format = "sdist" }
 ]
@@ -16,14 +16,15 @@
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: End Users/Desktop",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Utilities",
   "Topic :: Other/Nonlisted Topic",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: POSIX",
   "Operating System :: POSIX :: BSD",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows",
@@ -32,21 +33,22 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 mokkari = "^2.5.0"
 questionary = "^1.10.0"
 pyxdg = "^0.28"
 darkseid = "^2.0.1"
+lxml = "^4.9.2"
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^2.12.1"
 flake8 = "^3.9.2"
 pytest-mock = "^3.6.1"
 pre-commit = "^2.14.1"
-black = "^21.8b0"
+black = "^22.3.0"
 tox = "^3.24.3"
 flake8-builtins = "^1.5.3"
 flake8-blind-except = "^0.2.0"
 
 [tool.poetry.scripts]
 metron-tagger = "metrontagger.cli:main"
 
@@ -60,15 +62,15 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 line_length = 95
 default_section = "THIRDPARTY"
 known_first_party = []
-known_third_party = ["darkseid", "mokkari", "pytest", "questionary", "xdg"]
+known_third_party = ["darkseid", "lxml", "mokkari", "pytest", "questionary", "xdg"]
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/Metron-Project/metron-tagger"
 "Bug Tracker" = "https://github.com/Metron-Project/metron-tagger/issues"
 
 [tool.coverage.run]
 source = ["metrontagger"]
```

### Comparing `metron_tagger-1.4.4/tests/conftest.py` & `metron_tagger-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/tests/test_filerenamer.py` & `metron_tagger-1.5.0/tests/test_filerenamer.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/tests/test_filesorter.py` & `metron_tagger-1.5.0/tests/test_filesorter.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/tests/test_metron_tagger.py` & `metron_tagger-1.5.0/tests/test_metron_tagger.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/tests/test_options.py` & `metron_tagger-1.5.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/tests/test_settings.py` & `metron_tagger-1.5.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/tests/test_talker.py` & `metron_tagger-1.5.0/tests/test_talker.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/tests/test_utils.py` & `metron_tagger-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-1.4.4/PKG-INFO` & `metron_tagger-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: metron-tagger
-Version: 1.4.4
+Version: 1.5.0
 Summary: A program to write metadata from metron.cloud to a comic archive
 License: GPL-3.0-or-later
 Keywords: comics,comic,metadata,tagging,tagger
 Author: Brian Pepple
-Author-email: bdpepple@gmail.com
+Author-email: bpepple@metron.cloud
 Maintainer: Brian Pepple
-Maintainer-email: bdpepple@gmail.com
+Maintainer-email: bpepple@metron.cloud
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Topic :: Utilities
 Requires-Dist: darkseid (>=2.0.1,<3.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: mokkari (>=2.5.0,<3.0.0)
 Requires-Dist: pyxdg (>=0.28,<0.29)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/Metron-Project/metron-tagger/issues
 Project-URL: Homepage, https://github.com/Metron-Project/metron-tagger
 Description-Content-Type: text/x-rst
 
@@ -42,17 +43,14 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/metron-tagger.svg
     :target: https://pypi.org/project/metron-tagger/
 
 .. image:: https://img.shields.io/github/license/bpepple/metron-tagger
     :target: https://opensource.org/licenses/GPL-3.0
 
-.. image:: https://codecov.io/gh/Metron-Project/metron-tagger/branch/master/graph/badge.svg?token=d8TyzWM2Uz 
-    :target: https://codecov.io/gh/Metron-Project/metron-tagger
-
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 Quick Description
 -----------------
 
 A command-line tool to tag comic archives with metadata from metron.cloud_.
@@ -98,14 +96,15 @@
     -d, --delete         Delete the metadata tags from the file. (default: False)
     --ignore-existing    Ignore files that have existing metadata tag. (default: False)
     -i, --interactive    Interactively query the user when there are matches for an online search. (default: False)
     --missing            List files without metadata. (default: False)
     -s, --sort           Sort files that contain metadata tags. (default: False)
     -e, --export-to-cb7  Export a CBZ (zip) or CBR (rar) archive to a CB7 (7zip) archive. (default: False)
     -z, --export-to-cbz  Export a CB7 (7zip) or CBR (rar) archive to a CBZ (zip) archive. (default: False)
+    --validate           Verify that comic archive has a valid ComicInfo.xml. (default: False)
     --delete-original    Delete the original archive after successful export to another format. (default: False)
     --version            Show the version number and exit
 
 
 Bugs/Requests
 -------------
```

