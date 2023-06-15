# Comparing `tmp/mailbagit-0.5.0.tar.gz` & `tmp/mailbagit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailbagit-0.5.0.tar", last modified: Tue Feb 14 18:44:36 2023, max compression
+gzip compressed data, was "mailbagit-0.5.1.tar", last modified: Thu Jun 15 20:36:05 2023, max compression
```

## Comparing `mailbagit-0.5.0.tar` & `mailbagit-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 18:44:36.793672 mailbagit-0.5.0/
--rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     5923 2023-02-14 18:44:36.792672 mailbagit-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     5205 2023-02-14 18:29:58.000000 mailbagit-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-14 18:44:36.732671 mailbagit-0.5.0/mailbagit/
--rw-rw-rw-   0        0        0    12594 2023-02-14 18:30:56.000000 mailbagit-0.5.0/mailbagit/__init__.py
--rw-rw-rw-   0        0        0    13942 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/controller.py
--rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.5.0/mailbagit/derivative.py
-drwxrwxrwx   0        0        0        0 2023-02-14 18:44:36.773672 mailbagit-0.5.0/mailbagit/derivatives/
--rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/derivatives/eml.py
--rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/derivatives/example.py
--rw-rw-rw-   0        0        0     2773 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/derivatives/html.py
--rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/derivatives/mbox.py
--rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/derivatives/pdf.py
--rw-rw-rw-   0        0        0     4861 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/derivatives/pdf_chrome.py
--rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/derivatives/txt.py
--rw-rw-rw-   0        0        0    14159 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/derivatives/warc.py
--rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/email_account.py
-drwxrwxrwx   0        0        0        0 2023-02-14 18:44:36.780672 mailbagit-0.5.0/mailbagit/formats/
--rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/formats/eml.py
--rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/formats/example.py
--rw-rw-rw-   0        0        0     7245 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/formats/mbox.py
--rw-rw-rw-   0        0        0     9982 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/formats/msg.py
--rw-rw-rw-   0        0        0    19442 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/formats/pst.py
--rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/globals.py
--rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/guided.py
-drwxrwxrwx   0        0        0        0 2023-02-14 18:44:36.787672 mailbagit-0.5.0/mailbagit/helper/
--rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.5.0/mailbagit/helper/__init__.py
--rw-rw-rw-   0        0        0     3781 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/helper/common.py
--rw-rw-rw-   0        0        0     4808 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/helper/controller.py
--rw-rw-rw-   0        0        0     8257 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/helper/derivative.py
--rw-rw-rw-   0        0        0    16736 2023-02-14 18:29:58.000000 mailbagit-0.5.0/mailbagit/helper/format.py
--rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/loggerx.py
--rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.5.0/mailbagit/models.py
-drwxrwxrwx   0        0        0        0 2023-02-14 18:44:36.762678 mailbagit-0.5.0/mailbagit.egg-info/
--rw-rw-rw-   0        0        0     5923 2023-02-14 18:44:36.000000 mailbagit-0.5.0/mailbagit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2023-02-14 18:44:36.000000 mailbagit-0.5.0/mailbagit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 18:44:36.000000 mailbagit-0.5.0/mailbagit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-02-14 18:44:36.000000 mailbagit-0.5.0/mailbagit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      455 2023-02-14 18:44:36.000000 mailbagit-0.5.0/mailbagit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-02-14 18:44:36.000000 mailbagit-0.5.0/mailbagit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-14 18:44:36.793672 mailbagit-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1640 2023-02-14 18:30:56.000000 mailbagit-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-14 18:44:36.790672 mailbagit-0.5.0/tests/
--rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.5.0/tests/test_controller.py
--rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.5.0/tests/test_formats.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.537549 mailbagit-0.5.1/
+-rw-rw-rw-   0        0        0     1145 2022-03-31 19:54:35.000000 mailbagit-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     5882 2023-06-15 20:36:05.536548 mailbagit-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5205 2023-02-14 18:29:58.000000 mailbagit-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.463545 mailbagit-0.5.1/mailbagit/
+-rw-rw-rw-   0        0        0    12594 2023-06-15 20:22:51.000000 mailbagit-0.5.1/mailbagit/__init__.py
+-rw-rw-rw-   0        0        0    13942 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/controller.py
+-rw-rw-rw-   0        0        0     3205 2023-01-27 22:21:41.000000 mailbagit-0.5.1/mailbagit/derivative.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.500548 mailbagit-0.5.1/mailbagit/derivatives/
+-rw-rw-rw-   0        0        0     8658 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/eml.py
+-rw-rw-rw-   0        0        0      914 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/example.py
+-rw-rw-rw-   0        0        0     2773 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/html.py
+-rw-rw-rw-   0        0        0     7945 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/derivatives/mbox.py
+-rw-rw-rw-   0        0        0     5297 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/pdf.py
+-rw-rw-rw-   0        0        0     4861 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/pdf_chrome.py
+-rw-rw-rw-   0        0        0     2150 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/txt.py
+-rw-rw-rw-   0        0        0    14159 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/derivatives/warc.py
+-rw-rw-rw-   0        0        0     3136 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/email_account.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.517547 mailbagit-0.5.1/mailbagit/formats/
+-rw-rw-rw-   0        0        0     6989 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/eml.py
+-rw-rw-rw-   0        0        0      744 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/example.py
+-rw-rw-rw-   0        0        0     7378 2023-06-15 20:22:51.000000 mailbagit-0.5.1/mailbagit/formats/mbox.py
+-rw-rw-rw-   0        0        0     9982 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/msg.py
+-rw-rw-rw-   0        0        0    19442 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/formats/pst.py
+-rw-rw-rw-   0        0        0      245 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/globals.py
+-rw-rw-rw-   0        0        0     9765 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/guided.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.524546 mailbagit-0.5.1/mailbagit/helper/
+-rw-rw-rw-   0        0        0        0 2022-05-25 17:40:41.000000 mailbagit-0.5.1/mailbagit/helper/__init__.py
+-rw-rw-rw-   0        0        0     3781 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/helper/common.py
+-rw-rw-rw-   0        0        0     4808 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/helper/controller.py
+-rw-rw-rw-   0        0        0     8257 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/helper/derivative.py
+-rw-rw-rw-   0        0        0    16736 2023-02-14 18:29:58.000000 mailbagit-0.5.1/mailbagit/helper/format.py
+-rw-rw-rw-   0        0        0     3888 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/loggerx.py
+-rw-rw-rw-   0        0        0     6320 2023-02-14 18:20:25.000000 mailbagit-0.5.1/mailbagit/models.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.482553 mailbagit-0.5.1/mailbagit.egg-info/
+-rw-rw-rw-   0        0        0     5882 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      455 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-06-15 20:36:05.000000 mailbagit-0.5.1/mailbagit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2022-05-12 18:35:05.000000 mailbagit-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 20:36:05.537549 mailbagit-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2023-06-15 20:22:51.000000 mailbagit-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:36:05.535546 mailbagit-0.5.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-12 18:35:05.000000 mailbagit-0.5.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     3443 2022-05-16 18:54:07.000000 mailbagit-0.5.1/tests/test_controller.py
+-rw-rw-rw-   0        0        0     8452 2023-02-14 18:29:58.000000 mailbagit-0.5.1/tests/test_formats.py
```

### Comparing `mailbagit-0.5.0/LICENSE` & `mailbagit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/PKG-INFO` & `mailbagit-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool for preserving email with multiple masters.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 Provides-Extra: pst
@@ -154,9 +152,7 @@
 We owe a lot to the hard work that goes towards developing and maintaining the libraries `mailbagit` uses to parse email formats and make bags. We'd like to thank these awesome projects, without which `mailbagit` wouldn't be possible:  
 
 * [extractMsg](https://github.com/TeamMsgExtractor/msg-extractor)
 * [libpff](https://github.com/libyal/libpff)
 * [bagit-python](https://github.com/LibraryOfCongress/bagit-python)
 
 We'd also like to thank the [RATOM project](https://ratom.web.unc.edu/) whose documentation was super helpful in guiding us though some roadblocks.
-
-
```

### Comparing `mailbagit-0.5.0/README.md` & `mailbagit-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/__init__.py` & `mailbagit-0.5.1/mailbagit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __init__.py
 
 # Version of the mailbagit package
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 import os
 from pathlib import Path
 from bagit import _make_parser, Bag, BagHeaderAction, DEFAULT_CHECKSUMS
 import importlib
 from mailbagit.loggerx import setup_logging, get_logger
 from argparse import ArgumentParser, FileType
```

### Comparing `mailbagit-0.5.0/mailbagit/controller.py` & `mailbagit-0.5.1/mailbagit/controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivative.py` & `mailbagit-0.5.1/mailbagit/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/eml.py` & `mailbagit-0.5.1/mailbagit/derivatives/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/example.py` & `mailbagit-0.5.1/mailbagit/derivatives/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/html.py` & `mailbagit-0.5.1/mailbagit/derivatives/html.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/mbox.py` & `mailbagit-0.5.1/mailbagit/derivatives/mbox.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/pdf.py` & `mailbagit-0.5.1/mailbagit/derivatives/pdf.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/pdf_chrome.py` & `mailbagit-0.5.1/mailbagit/derivatives/pdf_chrome.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/txt.py` & `mailbagit-0.5.1/mailbagit/derivatives/txt.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/derivatives/warc.py` & `mailbagit-0.5.1/mailbagit/derivatives/warc.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/email_account.py` & `mailbagit-0.5.1/mailbagit/email_account.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/formats/eml.py` & `mailbagit-0.5.1/mailbagit/formats/eml.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/formats/example.py` & `mailbagit-0.5.1/mailbagit/formats/example.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/formats/mbox.py` & `mailbagit-0.5.1/mailbagit/formats/mbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,16 @@
             fileList = []
             for root, dirs, files in os.walk(self.path):
                 for file in files:
                     mailbag_path = os.path.join(self.path, self.mailbag_name) + os.sep
                     fileRoot = root + os.sep
                     # don't count the newly-created mailbag
                     if not fileRoot.startswith(mailbag_path):
-                        if file.lower().endswith("." + self.format_name):
+                        # Mac Mail export file is "mbox" without an extension, so this checks that
+                        if file.lower().endswith("." + self.format_name) or file.lower().strip() == "mbox":
                             fileList.append(os.path.join(root, file))
                         elif self.companion_files:
                             companion_files.append(os.path.join(root, file))
 
         for filePath in fileList:
             rel_path = format.relativePath(self.path, filePath)
             if len(rel_path) < 1:
```

### Comparing `mailbagit-0.5.0/mailbagit/formats/msg.py` & `mailbagit-0.5.1/mailbagit/formats/msg.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/formats/pst.py` & `mailbagit-0.5.1/mailbagit/formats/pst.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/guided.py` & `mailbagit-0.5.1/mailbagit/guided.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/helper/common.py` & `mailbagit-0.5.1/mailbagit/helper/common.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/helper/controller.py` & `mailbagit-0.5.1/mailbagit/helper/controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/helper/derivative.py` & `mailbagit-0.5.1/mailbagit/helper/derivative.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/helper/format.py` & `mailbagit-0.5.1/mailbagit/helper/format.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/loggerx.py` & `mailbagit-0.5.1/mailbagit/loggerx.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit/models.py` & `mailbagit-0.5.1/mailbagit/models.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/mailbagit.egg-info/PKG-INFO` & `mailbagit-0.5.1/mailbagit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mailbagit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool for preserving email with multiple masters.
 Home-page: https://github.com/UAlbanyArchives/mailbag
 Author: Gregory Wiedeman
 Author-email: gwiedeman@albany.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 Provides-Extra: pst
@@ -154,9 +152,7 @@
 We owe a lot to the hard work that goes towards developing and maintaining the libraries `mailbagit` uses to parse email formats and make bags. We'd like to thank these awesome projects, without which `mailbagit` wouldn't be possible:  
 
 * [extractMsg](https://github.com/TeamMsgExtractor/msg-extractor)
 * [libpff](https://github.com/libyal/libpff)
 * [bagit-python](https://github.com/LibraryOfCongress/bagit-python)
 
 We'd also like to thank the [RATOM project](https://ratom.web.unc.edu/) whose documentation was super helpful in guiding us though some roadblocks.
-
-
```

### Comparing `mailbagit-0.5.0/mailbagit.egg-info/SOURCES.txt` & `mailbagit-0.5.1/mailbagit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/setup.py` & `mailbagit-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mailbagit",
-    version="0.5.0",
+    version="0.5.1",
     author="Gregory Wiedeman",
     author_email="gwiedeman@albany.edu",
     description="A tool for preserving email with multiple masters.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UAlbanyArchives/mailbag",
     packages=setuptools.find_namespace_packages(exclude=("tests")),
```

### Comparing `mailbagit-0.5.0/tests/test_controller.py` & `mailbagit-0.5.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `mailbagit-0.5.0/tests/test_formats.py` & `mailbagit-0.5.1/tests/test_formats.py`

 * *Files identical despite different names*

