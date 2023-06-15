# Comparing `tmp/omero-weberror-0.4.1.tar.gz` & `tmp/omero-weberror-0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-weberror-0.4.1.tar", last modified: Thu Jun 15 12:53:28 2023, max compression
+gzip compressed data, was "dist/omero-weberror-0.4.dev1.tar", last modified: Fri Nov 22 12:34:58 2019, max compression
```

## Comparing `omero-weberror-0.4.1.tar` & `omero-weberror-0.4.dev1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:28.351873 omero-weberror-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-15 12:53:28.351873 omero-weberror-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:28.351873 omero-weberror-0.4.1/omero_weberror/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/omero_weberror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/omero_weberror/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:28.347873 omero-weberror-0.4.1/omero_weberror/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:28.351873 omero-weberror-0.4.1/omero_weberror/templates/weberror/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/omero_weberror/templates/weberror/404.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     1124 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/omero_weberror/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/omero_weberror/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:28.351873 omero-weberror-0.4.1/omero_weberror.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-15 12:53:28.000000 omero-weberror-0.4.1/omero_weberror.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-15 12:53:28.000000 omero-weberror-0.4.1/omero_weberror.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:53:28.000000 omero-weberror-0.4.1/omero_weberror.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:53:28.000000 omero-weberror-0.4.1/omero_weberror.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 12:53:28.000000 omero-weberror-0.4.1/omero_weberror.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 12:53:28.000000 omero-weberror-0.4.1/omero_weberror.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 12:53:28.351873 omero-weberror-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-15 12:53:26.000000 omero-weberror-0.4.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2696 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1113 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/omero_weberror/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror/templates/weberror/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/omero_weberror/templates/weberror/404.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      978 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/omero_weberror/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/omero_weberror/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1855 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/omero_weberror/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2696 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      378 2019-11-22 12:34:58.000000 omero-weberror-0.4.dev1/omero_weberror.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34501 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2699 2019-11-22 12:30:15.000000 omero-weberror-0.4.dev1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `omero-weberror-0.4.1/LICENSE` & `omero-weberror-0.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-weberror-0.4.1/omero_weberror/apps.py` & `omero-weberror-0.4.dev1/omero_weberror/apps.py`

 * *Files identical despite different names*

### Comparing `omero-weberror-0.4.1/omero_weberror/templates/weberror/404.html` & `omero-weberror-0.4.dev1/omero_weberror/templates/weberror/404.html`

 * *Files identical despite different names*

### Comparing `omero-weberror-0.4.1/omero_weberror/views.py` & `omero-weberror-0.4.dev1/omero_weberror/views.py`

 * *Files identical despite different names*

### Comparing `omero-weberror-0.4.1/setup.py` & `omero-weberror-0.4.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-VERSION = '0.4.1'
+VERSION = '0.4.dev1'
 
 
 setup(name="omero-weberror",
       packages=find_packages(exclude=['ez_setup']),
       version=VERSION,
       description="A Python plugin for OMERO.web",
       long_description=read('README.rst'),
@@ -44,14 +44,15 @@
           'Development Status :: 5 - Production/Stable',
           'Environment :: Web Environment',
           'Framework :: Django',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Programming Language :: JavaScript',
+          'Programming Language :: Python :: 2',
           'Programming Language :: Python :: 3',
           'Topic :: Internet :: WWW/HTTP',
           'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
           'Topic :: Internet :: WWW/HTTP :: WSGI',
           'Topic :: Software Development :: Libraries :: '
           'Application Frameworks',
           'Topic :: Software Development :: Testing',
@@ -60,12 +61,10 @@
           # http://pypi.python.org/pypi?%3Aaction=list_classifiers
       author='The Open Microscopy Team',
       author_email='ome-devel@lists.openmicroscopy.org.uk',
       license='AGPL-3.0',
       url="https://github.com/ome/omero-weberror",
       download_url='https://github.com/ome/omero-weberror/tarball/%s' % VERSION,  # NOQA
       keywords=['OMERO.web', 'plugin'],
-      install_requires=['omero-web>=5.6.0'],
-      python_requires='>=3',
       include_package_data=True,
       zip_safe=False,
       )
```

