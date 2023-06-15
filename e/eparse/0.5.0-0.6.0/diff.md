# Comparing `tmp/eparse-0.5.0.tar.gz` & `tmp/eparse-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.5.0.tar", last modified: Wed Jun 14 18:39:02 2023, max compression
+gzip compressed data, was "eparse-0.6.0.tar", last modified: Thu Jun 15 01:34:00 2023, max compression
```

## Comparing `eparse-0.5.0.tar` & `eparse-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.5.0/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.5.0/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.5.0/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.5.0/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 18:39:02.847827 eparse-0.5.0/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10996 2023-06-14 17:19:22.000000 eparse-0.5.0/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.5.0/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-14 18:26:31.000000 eparse-0.5.0/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    10257 2023-06-14 18:24:15.000000 eparse-0.5.0/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5034 2023-06-14 18:22:39.000000 eparse-0.5.0/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.5.0/eparse/interfaces.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.5.0/eparse/migrations.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12067 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-14 18:39:02.000000 eparse-0.5.0/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-14 18:39:02.847827 eparse-0.5.0/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-14 18:26:17.000000 eparse-0.5.0/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-14 18:39:02.847827 eparse-0.5.0/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.5.0/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.5.0/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.5.0/tests/fixtures.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.5.0/tests/test.db
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.5.0/tests/test_cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.5.0/tests/test_core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.5.0/tests/test_interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.6.0/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.6.0/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.6.0/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.6.0/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12670 2023-06-15 01:34:00.238480 eparse-0.6.0/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11599 2023-06-15 01:31:22.000000 eparse-0.6.0/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.6.0/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-15 01:21:07.000000 eparse-0.6.0/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9581 2023-06-15 01:18:10.000000 eparse-0.6.0/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5771 2023-06-15 01:08:49.000000 eparse-0.6.0/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.6.0/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.6.0/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    12670 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-15 01:34:00.000000 eparse-0.6.0/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      141 2023-06-15 01:34:00.238480 eparse-0.6.0/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-15 01:20:56.000000 eparse-0.6.0/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-15 01:34:00.238480 eparse-0.6.0/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.6.0/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.6.0/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.6.0/tests/fixtures.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.6.0/tests/test.db
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.6.0/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.6.0/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.6.0/tests/test_interfaces.py
```

### Comparing `eparse-0.5.0/CONTRIBUTING.rst` & `eparse-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/LICENSE` & `eparse-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/PKG-INFO` & `eparse-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.5.0
+Version: 0.6.0
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
@@ -33,20 +33,21 @@
 
 
 Description
 ===========
 Excel spreadsheet crawler and table parser for data extraction
 and querying.
 
+
 Features
 ========
 * Command-line interface
 * Recursive Excel file discovery
 * Tabular data extraction
-* SQLite database interface
+* SQLite and PostgreSQL database interfaces
 * CLI query tool
 * Summary data metrics
 
 
 Installation
 ============
 To install eparse, you can use pip and the latest version on PyPI:
@@ -82,16 +83,16 @@
 as ``postgres://user:pass@host:port/my_db`` that mentions the
 postgres driver is missing, then you know you haven't properly
 installed (and compiled)  ``psycopg2``.
 
 
 Usage
 =====
-eparse is intended to be used from the command-line.  You can view
-supported commands and usage with ``--help`` as follows:
+eparse can be used as either a python library or from the command-line.
+You can view supported CLI commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
 
     $ eparse --help
     Usage: eparse [OPTIONS] COMMAND [ARGS]...
 
     excel parser
@@ -109,14 +110,28 @@
 
     Commands:
     migrate  migrate eparse table
     parse    parse table(s) found in sheet for target(s)
     query    query eparse output
     scan     scan for excel files in target
 
+You can also use eparse from python like so:
+
+.. code-block:: python
+
+    from eparse.core import get_df_from_file
+
+    print([table for table in get_df_from_file('myfile.xlsx')])
+    102   Date  Principal Repayment   Date  Principal Repayment
+    103  44834        700757.679004  44926        430013.148303
+    104  44926         71957.776108  45016        100576.127808
+    105  45016         147578.19262  45107        898008.340095
+    106  45107         32801.363072  45199         841656.13896
+    ...
+
 
 Scan
 ----
 To scan one or more directories for Excel files with descriptive
 information, you can use the ``scan`` command like so:
 
 .. code-block:: bash
