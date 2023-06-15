# Comparing `tmp/afex-audit-trail-0.1.9.tar.gz` & `tmp/afex-audit-trail-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-audit-trail-0.1.9.tar", last modified: Tue Jun  6 11:54:25 2023, max compression
+gzip compressed data, was "afex-audit-trail-0.2.0.tar", last modified: Thu Jun 15 08:56:20 2023, max compression
```

## Comparing `afex-audit-trail-0.1.9.tar` & `afex-audit-trail-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 11:54:25.228233 afex-audit-trail-0.1.9/
--rw-rw-rw-   0        0        0     1062 2023-04-25 08:05:26.000000 afex-audit-trail-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6661 2023-06-06 11:54:25.228233 afex-audit-trail-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-06 11:54:25.212622 afex-audit-trail-0.1.9/afex_audit_trail.egg-info/
--rw-rw-rw-   0        0        0     6661 2023-06-06 11:54:25.000000 afex-audit-trail-0.1.9/afex_audit_trail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-06-06 11:54:25.000000 afex-audit-trail-0.1.9/afex_audit_trail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 11:54:25.000000 afex-audit-trail-0.1.9/afex_audit_trail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-06 11:54:25.000000 afex-audit-trail-0.1.9/afex_audit_trail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 11:54:25.000000 afex-audit-trail-0.1.9/afex_audit_trail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 11:54:25.228233 afex-audit-trail-0.1.9/audit_trails/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.9/audit_trails/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.9/audit_trails/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:54:25.228233 afex-audit-trail-0.1.9/audit_trails/api/
--rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.9/audit_trails/api/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.9/audit_trails/api/serializers.py
--rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.9/audit_trails/api/urls.py
--rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.1.9/audit_trails/api/views.py
--rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.9/audit_trails/apps.py
--rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.9/audit_trails/logger.py
--rw-rw-rw-   0        0        0     3280 2023-04-17 16:19:17.000000 afex-audit-trail-0.1.9/audit_trails/middleware.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:54:25.228233 afex-audit-trail-0.1.9/audit_trails/migrations/
--rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.9/audit_trails/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.9/audit_trails/migrations/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-06-06 08:15:12.000000 afex-audit-trail-0.1.9/audit_trails/models.py
--rw-rw-rw-   0        0        0     1416 2023-06-06 11:17:58.000000 afex-audit-trail-0.1.9/audit_trails/signals.py
--rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.9/audit_trails/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.9/audit_trails/urls.py
--rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.9/audit_trails/views.py
--rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0      987 2023-06-06 11:54:25.228233 afex-audit-trail-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:56:20.241531 afex-audit-trail-0.2.0/
+-rw-rw-rw-   0        0        0     1062 2023-04-25 08:05:26.000000 afex-audit-trail-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6661 2023-06-15 08:56:20.241531 afex-audit-trail-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 08:56:20.210261 afex-audit-trail-0.2.0/afex_audit_trail.egg-info/
+-rw-rw-rw-   0        0        0     6661 2023-06-15 08:56:20.000000 afex-audit-trail-0.2.0/afex_audit_trail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-06-15 08:56:20.000000 afex-audit-trail-0.2.0/afex_audit_trail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:56:20.000000 afex-audit-trail-0.2.0/afex_audit_trail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-15 08:56:20.000000 afex-audit-trail-0.2.0/afex_audit_trail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 08:56:20.000000 afex-audit-trail-0.2.0/afex_audit_trail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:56:20.225907 afex-audit-trail-0.2.0/audit_trails/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.0/audit_trails/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.0/audit_trails/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:56:20.241531 afex-audit-trail-0.2.0/audit_trails/api/
+-rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.2.0/audit_trails/api/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.2.0/audit_trails/api/serializers.py
+-rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.2.0/audit_trails/api/urls.py
+-rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.2.0/audit_trails/api/views.py
+-rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.0/audit_trails/apps.py
+-rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.2.0/audit_trails/logger.py
+-rw-rw-rw-   0        0        0     3280 2023-04-17 16:19:17.000000 afex-audit-trail-0.2.0/audit_trails/middleware.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:56:20.241531 afex-audit-trail-0.2.0/audit_trails/migrations/
+-rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.2.0/audit_trails/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.0/audit_trails/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-15 08:49:06.000000 afex-audit-trail-0.2.0/audit_trails/models.py
+-rw-rw-rw-   0        0        0     1416 2023-06-06 11:17:58.000000 afex-audit-trail-0.2.0/audit_trails/signals.py
+-rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.2.0/audit_trails/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.0/audit_trails/urls.py
+-rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.2.0/audit_trails/views.py
+-rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      987 2023-06-15 08:56:20.241531 afex-audit-trail-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.2.0/setup.py
```

### Comparing `afex-audit-trail-0.1.9/LICENSE` & `afex-audit-trail-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/PKG-INFO` & `afex-audit-trail-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.9/afex_audit_trail.egg-info/PKG-INFO` & `afex-audit-trail-0.2.0/afex_audit_trail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.9/afex_audit_trail.egg-info/SOURCES.txt` & `afex-audit-trail-0.2.0/afex_audit_trail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/api/serializers.py` & `afex-audit-trail-0.2.0/audit_trails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/api/urls.py` & `afex-audit-trail-0.2.0/audit_trails/api/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/api/views.py` & `afex-audit-trail-0.2.0/audit_trails/api/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/logger.py` & `afex-audit-trail-0.2.0/audit_trails/logger.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/middleware.py` & `afex-audit-trail-0.2.0/audit_trails/middleware.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/migrations/0001_initial.py` & `afex-audit-trail-0.2.0/audit_trails/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/models.py` & `afex-audit-trail-0.2.0/audit_trails/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 class Notification(models.Model):
     level = models.CharField(max_length=50, choices=LEVEL_CHOICES)
     recipient = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
         related_name='notifications'
     )
-    actor_object_id = models.CharField(max_length=255)
+    actor_object_id = models.CharField(max_length=255, null=True, blank=True)
     actor_object_type = models.ForeignKey(
         ContentType,
         on_delete=models.SET_NULL,
         null=True,
         blank=True
     )
     actor = GenericForeignKey('actor_object_type', 'actor_object_id')
```

### Comparing `afex-audit-trail-0.1.9/audit_trails/signals.py` & `afex-audit-trail-0.2.0/audit_trails/signals.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/urls.py` & `afex-audit-trail-0.2.0/audit_trails/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/audit_trails/views.py` & `afex-audit-trail-0.2.0/audit_trails/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.9/setup.cfg` & `afex-audit-trail-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6665 782d 6175 6469 742d 7472   = afex-audit-tr
 00000020: 6169 6c0d 0a76 6572 7369 6f6e 203d 2030  ail..version = 0
-00000030: 2e31 2e39 0d0a 6465 7363 7269 7074 696f  .1.9..descriptio
+00000030: 2e32 2e30 0d0a 6465 7363 7269 7074 696f  .2.0..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6372 6561 7465 2073 6572 7665   to create serve
 00000060: 7220 6c6f 6773 2061 6e64 2075 7365 7273  r logs and users
 00000070: 2720 6e6f 7469 6669 6361 7469 6f6e 2e0d  ' notification..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 000000a0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
```

