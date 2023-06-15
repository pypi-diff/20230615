# Comparing `tmp/mecapacktools-1.1.0.tar.gz` & `tmp/mecapacktools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecapacktools-1.1.0.tar", max compression
+gzip compressed data, was "mecapacktools-1.1.1.tar", max compression
```

## Comparing `mecapacktools-1.1.0.tar` & `mecapacktools-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.1.0/mecapacktools/__init__.py
--rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.1.0/mecapacktools/libCfg.py
--rw-r--r--   0        0        0     5025 2023-06-05 13:13:15.138222 mecapacktools-1.1.0/mecapacktools/libFTP.py
--rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.1.0/mecapacktools/libLog.py
--rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.1.0/mecapacktools/libMail.py
--rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.1.0/mecapacktools/libSql.py
--rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.1.0/mecapacktools/libTool.py
--rw-r--r--   0        0        0    20319 2023-06-07 08:51:38.798095 mecapacktools-1.1.0/mecapacktools/libWebServices.py
--rw-r--r--   0        0        0     1161 2023-06-14 10:11:29.107682 mecapacktools-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      676 2023-06-05 11:21:37.250074 mecapacktools-1.1.0/README.md
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 mecapacktools-1.1.0/setup.py
--rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 mecapacktools-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.1.1/mecapacktools/__init__.py
+-rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.1.1/mecapacktools/libCfg.py
+-rw-r--r--   0        0        0     5025 2023-06-05 13:13:15.138222 mecapacktools-1.1.1/mecapacktools/libFTP.py
+-rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.1.1/mecapacktools/libLog.py
+-rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.1.1/mecapacktools/libMail.py
+-rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.1.1/mecapacktools/libSql.py
+-rw-r--r--   0        0        0    16439 2023-06-15 09:51:12.020896 mecapacktools-1.1.1/mecapacktools/libTool.py
+-rw-r--r--   0        0        0    20319 2023-06-07 08:51:38.798095 mecapacktools-1.1.1/mecapacktools/libWebServices.py
+-rw-r--r--   0        0        0     1161 2023-06-15 09:57:51.924623 mecapacktools-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      676 2023-06-05 11:21:37.250074 mecapacktools-1.1.1/README.md
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 mecapacktools-1.1.1/setup.py
+-rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 mecapacktools-1.1.1/PKG-INFO
```

### Comparing `mecapacktools-1.1.0/LICENSE` & `mecapacktools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/mecapacktools/libCfg.py` & `mecapacktools-1.1.1/mecapacktools/libCfg.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/mecapacktools/libFTP.py` & `mecapacktools-1.1.1/mecapacktools/libFTP.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/mecapacktools/libLog.py` & `mecapacktools-1.1.1/mecapacktools/libLog.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/mecapacktools/libMail.py` & `mecapacktools-1.1.1/mecapacktools/libMail.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/mecapacktools/libSql.py` & `mecapacktools-1.1.1/mecapacktools/libSql.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/mecapacktools/libTool.py` & `mecapacktools-1.1.1/mecapacktools/libTool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #! /usr/bin/env python
 # -*- coding:Utf-8 -*-
-# pylint: disable=fixme,invalid-name,line-too-long
+# pylint: disable=fixme,invalid-name,line-too-long,too-many-arguments
 """Tools python."""
 # ============================================================
 #    Linux python path and Library import
 # ============================================================
 
 import calendar
 import datetime
 from collections import OrderedDict
+from enum import Enum
 from typing import Any, Iterable, Tuple
 
 import arrow
 
 # ============================================================
 #     Functions and Procedures
 # ============================================================
@@ -77,14 +78,58 @@
     for val in iterable:
         yield False, ret_var
         ret_var = val
     yield True, ret_var
 
 
 # ||||||||||||||||||||||||||||||||||||||||||||||||||
+#    convert_datetime
+# ||||||||||||||||||||||||||||||||||||||||||||||||||
+
+
+class mode_convert(Enum):
+    """Mode de conversion pour la fonction convert_datetime"""
+
+    SYLOB_PARAM = "%Y-%m-%d %H:%M:%S"
+    SYLOB_RETOUR = "%d/%m/%Y %H:%M"
+    INTERSYMEC = "%Y-%d-%m %H:%M:%S"
+    S9000 = "%Y-%m-%d"
+    S9000_FILE = "%d/%m/%Y"
+    SYLOB_TO_INTERSYMEC = 9
+
+
+def convert_datetime(dte, mode: mode_convert):
+    """
+    Conversion datetime multiples format
+
+    Args:
+        dte (datetime): date à convertir
+        mode (mode_convert): Mode de conversion='SYLOB_PARAM' ou 'SYLOB_RETOUR' ou 'INTERSYMEC' ou 'S9000'
+
+    Returns:
+        datetime ou str: date convertie
+    """
+    if mode.name == "SYLOB_RETOUR":
+        if " " in dte:
+            sylob_retour = mode_convert.SYLOB_RETOUR.value
+        else:
+            sylob_retour = mode_convert.SYLOB_RETOUR.value.split(" ", maxsplit=1)[0]
+        return datetime.datetime.strptime(dte, sylob_retour)
+    if mode.name in ("SYLOB_PARAM", "INTERSYMEC"):
+        return dte.strftime(mode.value)
+    if mode.name == "S9000_FILE":
+        return datetime.datetime.strptime(dte, mode.value)
+    if mode.name == "SYLOB_TO_S9000":
+        return convert_datetime(dte, mode_convert.SYLOB_RETOUR).strftime(mode_convert.S9000.value)
+    if mode.name == "SYLOB_TO_INTERSYMEC":
+        return convert_datetime(dte, mode_convert.SYLOB_RETOUR).strftime(mode_convert.INTERSYMEC.value)
+    return None
+
+
+# ||||||||||||||||||||||||||||||||||||||||||||||||||
 #    add_months
 # ||||||||||||||||||||||||||||||||||||||||||||||||||
 def add_months(pdate, pmonths):
     """
     Add pmonths months to pdate
 
     Args:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mecapacktools-1.1.0/mecapacktools/libWebServices.py` & `mecapacktools-1.1.1/mecapacktools/libWebServices.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/pyproject.toml` & `mecapacktools-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecapacktools"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["Informatique Mecapack <informatique@mecapack.com>"]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 exclude = ["mecapacktools/libExcel.py"]
```

### Comparing `mecapacktools-1.1.0/README.md` & `mecapacktools-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.1.0/setup.py` & `mecapacktools-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sql': ['pypyodbc>=1.3.6,<2.0.0'],
  'webservices': ['requests>=2.28.2,<3.0.0',
                  'suds>=1.1.2,<2.0.0',
                  'xmltodict>=0.13.0,<0.14.0']}
 
 setup_kwargs = {
     'name': 'mecapacktools',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': '',
     'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\n\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\n- excel \n- Sql \n- WebServices \n- FTP \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier sur pypi `poetry publish --build`\n\n\n\n',
     'author': 'Informatique Mecapack',
     'author_email': 'informatique@mecapack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mecapacktools-1.1.0/PKG-INFO` & `mecapacktools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecapacktools
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 Author: Informatique Mecapack
 Author-email: informatique@mecapack.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

