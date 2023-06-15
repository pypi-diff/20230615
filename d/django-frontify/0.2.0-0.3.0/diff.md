# Comparing `tmp/django-frontify-0.2.0.tar.gz` & `tmp/django-frontify-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-frontify-0.2.0.tar", last modified: Thu Jun 23 10:10:25 2022, max compression
+gzip compressed data, was "django-frontify-0.3.0.tar", last modified: Thu Jun 15 08:06:03 2023, max compression
```

## Comparing `django-frontify-0.2.0.tar` & `django-frontify-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.969803 django-frontify-0.2.0/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)      108 2022-05-23 13:36:03.000000 django-frontify-0.2.0/MANIFEST.in
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     3659 2022-06-23 10:10:25.969803 django-frontify-0.2.0/PKG-INFO
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     2130 2022-06-09 13:45:52.000000 django-frontify-0.2.0/README.rst
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.959803 django-frontify-0.2.0/django_frontify/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)       21 2022-06-17 13:58:42.000000 django-frontify-0.2.0/django_frontify/__init__.py
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.969803 django-frontify-0.2.0/django_frontify/djangocms_frontify/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/djangocms_frontify/__init__.py
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)      468 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/djangocms_frontify/cms_plugins.py
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.969803 django-frontify-0.2.0/django_frontify/djangocms_frontify/migrations/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     1434 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/djangocms_frontify/migrations/0001_initial.py
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/djangocms_frontify/migrations/__init__.py
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     1196 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/djangocms_frontify/models.py
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     8637 2022-06-17 11:00:28.000000 django-frontify-0.2.0/django_frontify/fields.py
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.959803 django-frontify-0.2.0/django_frontify/static/
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.969803 django-frontify-0.2.0/django_frontify/static/django_frontify/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     1664 2022-06-09 16:22:16.000000 django-frontify-0.2.0/django_frontify/static/django_frontify/widget.css
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     4400 2022-06-17 11:13:43.000000 django-frontify-0.2.0/django_frontify/static/django_frontify/widget.js
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.959803 django-frontify-0.2.0/django_frontify/templates/
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.959803 django-frontify-0.2.0/django_frontify/templates/admin/
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.959803 django-frontify-0.2.0/django_frontify/templates/admin/django_frontify/
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.969803 django-frontify-0.2.0/django_frontify/templates/admin/django_frontify/widgets/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     4421 2022-06-09 16:16:21.000000 django-frontify-0.2.0/django_frontify/templates/admin/django_frontify/widgets/admin_file.html
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.959803 django-frontify-0.2.0/django_frontify/templates/django_frontify/
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.969803 django-frontify-0.2.0/django_frontify/templates/django_frontify/plugins/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)       63 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/templates/django_frontify/plugins/image.html
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.969803 django-frontify-0.2.0/django_frontify/templatetags/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/templatetags/__init__.py
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)      606 2022-05-23 13:36:03.000000 django-frontify-0.2.0/django_frontify/templatetags/frontify_tags.py
-drwxr-xr-x   0 raphaelprader  (1000) raphaelprader  (1000)        0 2022-06-23 10:10:25.959803 django-frontify-0.2.0/django_frontify.egg-info/
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     3659 2022-06-23 10:10:25.000000 django-frontify-0.2.0/django_frontify.egg-info/PKG-INFO
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)      860 2022-06-23 10:10:25.000000 django-frontify-0.2.0/django_frontify.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)        1 2022-06-23 10:10:25.000000 django-frontify-0.2.0/django_frontify.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)        1 2022-05-23 13:37:17.000000 django-frontify-0.2.0/django_frontify.egg-info/not-zip-safe
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)       16 2022-06-23 10:10:25.000000 django-frontify-0.2.0/django_frontify.egg-info/top_level.txt
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)       38 2022-06-23 10:10:25.969803 django-frontify-0.2.0/setup.cfg
--rw-r--r--   0 raphaelprader  (1000) raphaelprader  (1000)     1127 2022-05-23 13:36:03.000000 django-frontify-0.2.0/setup.py
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/
+-rw-rw-r--   0 rb        (1000) rb        (1000)      108 2023-05-10 06:49:26.000000 django-frontify-0.3.0/MANIFEST.in
+-rw-rw-r--   0 rb        (1000) rb        (1000)     2827 2023-06-15 08:06:03.185393 django-frontify-0.3.0/PKG-INFO
+-rw-rw-r--   0 rb        (1000) rb        (1000)     2130 2023-06-15 06:41:51.000000 django-frontify-0.3.0/README.rst
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.181393 django-frontify-0.3.0/django_frontify/
+-rw-rw-r--   0 rb        (1000) rb        (1000)       22 2023-06-15 07:56:19.000000 django-frontify-0.3.0/django_frontify/__init__.py
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/django_frontify/djangocms_frontify/
+-rw-rw-r--   0 rb        (1000) rb        (1000)        0 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/djangocms_frontify/__init__.py
+-rw-rw-r--   0 rb        (1000) rb        (1000)      468 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/djangocms_frontify/cms_plugins.py
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/django_frontify/djangocms_frontify/migrations/
+-rw-rw-r--   0 rb        (1000) rb        (1000)     1434 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/djangocms_frontify/migrations/0001_initial.py
+-rw-rw-r--   0 rb        (1000) rb        (1000)        0 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/djangocms_frontify/migrations/__init__.py
+-rw-rw-r--   0 rb        (1000) rb        (1000)     1196 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/djangocms_frontify/models.py
+-rw-rw-r--   0 rb        (1000) rb        (1000)     9044 2023-06-15 07:55:16.000000 django-frontify-0.3.0/django_frontify/fields.py
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.181393 django-frontify-0.3.0/django_frontify/static/
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/django_frontify/static/django_frontify/
+-rw-rw-r--   0 rb        (1000) rb        (1000)     1664 2023-05-10 06:52:45.000000 django-frontify-0.3.0/django_frontify/static/django_frontify/widget.css
+-rw-rw-r--   0 rb        (1000) rb        (1000)     4421 2023-06-15 08:00:33.000000 django-frontify-0.3.0/django_frontify/static/django_frontify/widget.js
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.181393 django-frontify-0.3.0/django_frontify/templates/
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.181393 django-frontify-0.3.0/django_frontify/templates/admin/
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.181393 django-frontify-0.3.0/django_frontify/templates/admin/django_frontify/
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/django_frontify/templates/admin/django_frontify/widgets/
+-rw-rw-r--   0 rb        (1000) rb        (1000)     4421 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/templates/admin/django_frontify/widgets/admin_file.html
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.181393 django-frontify-0.3.0/django_frontify/templates/django_frontify/
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/django_frontify/templates/django_frontify/plugins/
+-rw-rw-r--   0 rb        (1000) rb        (1000)       63 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/templates/django_frontify/plugins/image.html
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/django_frontify/templatetags/
+-rw-rw-r--   0 rb        (1000) rb        (1000)        0 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/templatetags/__init__.py
+-rw-rw-r--   0 rb        (1000) rb        (1000)      606 2023-05-10 06:49:26.000000 django-frontify-0.3.0/django_frontify/templatetags/frontify_tags.py
+drwxrwxr-x   0 rb        (1000) rb        (1000)        0 2023-06-15 08:06:03.185393 django-frontify-0.3.0/django_frontify.egg-info/
+-rw-rw-r--   0 rb        (1000) rb        (1000)     2827 2023-06-15 08:06:03.000000 django-frontify-0.3.0/django_frontify.egg-info/PKG-INFO
+-rw-rw-r--   0 rb        (1000) rb        (1000)      860 2023-06-15 08:06:03.000000 django-frontify-0.3.0/django_frontify.egg-info/SOURCES.txt
+-rw-rw-r--   0 rb        (1000) rb        (1000)        1 2023-06-15 08:06:03.000000 django-frontify-0.3.0/django_frontify.egg-info/dependency_links.txt
+-rw-rw-r--   0 rb        (1000) rb        (1000)        1 2023-05-10 06:50:04.000000 django-frontify-0.3.0/django_frontify.egg-info/not-zip-safe
+-rw-rw-r--   0 rb        (1000) rb        (1000)       16 2023-06-15 08:06:03.000000 django-frontify-0.3.0/django_frontify.egg-info/top_level.txt
+-rw-rw-r--   0 rb        (1000) rb        (1000)       38 2023-06-15 08:06:03.185393 django-frontify-0.3.0/setup.cfg
+-rw-rw-r--   0 rb        (1000) rb        (1000)     1127 2023-05-10 06:49:26.000000 django-frontify-0.3.0/setup.py
```

### Comparing `django-frontify-0.2.0/README.rst` & `django-frontify-0.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 See ``REQUIREMENTS`` in the `setup.py <https://github.com/lab360-ch/django-frontify/blob/master/setup.py>`_
 file for additional dependencies:
 
 Installation
 ------------
 
  * run ``pip install django-frontify``
