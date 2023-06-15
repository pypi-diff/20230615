# Comparing `tmp/p3do-0.7.0.tar.gz` & `tmp/p3do-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3do-0.7.0.tar", max compression
+gzip compressed data, was "p3do-0.7.1.tar", max compression
```

## Comparing `p3do-0.7.0.tar` & `p3do-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-15 11:14:09.440278 p3do-0.7.0/LICENSE
--rw-r--r--   0        0        0    15444 2023-06-15 11:14:09.440278 p3do-0.7.0/README.md
--rw-r--r--   0        0        0       22 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/__init__.py
--rw-r--r--   0        0        0    13964 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/cli.py
--rw-r--r--   0        0        0      274 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/github.py
--rw-r--r--   0        0        0     1832 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/jenkins.py
--rw-r--r--   0        0        0     1161 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/keycloak.py
--rw-r--r--   0        0        0     4626 2023-06-15 11:14:09.440278 p3do-0.7.0/p3do/poolparty.py
--rw-r--r--   0        0        0      936 2023-06-15 11:14:09.444278 p3do-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    16424 1970-01-01 00:00:00.000000 p3do-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-15 11:36:21.727748 p3do-0.7.1/LICENSE
+-rw-r--r--   0        0        0    15444 2023-06-15 11:36:21.727748 p3do-0.7.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/__init__.py
+-rw-r--r--   0        0        0    13964 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/cli.py
+-rw-r--r--   0        0        0      274 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/github.py
+-rw-r--r--   0        0        0     1832 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/jenkins.py
+-rw-r--r--   0        0        0     1161 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/keycloak.py
+-rw-r--r--   0        0        0     4626 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/poolparty.py
+-rw-r--r--   0        0        0      936 2023-06-15 11:36:21.727748 p3do-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    16424 1970-01-01 00:00:00.000000 p3do-0.7.1/PKG-INFO
```

### Comparing `p3do-0.7.0/LICENSE` & `p3do-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `p3do-0.7.0/README.md` & `p3do-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `p3do-0.7.0/p3do/cli.py` & `p3do-0.7.1/p3do/cli.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.0/p3do/jenkins.py` & `p3do-0.7.1/p3do/jenkins.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.0/p3do/keycloak.py` & `p3do-0.7.1/p3do/keycloak.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.0/p3do/poolparty.py` & `p3do-0.7.1/p3do/poolparty.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.0/pyproject.toml` & `p3do-0.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "p3do"
-version = "0.7.0"
+version = "0.7.1"
 description = "CLI utilities for p3d"
 authors = ["Armin Friedl <armin.friedl@semantic-web.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-keycloak = "^0.27"
 click = "^8.1"
 urllib3 = "^1.26.9" # we don't actually need that directly but older versions
                     # are incompatible with python-keycloak
 requests = "^2.27.1" # must align with what python-keycloak needs, older versions
                      # are incompatible with python-keycloak
-cryptography = ">=37.0.3,<40.0.0"
+cryptography = ">=37.0.3,<42.0.0"
 appdirs = "^1.4.4"
 jenkinsapi = "^0.3.11"
 loguru = "^0.6.0"
 rich = "^12.4.4"
 Flask = "^2.1.3"
 pygithub = "^1.58.2"
```

### Comparing `p3do-0.7.0/PKG-INFO` & `p3do-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: p3do
-Version: 0.7.0
+Version: 0.7.1
 Summary: CLI utilities for p3d
 License: MIT
 Author: Armin Friedl
 Author-email: armin.friedl@semantic-web.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2.1.3,<3.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: cryptography (>=37.0.3,<40.0.0)
+Requires-Dist: cryptography (>=37.0.3,<42.0.0)
 Requires-Dist: jenkinsapi (>=0.3.11,<0.4.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pygithub (>=1.58.2,<2.0.0)
 Requires-Dist: python-keycloak (>=0.27,<0.28)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
```

