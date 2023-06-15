# Comparing `tmp/outputfile-0.1.0.tar.gz` & `tmp/outputfile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outputfile-0.1.0.tar", max compression
+gzip compressed data, was "outputfile-0.2.0.tar", max compression
```

## Comparing `outputfile-0.1.0.tar` & `outputfile-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-14 21:28:00.000250 outputfile-0.1.0/LICENSE
--rw-r--r--   0        0        0      938 2023-06-14 21:28:00.004250 outputfile-0.1.0/README.md
--rw-r--r--   0        0        0     1366 2023-06-14 21:28:00.004250 outputfile-0.1.0/outputfile/__init__.py
--rw-r--r--   0        0        0     2124 2023-06-14 21:28:00.000250 outputfile-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 outputfile-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-15 05:26:18.116703 outputfile-0.2.0/LICENSE
+-rw-r--r--   0        0        0      938 2023-06-14 21:28:00.004250 outputfile-0.2.0/README.md
+-rw-r--r--   0        0        0    10492 2023-06-15 06:51:24.104355 outputfile-0.2.0/outputfile/__init__.py
+-rw-r--r--   0        0        0     2124 2023-06-15 14:30:43.754741 outputfile-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 outputfile-0.2.0/PKG-INFO
```

### Comparing `outputfile-0.1.0/LICENSE` & `outputfile-0.2.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 outputfile
+Copyright (c) 2023 nbiotcloud
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `outputfile-0.1.0/README.md` & `outputfile-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `outputfile-0.1.0/pyproject.toml` & `outputfile-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "outputfile"
-version = "0.1.0"
+version = "0.2.0"
 description = "Timestamp Preserving Output File Writer"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -23,20 +23,20 @@
 #[tool.poetry.scripts]
 
 
 [tool.poetry.dependencies]
 python = '^3.7.2'
 
 [tool.poetry.group.test.dependencies]
-black = '^22.3.0'
+black = '^23.3.0'
 coverage = '^6.4.4'
 isort = '^5.9'
-mypy = "~1.0.0"
+mypy = "^1.3.0"
 pylint = '^2.15'
-pytest = '^6.2'
+pytest = '^7.3'
 
 [tool.poetry.group.doc.dependencies]
 sphinx = '^5.1.1'
 sphinx-rtd-theme = "^1.0.0"
 sphinxemoji = ">=0.2.0"
 
 [build-system]
```

### Comparing `outputfile-0.1.0/PKG-INFO` & `outputfile-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outputfile
-Version: 0.1.0
+Version: 0.2.0
 Summary: Timestamp Preserving Output File Writer
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