- * add ``django-frontify`` to your ``INSTALLED_APPS``
+ * add ``django_frontify`` to your ``INSTALLED_APPS``
  * add configuration (as mentioned below) to your settings file
 
 
 Configuration
 -------------
 
 * Set ``DJANGO_FRONTIFY_DOMAIN="<your-frontify-donmain>"`` in your settings.py
```

### Comparing `django-frontify-0.2.0/django_frontify/djangocms_frontify/migrations/0001_initial.py` & `django-frontify-0.3.0/django_frontify/djangocms_frontify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-frontify-0.2.0/django_frontify/djangocms_frontify/models.py` & `django-frontify-0.3.0/django_frontify/djangocms_frontify/models.py`

 * *Files identical despite different names*

### Comparing `django-frontify-0.2.0/django_frontify/fields.py` & `django-frontify-0.3.0/django_frontify/fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,207 @@
 import json
 import urllib
+import logging
 
+from typing import Optional, Literal, Tuple
 from django import forms
 from django.conf import settings
 from django.db import models
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _
 
+logger = logging.getLogger(__name__)
+
 
 class FrontifyImage:
-    SUPPORTED_FORMATS = ["jpg", "jpeg", "png", "webp"]
+    SUPPORTED_FORMATS = [
+        "jpg",
+        "jpeg",
+        "png",
+        "webp",
+    ]
 
     def __init__(self, data):
         data_dict = json.loads(data)
         self.json_data = data
 
         self.name = data_dict.get("name", "")
         self.id = data_dict.get("id", "")
