# Comparing `tmp/filedepot-0.8.0.tar.gz` & `tmp/filedepot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/filedepot-0.8.0.tar", last modified: Mon Jul 27 18:27:15 2020, max compression
+gzip compressed data, was "filedepot-0.9.0.tar", last modified: Sun Dec 11 23:01:53 2022, max compression
```

## Comparing `filedepot-0.8.0.tar` & `filedepot-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 amol      (1000) amol      (1000)        0 2020-07-27 18:27:15.000000 filedepot-0.8.0/
-drwxrwxr-x   0 amol      (1000) amol      (1000)        0 2020-07-27 18:27:15.000000 filedepot-0.8.0/depot/
--rw-r--r--   0 amol      (1000) amol      (1000)        0 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/__init__.py
--rw-r--r--   0 amol      (1000) amol      (1000)     7130 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/middleware.py
--rw-r--r--   0 amol      (1000) amol      (1000)     6155 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/manager.py
--rw-r--r--   0 amol      (1000) amol      (1000)     1523 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/validators.py
--rw-r--r--   0 amol      (1000) amol      (1000)     1229 2019-11-25 17:52:46.000000 filedepot-0.8.0/depot/_compat.py
--rw-rw-r--   0 amol      (1000) amol      (1000)      649 2020-07-27 18:20:46.000000 filedepot-0.8.0/depot/utils.py
-drwxrwxr-x   0 amol      (1000) amol      (1000)        0 2020-07-27 18:27:15.000000 filedepot-0.8.0/depot/fields/
--rw-r--r--   0 amol      (1000) amol      (1000)        0 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/__init__.py
--rw-r--r--   0 amol      (1000) amol      (1000)     5877 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/ming.py
--rw-r--r--   0 amol      (1000) amol      (1000)     2857 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/upload.py
--rw-r--r--   0 amol      (1000) amol      (1000)     8652 2018-12-01 11:20:03.000000 filedepot-0.8.0/depot/fields/sqlalchemy.py
-drwxrwxr-x   0 amol      (1000) amol      (1000)        0 2020-07-27 18:27:15.000000 filedepot-0.8.0/depot/fields/specialized/
--rw-r--r--   0 amol      (1000) amol      (1000)        0 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/specialized/__init__.py
--rw-r--r--   0 amol      (1000) amol      (1000)     2428 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/specialized/image.py
-drwxrwxr-x   0 amol      (1000) amol      (1000)        0 2020-07-27 18:27:15.000000 filedepot-0.8.0/depot/fields/filters/
--rw-r--r--   0 amol      (1000) amol      (1000)        2 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/filters/__init__.py
--rw-r--r--   0 amol      (1000) amol      (1000)     1781 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/filters/thumbnails.py
--rw-r--r--   0 amol      (1000) amol      (1000)     3664 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/fields/interfaces.py
-drwxrwxr-x   0 amol      (1000) amol      (1000)        0 2020-07-27 18:27:15.000000 filedepot-0.8.0/depot/io/
--rw-r--r--   0 amol      (1000) amol      (1000)        2 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/io/__init__.py
--rw-r--r--   0 amol      (1000) amol      (1000)     7985 2019-11-25 17:52:46.000000 filedepot-0.8.0/depot/io/boto3.py
--rw-r--r--   0 amol      (1000) amol      (1000)     4033 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/io/gridfs.py
--rw-r--r--   0 amol      (1000) amol      (1000)     3621 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/io/utils.py
--rw-r--r--   0 amol      (1000) amol      (1000)     5471 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/io/local.py
--rw-r--r--   0 amol      (1000) amol      (1000)     3753 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/io/memory.py
--rw-r--r--   0 amol      (1000) amol      (1000)     7328 2019-11-25 17:52:46.000000 filedepot-0.8.0/depot/io/awss3.py
--rw-r--r--   0 amol      (1000) amol      (1000)     6782 2018-12-01 10:12:21.000000 filedepot-0.8.0/depot/io/interfaces.py
--rw-rw-r--   0 amol      (1000) amol      (1000)       38 2020-07-27 18:27:15.000000 filedepot-0.8.0/setup.cfg
--rw-rw-r--   0 amol      (1000) amol      (1000)     9426 2020-07-27 18:27:15.000000 filedepot-0.8.0/PKG-INFO
--rw-rw-r--   0 amol      (1000) amol      (1000)     6993 2020-07-27 18:22:33.000000 filedepot-0.8.0/README.rst
--rw-rw-r--   0 amol      (1000) amol      (1000)     2020 2020-07-27 18:21:07.000000 filedepot-0.8.0/setup.py
-drwxrwxr-x   0 amol      (1000) amol      (1000)        0 2020-07-27 18:27:15.000000 filedepot-0.8.0/filedepot.egg-info/
--rw-r--r--   0 amol      (1000) amol      (1000)      738 2020-07-27 18:27:15.000000 filedepot-0.8.0/filedepot.egg-info/SOURCES.txt
--rw-r--r--   0 amol      (1000) amol      (1000)        6 2020-07-27 18:27:15.000000 filedepot-0.8.0/filedepot.egg-info/top_level.txt
--rw-r--r--   0 amol      (1000) amol      (1000)        1 2020-07-27 18:27:15.000000 filedepot-0.8.0/filedepot.egg-info/dependency_links.txt
--rw-r--r--   0 amol      (1000) amol      (1000)       94 2020-07-27 18:27:15.000000 filedepot-0.8.0/filedepot.egg-info/requires.txt
--rw-r--r--   0 amol      (1000) amol      (1000)     9426 2020-07-27 18:27:15.000000 filedepot-0.8.0/filedepot.egg-info/PKG-INFO
--rw-r--r--   0 amol      (1000) amol      (1000)        1 2018-12-01 10:22:29.000000 filedepot-0.8.0/filedepot.egg-info/not-zip-safe
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-12-11 23:01:53.273934 filedepot-0.9.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2022-12-11 19:28:50.000000 filedepot-0.9.0/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7724 2022-12-11 23:01:53.273934 filedepot-0.9.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7164 2022-12-11 22:58:04.000000 filedepot-0.9.0/README.rst
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-12-11 23:01:53.265934 filedepot-0.9.0/depot/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1229 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/_compat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-12-11 23:01:53.269934 filedepot-0.9.0/depot/fields/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-12-11 23:01:53.269934 filedepot-0.9.0/depot/fields/filters/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        2 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/filters/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1781 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/filters/thumbnails.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3664 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/interfaces.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5877 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/ming.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-12-11 23:01:53.269934 filedepot-0.9.0/depot/fields/specialized/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/specialized/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2428 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/specialized/image.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8357 2022-12-11 22:52:07.000000 filedepot-0.9.0/depot/fields/sqlalchemy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2857 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/fields/upload.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-12-11 23:01:53.269934 filedepot-0.9.0/depot/io/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        2 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/io/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7328 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/io/awss3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7985 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/io/boto3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4033 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/io/gridfs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6782 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/io/interfaces.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5471 2022-12-11 20:01:07.000000 filedepot-0.9.0/depot/io/local.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3753 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/io/memory.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3621 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/io/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6155 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/manager.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7130 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/middleware.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      669 2022-12-11 22:26:51.000000 filedepot-0.9.0/depot/utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1523 2022-12-11 19:28:50.000000 filedepot-0.9.0/depot/validators.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-12-11 23:01:53.273934 filedepot-0.9.0/filedepot.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7724 2022-12-11 23:01:53.000000 filedepot-0.9.0/filedepot.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      746 2022-12-11 23:01:53.000000 filedepot-0.9.0/filedepot.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-12-11 23:01:53.000000 filedepot-0.9.0/filedepot.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-12-11 19:29:15.000000 filedepot-0.9.0/filedepot.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      103 2022-12-11 23:01:53.000000 filedepot-0.9.0/filedepot.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2022-12-11 23:01:53.000000 filedepot-0.9.0/filedepot.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2022-12-11 23:01:53.273934 filedepot-0.9.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1866 2022-12-11 22:59:28.000000 filedepot-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `filedepot-0.8.0/depot/middleware.py` & `filedepot-0.9.0/depot/middleware.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/manager.py` & `filedepot-0.9.0/depot/manager.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/validators.py` & `filedepot-0.9.0/depot/validators.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/_compat.py` & `filedepot-0.9.0/depot/_compat.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/utils.py` & `filedepot-0.9.0/depot/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ._compat import percent_encode, unicode_text
 
 try:
     from anyascii import anyascii
-except ImportError:
+except ImportError:  # pragma: no cover
     # Python2 doesn't support anyascii
     import unicodedata
     def anyascii(text):
         if not isinstance(text, unicode_text):
             text = text.decode("utf-8")
         return unicodedata.normalize("NFKD", text).encode("ascii", "ignore") or "unknown"
```