@@ -143,15 +158,16 @@
 (or sheet boundaries).  A densely or sparsely populated 2x2 table must
 follow in order for data to be extracted in relation to that cell.
 eparse will automatically adjust for rowspan labels and empty table
 corners and the dense vs. sparse criterion can be controlled with
 the ``--loose`` flag.
 
 eparse was written to accomodate various types of output formats and
-endpoints, including ``null:///``, ``stdout:///``, and ``sqlite3:///``.
+endpoints, including ``null:///``, ``stdout:///``, ``sqlite3:///db_name``,
+and ``postgres://user:password@host:port/db_name``.
 
 null
 ^^^^
 This mode is useful for validating files and generating descriptive
 info, and is the default.  The command above with `-v` is an example
 of this mode, which lists out the tables found.
```

### Comparing `eparse-0.5.0/README.rst` & `eparse-0.6.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 
 
 Description
 ===========
 Excel spreadsheet crawler and table parser for data extraction
 and querying.
 
+
 Features
 ========
 * Command-line interface
 * Recursive Excel file discovery
 * Tabular data extraction
-* SQLite database interface
+* SQLite and PostgreSQL database interfaces
 * CLI query tool
 * Summary data metrics
 
 
 Installation
 ============
 To install eparse, you can use pip and the latest version on PyPI:
@@ -61,16 +62,16 @@
 as ``postgres://user:pass@host:port/my_db`` that mentions the
 postgres driver is missing, then you know you haven't properly
 installed (and compiled)  ``psycopg2``.
 
 
 Usage
 =====
-eparse is intended to be used from the command-line.  You can view
-supported commands and usage with ``--help`` as follows:
+eparse can be used as either a python library or from the command-line.
+You can view supported CLI commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
 
     $ eparse --help
     Usage: eparse [OPTIONS] COMMAND [ARGS]...
 
     excel parser
@@ -88,14 +89,28 @@
 
     Commands:
     migrate  migrate eparse table
     parse    parse table(s) found in sheet for target(s)
     query    query eparse output
     scan     scan for excel files in target
 
+You can also use eparse from python like so:
+
+.. code-block:: python
+
+    from eparse.core import get_df_from_file
+
+    print([table for table in get_df_from_file('myfile.xlsx')])
+    102   Date  Principal Repayment   Date  Principal Repayment
+    103  44834        700757.679004  44926        430013.148303
+    104  44926         71957.776108  45016        100576.127808
+    105  45016         147578.19262  45107        898008.340095
+    106  45107         32801.363072  45199         841656.13896
+    ...
+
 
 Scan
 ----
 To scan one or more directories for Excel files with descriptive
 information, you can use the ``scan`` command like so:
 
 .. code-block:: bash
@@ -122,15 +137,16 @@
 (or sheet boundaries).  A densely or sparsely populated 2x2 table must
 follow in order for data to be extracted in relation to that cell.
 eparse will automatically adjust for rowspan labels and empty table
 corners and the dense vs. sparse criterion can be controlled with
 the ``--loose`` flag.
 
 eparse was written to accomodate various types of output formats and
-endpoints, including ``null:///``, ``stdout:///``, and ``sqlite3:///``.
+endpoints, including ``null:///``, ``stdout:///``, ``sqlite3:///db_name``,
+and ``postgres://user:password@host:port/db_name``.
 
 null
 ^^^^
 This mode is useful for validating files and generating descriptive
 info, and is the default.  The command above with `-v` is an example
 of this mode, which lists out the tables found.
