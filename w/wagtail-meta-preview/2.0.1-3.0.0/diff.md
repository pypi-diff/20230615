# Comparing `tmp/wagtail-meta-preview-2.0.1.tar.gz` & `tmp/wagtail-meta-preview-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-meta-preview-2.0.1.tar", last modified: Sun May 21 05:15:53 2023, max compression
+gzip compressed data, was "wagtail-meta-preview-3.0.0.tar", last modified: Thu Jun 15 19:36:56 2023, max compression
```

## Comparing `wagtail-meta-preview-2.0.1.tar` & `wagtail-meta-preview-3.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_panels_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_panels_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_panels_twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/meta_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.746583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_google.html
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-21 05:15:32.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 05:15:53.750583 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 05:15:53.000000 wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.214023 wagtail-meta-preview-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-15 19:36:56.214023 wagtail-meta-preview-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:36:56.214023 wagtail-meta-preview-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.210023 wagtail-meta-preview-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/tests/test_panels_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/tests/test_panels_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/tests/test_panels_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.210023 wagtail-meta-preview-3.0.0/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/meta_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.210023 wagtail-meta-preview-3.0.0/wagtail_meta_preview/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.214023 wagtail-meta-preview-3.0.0/wagtail_meta_preview/static/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.210023 wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.214023 wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_google.html
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-15 19:36:36.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:56.214023 wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-15 19:36:56.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 19:36:56.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:36:56.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:36:56.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 19:36:56.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 19:36:56.000000 wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/top_level.txt
```

### Comparing `wagtail-meta-preview-2.0.1/LICENSE` & `wagtail-meta-preview-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/PKG-INFO` & `wagtail-meta-preview-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: wagtail-meta-preview
-Version: 2.0.1
+Version: 3.0.0
 Summary: Add preview panels for meta data to wagtail
 Home-page: https://github.com/Frojd/wagtail-meta-preview
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Frojd/wagtail-meta-preview/
 Project-URL: Changelog, https://github.com/Frojd/wagtail-meta-preview/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
 Classifier: Framework :: Wagtail :: 5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
 
 # wagtail meta preview
 
 ## Current supported versions
 