### Comparing `filedepot-0.8.0/depot/fields/ming.py` & `filedepot-0.9.0/depot/fields/ming.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/fields/upload.py` & `filedepot-0.9.0/depot/fields/upload.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/fields/sqlalchemy.py` & `filedepot-0.9.0/depot/fields/sqlalchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,44 +150,38 @@
 
                 session._depot_new = getattr(session, '_depot_new', set())
                 session._depot_new.update(added_files)
                 session._depot_old = getattr(session, '_depot_old', set())
                 session._depot_old.update(deleted_files)
 
     @classmethod
-    def _session_after_flush(cls, session, flush_context):
-        # Tracking deleted object _after_ flush
-        # is the way we can track for objects deleted through
-        # a relationship.remove, because those only get
-        # deleted _after_ the session was flushed. Not before.
-        for state in flush_context.states.keys():
-            if not state.deleted:
-                continue
-            obj = state.obj()
-            class_ = obj.__class__
-            tracked_columns = cls.mapped_entities.get(class_, tuple())
-            for col in tracked_columns:
-                value = getattr(obj, col)
-                if value is not None:
-                    session._depot_old = getattr(session, '_depot_old', set())
-                    session._depot_old.update(value.files)
+    def _session_deleted_obj(cls, session, obj):
+        # Tracking indirectly deleted objects
+        # a relationship.remove, or a query().filter().delete()
+        class_ = obj.__class__
+        tracked_columns = cls.mapped_entities.get(class_, tuple())
+        for col in tracked_columns:
+            value = getattr(obj, col)
+            if value is not None:
+                session._depot_old = getattr(session, '_depot_old', set())
+                session._depot_old.update(value.files)
 
     @classmethod
     def _session_attached(cls, session, instance):
         session._depot_new = getattr(session, '_depot_new', set())
         session._depot_new.update(getattr(instance, '_depot_new', set()))
 
     @classmethod
     def setup(cls):
         event.listen(orm.mapper, 'mapper_configured', cls._mapper_configured)
         event.listen(Session, 'after_soft_rollback', cls._session_rollback)
         event.listen(Session, 'after_commit', cls._session_committed)
         event.listen(Session, 'before_attach', cls._session_attached)
         event.listen(Session, 'before_flush', cls._session_flush)