-        self.project = data_dict.get("project", "") # unavailable in v2
+        self.project = data_dict.get("project", "")  # unavailable in v2
         self.creator_name = data_dict.get("creator_name", "")
         self.created = data_dict.get("created", "")
-        self.modifier_name = data_dict.get("modifier_name", "") # unavailable in v2
-        self.modified = data_dict.get("modified", "") # unavailable in v2
+        self.modifier_name = data_dict.get("modifier_name", "")  # unavailable in v2
+        self.modified = data_dict.get("modified", "")  # unavailable in v2
         self.object_type = data_dict.get("object_type", "")
-        self.media_type = data_dict.get("media_type", "") # unavailable in v2
+        self.media_type = data_dict.get("media_type", "")  # unavailable in v2
         self.title = data_dict.get("title", "")
         self.description = data_dict.get("description", "")
         self.ext = data_dict.get("ext", "")
         self.width = data_dict.get("width", "")
         self.height = data_dict.get("height", "")
-        self.filesize = data_dict.get("filesize", "") # seems to differ in v2
-        self.asset_status = data_dict.get("asset_status", "") # unavailable in v2
+        self.filesize = data_dict.get("filesize", "")  # seems to differ in v2
+        self.asset_status = data_dict.get("asset_status", "")  # unavailable in v2
         self.generic_url = data_dict.get("generic_url", "").split("?")[0]
         self.preview_url = data_dict.get("previewUrl", "")
         self.download_url = data_dict.get("download_url", "")
 
-        if 'downloadUrl' in data_dict:
+        if "downloadUrl" in data_dict:
             # New response when using FrontifyFinderV2
             self.ext = data_dict.get("extension", "")
             self.title = data_dict.get("title", "")
             self.name = f"{self.title}.{self.ext}"
-            self.creator_name = data_dict.get("creator", {}).get('name')
+            self.creator_name = data_dict.get("creator", {}).get("name")
             self.created = data_dict.get("createdAt", "")
             self.object_type = data_dict.get("type", "")
-            self.filesize = data_dict.get("size", "") # seems to differ in v2
+            self.filesize = data_dict.get("size", "")  # seems to differ in v2
             self.generic_url = data_dict.get("previewUrl", "").split("?")[0]
             self.download_url = data_dict.get("downloadUrl", "")
 
     @property
     def admin_preview(self):
         return self.thumbnail_url(height=36)
 
     def __str__(self):
         return self.json_data
 
