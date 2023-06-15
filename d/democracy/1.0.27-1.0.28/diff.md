# Comparing `tmp/democracy-1.0.27.tar.gz` & `tmp/democracy-1.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democracy-1.0.27.tar", last modified: Thu Jun 15 05:54:23 2023, max compression
+gzip compressed data, was "democracy-1.0.28.tar", last modified: Thu Jun 15 06:00:33 2023, max compression
```

## Comparing `democracy-1.0.27.tar` & `democracy-1.0.28.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 05:54:23.914591 democracy-1.0.27/
--rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 05:54:23.914591 democracy-1.0.27/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)    38067 2023-06-15 05:29:06.000000 democracy-1.0.27/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 05:54:23.914591 democracy-1.0.27/democracy.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 05:54:23.000000 democracy-1.0.27/democracy.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-15 05:54:23.000000 democracy-1.0.27/democracy.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 05:54:23.000000 democracy-1.0.27/democracy.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 05:54:23.000000 democracy-1.0.27/democracy.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     5603 2023-06-15 05:53:56.000000 democracy-1.0.27/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-15 05:54:23.914591 democracy-1.0.27/setup.cfg
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:00:33.849590 democracy-1.0.28/
+-rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 06:00:33.849590 democracy-1.0.28/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)    38067 2023-06-15 05:29:06.000000 democracy-1.0.28/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:00:33.849590 democracy-1.0.28/democracy.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        5 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     5609 2023-06-15 06:00:14.000000 democracy-1.0.28/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-15 06:00:33.849590 democracy-1.0.28/setup.cfg
```

### Comparing `democracy-1.0.27/PKG-INFO` & `democracy-1.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.27
+Version: 1.0.28
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `democracy-1.0.27/README.md` & `democracy-1.0.28/README.md`

 * *Files identical despite different names*

### Comparing `democracy-1.0.27/democracy.egg-info/PKG-INFO` & `democracy-1.0.28/democracy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.27
+Version: 1.0.28
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `democracy-1.0.27/pyproject.toml` & `democracy-1.0.28/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "democracy"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.27"  # Required
+version = "1.0.28"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Trying to help with democracy, see https://github.com/gregoryc/democracy"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -124,14 +124,14 @@
 # which executes the function `main` from this package when invoked.
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
-package-data = {"sample" = ["*/*"]}
+package-data = {"democracy" = ["data/*"]}
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

