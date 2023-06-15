# Comparing `tmp/django-tracking-fields-1.3.7.tar.gz` & `tmp/django-tracking-fields-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tracking-fields-1.3.7.tar", last modified: Thu Apr  7 08:52:19 2022, max compression
+gzip compressed data, was "django-tracking-fields-1.4.0.tar", last modified: Thu Jun 15 13:09:24 2023, max compression
```

## Comparing `django-tracking-fields-1.3.7.tar` & `django-tracking-fields-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      227 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/MANIFEST.in
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       38 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/setup.cfg
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1744 2022-04-07 08:51:54.000000 django-tracking-fields-1.3.7/CHANGES.rst
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    15938 2022-04-07 08:47:01.000000 django-tracking-fields-1.3.7/tracking_fields/tracking.py
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/migrations/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/migrations/__init__.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2928 2019-01-23 11:08:08.000000 django-tracking-fields-1.3.7/tracking_fields/migrations/0001_initial.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      442 2021-02-19 10:33:52.000000 django-tracking-fields-1.3.7/tracking_fields/migrations/0002_auto_20160209_0356.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      450 2022-03-09 09:47:31.000000 django-tracking-fields-1.3.7/tracking_fields/migrations/0003_auto_20220309_0347.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     3423 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/tracking_fields/models.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/__init__.py
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/templates/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/templates/tracking_fields/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/templates/tracking_fields/admin/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      384 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/templates/tracking_fields/admin/change_list_event.html
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      366 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/templates/tracking_fields/admin/change_form_object.html
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       21 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/templates/tracking_fields/admin/filter.html
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/locale/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/locale/fr/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2389 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1826 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/locale/fr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/tracking_fields/tests/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1474 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/tracking_fields/tests/models.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2019-01-23 15:34:05.000000 django-tracking-fields-1.3.7/tracking_fields/tests/__init__.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    21579 2022-04-07 08:50:22.000000 django-tracking-fields-1.3.7/tracking_fields/tests/tests.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2259 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/tracking_fields/tests/settings.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      198 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/tracking_fields/tests/urls.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      234 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/tracking_fields/tests/admin.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1020 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/tracking_fields/settings.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     4163 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/tracking_fields/decorators.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5109 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/tracking_fields/admin.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       18 2019-01-23 13:58:09.000000 django-tracking-fields-1.3.7/requirements.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      206 2022-04-07 08:29:46.000000 django-tracking-fields-1.3.7/dev-requirements.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    35146 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/LICENSE
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2315 2021-02-19 10:30:11.000000 django-tracking-fields-1.3.7/README.rst
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/doc/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/doc/TODO
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    30280 2019-01-23 11:04:42.000000 django-tracking-fields-1.3.7/doc/activated_mixin_listing.png
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/django_tracking_fields.egg-info/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       16 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/django_tracking_fields.egg-info/top_level.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/django_tracking_fields.egg-info/dependency_links.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1160 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/django_tracking_fields.egg-info/SOURCES.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     6391 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/django_tracking_fields.egg-info/PKG-INFO
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1379 2022-04-07 08:52:00.000000 django-tracking-fields-1.3.7/setup.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     6391 2022-04-07 08:52:19.000000 django-tracking-fields-1.3.7/PKG-INFO
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1943 2023-06-15 13:08:44.000000 django-tracking-fields-1.4.0/CHANGES.rst
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    35146 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/LICENSE
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      227 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/MANIFEST.in
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5093 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/PKG-INFO
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2315 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/README.rst
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      206 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/dev-requirements.txt
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.663663 django-tracking-fields-1.4.0/django_tracking_fields.egg-info/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5093 2023-06-15 13:09:24.000000 django-tracking-fields-1.4.0/django_tracking_fields.egg-info/PKG-INFO
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1160 2023-06-15 13:09:24.000000 django-tracking-fields-1.4.0/django_tracking_fields.egg-info/SOURCES.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2023-06-15 13:09:24.000000 django-tracking-fields-1.4.0/django_tracking_fields.egg-info/dependency_links.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       16 2023-06-15 13:09:24.000000 django-tracking-fields-1.4.0/django_tracking_fields.egg-info/top_level.txt
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.663663 django-tracking-fields-1.4.0/doc/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/doc/TODO
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    30280 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/doc/activated_mixin_listing.png
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       18 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/requirements.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       38 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/setup.cfg
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1379 2023-06-15 13:08:44.000000 django-tracking-fields-1.4.0/setup.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/tracking_fields/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/__init__.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5131 2023-06-15 13:05:33.000000 django-tracking-fields-1.4.0/tracking_fields/admin.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     4163 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/decorators.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.663663 django-tracking-fields-1.4.0/tracking_fields/locale/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.663663 django-tracking-fields-1.4.0/tracking_fields/locale/fr/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/tracking_fields/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1826 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2389 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/tracking_fields/migrations/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2928 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/migrations/0001_initial.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      442 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/migrations/0002_auto_20160209_0356.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      450 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/migrations/0003_auto_20220309_0347.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/migrations/__init__.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     3423 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/models.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1020 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/settings.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.663663 django-tracking-fields-1.4.0/tracking_fields/templates/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.663663 django-tracking-fields-1.4.0/tracking_fields/templates/tracking_fields/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/tracking_fields/templates/tracking_fields/admin/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      366 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/templates/tracking_fields/admin/change_form_object.html
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      384 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/templates/tracking_fields/admin/change_list_event.html
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       21 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/templates/tracking_fields/admin/filter.html
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-06-15 13:09:24.667663 django-tracking-fields-1.4.0/tracking_fields/tests/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/tests/__init__.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      234 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/tests/admin.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1474 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/tests/models.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2259 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/tests/settings.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    21579 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/tests/tests.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      198 2022-05-25 08:35:48.000000 django-tracking-fields-1.4.0/tracking_fields/tests/urls.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    16104 2023-06-15 12:15:06.000000 django-tracking-fields-1.4.0/tracking_fields/tracking.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-tracking-fields-1.3.7/CHANGES.rst` & `django-tracking-fields-1.4.0/CHANGES.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
 Changelog
 =========
 
