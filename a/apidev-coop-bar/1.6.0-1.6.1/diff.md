# Comparing `tmp/apidev-coop_bar-1.6.0.tar.gz` & `tmp/apidev-coop_bar-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidev-coop_bar-1.6.0.tar", last modified: Mon Jun 12 12:54:32 2023, max compression
+gzip compressed data, was "apidev-coop_bar-1.6.1.tar", last modified: Thu Jun 15 07:09:06 2023, max compression
```

## Comparing `apidev-coop_bar-1.6.0.tar` & `apidev-coop_bar-1.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/MANIFEST.in
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/PKG-INFO
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2072 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/README.rst
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/PKG-INFO
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      453 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/SOURCES.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/dependency_links.txt
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:13:33.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/not-zip-safe
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        9 2023-06-12 12:54:32.000000 apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/top_level.txt
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      230 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      178 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/apps.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3869 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/bar.py
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.459626 apidev-coop_bar-1.6.0/coop_bar/static/
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/static/css/
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1998 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/coop_bar/static/css/coop_bar.css
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/templates/
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      372 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/coop_bar/templates/coop_bar.html
-drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/coop_bar/templatetags/
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)       25 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.0/coop_bar/templatetags/__init__.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1926 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/templatetags/coop_bar_tags.py
--rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      103 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/urls.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1079 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/coop_bar/utils.py
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       38 2023-06-12 12:54:32.463626 apidev-coop_bar-1.6.0/setup.cfg
--rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1328 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.0/setup.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      243 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.1/MANIFEST.in
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/PKG-INFO
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)     2072 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.1/README.rst
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/apidev_coop_bar.egg-info/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     2872 2023-06-15 07:09:06.000000 apidev-coop_bar-1.6.1/apidev_coop_bar.egg-info/PKG-INFO
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      453 2023-06-15 07:09:06.000000 apidev-coop_bar-1.6.1/apidev_coop_bar.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-06-15 07:09:06.000000 apidev-coop_bar-1.6.1/apidev_coop_bar.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        1 2023-05-22 10:13:33.000000 apidev-coop_bar-1.6.1/apidev_coop_bar.egg-info/not-zip-safe
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)        9 2023-06-15 07:09:06.000000 apidev-coop_bar-1.6.1/apidev_coop_bar.egg-info/top_level.txt
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/coop_bar/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      230 2023-06-15 07:08:10.000000 apidev-coop_bar-1.6.1/coop_bar/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)      178 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.1/coop_bar/apps.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     3869 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.1/coop_bar/bar.py
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/coop_bar/static/
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/coop_bar/static/css/
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1998 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.1/coop_bar/static/css/coop_bar.css
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/coop_bar/templates/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      372 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.1/coop_bar/templates/coop_bar.html
+drwxrwxr-x   0 lucjean   (1001) lucjean   (1001)        0 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/coop_bar/templatetags/
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)       25 2023-05-22 07:02:21.000000 apidev-coop_bar-1.6.1/coop_bar/templatetags/__init__.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1994 2023-06-13 12:41:28.000000 apidev-coop_bar-1.6.1/coop_bar/templatetags/coop_bar_tags.py
+-rwxrwxr-x   0 lucjean   (1001) lucjean   (1001)      103 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.1/coop_bar/urls.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1079 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.1/coop_bar/utils.py
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)       38 2023-06-15 07:09:06.365624 apidev-coop_bar-1.6.1/setup.cfg
+-rw-rw-r--   0 lucjean   (1001) lucjean   (1001)     1328 2023-06-12 12:49:28.000000 apidev-coop_bar-1.6.1/setup.py
```

### Comparing `apidev-coop_bar-1.6.0/PKG-INFO` & `apidev-coop_bar-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidev-coop_bar
-Version: 1.6.0
+Version: 1.6.1
 Summary: Pluggable admin bar system , works well with coop_cms
 Home-page: https://github.com/ljean/coop-bar/
 Download-URL: https://github.com/ljean/coop-bar/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apidev-coop_bar-1.6.0/README.rst` & `apidev-coop_bar-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `apidev-coop_bar-1.6.0/apidev_coop_bar.egg-info/PKG-INFO` & `apidev-coop_bar-1.6.1/apidev_coop_bar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidev-coop-bar
-Version: 1.6.0
+Version: 1.6.1
 Summary: Pluggable admin bar system , works well with coop_cms
 Home-page: https://github.com/ljean/coop-bar/
 Download-URL: https://github.com/ljean/coop-bar/tarball/master
 Author: Luc Jean
 Author-email: ljean@apidev.fr
 License: BSD
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apidev-coop_bar-1.6.0/coop_bar/bar.py` & `apidev-coop_bar-1.6.1/coop_bar/bar.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_bar-1.6.0/coop_bar/static/css/coop_bar.css` & `apidev-coop_bar-1.6.1/coop_bar/static/css/coop_bar.css`

 * *Files identical despite different names*

### Comparing `apidev-coop_bar-1.6.0/coop_bar/templatetags/coop_bar_tags.py` & `apidev-coop_bar-1.6.1/coop_bar/templatetags/coop_bar_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,20 @@
             if self.option == "auth-only" and not request.user.is_authenticated():
                 return ''
 
         static_url = getattr(settings, 'STATIC_URL', '')
         url = '<link rel="stylesheet" href="{0}css/coop_bar.css?v={1}" type="text/css" />'.format(
             static_url, get_version()
         )
-        headers = [mark_safe(url), mark_safe('<link rel="stylesheet" href="{0}fontawesome/css/all.css" type="text/css" />'.format(static_url))]
+        headers = [
+            mark_safe(url),
+            # mark_safe(
+            #   '<link rel="stylesheet" href="{0}fontawesome/css/all.css" type="text/css" />'.format(static_url)
+            # )
+        ]
         headers += CoopBar().get_headers(request, context_to_dict(context))
         return "\n".join(headers)
 
 
 @register.tag
 def coop_bar_headers(parser, token):
     args = token.split_contents()
```

### Comparing `apidev-coop_bar-1.6.0/coop_bar/utils.py` & `apidev-coop_bar-1.6.1/coop_bar/utils.py`

 * *Files identical despite different names*

### Comparing `apidev-coop_bar-1.6.0/setup.py` & `apidev-coop_bar-1.6.1/setup.py`

 * *Files identical despite different names*

