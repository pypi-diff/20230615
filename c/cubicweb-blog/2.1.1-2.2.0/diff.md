# Comparing `tmp/cubicweb-blog-2.1.1.tar.gz` & `tmp/cubicweb-blog-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-blog-2.1.1.tar", last modified: Tue Feb 28 17:22:50 2023, max compression
+gzip compressed data, was "cubicweb-blog-2.2.0.tar", last modified: Thu Jun 15 13:19:26 2023, max compression
```

## Comparing `cubicweb-blog-2.1.1.tar` & `cubicweb-blog-2.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.086679 cubicweb-blog-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2918 2023-02-28 17:22:50.086679 cubicweb-blog-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.070679 cubicweb-blog-2.1.1/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.078679 cubicweb-blog-2.1.1/cubicweb_blog/data/
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/data/cubes.blog.css
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/data/icon_blog.gif
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/data/postdatabg.jpg
--rw-rw-rw-   0 root         (0) root         (0)     7570 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.078679 cubicweb-blog-2.1.1/cubicweb_blog/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     5555 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     4787 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.082679 cubicweb-blog-2.1.1/cubicweb_blog/migration/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/1.2.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/1.4.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/1.5.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/1.7.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/1.7.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/1.7.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/1.9.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     8017 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/sobjects.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.086679 cubicweb-blog-2.1.1/cubicweb_blog/views/
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/views/blog.py
--rw-rw-rw-   0 root         (0) root         (0)     6377 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)    10421 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/views/entry.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/cubicweb_blog/views/urlpublishing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.074679 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2918 2023-02-28 17:22:47.000000 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1224 2023-02-28 17:22:49.000000 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 17:22:47.000000 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 17:22:48.000000 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 17:22:47.000000 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       57 2023-02-28 17:22:49.000000 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-28 17:22:49.000000 cubicweb-blog-2.1.1/cubicweb_blog.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 17:22:50.086679 cubicweb-blog-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2594 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.086679 cubicweb-blog-2.1.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:22:50.086679 cubicweb-blog-2.1.1/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/test/test_blog.py
--rw-rw-rw-   0 root         (0) root         (0)     2754 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/test/unittest_blog.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-02-28 17:22:09.000000 cubicweb-blog-2.1.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.127096 cubicweb-blog-2.2.0/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.131096 cubicweb-blog-2.2.0/cubicweb_blog/data/
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/data/cubes.blog.css
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/data/icon_blog.gif
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/data/postdatabg.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8283 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.131096 cubicweb-blog-2.2.0/cubicweb_blog/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     5555 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)     5795 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.135095 cubicweb-blog-2.2.0/cubicweb_blog/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.4.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.9.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     8017 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.135095 cubicweb-blog-2.2.0/cubicweb_blog/views/
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/blog.py
+-rw-rw-rw-   0 root         (0) root         (0)     6377 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)    10421 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/urlpublishing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.127096 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/test/test_blog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/test/unittest_blog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/tox.ini
```

### Comparing `cubicweb-blog-2.1.1/PKG-INFO` & `cubicweb-blog-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-blog
-Version: 2.1.1
+Version: 2.2.0
 Summary: blogging component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-blog
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -82,9 +81,7 @@
   year YYYY through a RSS feed
 
 Documentation
 -------------
 
 Look in the ``doc/`` subdirectory or read
 http://www.cubicweb.org/doc/en/
-
-
```

### Comparing `cubicweb-blog-2.1.1/README.rst` & `cubicweb-blog-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/__pkginfo__.py` & `cubicweb-blog-2.2.0/cubicweb_blog/__pkginfo__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable-msg=W0622
 """cubicweb-blog packaging information"""
 
 modname = "blog"
 distname = "cubicweb-%s" % modname
 
