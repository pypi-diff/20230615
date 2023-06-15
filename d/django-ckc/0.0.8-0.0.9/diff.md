# Comparing `tmp/django-ckc-0.0.8.tar.gz` & `tmp/django-ckc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ckc-0.0.8.tar", last modified: Sat Jul 16 20:28:42 2022, max compression
+gzip compressed data, was "django-ckc-0.0.9.tar", last modified: Mon Oct 31 16:44:56 2022, max compression
```

## Comparing `django-ckc-0.0.8.tar` & `django-ckc-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.246687 django-ckc-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-07-16 20:28:31.000000 django-ckc-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-07-16 20:28:42.246687 django-ckc-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4291 2022-07-16 20:28:31.000000 django-ckc-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.242687 django-ckc-0.0.8/ckc/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.242687 django-ckc-0.0.8/ckc/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.242687 django-ckc-0.0.8/ckc/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/management/commands/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-07-16 20:28:31.000000 django-ckc-0.0.8/ckc/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.242687 django-ckc-0.0.8/django_ckc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-07-16 20:28:42.000000 django-ckc-0.0.8/django_ckc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-07-16 20:28:42.000000 django-ckc-0.0.8/django_ckc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-16 20:28:42.000000 django-ckc-0.0.8/django_ckc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-16 20:28:42.000000 django-ckc-0.0.8/django_ckc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-16 20:28:42.000000 django-ckc-0.0.8/django_ckc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-07-16 20:28:42.246687 django-ckc-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       61 2022-07-16 20:28:31.000000 django-ckc-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.242687 django-ckc-0.0.8/testproject/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      242 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.246687 django-ckc-0.0.8/testproject/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/testapp/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/testapp/misconfigured_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/testapp/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/testapp/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-07-16 20:28:31.000000 django-ckc-0.0.8/testproject/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.246687 django-ckc-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:31.000000 django-ckc-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:42.246687 django-ckc-0.0.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 20:28:31.000000 django-ckc-0.0.8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-07-16 20:28:31.000000 django-ckc-0.0.8/tests/integration/test_default_user_create_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-07-16 20:28:31.000000 django-ckc-0.0.8/tests/integration/test_factories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-07-16 20:28:31.000000 django-ckc-0.0.8/tests/integration/test_primary_key_write_serializer_read_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-07-16 20:28:31.000000 django-ckc-0.0.8/tests/integration/test_soft_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.547857 django-ckc-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-31 16:44:42.000000 django-ckc-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-10-31 16:44:56.547857 django-ckc-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4291 2022-10-31 16:44:42.000000 django-ckc-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.535856 django-ckc-0.0.9/ckc/
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.539856 django-ckc-0.0.9/ckc/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.539856 django-ckc-0.0.9/ckc/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/management/commands/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/providers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-10-31 16:44:42.000000 django-ckc-0.0.9/ckc/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.539856 django-ckc-0.0.9/django_ckc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-10-31 16:44:56.000000 django-ckc-0.0.9/django_ckc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-31 16:44:56.000000 django-ckc-0.0.9/django_ckc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 16:44:56.000000 django-ckc-0.0.9/django_ckc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 16:44:56.000000 django-ckc-0.0.9/django_ckc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-31 16:44:56.000000 django-ckc-0.0.9/django_ckc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-31 16:44:56.547857 django-ckc-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)       61 2022-10-31 16:44:42.000000 django-ckc-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.543856 django-ckc-0.0.9/testproject/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      242 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.543856 django-ckc-0.0.9/testproject/testapp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/testapp/factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/testapp/misconfigured_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/testapp/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/testapp/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-31 16:44:42.000000 django-ckc-0.0.9/testproject/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.543856 django-ckc-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:42.000000 django-ckc-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:56.547857 django-ckc-0.0.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 16:44:42.000000 django-ckc-0.0.9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-10-31 16:44:42.000000 django-ckc-0.0.9/tests/integration/test_default_user_create_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-31 16:44:42.000000 django-ckc-0.0.9/tests/integration/test_factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-10-31 16:44:42.000000 django-ckc-0.0.9/tests/integration/test_json_model_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-10-31 16:44:42.000000 django-ckc-0.0.9/tests/integration/test_primary_key_write_serializer_read_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-10-31 16:44:42.000000 django-ckc-0.0.9/tests/integration/test_soft_delete.py
```

### Comparing `django-ckc-0.0.8/LICENSE` & `django-ckc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/PKG-INFO` & `django-ckc-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: django-ckc
-Version: 0.0.8
+Version: 0.0.9
 Summary: tools, utilities, etc. we use across projects @ ckc
 Home-page: https://github.com/ckcollab/django-ckc
 Author: Eric Carmichael
 Author-email: eric@ckcollab.com
