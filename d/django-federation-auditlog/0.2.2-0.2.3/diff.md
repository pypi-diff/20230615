# Comparing `tmp/django_federation_auditlog-0.2.2.tar.gz` & `tmp/django_federation_auditlog-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_federation_auditlog-0.2.2.tar", max compression
+gzip compressed data, was "django_federation_auditlog-0.2.3.tar", max compression
```

## Comparing `django_federation_auditlog-0.2.2.tar` & `django_federation_auditlog-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       17 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/__init__.py
--rw-r--r--   0        0        0      799 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/admin.py
--rw-r--r--   0        0        0      127 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/apps.py
--rw-r--r--   0        0        0     5513 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/diff.py
--rw-r--r--   0        0        0     4175 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/middleware.py
--rw-r--r--   0        0        0     3212 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/migrations/__init__.py
--rw-r--r--   0        0        0     2373 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/mixins.py
--rw-r--r--   0        0        0    15062 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/models.py
--rw-r--r--   0        0        0     2084 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/receivers.py
--rw-r--r--   0        0        0     4720 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/registry.py
--rw-r--r--   0        0        0       60 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/tests.py
--rw-r--r--   0        0        0      742 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1432 2023-06-15 20:35:58.385636 django_federation_auditlog-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 20:35:58.385636 django_federation_auditlog-0.2.3/django_federation_auditlog/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/admin.py
+-rw-r--r--   0        0        0      127 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/apps.py
+-rw-r--r--   0        0        0     5513 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/diff.py
+-rw-r--r--   0        0        0     4175 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/middleware.py
+-rw-r--r--   0        0        0     3212 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0     2373 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/mixins.py
+-rw-r--r--   0        0        0    15062 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/models.py
+-rw-r--r--   0        0        0     2084 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/receivers.py
+-rw-r--r--   0        0        0     4720 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/registry.py
+-rw-r--r--   0        0        0       60 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/django_federation_auditlog/tests.py
+-rw-r--r--   0        0        0      742 2023-06-15 20:35:58.389636 django_federation_auditlog-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.3/PKG-INFO
```

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/admin.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/diff.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/middleware.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/migrations/0001_initial.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/mixins.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/mixins.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/models.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/receivers.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/receivers.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/django_federation_auditlog/registry.py` & `django_federation_auditlog-0.2.3/django_federation_auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.2/pyproject.toml` & `django_federation_auditlog-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-federation-auditlog"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Anderson Marques <anderson89marques@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 djangorestframework = "==3.11.1"
```

