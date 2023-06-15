# Comparing `tmp/sqscraper-0.2.0.tar.gz` & `tmp/sqscraper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqscraper-0.2.0.tar", last modified: Wed Jun 14 06:38:35 2023, max compression
+gzip compressed data, was "sqscraper-0.3.0.tar", last modified: Thu Jun 15 19:47:31 2023, max compression
```

## Comparing `sqscraper-0.2.0.tar` & `sqscraper-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:38:35.265382 sqscraper-0.2.0/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2296 2023-06-14 06:38:35.265382 sqscraper-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-14 06:29:52.000000 sqscraper-0.2.0/README.md
--rw-rw-rw-   0        0        0     1610 2023-06-14 06:37:32.000000 sqscraper-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 06:38:35.281025 sqscraper-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 06:38:35.202871 sqscraper-0.2.0/sqscraper/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:55:42.000000 sqscraper-0.2.0/sqscraper/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:16:53.000000 sqscraper-0.2.0/sqscraper/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:38:35.265382 sqscraper-0.2.0/sqscraper/cnbc/
--rw-rw-rw-   0        0        0       49 2023-06-13 21:33:37.000000 sqscraper-0.2.0/sqscraper/cnbc/__init__.py
--rw-rw-rw-   0        0        0     7647 2023-06-13 22:18:31.000000 sqscraper-0.2.0/sqscraper/cnbc/quote_strip.py
--rw-rw-rw-   0        0        0      835 2023-06-13 22:18:02.000000 sqscraper-0.2.0/sqscraper/cnbc/stock_quote.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:38:35.218510 sqscraper-0.2.0/sqscraper.egg-info/
--rw-rw-rw-   0        0        0     2296 2023-06-14 06:38:35.000000 sqscraper-0.2.0/sqscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-06-14 06:38:35.000000 sqscraper-0.2.0/sqscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:38:35.000000 sqscraper-0.2.0/sqscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      271 2023-06-14 06:38:35.000000 sqscraper-0.2.0/sqscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 06:38:35.000000 sqscraper-0.2.0/sqscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.897035 sqscraper-0.3.0/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2312 2023-06-15 19:47:31.897035 sqscraper-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-14 06:29:52.000000 sqscraper-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1550 2023-06-15 19:43:45.000000 sqscraper-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:47:31.897035 sqscraper-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.856765 sqscraper-0.3.0/sqscraper/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:55:42.000000 sqscraper-0.3.0/sqscraper/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:16:53.000000 sqscraper-0.3.0/sqscraper/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.881403 sqscraper-0.3.0/sqscraper/cnbc/
+-rw-rw-rw-   0        0        0       50 2023-06-14 22:43:38.000000 sqscraper-0.3.0/sqscraper/cnbc/__init__.py
+-rw-rw-rw-   0        0        0     2337 2023-06-15 19:28:11.000000 sqscraper-0.3.0/sqscraper/cnbc/quote_strip.py
+-rw-rw-rw-   0        0        0     2618 2023-06-15 19:29:01.000000 sqscraper-0.3.0/sqscraper/cnbc/stock_quote.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:47:31.881403 sqscraper-0.3.0/sqscraper.egg-info/
+-rw-rw-rw-   0        0        0     2312 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      219 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 19:47:31.000000 sqscraper-0.3.0/sqscraper.egg-info/top_level.txt
```

### Comparing `sqscraper-0.2.0/LICENSE` & `sqscraper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqscraper-0.2.0/PKG-INFO` & `sqscraper-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.2.0
-Summary: Web scraper for various stock quote websites.
+Version: 0.3.0
+Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/JacobLee23/SQScraper
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `sqscraper-0.2.0/pyproject.toml` & `sqscraper-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqscraper"
-version = "0.2.0"
-description = "Web scraper for various stock quote websites."
+version = "0.3.0"
+description = "API wrapper and web scraper for select stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Financial and Insurance Industry",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
@@ -23,30 +23,28 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development"
 ]
 requires-python = ">=3.6"
 dependencies = [
-    "beautifulsoup4==4.12.2",
     "certifi==2023.5.7 ; python_version >= '3.6'",
     "charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'",
     "idna==3.4 ; python_version >= '3.5'",
-    "lxml==4.9.2",
     "numpy==1.24.3",
     "requests==2.31.0",
-    "soupsieve==2.4.1; python_version >= '3.7'",
     "urllib3==2.0.3 ; python_version >= '3.7'"
 ]
 
 [project.urls]
 homepage = "https://github.com/JacobLee23/SQScraper"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = [
     "sqscraper",
     "sqscraper.*"
 ]
 exclude = [
-    "sqscraper.tests*"
+    "sqscraper.tests",
+    "sqscraper.tests.*"
 ]
```

### Comparing `sqscraper-0.2.0/sqscraper.egg-info/PKG-INFO` & `sqscraper-0.3.0/sqscraper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.2.0
-Summary: Web scraper for various stock quote websites.
+Version: 0.3.0
+Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/JacobLee23/SQScraper
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

