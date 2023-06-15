# Comparing `tmp/democracy-1.0.28.tar.gz` & `tmp/democracy-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democracy-1.0.28.tar", last modified: Thu Jun 15 06:00:33 2023, max compression
+gzip compressed data, was "democracy-1.0.29.tar", last modified: Thu Jun 15 06:03:07 2023, max compression
```

## Comparing `democracy-1.0.28.tar` & `democracy-1.0.29.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:00:33.849590 democracy-1.0.28/
--rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 06:00:33.849590 democracy-1.0.28/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)    38067 2023-06-15 05:29:06.000000 democracy-1.0.28/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:00:33.849590 democracy-1.0.28/democracy.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)    38830 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        5 2023-06-15 06:00:33.000000 democracy-1.0.28/democracy.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     5609 2023-06-15 06:00:14.000000 democracy-1.0.28/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-15 06:00:33.849590 democracy-1.0.28/setup.cfg
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:03:07.411506 democracy-1.0.29/
+-rw-rw-r--   0 a         (1000) a         (1000)    39090 2023-06-15 06:03:07.411506 democracy-1.0.29/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)    38327 2023-06-15 06:02:45.000000 democracy-1.0.29/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-15 06:03:07.407506 democracy-1.0.29/democracy.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)    39090 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      156 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        5 2023-06-15 06:03:07.000000 democracy-1.0.29/democracy.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     5609 2023-06-15 06:02:03.000000 democracy-1.0.29/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-06-15 06:03:07.411506 democracy-1.0.29/setup.cfg
```

### Comparing `democracy-1.0.28/PKG-INFO` & `democracy-1.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.28
+Version: 1.0.29
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -13,16 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.0
 Description-Content-Type: text/markdown
 
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
-  
-  
+      <iframe width="80%" height="600" src="https://www.youtube.com/embed/Fx9x8cArK30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.
```

### Comparing `democracy-1.0.28/README.md` & `democracy-1.0.29/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
-  
-  
+      <iframe width="80%" height="600" src="https://www.youtube.com/embed/Fx9x8cArK30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.
```

### Comparing `democracy-1.0.28/democracy.egg-info/PKG-INFO` & `democracy-1.0.29/democracy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.28
+Version: 1.0.29
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -13,16 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.0
 Description-Content-Type: text/markdown
 
 <h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life </h1>
-  
-  
+      <iframe width="80%" height="600" src="https://www.youtube.com/embed/Fx9x8cArK30" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
   
   
   
   
   These tools are for everyone  
   
 It doesn't matter what political ideology you favor, these tools are all still very valuable.
```

### Comparing `democracy-1.0.28/pyproject.toml` & `democracy-1.0.29/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "democracy"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.28"  # Required
+version = "1.0.29"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Trying to help with democracy, see https://github.com/gregoryc/democracy"  # Optional
 
 # This is an optional longer description of your project that represents
```