```

### Comparing `eparse-0.5.0/docs/Makefile` & `eparse-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/docs/conf.py` & `eparse-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/docs/installation.rst` & `eparse-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/docs/make.bat` & `eparse-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/eparse/cli.py` & `eparse-0.6.0/eparse/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from pprint import PrettyPrinter
 import sys
 
 import pandas as pd
 
 from .core import (
     df_find_tables,
-    df_parse_table,
     df_normalize_data,
     df_serialize_table,
+    get_df_from_file,
 )
 from .interfaces import ExcelParse, i_factory
 
 
 def handle(e, exceptions=None, msg=None, debug=False, exit=True):
     '''
     handle exceptions based on settings
@@ -272,71 +272,57 @@
     ctx.obj['sheet'] = sheet
     ctx.obj['serialize'] = serialize
     ctx.obj['table'] = table
 
     if ctx.obj['debug']:
         PrettyPrinter().pprint(ctx.obj)
 
-    # process each Excel file in files
-    for i, f in enumerate(ctx.obj['files']):
+    for f in ctx.obj['files']:
         if f.is_file() and 'xls' in f.name:
+            print(f'{f.name}')
+
             try:
-                e_file = pd.read_excel(
+                for (
+                    output,
+                    excel_RC,
+                    name,
+                    s,
+                ) in get_df_from_file(
                     f,
-                    sheet_name=list(sheet) or None,
-                    header=None,
-                    index_col=None,
-                )
-            except Exception as e:
-                msg = f'skipping {f} - {e}'
-                handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
-                continue
-
-            if not ctx.obj['verbose']:
-                print(f'{f.name}')
-
-            # convert e_file to dict if single sheet
-            if type(e_file) is not dict:
-                e_file = {s: e_file for s in sheet}
-
-            # process each table found in each sheet of file
-            for s in e_file.keys():
-                for r, c, excel_RC, name in df_find_tables(
-                    e_file[s],
                     ctx.obj['loose'],
+                    sheet,
+                    table,
                 ):
-                    if table is not None and table.lower() not in name.lower():
-                        continue
-
-                    # parse and serialize (if enabled) table
-                    output = df_parse_table(e_file[s], r, c)
-
                     if ctx.obj['verbose']:
                         m = '{} table {} {} found at {} in {}'
                         v = (f.name, name, output.shape, excel_RC, s)
                         print(m.format(*v))
 
                     if serialize:
                         output = df_serialize_table(
                             output,
-                            name=str(name),
-                            sheet=str(s),
-                            f_name=str(f.name),
+                            name=name,
+                            sheet=s,
+                            f_name=f.name,
                         )
 
                     if ctx.obj['debug']:
                         PrettyPrinter().pprint(output)
 
-                    # output table
                     try:
                         ctx.obj['output_obj'].output(output, ctx)
                     except Exception as e:
                         msg = f'output to {ctx.obj["output"]} failed - {e}'
                         handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
-                        continue
+                        break
+
+            except Exception as e:
+                msg = f'skipping {f} - {e}'
+                handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
+                continue
 
 
 @main.command()
 @click.pass_context
 @click.option(
     '--filter',
     '-f',
```

### Comparing `eparse-0.5.0/eparse/core.py` & `eparse-0.6.0/eparse/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding: utf-8 -*-
 
 '''
 excel parser core module
 '''
 
-from typing import Dict, List, Tuple
+from typing import Dict, Iterable, List, Tuple
 
 from openpyxl.utils.cell import get_column_letter
 import pandas as pd
 
 
 TableRef = Tuple[int, int, str, str]  # r, c, excel RC, value
-TableRec = Tuple[str, str, pd.DataFrame]  # name, excel RC, table
 
 
 # NOTE: df[n] df.at[r,c] and df.iloc[r,c] are not all the same
 #       only with .iloc is it safe to assume index and column
 #       names will be ingored ; use iloc when working with
 #       sub-tables, e.g. the output from df_parse_table
 
 
-def df_find_tables(df: pd.DataFrame, loose=False) -> List[TableRef]:
+def df_find_tables(
+    df: pd.DataFrame,
+    loose: bool = False,
+) -> List[TableRef]:
     '''
     finds table corners in a dataframe
     '''
 
     result = []
 
     # for each row
@@ -202,7 +204,43 @@
                         'excel_RC': f'{get_column_letter(_c+1)}{_r+1}',
                         **other_data,
                     }
                 )
             )
 
     return result
+
+
+def get_df_from_file(
+    filename: str,
+    loose: bool = True,
+    sheet: Iterable = [],
+    table: str = None,
+):
+    '''
+    helper function to yield tables from a file
+    '''
+
+    f = pd.read_excel(
+        filename,
+        sheet_name=list(sheet) or None,
+        header=None,
+        index_col=None,
+    )
+
+    # convert to dict if single sheet
+    if type(f) is not dict:
+        f = {s: f for s in sheet}
+
+    for s in f.keys():
+        tables = df_find_tables(f[s], loose)
+
+        for r, c, excel_RC, name in tables:
+            if table is not None and table.lower() not in name.lower():
+                continue
+
+            yield (
+                df_parse_table(f[s], r, c),
+                excel_RC,
+                name,
+                s,
+            )
```

### Comparing `eparse-0.5.0/eparse/interfaces.py` & `eparse-0.6.0/eparse/interfaces.py`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/eparse/migrations.py` & `eparse-0.6.0/eparse/migrations.py`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/eparse.egg-info/PKG-INFO` & `eparse-0.6.0/eparse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.5.0
+Version: 0.6.0
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
@@ -33,20 +33,21 @@
 
 
 Description
 ===========
 Excel spreadsheet crawler and table parser for data extraction
 and querying.
 
+
 Features
 ========
 * Command-line interface
 * Recursive Excel file discovery
 * Tabular data extraction
-* SQLite database interface
+* SQLite and PostgreSQL database interfaces
 * CLI query tool
 * Summary data metrics
 
 
 Installation
 ============
 To install eparse, you can use pip and the latest version on PyPI:
@@ -82,16 +83,16 @@
 as ``postgres://user:pass@host:port/my_db`` that mentions the
 postgres driver is missing, then you know you haven't properly
 installed (and compiled)  ``psycopg2``.
 
 
 Usage
 =====
-eparse is intended to be used from the command-line.  You can view
-supported commands and usage with ``--help`` as follows:
+eparse can be used as either a python library or from the command-line.
+You can view supported CLI commands and usage with ``--help`` as follows:
 
 .. code-block:: bash
 
     $ eparse --help
     Usage: eparse [OPTIONS] COMMAND [ARGS]...
 
     excel parser
@@ -109,14 +110,28 @@
 
     Commands:
     migrate  migrate eparse table
     parse    parse table(s) found in sheet for target(s)
     query    query eparse output
     scan     scan for excel files in target
 
+You can also use eparse from python like so:
+
+.. code-block:: python
+
+    from eparse.core import get_df_from_file
+
+    print([table for table in get_df_from_file('myfile.xlsx')])
+    102   Date  Principal Repayment   Date  Principal Repayment
+    103  44834        700757.679004  44926        430013.148303
+    104  44926         71957.776108  45016        100576.127808
+    105  45016         147578.19262  45107        898008.340095
+    106  45107         32801.363072  45199         841656.13896
+    ...
+
 
 Scan
 ----
 To scan one or more directories for Excel files with descriptive
 information, you can use the ``scan`` command like so:
 
 .. code-block:: bash
@@ -143,15 +158,16 @@
 (or sheet boundaries).  A densely or sparsely populated 2x2 table must
 follow in order for data to be extracted in relation to that cell.
 eparse will automatically adjust for rowspan labels and empty table
 corners and the dense vs. sparse criterion can be controlled with
 the ``--loose`` flag.
 
 eparse was written to accomodate various types of output formats and
-endpoints, including ``null:///``, ``stdout:///``, and ``sqlite3:///``.
+endpoints, including ``null:///``, ``stdout:///``, ``sqlite3:///db_name``,
+and ``postgres://user:password@host:port/db_name``.
 
 null
 ^^^^
 This mode is useful for validating files and generating descriptive
 info, and is the default.  The command above with `-v` is an example
 of this mode, which lists out the tables found.
```

### Comparing `eparse-0.5.0/eparse.egg-info/SOURCES.txt` & `eparse-0.6.0/eparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/setup.py` & `eparse-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,10 +55,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.5.0',
+    version='0.6.0',
     zip_safe=False,
 )
```

### Comparing `eparse-0.5.0/tests/eparse_unit_test_data.xlsx` & `eparse-0.6.0/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/tests/fixtures.py` & `eparse-0.6.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/tests/test.db` & `eparse-0.6.0/tests/test.db`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/tests/test_cli.py` & `eparse-0.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/tests/test_core.py` & `eparse-0.6.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.5.0/tests/test_interfaces.py` & `eparse-0.6.0/tests/test_interfaces.py`

 * *Files identical despite different names*