-    def thumbnail_url(self, width=None, height=None, format=None, rect=None, reference_width=None):
+    def thumbnail_url(
+        self,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        format: Optional[str] = None,
+        quality: Optional[int] = None,
+        fp: Optional[Tuple[float, float]] = None,
+        crop: Literal["fp"] = None,
+        fp_zoom: Optional[float] = None,
+        rect=None,
+        reference_width=None,
+    ):
         """
-            width (Integer, px), height (Integer, px): 
-                diese werden verwendet um das bild zu skalieren. Dabei wird kein cropping eingesetzt.
-                Dies bedeuted, dass das Bild so skaliert wird, dass es in dieses Frame passt.
-                Es müssen nicht beide gegeben sein.
-                    Example: https://.../asdkebfuef&width=400
-                    Example: https://.../asdkebfuef&width=400&height=800
-            format (string, jpg, jpeg, png): 
-                Das format des Bildes. Standardmäßig entweder png (für png, tiff, dng, ...), jpg (für jpg)
-                    Example: https://.../asdkebfuef&format=jpg
-                    Example: https://.../asdkebfuef&format=png
-            rect (Array, kommagetrennt Integer[], [offsetX, offsetY, width, height]) & reference_width (Integer):
-                Dieses wird verwendet um ein Bild auf einen Ausschnitt zu beschneiden (cropping).
-                Diese Werte werden relativ zur gegebenen reference_width auf das Original angewendet.
-                Das bedeutet, wenn das Bild im cropper 1000px breit ist, so können OffsetX / Y und Dimensionen
-                übernommen werden und als Referenz 1000px übergeben werden. 
-                Des weiteren wichtig: Wird zusätzlich ein width (or and height) Parameter übergeben,
-                wird anschliessend das beschnittene Resultat zusätzlich skaliert.
-
-            Ausblick: Da der Rect Parameter nicht so intuitiv ist,
-            werden zur Zeit neue Optionen die mit Prozentangaben funktionieren entwickelt.
-            Zusäzlich dazu sind wir an der Implementation des Focal Point cropping.
-            Diese Funktionen sollten ende Q4 Anfang Q1 2021 bereit sein und in der neuen Dokumentation enthalten sein.
+        https://developer.frontify.com/d/XFPCrGNrXQQM/asset-processing-api
         """
+        if rect is not None or reference_width is not None:
+            logging.warn(
+                """\n
+The attributes `rect` and `reference_with` are no longer used.
+Please use `crop=\"fp\"` and `fp=(0.5,0.5)` instead.
+More detailed information can be found here: https://developer.frontify.com/d/XFPCrGNrXQQM/asset-processing-api#/operations/cropping-focal-point
+            \n"""
+            )
         params = []
         if width is not None:
             if isinstance(width, str):
                 width = int(width)
             if not isinstance(width, int):
                 raise ValueError(_("width has to be a int or int as str"))
             params.append(("width", width))
         if height is not None:
             if isinstance(height, str):
                 height = int(height)
             if not isinstance(height, int):
                 raise ValueError(_("height has to be a int or int as str"))
             params.append(("height", height))
-        if reference_width is not None:
-            if isinstance(reference_width, str):
-                reference_width = int(reference_width)
-            if not isinstance(reference_width, int):
-                raise ValueError(
-                    _("reference_width has to be a int or int as str"))
-            params.append(("reference_width", reference_width))
         if format:
             if format not in FrontifyImage.SUPPORTED_FORMATS:
                 raise ValueError(
-                    _(f"{format} is not a allowed format. Allowed formats are {','.join(FrontifyImage.SUPPORTED_FORMATS)}"))
+                    _(
+                        f"{format} is not a allowed format. Allowed formats are {','.join(FrontifyImage.SUPPORTED_FORMATS)}"
+                    )
+                )
             params.append(("format", format))
