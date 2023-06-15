# Comparing `tmp/chartstag-0.8.1.tar.gz` & `tmp/chartstag-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartstag-0.8.1.tar", max compression
+gzip compressed data, was "chartstag-0.8.2.tar", max compression
```

## Comparing `chartstag-0.8.1.tar` & `chartstag-0.8.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-02-05 10:23:13.983532 chartstag-0.8.1/LICENSE
--rw-r--r--   0        0        0     1102 2023-02-05 10:36:31.407336 chartstag-0.8.1/README.md
--rw-r--r--   0        0        0       50 2023-02-05 10:38:42.488623 chartstag-0.8.1/chartstag/__init__.py
--rw-r--r--   0        0        0      530 2023-02-05 10:49:15.918849 chartstag-0.8.1/chartstag/mermaid/__init__.py
--rw-r--r--   0        0        0   258567 2023-01-18 13:21:55.123000 chartstag-0.8.1/chartstag/mermaid/data/mermaid_min.zip
--rw-r--r--   0        0        0     2183 2023-02-05 10:54:24.773853 chartstag-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 chartstag-0.8.1/setup.py
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 chartstag-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-02-05 10:57:52.115805 chartstag-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1157 2023-06-15 21:19:15.705934 chartstag-0.8.2/README.md
+-rw-r--r--   0        0        0       50 2023-02-05 10:38:42.488623 chartstag-0.8.2/chartstag/__init__.py
+-rw-r--r--   0        0        0      530 2023-02-05 10:49:15.918849 chartstag-0.8.2/chartstag/mermaid/__init__.py
+-rw-r--r--   0        0        0   863091 2023-06-15 21:13:17.628375 chartstag-0.8.2/chartstag/mermaid/data/mermaid_min.zip
+-rw-r--r--   0        0        0     2133 2023-06-15 21:26:04.508279 chartstag-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 chartstag-0.8.2/PKG-INFO
```

### Comparing `chartstag-0.8.1/LICENSE` & `chartstag-0.8.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Michael Ikemann
+Copyright (c) 2023 SciStag
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `chartstag-0.8.1/README.md` & `chartstag-0.8.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # ChartStag
 
+## v0.8.2
+
 ChartStag is an extension for the [SciStag](https://github.com/scistag/scistag) package
-which supports you in your computer vision, data science and data engineering 
+which supports you in your computer vision, data science and data engineering
 projects.
 
 It extends SciStag with diagram and chart plotting capabilities. As of now solely by
-integrating [mermaid](https://github.com/mermaid-js/mermaid), an awesome diagram and 
+integrating [mermaid](https://github.com/mermaid-js/mermaid), an awesome diagram and
 charting tool written in JavaScript, into SciStag VisualLog.
 
-mermaid is licensed under the terms of the [MIT license](https://github.com/mermaid-js/mermaid/blob/develop/LICENSE) -
-for further details about mermaid visit https://github.com/mermaid-js/mermaid or 
+mermaid is licensed under the terms of
+the [MIT license](https://github.com/mermaid-js/mermaid/blob/develop/LICENSE) -
+for further details about mermaid visit https://github.com/mermaid-js/mermaid or
 https://mermaid.js.org/.
 
 At this point huge thanks to [Knut Sveidqvist](https://github.com/knsv) and the whole
 mermaid team for their awesome work.
 
+Embedded tools versions:
+
+* **Mermaid 10.2.3**
+
 ---
 
-ChartStag itself is as well licensed under the terms of the MIT license and 
+ChartStag itself is as well licensed under the terms of the MIT license and
 Copyright (c) 2023 [Michael Ikemann](https://github.com/alyxion).
 
-For examples about how to use ChartStag in SciStag install scistag via `pip install scistag[common]`
+For examples about how to use ChartStag in SciStag install scistag
+via `pip install scistag[common]`
 and see https://github.com/SciStag/SciStag/tree/main/scistag/examples/vislog.
```

### Comparing `chartstag-0.8.1/chartstag/mermaid/__init__.py` & `chartstag-0.8.2/chartstag/mermaid/__init__.py`

 * *Files identical despite different names*

### Comparing `chartstag-0.8.1/pyproject.toml` & `chartstag-0.8.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chartstag"
-version = "0.8.1"
+version = "0.8.2"
 description = "Charting and diagram extension for SciStag"
 authors = ["Michael Ikemann"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/scistag/chartstag"
 homepage = "https://github.com/scistag/chartstag"
 documentation = "https://scistag.readthedocs.io"
@@ -14,32 +14,29 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.2.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = ">=3.9 <3.12"
-scistag = "^0.8.1"
+python = ">=3.9"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.14.0"
 coverage = { version = "^6.4.1", extras = ["toml"] }
 pytest = "^7.1.2"
-pytest-mock = "^3.7.0"
-pytest-order = "^1.0.1"
-pytest-xdist = "^2.5.0"
 coveralls = "^3.3.1"
 black = { version = "^22.10.0", extras = ["d", "jupyter"] }
 pytest-cov = "^4.0.0"
 
 
 [tool.coverage.report]
 skip_empty = true
```

### Comparing `chartstag-0.8.1/PKG-INFO` & `chartstag-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: chartstag
-Version: 0.8.1
+Version: 0.8.2
 Summary: Charting and diagram extension for SciStag
 Home-page: https://github.com/scistag/chartstag
 License: MIT
 Keywords: Data Science,Data Engineering,Data Visualization
 Author: Michael Ikemann
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: scistag (>=0.8.1,<0.9.0)
 Project-URL: Documentation, https://scistag.readthedocs.io
 Project-URL: Repository, https://github.com/scistag/chartstag
 Description-Content-Type: text/markdown
 
 # ChartStag
 
+## v0.8.2
+
 ChartStag is an extension for the [SciStag](https://github.com/scistag/scistag) package
-which supports you in your computer vision, data science and data engineering 
+which supports you in your computer vision, data science and data engineering
 projects.
 
 It extends SciStag with diagram and chart plotting capabilities. As of now solely by
-integrating [mermaid](https://github.com/mermaid-js/mermaid), an awesome diagram and 
+integrating [mermaid](https://github.com/mermaid-js/mermaid), an awesome diagram and
 charting tool written in JavaScript, into SciStag VisualLog.
 
-mermaid is licensed under the terms of the [MIT license](https://github.com/mermaid-js/mermaid/blob/develop/LICENSE) -
-for further details about mermaid visit https://github.com/mermaid-js/mermaid or 
+mermaid is licensed under the terms of
+the [MIT license](https://github.com/mermaid-js/mermaid/blob/develop/LICENSE) -
+for further details about mermaid visit https://github.com/mermaid-js/mermaid or
 https://mermaid.js.org/.
 
 At this point huge thanks to [Knut Sveidqvist](https://github.com/knsv) and the whole
 mermaid team for their awesome work.
 
+Embedded tools versions:
+
+* **Mermaid 10.2.3**
+
 ---
 
-ChartStag itself is as well licensed under the terms of the MIT license and 
+ChartStag itself is as well licensed under the terms of the MIT license and
 Copyright (c) 2023 [Michael Ikemann](https://github.com/alyxion).
 
-For examples about how to use ChartStag in SciStag install scistag via `pip install scistag[common]`
+For examples about how to use ChartStag in SciStag install scistag
+via `pip install scistag[common]`
 and see https://github.com/SciStag/SciStag/tree/main/scistag/examples/vislog.
```