+1.4.0 (2023-06-15)
+------------------
+
+* Drop Django < 3.2 support
+* Add Django 4.2 support
+* Do not store M2M managers on the instance as original values.
+* Fix TrackerEventUserFilter performance.
+
 1.3.7 (2022-04-07)
 ------------------
 
 * Do not tracked deferred related fields.
 
 1.3.6 (2022-03-16)
 ------------------
```

### Comparing `django-tracking-fields-1.3.7/tracking_fields/tracking.py` & `django-tracking-fields-1.4.0/tracking_fields/tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,18 @@
     """
     original_fields = {}
 
     def _set_original_field(instance, field):
         if instance.pk is None:
             original_fields[field] = None
         else:
-            if isinstance(instance._meta.get_field(field), ForeignKey):
+            if isinstance(instance._meta.get_field(field), ManyToManyField):
+                # Do not store M2M manager as we won't use them
+                return
+            elif isinstance(instance._meta.get_field(field), ForeignKey):
                 # Do not store deferred fields
                 field_id = f"{field}_id"
                 if field_id not in instance.get_deferred_fields():
                     # Only get the PK, we don't want to get the object
                     # (which would make an additional request)
                     original_fields[field] = getattr(instance, field_id)
             else:
```

### Comparing `django-tracking-fields-1.3.7/tracking_fields/migrations/0001_initial.py` & `django-tracking-fields-1.4.0/tracking_fields/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/models.py` & `django-tracking-fields-1.4.0/tracking_fields/models.py`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/locale/fr/LC_MESSAGES/django.po` & `django-tracking-fields-1.4.0/tracking_fields/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/locale/fr/LC_MESSAGES/django.mo` & `django-tracking-fields-1.4.0/tracking_fields/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/tests/models.py` & `django-tracking-fields-1.4.0/tracking_fields/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/tests/tests.py` & `django-tracking-fields-1.4.0/tracking_fields/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/tests/settings.py` & `django-tracking-fields-1.4.0/tracking_fields/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/settings.py` & `django-tracking-fields-1.4.0/tracking_fields/settings.py`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/decorators.py` & `django-tracking-fields-1.4.0/tracking_fields/decorators.py`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/tracking_fields/admin.py` & `django-tracking-fields-1.4.0/tracking_fields/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     parameter_name = "user"
 
     def lookups(self, request, model_admin):
         qs = model_admin.get_queryset(request)
         users = qs.values(
             "user_content_type",
             "user_id",
-        )
+        ).order_by().distinct()
         lookups = {}
         for user in users:
             if user["user_content_type"] is None:
                 continue
             value = "{0}:{1}".format(user["user_content_type"], user["user_id"])
             try:
                 user_obj = ContentType.objects.get_for_id(
```

### Comparing `django-tracking-fields-1.3.7/LICENSE` & `django-tracking-fields-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/README.rst` & `django-tracking-fields-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/doc/activated_mixin_listing.png` & `django-tracking-fields-1.4.0/doc/activated_mixin_listing.png`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/django_tracking_fields.egg-info/SOURCES.txt` & `django-tracking-fields-1.4.0/django_tracking_fields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tracking-fields-1.3.7/setup.py` & `django-tracking-fields-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                        encoding='utf-8').read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-tracking-fields',
-    version='1.3.7',
+    version='1.4.0',
     packages=find_packages(),
     include_package_data=True,
     license='GPLv3+',
     description=(
         'A Django app allowing the tracking of objects field '
         'in the admin site.'
     ),
```

