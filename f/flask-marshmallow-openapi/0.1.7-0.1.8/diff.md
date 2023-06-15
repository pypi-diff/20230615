# Comparing `tmp/flask-marshmallow-openapi-0.1.7.tar.gz` & `tmp/flask-marshmallow-openapi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.1.7.tar", last modified: Wed Jun 14 14:07:56 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.1.8.tar", last modified: Thu Jun 15 06:35:22 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.1.7.tar` & `flask-marshmallow-openapi-0.1.8.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-14 14:07:20.000000 flask-marshmallow-openapi-0.1.7/.bumpversion.cfg
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.7/.gitignore
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.7/.python-version
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.7/LICENSE
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      838 2023-06-09 19:55:49.000000 flask-marshmallow-openapi-0.1.7/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/PKG-INFO
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.7/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-14 14:07:20.000000 flask-marshmallow-openapi-0.1.7/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      176 2023-06-14 14:07:20.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    13858 2023-06-14 14:03:50.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/middleware.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      641 2023-06-09 19:37:02.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/models.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.849251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static_collector.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.853251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-14 14:07:56.837251 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1651 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-14 14:07:56.000000 flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:35:22.356003 flask-marshmallow-openapi-0.1.8/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-15 06:34:03.000000 flask-marshmallow-openapi-0.1.8/.bumpversion.cfg
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.8/.gitignore
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.8/.python-version
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.8/LICENSE
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      838 2023-06-09 19:55:49.000000 flask-marshmallow-openapi-0.1.8/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-15 06:35:22.356003 flask-marshmallow-openapi-0.1.8/PKG-INFO
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.8/README.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-15 06:34:03.000000 flask-marshmallow-openapi-0.1.8/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-15 06:35:22.356003 flask-marshmallow-openapi-0.1.8/setup.cfg
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:35:22.340003 flask-marshmallow-openapi-0.1.8/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:35:22.344003 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      176 2023-06-15 06:34:03.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    13858 2023-06-15 06:33:38.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/decorators.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/helpers.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/middleware.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      641 2023-06-09 19:37:02.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/models.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:35:22.344003 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     8215 2023-06-15 06:34:03.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:35:22.352003 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static_collector.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:35:22.356003 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      981 2023-06-15 06:34:03.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:35:22.344003 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-15 06:35:22.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1706 2023-06-15 06:35:22.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-15 06:35:22.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-15 06:35:22.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-15 06:35:22.000000 flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.1.7/.gitignore` & `flask-marshmallow-openapi-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/LICENSE` & `flask-marshmallow-openapi-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/MANIFEST.in` & `flask-marshmallow-openapi-0.1.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/PKG-INFO` & `flask-marshmallow-openapi-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.7
+Version: 0.1.8
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.7/README.md` & `flask-marshmallow-openapi-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/pyproject.toml` & `flask-marshmallow-openapi-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.1.7"
+version = "0.1.8"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/decorators.py` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/models.py` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/models.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,17 @@
   <title>{{ api_name }} ReDoc</title>
   <!-- needed for adaptive design -->
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1" />
   <meta http-equiv="Cache-Control" content="no-store" />
   <link href="https://fonts.googleapis.com/css?family=Montserrat:300,400,700|Roboto:300,400,700" rel="stylesheet" />
 
+  <link rel="icon" type="image/png" href="{{ url_for('openapi.static', filename='redoc_favicon.png') }}"
+    sizes="200x200" />
+
   <!-- ReDoc doesn't change outer page styles -->
   <style>
     body {
       margin: 0;
       padding: 0;
     }
   </style>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 
 
 
 
 
+
```

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.7
+Version: 0.1.8
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.7/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.1.8/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/flask_marshmallow_openapi/static_collector.py
 src/flask_marshmallow_openapi.egg-info/PKG-INFO
 src/flask_marshmallow_openapi.egg-info/SOURCES.txt
 src/flask_marshmallow_openapi.egg-info/dependency_links.txt
 src/flask_marshmallow_openapi.egg-info/not-zip-safe
 src/flask_marshmallow_openapi.egg-info/requires.txt
 src/flask_marshmallow_openapi.egg-info/top_level.txt
+src/flask_marshmallow_openapi/static/redoc_favicon.png
 src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
 src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
 src/flask_marshmallow_openapi/static/swagger_ui/index.css
 src/flask_marshmallow_openapi/static/swagger_ui/index.html
 src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
 src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
 src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
```