-        if rect is not None:
-            if isinstance(rect, str):
-                rect = [int(x) for x in rect.split(",")]
-            if not isinstance(rect, list) or len(rect) != 4:
+        if quality is not None:
+            try:
+                quality = int(quality)
+            except ValueError:
+                raise ValueError(
+                    _(
+                        f"quality has to be an int between 0 and 100. `{quality}` is not a valid value"
+                    )
+                )
+            else:
+                if quality > 100 or quality < 0:
+                    raise ValueError(
+                        _(
+                            f"quality has to be an int between 0 and 100. `{quality}` is not a valid value"
+                        )
+                    )
+                params.append(("quality", quality))
+
+        if crop is not None:
+            if crop == "fp":
+                params.append(("crop", crop))
+                if fp is None:
+                    params.append(("fp", "0.5,0.5"))
+                try:
+                    (x, y) = fp
+                except TypeError:
+                    raise ValueError(
+                        "The argument `fp` must be a tuple of two floats between 0.0 and 1.0"
+                    )
+                if x > 1.0 or x < 0.0 or y > 1.0 or y < 0.0:
+                    raise ValueError(
+                        "The argument `fp` must be a tuple of two floats between 0.0 and 1.0"
+                    )
+                params.append(("fp", f"{x},{y}"))
+                if fp_zoom is not None:
+                    try:
+                        fp_zoom = float(fp_zoom)
+                    except ValueError:
+                        raise ValueError(
+                            "The argument `fp_zoom` need to be a float between 1.0 and 3.0"
+                        )
+                    if fp_zoom > 3.0 or fp_zoom < 1.0:
+                        raise ValueError(
+                            "The argument `fp_zoom` need to be a float between 1.0 and 3.0"
+                        )
+                    params.append(("fp_zoom", fp_zoom))
+            else:
                 raise ValueError(
-                    _("rect has to be a list of four values or a string of four comma separated numbers"))
-            params.append(("rect", rect))
+                    _("Only `fp` as value for the crop argument is allowed.")
+                )
 
-        return "{}?{}".format(
-            self.generic_url,
-            urllib.parse.urlencode(params)
-        )
+        return "{}?{}".format(self.generic_url, urllib.parse.urlencode(params))
 
 
 def convert_to_frontify_image_instance(value):
     if isinstance(value, FrontifyImage) or value is None:
         return value
     if not value:
         return None
     return FrontifyImage(value)
 
 
 class AdminFrontifyWidget(forms.Textarea):
-
-
     def render(self, name, value, attrs=None, renderer=None):
         hidden_input = super().render(name, value, attrs=attrs, renderer=renderer)
         instance = convert_to_frontify_image_instance(value)
         context = {
             "instance": instance,
             "hidden_input": hidden_input,
             "domain": settings.DJANGO_FRONTIFY_DOMAIN,
-            "client_id": getattr(settings, 'DJANGO_FRONTIFY_CLIENT_ID', ''),
-            "finder_version": getattr(settings, 'DJANGO_FRONTIFY_FINDER_VERSION', 2),
-            ** attrs
+            "client_id": getattr(settings, "DJANGO_FRONTIFY_CLIENT_ID", ""),
+            "finder_version": getattr(settings, "DJANGO_FRONTIFY_FINDER_VERSION", 2),
+            **attrs,
         }
         html = render_to_string(
-            'admin/django_frontify/widgets/admin_file.html',
-            context
+            "admin/django_frontify/widgets/admin_file.html", context
         )
         return mark_safe(html)
 
     class Media(object):
-        css = {
-            'all': [
-                'django_frontify/widget.css'
-            ]
-        }
-        if getattr(settings, 'DJANGO_FRONTIFY_FINDER_VERSION', 2) == 2:
+        css = {"all": ["django_frontify/widget.css"]}
+        if getattr(settings, "DJANGO_FRONTIFY_FINDER_VERSION", 2) == 2:
             js = (
-                'https://unpkg.com/@frontify/frontify-finder@2.0.1/dist/index.js',
-                'django_frontify/widget.js',
+                "https://unpkg.com/@frontify/frontify-finder@2.0.1/dist/index.js",
+                "django_frontify/widget.js",
             )
         else:
             js = (
-                'https://cdn.frontify.com/finder/frontify-finder-latest.min.js',
-                'django_frontify/widget.js',
+                "https://cdn.frontify.com/finder/frontify-finder-latest.min.js",
+                "django_frontify/widget.js",
             )
 
 
 class AdminFrontifyFormField(forms.CharField):
     widget = AdminFrontifyWidget
 
 
@@ -195,11 +231,9 @@
             return value.json_data
         return value
 
     def from_db_value(self, value, expression, connection):
         return self._parse_string(value)
 
     def formfield(self, **kwargs):
-        kwargs.update({
-            "form_class": AdminFrontifyFormField
-        })
+        kwargs.update({"form_class": AdminFrontifyFormField})
         return super().formfield(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-frontify-0.2.0/django_frontify/static/django_frontify/widget.css` & `django-frontify-0.3.0/django_frontify/static/django_frontify/widget.css`

 * *Files identical despite different names*

### Comparing `django-frontify-0.2.0/django_frontify/static/django_frontify/widget.js` & `django-frontify-0.3.0/django_frontify/static/django_frontify/widget.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -41,68 +41,68 @@
             next: a(0),
             throw: a(1),
             return: a(2)
         }, "function" == typeof Symbol && (i[Symbol.iterator] = function() {
             return this
         }), i;
 