-Wagtail Meta Preview >= 2 requires Django 4 and Wagtail 3
+Wagtail Meta Preview requires Wagtail 4.1+
 
 ## Preview
 
 Wagtail Meta Preview provides panels for previewing Facebook sharing, Twitter sharing and Google search results in the Wagtail admin.
 Example of how the Facebook share looks like:
 
 ![example-facebook-preview](https://raw.githubusercontent.com/rinti/wagtail-meta-preview/master/docs/img/facebook-preview-example.PNG)
@@ -54,7 +54,12 @@
 
 The easiest way is to clone this repo, cd into it and just `docker-compose up`, this should
 start a server on http://localhost:8123/admin/ (user: admin, pw: admin) with a couple of page types to test with.
 
 ### Running tests
 
 `docker-compose exec web python runtests.py`
+
+
+## License
+
+Wagtail Meta Preview is released under the [MIT License](http://www.opensource.org/licenses/MIT).
```

### Comparing `wagtail-meta-preview-2.0.1/README.md` & `wagtail-meta-preview-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
 
 # wagtail meta preview
 
 ## Current supported versions
 
-Wagtail Meta Preview >= 2 requires Django 4 and Wagtail 3
+Wagtail Meta Preview requires Wagtail 4.1+
 
 ## Preview
 
 Wagtail Meta Preview provides panels for previewing Facebook sharing, Twitter sharing and Google search results in the Wagtail admin.
 Example of how the Facebook share looks like:
 
 ![example-facebook-preview](https://raw.githubusercontent.com/rinti/wagtail-meta-preview/master/docs/img/facebook-preview-example.PNG)
@@ -26,7 +26,12 @@
 
 The easiest way is to clone this repo, cd into it and just `docker-compose up`, this should
 start a server on http://localhost:8123/admin/ (user: admin, pw: admin) with a couple of page types to test with.
 
 ### Running tests
 
 `docker-compose exec web python runtests.py`
+
+
+## License
+
+Wagtail Meta Preview is released under the [MIT License](http://www.opensource.org/licenses/MIT).
```

### Comparing `wagtail-meta-preview-2.0.1/setup.py` & `wagtail-meta-preview-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,36 +15,36 @@
     version=version,
     description="Add preview panels for meta data to wagtail",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Andreas Bernacca",
     author_email="ante.bernacca@gmail.com",
     url="https://github.com/Frojd/wagtail-meta-preview",
-    install_requires=["wagtail>=3.0"],
+    install_requires=["wagtail>=4.1"],
     extras_require={
         "testing": testing_extras,
     },
     setup_requires=["wheel"],
     zip_safe=False,
     license="MIT License",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     package_data={},
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Framework :: Django",
         "Framework :: Wagtail",
-        "Framework :: Wagtail :: 3",
         "Framework :: Wagtail :: 4",
         "Framework :: Wagtail :: 5",
         "License :: OSI Approved :: MIT License",
     ],
     project_urls={
         "Source": "https://github.com/Frojd/wagtail-meta-preview/",
         "Changelog": "https://github.com/Frojd/wagtail-meta-preview/blob/main/CHANGELOG.md",
```

### Comparing `wagtail-meta-preview-2.0.1/tests/test_admin.py` & `wagtail-meta-preview-3.0.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/tests/test_panels_facebook.py` & `wagtail-meta-preview-3.0.0/tests/test_panels_facebook.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/tests/test_panels_google.py` & `wagtail-meta-preview-3.0.0/tests/test_panels_google.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/tests/test_panels_twitter.py` & `wagtail-meta-preview-3.0.0/tests/test_panels_twitter.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/tests/test_utils.py` & `wagtail-meta-preview-3.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/meta_settings.py` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/meta_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/panels.py` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/panels.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.css`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     overflow: hidden;
     text-overflow: ellipsis;
     font-size: 14px;
     font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
     line-height: 1.3em;
     max-height: 3.9em;
     margin-top: .32333em;
+    color: #262626;
 }
 
 .meta-twitter-preview-link {
     text-transform: lowercase;
     color: #8899A6;
     max-height: 1.3em;
     white-space: nowrap;
@@ -240,14 +241,15 @@
     overflow: hidden;
     text-overflow: ellipsis;
     font-size: 14px;
     font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
     line-height: 1.3em;
     max-height: 3.9em;
     margin-top: .32333em;
+    color: #262626;
 }
 
 .meta-facebook-preview-link {
     text-transform: lowercase;
     color: #8899A6;
     max-height: 1.3em;
     white-space: nowrap;
@@ -320,14 +322,15 @@
     overflow: hidden;
     text-overflow: ellipsis;
     font-size: 1.1em;
     font-family: arial ,sans-serif;
     line-height: 1.3em;
     font-weight: 400;
     margin-top: .32333em;
+    color: #262626;
 }
 
 .meta-google-preview-link {
     text-transform: lowercase;
     color: #000;
     max-height: 1.3em;
     white-space: nowrap;
```

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/static/wagtail_meta_preview/wagtail-meta-preview.js`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_facebook.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/_twitter.html`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/templates/wagtail_meta_preview/preview_panel.html`

 * *Files 24% similar despite different names*

```diff
@@ -12,18 +12,18 @@
         window.google_description_fields = "{{ description_fallback_fields }}";
     {% endif %}
 </script>
 
 <div class="meta-preview{% if is_single %} meta-preview--single{% endif %}">
     {% if not is_single %}
     <fieldset>
-        <legend>{{ self.heading }}</legend>
         <ul class="fields">
             {% for child in self.children %}
-            <li class="{{ child.classes|join:" " }}">{{ child.render_as_field }}</li>
+
+                {% include "wagtailadmin/shared/field_as_li.html" with field=child.bound_field %}
             {% endfor %}
         </ul>
     </fieldset>
     {% endif %}
     {% if is_twitter %}
         {% include "wagtail_meta_preview/_twitter.html" %}
     {% elif is_facebook %}
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
-{% if not is_single %}  {{ self.heading }}
-    * {% for child in self.children %}
-    *  }}">{{ child.render_as_field }}
-{% endfor %}
+{% if not is_single %}
+    * {% for child in self.children %} {% include "wagtailadmin/shared/
+      field_as_li.html" with field=child.bound_field %} {% endfor %}
  {% endif %} {% if is_twitter %} {% include "wagtail_meta_preview/
 _twitter.html" %} {% elif is_facebook %} {% include "wagtail_meta_preview/
 _facebook.html" %} {% else %} {% include "wagtail_meta_preview/_google.html" %}
 {% endif %}
```

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/utils.py` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/views.py` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview/wagtail_hooks.py` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/PKG-INFO` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: wagtail-meta-preview
-Version: 2.0.1
+Version: 3.0.0
 Summary: Add preview panels for meta data to wagtail
 Home-page: https://github.com/Frojd/wagtail-meta-preview
 Author: Andreas Bernacca
 Author-email: ante.bernacca@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Frojd/wagtail-meta-preview/
 Project-URL: Changelog, https://github.com/Frojd/wagtail-meta-preview/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
 Classifier: Framework :: Wagtail :: 5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 ![wagtail-meta-preview](https://github.com/rinti/wagtail-meta-preview/workflows/wagtail-meta-preview/badge.svg)
 [![PyPI version](https://badge.fury.io/py/wagtail-meta-preview.svg)](https://badge.fury.io/py/wagtail-meta-preview)
 
 # wagtail meta preview
 
 ## Current supported versions
 
-Wagtail Meta Preview >= 2 requires Django 4 and Wagtail 3
+Wagtail Meta Preview requires Wagtail 4.1+
 
 ## Preview
 
 Wagtail Meta Preview provides panels for previewing Facebook sharing, Twitter sharing and Google search results in the Wagtail admin.
 Example of how the Facebook share looks like:
 
 ![example-facebook-preview](https://raw.githubusercontent.com/rinti/wagtail-meta-preview/master/docs/img/facebook-preview-example.PNG)
@@ -54,7 +54,12 @@
 
 The easiest way is to clone this repo, cd into it and just `docker-compose up`, this should
 start a server on http://localhost:8123/admin/ (user: admin, pw: admin) with a couple of page types to test with.
 
 ### Running tests
 
 `docker-compose exec web python runtests.py`
+
+
+## License
+
+Wagtail Meta Preview is released under the [MIT License](http://www.opensource.org/licenses/MIT).
```

### Comparing `wagtail-meta-preview-2.0.1/wagtail_meta_preview.egg-info/SOURCES.txt` & `wagtail-meta-preview-3.0.0/wagtail_meta_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