-numversion = (2, 1, 1)
+numversion = (2, 2, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 description = "blogging component for the CubicWeb framework"
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
 mailinglist = "mailto://cubicweb@lists.logilab.org"
 author = "Logilab"
```

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/data/cubes.blog.css` & `cubicweb-blog-2.2.0/cubicweb_blog/data/cubes.blog.css`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/data/postdatabg.jpg` & `cubicweb-blog-2.2.0/cubicweb_blog/data/postdatabg.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/entities.py` & `cubicweb-blog-2.2.0/cubicweb_blog/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,30 +78,42 @@
         yield (uri, RDF.type, SIOCT.BlogPost)
         yield (uri, DCTERMS.title, Literal(self.entity.dc_title()))
         yield (uri, DCTERMS.date, Literal(self.entity.creation_date))
         yield (uri, DCTERMS.modified, Literal(self.entity.modification_date))
         yield (uri, SIOC.content, Literal(self.entity.content))
         yield (uri, DCTERMS["format"], Literal(self.entity.content_format))
         if self.entity.entry_of:
-            yield (uri, SIOC.container, URIRef(self.entity.entry_of[0].cwuri))
+            blog_uri = URIRef(self.entity.entry_of[0].cwuri)
+            yield (uri, SIOC.container, blog_uri)
+            # we need to add the type specification, even if it is not supposed to be mandatory,
+            # since the RDFLib json-ld serializer force to export as object
+            # (`{ "@id": ...}`)
+            # google parser needs "@type" if defined as an object
+            yield (blog_uri, RDF.type, SIOC.Container)
         if self.entity.creator:
             yield (uri, SIOC.has_owner, URIRef(self.entity.creator.cwuri))
 
     def schema_triples(self):
         RDF = self._use_namespace("rdf")
         SCHEMA = self._use_namespace("schema")
         uri = URIRef(self.uri)
         yield (uri, RDF.type, SCHEMA.BlogPosting)
         yield (uri, SCHEMA.headline, Literal(self.entity.dc_title()))
         yield (uri, SCHEMA.dateCreated, Literal(self.entity.creation_date))
         yield (uri, SCHEMA.dateModified, Literal(self.entity.modification_date))
         yield (uri, SCHEMA.text, Literal(self.entity.content))
         # yield (uri, DCTERMS["format"], Literal(self.entity.content_format))
         if self.entity.entry_of:
-            yield (URIRef(self.entity.entry_of[0].cwuri), SCHEMA.blogPost, uri)
+            blog_uri = URIRef(self.entity.entry_of[0].cwuri)
+            yield (blog_uri, SCHEMA.blogPost, uri)
+            # we need to add the type specification, even if it is not supposed to be mandatory,
+            # since the RDFLib json-ld serializer force to export as object
+            # (`{ "@id": ...}`)
+            # google parser needs "@type" if defined as an object
+            yield (blog_uri, RDF.type, SCHEMA.Blog)
         if self.entity.creator:
             yield (uri, SCHEMA.creator, URIRef(self.entity.creator.cwuri))
 
 
 class MicroBlogRDFAdapter(BlogRDFAdapter):
     __regid__ = "rdf"
     __select__ = is_instance("MicroBlog")
```

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/i18n/en.po` & `cubicweb-blog-2.2.0/cubicweb_blog/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/i18n/es.po` & `cubicweb-blog-2.2.0/cubicweb_blog/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/i18n/fr.po` & `cubicweb-blog-2.2.0/cubicweb_blog/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/migration/1.7.0_Any.py` & `cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/schema.py` & `cubicweb-blog-2.2.0/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/sobjects.py` & `cubicweb-blog-2.2.0/cubicweb_blog/sobjects.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/views/__init__.py` & `cubicweb-blog-2.2.0/cubicweb_blog/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/views/blog.py` & `cubicweb-blog-2.2.0/cubicweb_blog/views/blog.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/views/boxes.py` & `cubicweb-blog-2.2.0/cubicweb_blog/views/boxes.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/views/entry.py` & `cubicweb-blog-2.2.0/cubicweb_blog/views/entry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog/views/urlpublishing.py` & `cubicweb-blog-2.2.0/cubicweb_blog/views/urlpublishing.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog.egg-info/PKG-INFO` & `cubicweb-blog-2.2.0/cubicweb_blog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-blog
-Version: 2.1.1
+Version: 2.2.0
 Summary: blogging component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-blog
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -82,9 +81,7 @@
   year YYYY through a RSS feed
 
 Documentation
 -------------
 
 Look in the ``doc/`` subdirectory or read
 http://www.cubicweb.org/doc/en/
-
-
```

### Comparing `cubicweb-blog-2.1.1/cubicweb_blog.egg-info/SOURCES.txt` & `cubicweb-blog-2.2.0/cubicweb_blog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/setup.py` & `cubicweb-blog-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/test/unittest_blog.py` & `cubicweb-blog-2.2.0/test/unittest_blog.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.1.1/tox.ini` & `cubicweb-blog-2.2.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   check-manifest
 commands =
   {envpython} -m check_manifest
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -64,8 +64,8 @@
 commands = black --check .
 
 [testenv:black-run]
 basepython = python3
 skip_install = true
 deps =
   black >= 22.12
-commands = black .
+commands = black .
```