-        function a(i) {
-            return function(a) {
-                return function(i) {
+        function a(a) {
+            return function(c) {
+                return function(a) {
                     if (t) throw new TypeError("Generator is already executing.");
-                    for (; l;) try {
-                        if (t = 1, r && (o = 2 & i[0] ? r.return : i[0] ? r.throw || ((o = r.return) && o.call(r), 0) : r.next) && !(o = o.call(r, i[1])).done) return o;
-                        switch (r = 0, o && (i = [2 & i[0], o.value]), i[0]) {
+                    for (; i && (i = 0, a[0] && (l = 0)), l;) try {
+                        if (t = 1, r && (o = 2 & a[0] ? r.return : a[0] ? r.throw || ((o = r.return) && o.call(r), 0) : r.next) && !(o = o.call(r, a[1])).done) return o;
+                        switch (r = 0, o && (a = [2 & a[0], o.value]), a[0]) {
                             case 0:
                             case 1:
-                                o = i;
+                                o = a;
                                 break;
                             case 4:
                                 return l.label++, {
-                                    value: i[1],
+                                    value: a[1],
                                     done: !1
                                 };
                             case 5:
-                                l.label++, r = i[1], i = [0];
+                                l.label++, r = a[1], a = [0];
                                 continue;
                             case 7:
-                                i = l.ops.pop(), l.trys.pop();
+                                a = l.ops.pop(), l.trys.pop();
                                 continue;
                             default:
-                                if (!((o = (o = l.trys).length > 0 && o[o.length - 1]) || 6 !== i[0] && 2 !== i[0])) {
+                                if (!((o = (o = l.trys).length > 0 && o[o.length - 1]) || 6 !== a[0] && 2 !== a[0])) {
                                     l = 0;
                                     continue
                                 }
-                                if (3 === i[0] && (!o || i[1] > o[0] && i[1] < o[3])) {
-                                    l.label = i[1];
+                                if (3 === a[0] && (!o || a[1] > o[0] && a[1] < o[3])) {
+                                    l.label = a[1];
                                     break
                                 }
-                                if (6 === i[0] && l.label < o[1]) {
-                                    l.label = o[1], o = i;
+                                if (6 === a[0] && l.label < o[1]) {
+                                    l.label = o[1], o = a;
                                     break
                                 }
                                 if (o && l.label < o[2]) {
-                                    l.label = o[2], l.ops.push(i);
+                                    l.label = o[2], l.ops.push(a);
                                     break
                                 }
                                 o[2] && l.ops.pop(), l.trys.pop();
                                 continue
                         }
-                        i = n.call(e, l)
+                        a = n.call(e, l)
                     } catch (e) {
-                        i = [6, e], r = 0
+                        a = [6, e], r = 0
                     } finally {
                         t = o = 0
                     }
-                    if (5 & i[0]) throw i[1];
+                    if (5 & a[0]) throw a[1];
                     return {
-                        value: i[0] ? i[1] : void 0,
+                        value: a[0] ? a[1] : void 0,
                         done: !0
                     }
-                }([i, a])
+                }([a, c])
             }
         }
     }, window.addEventListener("load", (function() {
         for (var t = "frontify-image-field--selected", r = document.querySelectorAll(".frontify-image-field"), o = function(o) {
                 var i = r[o],
                     l = i.getAttribute("data-id"),
                     a = i.getAttribute("data-domain"),
```

### Comparing `django-frontify-0.2.0/django_frontify/templates/admin/django_frontify/widgets/admin_file.html` & `django-frontify-0.3.0/django_frontify/templates/admin/django_frontify/widgets/admin_file.html`

 * *Files identical despite different names*

### Comparing `django-frontify-0.2.0/django_frontify/templatetags/frontify_tags.py` & `django-frontify-0.3.0/django_frontify/templatetags/frontify_tags.py`

 * *Files identical despite different names*

### Comparing `django-frontify-0.2.0/django_frontify.egg-info/SOURCES.txt` & `django-frontify-0.3.0/django_frontify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-frontify-0.2.0/setup.py` & `django-frontify-0.3.0/setup.py`

 * *Files identical despite different names*