-        event.listen(Session, 'after_flush_postexec', cls._session_after_flush)
+        event.listen(Session, 'persistent_to_deleted', cls._session_deleted_obj)
 
 _SQLAMutationTracker.setup()
 
 try:  # pragma: no cover
     from sprox.sa.widgetselector import SAWidgetSelector
     from tw2.forms import FileField as TW2FileField
     SAWidgetSelector.default_widgets.setdefault(UploadedFileField, TW2FileField)
```

### Comparing `filedepot-0.8.0/depot/fields/specialized/image.py` & `filedepot-0.9.0/depot/fields/specialized/image.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/fields/filters/thumbnails.py` & `filedepot-0.9.0/depot/fields/filters/thumbnails.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/fields/interfaces.py` & `filedepot-0.9.0/depot/fields/interfaces.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/io/boto3.py` & `filedepot-0.9.0/depot/io/boto3.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/io/gridfs.py` & `filedepot-0.9.0/depot/io/gridfs.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/io/utils.py` & `filedepot-0.9.0/depot/io/utils.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/io/local.py` & `filedepot-0.9.0/depot/io/local.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/io/memory.py` & `filedepot-0.9.0/depot/io/memory.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/io/awss3.py` & `filedepot-0.9.0/depot/io/awss3.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/depot/io/interfaces.py` & `filedepot-0.9.0/depot/io/interfaces.py`

 * *Files identical despite different names*

### Comparing `filedepot-0.8.0/README.rst` & `filedepot-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: filedepot
+Version: 0.9.0
+Summary: Toolkit for storing files and attachments in web applications
+Home-page: https://github.com/amol-/depot
+Author: Alessandro Molina
+Author-email: amol@turbogears.org
+License: MIT
+Keywords: storage files s3 gridfs mongodb aws sqlalchemy wsgi
+Classifier: Environment :: Web Environment
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
+Provides-Extra: testing
+License-File: LICENSE
+
 
 .. image:: https://raw.github.com/amol-/depot/master/docs/_static/logo.png
 
 DEPOT - File Storage Made Easy
 ==============================
 
 .. image:: https://travis-ci.org/amol-/depot.png?branch=master 
@@ -93,14 +109,21 @@
 
     # DEPOT is session aware, commit/rollback to keep or delete the stored files.
     DBSession.commit()
 
 ChangeLog
 ---------
 
+0.9.0
+~~~~~
+
+- Support for SQLAlchemy 1.4 and 2.0
+- Support for SQLAlchemy objects deleted with ``.delete(synchronize_session="fetch")``
+- Tests migrated to ``unittest``
+
 0.8.0
 ~~~~~
 
 - Replaced ``unidecode`` dependency with ``anyascii`` to better cope with MIT License.
 
 0.7.1
 ~~~~~
```

### Comparing `filedepot-0.8.0/setup.py` & `filedepot-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os, sys
 
-version = '0.8.0'
+version = '0.9.0'
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
     README = open(os.path.join(here, 'README.rst')).read()
 except IOError:
     README = ''
 
@@ -51,14 +51,11 @@
       url='https://github.com/amol-/depot',
       license='MIT',
       packages=find_packages(exclude=['ez_setup', 'tests']),
       include_package_data=True,
       install_requires=INSTALL_DEPENDENCIES,
       tests_require=TEST_DEPENDENCIES,
       extras_require={
-         # Used by Travis and Coverage due to setup.py nosetests
-         # causing a coredump when used with coverage
          'testing': TEST_DEPENDENCIES,
       },
-      test_suite='nose.collector',
       zip_safe=False,
 )
```

### Comparing `filedepot-0.8.0/filedepot.egg-info/SOURCES.txt` & `filedepot-0.9.0/filedepot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.py
 depot/__init__.py
 depot/_compat.py
 depot/manager.py
 depot/middleware.py
 depot/utils.py
```