-License: UNKNOWN
 Keywords: django
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
@@ -181,9 +179,7 @@
 
 
 #### `./manage.py` commands
 
 | command | description|
 | :---        |    :----:   |
 | `upload_file <source> <destination>` | uses `django-storages` settings to upload a file |
-
-
```

### Comparing `django-ckc-0.0.8/README.md` & `django-ckc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/ckc/fields.py` & `django-ckc-0.0.9/ckc/fields.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/ckc/logging.py` & `django-ckc-0.0.9/ckc/logging.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/ckc/management/commands/upload_file.py` & `django-ckc-0.0.9/ckc/management/commands/upload_file.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/ckc/providers.py` & `django-ckc-0.0.9/ckc/providers.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,19 @@
             location = factory.Faker('geo_point', country_code='US')
 
         (note, you must call factory.Faker.add_provider(DjangoGeoPointProvider) to add
         this provider!)
         """
 
         def geo_point(self, **kwargs):
-            kwargs['coords_only'] = True
             faker = factory.faker.faker.Faker()
 
-            # local_latlng returns something like:
+            # local_latlng normally returns something like:
             #   ('40.72371', '-73.95097', 'Greenpoint', 'US', 'America/New_York')
-            coords = faker.local_latlng(**kwargs)
-            return Point(x=float(coords[1]), y=float(coords[0]), srid=4326)
+            # with coords_only kwarg, it returns something like:
+            #   ('40.72371', '-73.95097')
+            kwargs.setdefault('coords_only', True)
+            lat, lon, *_ = faker.local_latlng(**kwargs)
+            # Point calls for longitude as x and latitude as y
+            return Point(x=float(lon), y=float(lat), srid=4326)
 except (ImportError, ImproperlyConfigured):
     pass
```

### Comparing `django-ckc-0.0.8/ckc/serializers.py` & `django-ckc-0.0.9/ckc/serializers.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/django_ckc.egg-info/PKG-INFO` & `django-ckc-0.0.9/django_ckc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: django-ckc
-Version: 0.0.8
+Version: 0.0.9
 Summary: tools, utilities, etc. we use across projects @ ckc
 Home-page: https://github.com/ckcollab/django-ckc
 Author: Eric Carmichael
 Author-email: eric@ckcollab.com
-License: UNKNOWN
 Keywords: django
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
@@ -181,9 +179,7 @@
 
 
 #### `./manage.py` commands
 
 | command | description|
 | :---        |    :----:   |
 | `upload_file <source> <destination>` | uses `django-storages` settings to upload a file |
-
-
```

### Comparing `django-ckc-0.0.8/django_ckc.egg-info/SOURCES.txt` & `django-ckc-0.0.9/django_ckc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 testproject/testapp/models.py
 testproject/testapp/serializers.py
 testproject/testapp/viewsets.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/test_default_user_create_mixin.py
 tests/integration/test_factories.py
+tests/integration/test_json_model_snapshots.py
 tests/integration/test_primary_key_write_serializer_read_field.py
 tests/integration/test_soft_delete.py
```

### Comparing `django-ckc-0.0.8/setup.cfg` & `django-ckc-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	tests/functional/*.py
 
 [metadata]
 name = django-ckc
 author = Eric Carmichael
 author_email = eric@ckcollab.com
 description = tools, utilities, etc. we use across projects @ ckc
-version = 0.0.8
+version = 0.0.9
 url = https://github.com/ckcollab/django-ckc
 keywords = 
 	django
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3.6
```

### Comparing `django-ckc-0.0.8/testproject/settings.py` & `django-ckc-0.0.9/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/testproject/testapp/serializers.py` & `django-ckc-0.0.9/testproject/testapp/serializers.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/testproject/testapp/viewsets.py` & `django-ckc-0.0.9/testproject/testapp/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/tests/integration/test_default_user_create_mixin.py` & `django-ckc-0.0.9/tests/integration/test_default_user_create_mixin.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/tests/integration/test_primary_key_write_serializer_read_field.py` & `django-ckc-0.0.9/tests/integration/test_primary_key_write_serializer_read_field.py`

 * *Files identical despite different names*

### Comparing `django-ckc-0.0.8/tests/integration/test_soft_delete.py` & `django-ckc-0.0.9/tests/integration/test_soft_delete.py`

 * *Files identical despite different names*

