# Comparing `tmp/django-cleanup-7.0.0.tar.gz` & `tmp/django-cleanup-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cleanup-7.0.0.tar", last modified: Sat Feb 11 16:41:53 2023, max compression
+gzip compressed data, was "django-cleanup-8.0.0.tar", last modified: Wed Jun 14 22:09:38 2023, max compression
```

## Comparing `django-cleanup-7.0.0.tar` & `django-cleanup-8.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-02-11 16:41:53.310661 django-cleanup-7.0.0/
--rw-r--r--   0 MarioRosa   (501) staff       (20)     6066 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/CHANGELOG.md
--rw-r--r--   0 MarioRosa   (501) staff       (20)     1096 2020-06-07 11:56:31.000000 django-cleanup-7.0.0/LICENSE
--rw-r--r--   0 MarioRosa   (501) staff       (20)       56 2020-09-15 20:45:11.000000 django-cleanup-7.0.0/MANIFEST.in
--rw-r--r--   0 MarioRosa   (501) staff       (20)    10601 2023-02-11 16:41:53.310858 django-cleanup-7.0.0/PKG-INFO
--rw-r--r--   0 MarioRosa   (501) staff       (20)     9236 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/README.rst
--rw-r--r--   0 MarioRosa   (501) staff       (20)       67 2023-02-11 16:41:53.311474 django-cleanup-7.0.0/setup.cfg
--rw-r--r--   0 MarioRosa   (501) staff       (20)     2261 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/setup.py
-drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-02-11 16:41:53.303337 django-cleanup-7.0.0/src/
-drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-02-11 16:41:53.307711 django-cleanup-7.0.0/src/django_cleanup/
--rw-r--r--   0 MarioRosa   (501) staff       (20)      237 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/src/django_cleanup/__init__.py
--rw-r--r--   0 MarioRosa   (501) staff       (20)      530 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/src/django_cleanup/apps.py
--rw-r--r--   0 MarioRosa   (501) staff       (20)     5055 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/src/django_cleanup/cache.py
--rw-r--r--   0 MarioRosa   (501) staff       (20)      655 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/src/django_cleanup/cleanup.py
--rw-r--r--   0 MarioRosa   (501) staff       (20)     4714 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/src/django_cleanup/handlers.py
--rw-r--r--   0 MarioRosa   (501) staff       (20)      368 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/src/django_cleanup/signals.py
-drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-02-11 16:41:53.309105 django-cleanup-7.0.0/src/django_cleanup.egg-info/
--rw-r--r--   0 MarioRosa   (501) staff       (20)    10601 2023-02-11 16:41:53.000000 django-cleanup-7.0.0/src/django_cleanup.egg-info/PKG-INFO
--rw-r--r--   0 MarioRosa   (501) staff       (20)      473 2023-02-11 16:41:53.000000 django-cleanup-7.0.0/src/django_cleanup.egg-info/SOURCES.txt
--rw-r--r--   0 MarioRosa   (501) staff       (20)        1 2023-02-11 16:41:53.000000 django-cleanup-7.0.0/src/django_cleanup.egg-info/dependency_links.txt
--rw-r--r--   0 MarioRosa   (501) staff       (20)       15 2023-02-11 16:41:53.000000 django-cleanup-7.0.0/src/django_cleanup.egg-info/top_level.txt
-drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-02-11 16:41:53.310356 django-cleanup-7.0.0/test/
--rw-r--r--   0 MarioRosa   (501) staff       (20)    16909 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/test/test_all.py
--rw-r--r--   0 MarioRosa   (501) staff       (20)     3650 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/test/test_integration.py
--rw-r--r--   0 MarioRosa   (501) staff       (20)      301 2023-02-11 16:39:29.000000 django-cleanup-7.0.0/test/testing_helpers.py
+drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-06-14 22:09:38.437482 django-cleanup-8.0.0/
+-rw-r--r--   0 MarioRosa   (501) staff       (20)     6363 2023-06-14 22:04:05.000000 django-cleanup-8.0.0/CHANGELOG.md
+-rw-r--r--   0 MarioRosa   (501) staff       (20)     1096 2020-06-07 11:56:31.000000 django-cleanup-8.0.0/LICENSE
+-rw-r--r--   0 MarioRosa   (501) staff       (20)       56 2020-09-15 20:45:11.000000 django-cleanup-8.0.0/MANIFEST.in
+-rw-r--r--   0 MarioRosa   (501) staff       (20)    10601 2023-06-14 22:09:38.437699 django-cleanup-8.0.0/PKG-INFO
+-rw-r--r--   0 MarioRosa   (501) staff       (20)     9236 2023-06-14 22:04:05.000000 django-cleanup-8.0.0/README.rst
+-rw-r--r--   0 MarioRosa   (501) staff       (20)       67 2023-06-14 22:09:38.438435 django-cleanup-8.0.0/setup.cfg
+-rw-r--r--   0 MarioRosa   (501) staff       (20)     2261 2023-06-14 22:04:05.000000 django-cleanup-8.0.0/setup.py
+drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-06-14 22:09:38.428912 django-cleanup-8.0.0/src/
+drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-06-14 22:09:38.433899 django-cleanup-8.0.0/src/django_cleanup/
+-rw-r--r--   0 MarioRosa   (501) staff       (20)      237 2023-06-14 22:04:05.000000 django-cleanup-8.0.0/src/django_cleanup/__init__.py
+-rw-r--r--   0 MarioRosa   (501) staff       (20)      530 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/src/django_cleanup/apps.py
+-rw-r--r--   0 MarioRosa   (501) staff       (20)     5055 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/src/django_cleanup/cache.py
+-rw-r--r--   0 MarioRosa   (501) staff       (20)      655 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/src/django_cleanup/cleanup.py
+-rw-r--r--   0 MarioRosa   (501) staff       (20)     4714 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/src/django_cleanup/handlers.py
+-rw-r--r--   0 MarioRosa   (501) staff       (20)      368 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/src/django_cleanup/signals.py
+drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-06-14 22:09:38.435897 django-cleanup-8.0.0/src/django_cleanup.egg-info/
+-rw-r--r--   0 MarioRosa   (501) staff       (20)    10601 2023-06-14 22:09:38.000000 django-cleanup-8.0.0/src/django_cleanup.egg-info/PKG-INFO
+-rw-r--r--   0 MarioRosa   (501) staff       (20)      473 2023-06-14 22:09:38.000000 django-cleanup-8.0.0/src/django_cleanup.egg-info/SOURCES.txt
+-rw-r--r--   0 MarioRosa   (501) staff       (20)        1 2023-06-14 22:09:38.000000 django-cleanup-8.0.0/src/django_cleanup.egg-info/dependency_links.txt
+-rw-r--r--   0 MarioRosa   (501) staff       (20)       15 2023-06-14 22:09:38.000000 django-cleanup-8.0.0/src/django_cleanup.egg-info/top_level.txt
+drwxr-xr-x   0 MarioRosa   (501) staff       (20)        0 2023-06-14 22:09:38.437143 django-cleanup-8.0.0/test/
+-rw-r--r--   0 MarioRosa   (501) staff       (20)    16909 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/test/test_all.py
+-rw-r--r--   0 MarioRosa   (501) staff       (20)     3650 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/test/test_integration.py
+-rw-r--r--   0 MarioRosa   (501) staff       (20)      301 2023-02-11 16:39:29.000000 django-cleanup-8.0.0/test/testing_helpers.py
```

### Comparing `django-cleanup-7.0.0/CHANGELOG.md` & `django-cleanup-8.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [8.0.0] - 2023-06-14
+### Added
+- Run tests for django 4.2. PR [#100] from [@johnthagen](https://github.com/johnthagen).
+
+### Removed
+- Dropped support for django 4.0.
+
 ## [7.0.0] - 2023-02-11
 ### Added
 - Run tests for django 4.1.
 - Run tests on python 3.11 with django 4.1.
 - Select mode, with the ability to only cleanup selected models using a `select` decorator. Resolves issue [#75] for [@daviddavis](https://github.com/daviddavis).
 - Documentation on the known limitations of referencing a file by multiple model instances. Resolves issue [#98] for [@Grosskopf](https://github.com/Grosskopf)
 
@@ -78,15 +85,16 @@
 ## [0.1.8] - 2013-04-07
 ## [0.1.7] - 2013-04-03
 ## [0.1.6] - 2013-02-12
 ## [0.1.5] - 2012-08-17
 ## [0.1.4] - 2012-08-16
 ## [0.1.0] - 2012-08-14
 
-[Unreleased]: https://github.com/un1t/django-cleanup/compare/7.0.0...HEAD
+[Unreleased]: https://github.com/un1t/django-cleanup/compare/8.0.0...HEAD
+[8.0.0]: https://github.com/un1t/django-cleanup/compare/7.0.0...8.0.0
 [7.0.0]: https://github.com/un1t/django-cleanup/compare/6.0.0...7.0.0
 [6.0.0]: https://github.com/un1t/django-cleanup/compare/5.2.0...6.0.0
 [5.2.0]: https://github.com/un1t/django-cleanup/compare/5.1.0...5.2.0
 [5.1.0]: https://github.com/un1t/django-cleanup/compare/5.0.0...5.1.0
 [5.0.0]: https://github.com/un1t/django-cleanup/compare/4.0.1...5.0.0
 [4.0.1]: https://github.com/un1t/django-cleanup/compare/4.0.0...4.0.1
 [4.0.0]: https://github.com/un1t/django-cleanup/compare/3.2.0...4.0.0
@@ -114,14 +122,15 @@
 [0.1.8]: https://github.com/un1t/django-cleanup/compare/0.1.7...0.1.8
 [0.1.7]: https://github.com/un1t/django-cleanup/compare/0.1.6...0.1.7
 [0.1.6]: https://github.com/un1t/django-cleanup/compare/0.1.5...0.1.6
 [0.1.5]: https://github.com/un1t/django-cleanup/compare/0.1.4...0.1.5
 [0.1.4]: https://github.com/un1t/django-cleanup/compare/0.1.0...0.1.4
 [0.1.0]: https://github.com/un1t/django-cleanup/releases/tag/0.1.0
 
+[#100]: https://github.com/un1t/django-cleanup/pull/100
 [#98]: https://github.com/un1t/django-cleanup/issues/98
 [#96]: https://github.com/un1t/django-cleanup/issues/96
 [#89]: https://github.com/un1t/django-cleanup/issues/89
 [#88]: https://github.com/un1t/django-cleanup/pull/88
 [#86]: https://github.com/un1t/django-cleanup/pull/86
 [#81]: https://github.com/un1t/django-cleanup/pull/81
 [#80]: https://github.com/un1t/django-cleanup/pull/80
```

### Comparing `django-cleanup-7.0.0/LICENSE` & `django-cleanup-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cleanup-7.0.0/PKG-INFO` & `django-cleanup-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-cleanup
-Version: 7.0.0
+Version: 8.0.0
 Summary: Deletes old files.
 Home-page: https://github.com/un1t/django-cleanup
 Download-URL: https://github.com/un1t/django-cleanup/tarball/master
 Author: Ilya Shalyapin
 Author-email: ishalyapin@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -42,15 +42,15 @@
 The django-cleanup app automatically deletes files for :code:`FileField`, :code:`ImageField` and
 subclasses. When a :code:`FileField`'s value is changed and the model is saved, the old file is
 deleted. When a model that has a :code:`FileField` is deleted, the file is also deleted. A file that
 is set as the :code:`FileField`'s default value will not be deleted.
 
 Compatibility
 -------------
-- Django 3.2, 4.0, 4.1 (`See Django Supported Versions <https://www.djangoproject.com/download/#supported-versions>`_)
+- Django 3.2, 4.1, 4.2 (`See Django Supported Versions <https://www.djangoproject.com/download/#supported-versions>`_)
 - Python 3.6+
 - Compatible with `sorl-thumbnail <https://github.com/jazzband/sorl-thumbnail>`_
 - Compatible with `easy-thumbnail <https://github.com/SmileyChris/easy-thumbnails>`_
 
 How does it work?
 =================
 In order to track changes of a :code:`FileField` and facilitate file deletions, django-cleanup
@@ -195,17 +195,17 @@
 
 How to run tests
 ================
 Install, setup and use pyenv_ to install all the required versions of cPython
 (see the `tox.ini <https://github.com/un1t/django-cleanup/blob/master/tox.ini>`_).
 
 Setup pyenv_ to have all versions of python activated within your local django-cleanup repository.
-Ensuring that the python 3.10 that was installed is first priority.
+Ensuring that the python 3.11 that was installed is first priority.
 
-Install tox_ on python 3.10 and run the :code:`tox` command from your local django-cleanup
+Install tox_ on python 3.11 and run the :code:`tox` command from your local django-cleanup
 repository.
 
 How to write tests
 ==================
 This app requires the use of django.test.TransactionTestCase_ when writing tests.
 
 For details on why this is required see `here
```

### Comparing `django-cleanup-7.0.0/README.rst` & `django-cleanup-8.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 The django-cleanup app automatically deletes files for :code:`FileField`, :code:`ImageField` and
 subclasses. When a :code:`FileField`'s value is changed and the model is saved, the old file is
 deleted. When a model that has a :code:`FileField` is deleted, the file is also deleted. A file that
 is set as the :code:`FileField`'s default value will not be deleted.
 
 Compatibility
 -------------
-- Django 3.2, 4.0, 4.1 (`See Django Supported Versions <https://www.djangoproject.com/download/#supported-versions>`_)
+- Django 3.2, 4.1, 4.2 (`See Django Supported Versions <https://www.djangoproject.com/download/#supported-versions>`_)
 - Python 3.6+
 - Compatible with `sorl-thumbnail <https://github.com/jazzband/sorl-thumbnail>`_
 - Compatible with `easy-thumbnail <https://github.com/SmileyChris/easy-thumbnails>`_
 
 How does it work?
 =================
 In order to track changes of a :code:`FileField` and facilitate file deletions, django-cleanup
@@ -160,17 +160,17 @@
 
 How to run tests
 ================
 Install, setup and use pyenv_ to install all the required versions of cPython
 (see the `tox.ini <https://github.com/un1t/django-cleanup/blob/master/tox.ini>`_).
 
 Setup pyenv_ to have all versions of python activated within your local django-cleanup repository.
-Ensuring that the python 3.10 that was installed is first priority.
+Ensuring that the python 3.11 that was installed is first priority.
 
-Install tox_ on python 3.10 and run the :code:`tox` command from your local django-cleanup
+Install tox_ on python 3.11 and run the :code:`tox` command from your local django-cleanup
 repository.
 
 How to write tests
 ==================
 This app requires the use of django.test.TransactionTestCase_ when writing tests.
 
 For details on why this is required see `here
```

### Comparing `django-cleanup-7.0.0/setup.py` & `django-cleanup-8.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     license='MIT License',
     keywords='django',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `django-cleanup-7.0.0/src/django_cleanup/apps.py` & `django-cleanup-8.0.0/src/django_cleanup/apps.py`

 * *Files identical despite different names*

### Comparing `django-cleanup-7.0.0/src/django_cleanup/cache.py` & `django-cleanup-8.0.0/src/django_cleanup/cache.py`

 * *Files identical despite different names*

### Comparing `django-cleanup-7.0.0/src/django_cleanup/cleanup.py` & `django-cleanup-8.0.0/src/django_cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `django-cleanup-7.0.0/src/django_cleanup/handlers.py` & `django-cleanup-8.0.0/src/django_cleanup/handlers.py`

 * *Files identical despite different names*

### Comparing `django-cleanup-7.0.0/src/django_cleanup.egg-info/PKG-INFO` & `django-cleanup-8.0.0/src/django_cleanup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-cleanup
-Version: 7.0.0
+Version: 8.0.0
 Summary: Deletes old files.
 Home-page: https://github.com/un1t/django-cleanup
 Download-URL: https://github.com/un1t/django-cleanup/tarball/master
 Author: Ilya Shalyapin
 Author-email: ishalyapin@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -42,15 +42,15 @@
 The django-cleanup app automatically deletes files for :code:`FileField`, :code:`ImageField` and
 subclasses. When a :code:`FileField`'s value is changed and the model is saved, the old file is
 deleted. When a model that has a :code:`FileField` is deleted, the file is also deleted. A file that
 is set as the :code:`FileField`'s default value will not be deleted.
 
 Compatibility
 -------------
-- Django 3.2, 4.0, 4.1 (`See Django Supported Versions <https://www.djangoproject.com/download/#supported-versions>`_)
+- Django 3.2, 4.1, 4.2 (`See Django Supported Versions <https://www.djangoproject.com/download/#supported-versions>`_)
 - Python 3.6+
 - Compatible with `sorl-thumbnail <https://github.com/jazzband/sorl-thumbnail>`_
 - Compatible with `easy-thumbnail <https://github.com/SmileyChris/easy-thumbnails>`_
 
 How does it work?
 =================
 In order to track changes of a :code:`FileField` and facilitate file deletions, django-cleanup
@@ -195,17 +195,17 @@
 
 How to run tests
 ================
 Install, setup and use pyenv_ to install all the required versions of cPython
 (see the `tox.ini <https://github.com/un1t/django-cleanup/blob/master/tox.ini>`_).
 
 Setup pyenv_ to have all versions of python activated within your local django-cleanup repository.
-Ensuring that the python 3.10 that was installed is first priority.
+Ensuring that the python 3.11 that was installed is first priority.
 
-Install tox_ on python 3.10 and run the :code:`tox` command from your local django-cleanup
+Install tox_ on python 3.11 and run the :code:`tox` command from your local django-cleanup
 repository.
 
 How to write tests
 ==================
 This app requires the use of django.test.TransactionTestCase_ when writing tests.
 
 For details on why this is required see `here
```

### Comparing `django-cleanup-7.0.0/test/test_all.py` & `django-cleanup-8.0.0/test/test_all.py`

 * *Files identical despite different names*

### Comparing `django-cleanup-7.0.0/test/test_integration.py` & `django-cleanup-8.0.0/test/test_integration.py`

 * *Files identical despite different names*

