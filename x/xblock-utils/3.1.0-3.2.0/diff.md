# Comparing `tmp/xblock-utils-3.1.0.tar.gz` & `tmp/xblock-utils-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-utils-3.1.0.tar", last modified: Mon May 29 23:23:17 2023, max compression
+gzip compressed data, was "xblock-utils-3.2.0.tar", last modified: Thu Jun 15 19:15:33 2023, max compression
```

## Comparing `xblock-utils-3.1.0.tar` & `xblock-utils-3.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12387 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.441969 xblock-utils-3.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblock_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7680 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/base_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/public/
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/public/studio_container.js
--rw-r--r--   0 runner    (1001) docker     (122)     7605 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/public/studio_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/publish_event.py
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    22344 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/studio_editable.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/studio_editable_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templates/add_buttons.html
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templates/default_preview_view.html
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templates/studio_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templatetags/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12387 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.028771 xblock-utils-3.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.028771 xblock-utils-3.2.0/xblock_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-15 19:15:33.000000 xblock-utils-3.2.0/xblock_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.028771 xblock-utils-3.2.0/xblockutils/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7680 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/xblockutils/public/
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/public/studio_container.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/public/studio_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/publish_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22344 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/studio_editable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/studio_editable_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/xblockutils/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templates/add_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templates/default_preview_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templates/studio_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/xblockutils/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templatetags/i18n.py
```

### Comparing `xblock-utils-3.1.0/LICENSE` & `xblock-utils-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/PKG-INFO` & `xblock-utils-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xblock-utils
-Version: 3.1.0
+Version: 3.2.0
 Summary: Various utilities for XBlocks
 Home-page: https://github.com/openedx/xblock-utils
 Author: edX
 Author-email: oscm@edx.org
 License: UNKNOWN
 Description: xblock-utils: Various utilities for XBlocks
         ###########################################
```

### Comparing `xblock-utils-3.1.0/README.rst` & `xblock-utils-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/setup.py` & `xblock-utils-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblock_utils.egg-info/PKG-INFO` & `xblock-utils-3.2.0/xblock_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xblock-utils
-Version: 3.1.0
+Version: 3.2.0
 Summary: Various utilities for XBlocks
 Home-page: https://github.com/openedx/xblock-utils
 Author: edX
 Author-email: oscm@edx.org
 License: UNKNOWN
 Description: xblock-utils: Various utilities for XBlocks
         ###########################################
```

### Comparing `xblock-utils-3.1.0/xblock_utils.egg-info/SOURCES.txt` & `xblock-utils-3.2.0/xblock_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/base_test.py` & `xblock-utils-3.2.0/xblockutils/base_test.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/helpers.py` & `xblock-utils-3.2.0/xblockutils/helpers.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/public/studio_container.js` & `xblock-utils-3.2.0/xblockutils/public/studio_container.js`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/public/studio_edit.js` & `xblock-utils-3.2.0/xblockutils/public/studio_edit.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -51,31 +51,32 @@
             $field.val($wrapper.attr('data-default')); // Use attr instead of data to force treating the default value as a string
             $wrapper.removeClass('is-set');
             $resetButton.removeClass('active').addClass('inactive');
         });
         if (type == 'html' && tinyMceAvailable) {
             tinyMCE.baseURL = baseUrl + "/js/vendor/tinymce/js/tinymce";
             $field.tinymce({
-                theme: 'modern',
-                skin: 'studio-tmce4',
+                theme: 'silver',
+                skin: 'studio-tmce5',
+                content_css: 'studio-tmce5',
                 height: '200px',
                 formats: {
                     code: {
                         inline: 'code'
                     }
                 },
                 codemirror: {
                     path: "" + baseUrl + "/js/vendor"
                 },
                 convert_urls: false,
-                plugins: "link codemirror",
+                plugins: "lists, link, codemirror",
                 menubar: false,
                 statusbar: false,
                 toolbar_items_size: 'small',
-                toolbar: "formatselect | styleselect | bold italic underline forecolor wrapAsCode | bullist numlist outdent indent blockquote | link unlink | code",
+                toolbar: "formatselect | styleselect | bold italic underline forecolor | bullist numlist outdent indent blockquote | link unlink | code",
                 resize: "both",
                 extended_valid_elements: 'i[class],span[class]',
                 setup: function(ed) {
                     ed.on('change', fieldChanged);
                 }
             });
         }
```

### Comparing `xblock-utils-3.1.0/xblockutils/publish_event.py` & `xblock-utils-3.2.0/xblockutils/publish_event.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/resources.py` & `xblock-utils-3.2.0/xblockutils/resources.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/settings.py` & `xblock-utils-3.2.0/xblockutils/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/studio_editable.py` & `xblock-utils-3.2.0/xblockutils/studio_editable.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/studio_editable_test.py` & `xblock-utils-3.2.0/xblockutils/studio_editable_test.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/templates/add_buttons.html` & `xblock-utils-3.2.0/xblockutils/templates/add_buttons.html`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/templates/studio_edit.html` & `xblock-utils-3.2.0/xblockutils/templates/studio_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.1.0/xblockutils/templatetags/i18n.py` & `xblock-utils-3.2.0/xblockutils/templatetags/i18n.py`

 * *Files identical despite different names*

