# Comparing `tmp/emi-0.0.8.tar.gz` & `tmp/emi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emi-0.0.8.tar", last modified: Wed Aug 31 03:30:38 2022, max compression
+gzip compressed data, was "emi-0.0.9.tar", last modified: Thu Sep  1 23:12:15 2022, max compression
```

## Comparing `emi-0.0.8.tar` & `emi-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 03:30:38.388301 emi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     8092 2022-08-31 03:30:38.388301 emi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7599 2022-08-31 03:30:24.000000 emi-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 03:30:38.384301 emi-0.0.8/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 03:30:38.384301 emi-0.0.8/pkg/emi/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-31 03:30:26.000000 emi-0.0.8/pkg/emi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-31 03:30:26.000000 emi-0.0.8/pkg/emi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12254 2022-08-31 03:30:26.000000 emi-0.0.8/pkg/emi/emi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 03:30:38.388301 emi-0.0.8/pkg/emi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8092 2022-08-31 03:30:38.000000 emi-0.0.8/pkg/emi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-08-31 03:30:38.000000 emi-0.0.8/pkg/emi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 03:30:38.000000 emi-0.0.8/pkg/emi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-31 03:30:38.000000 emi-0.0.8/pkg/emi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-31 03:30:38.000000 emi-0.0.8/pkg/emi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-31 03:30:38.000000 emi-0.0.8/pkg/emi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-31 03:30:26.000000 emi-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-31 03:30:38.388301 emi-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 23:12:15.169218 emi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-09-01 23:12:15.169218 emi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7505 2022-09-01 23:12:03.000000 emi-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 23:12:15.169218 emi-0.0.9/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 23:12:15.169218 emi-0.0.9/pkg/emi/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-01 23:12:04.000000 emi-0.0.9/pkg/emi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-01 23:12:04.000000 emi-0.0.9/pkg/emi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12231 2022-09-01 23:12:04.000000 emi-0.0.9/pkg/emi/emi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 23:12:15.169218 emi-0.0.9/pkg/emi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-09-01 23:12:15.000000 emi-0.0.9/pkg/emi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-01 23:12:15.000000 emi-0.0.9/pkg/emi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 23:12:15.000000 emi-0.0.9/pkg/emi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-01 23:12:15.000000 emi-0.0.9/pkg/emi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-01 23:12:15.000000 emi-0.0.9/pkg/emi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-01 23:12:15.000000 emi-0.0.9/pkg/emi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-01 23:12:04.000000 emi-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2022-09-01 23:12:15.169218 emi-0.0.9/setup.cfg
```

### Comparing `emi-0.0.8/PKG-INFO` & `emi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: emi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Eons Modular Installer
 Home-page: https://github.com/eons-dev/bin_emi
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_emi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # eons Modular Installer
 
-![build](https://github.com/eons-dev/bin_emi/actions/workflows/python-package.yml/badge.svg)
-
 Use the eons modular installer (EMI) to configure systems.
 
 EMI is a package manager that uses the [eons python library](https://github.com/eons-dev/lib_eons) by executing arbitrary "actions" which are provided by the repository (per eons).  
 The default repository is https://infrastructure.tech.
 
 This means `emi install a_package` will execute the "install" action and provide it with the arguments "a_package".
```

### Comparing `emi-0.0.8/README.md` & `emi-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # eons Modular Installer
 
-![build](https://github.com/eons-dev/bin_emi/actions/workflows/python-package.yml/badge.svg)
-
 Use the eons modular installer (EMI) to configure systems.
 
 EMI is a package manager that uses the [eons python library](https://github.com/eons-dev/lib_eons) by executing arbitrary "actions" which are provided by the repository (per eons).  
 The default repository is https://infrastructure.tech.
 
 This means `emi install a_package` will execute the "install" action and provide it with the arguments "a_package".
```

### Comparing `emi-0.0.8/pkg/emi/emi.py` & `emi-0.0.9/pkg/emi/emi.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,21 +269,21 @@
     # Hook for any post-transaction configuration
     def PostTransaction(this):
         pass
 
 
     # Grab any known and necessary args from kwargs before any Fetch calls are made.
     # Override of eons.UserFunctor method.
-    def ParseInitialArgs(this, **kwargs):
-        super().ParseInitialArgs(**kwargs)
-        setattr(this, 'catalog', kwargs['catalog'])
+    def ParseInitialArgs(this):
+        super().ParseInitialArgs()
+        setattr(this, 'catalog', this.kwargs['catalog'])
 
 
     # Override of eons.Functor method. See that class for details
-    def UserFunction(this, **kwargs):
+    def UserFunction(this):
         logging.info(f"Initiating Transaction {this.name} for {this.tomes}")
 
         this.PreTransaction()
         this.Transaction()
         this.PostTransaction()
```

### Comparing `emi-0.0.8/pkg/emi.egg-info/PKG-INFO` & `emi-0.0.9/pkg/emi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: emi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Eons Modular Installer
 Home-page: https://github.com/eons-dev/bin_emi
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_emi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # eons Modular Installer
 
-![build](https://github.com/eons-dev/bin_emi/actions/workflows/python-package.yml/badge.svg)
-
 Use the eons modular installer (EMI) to configure systems.
 
 EMI is a package manager that uses the [eons python library](https://github.com/eons-dev/lib_eons) by executing arbitrary "actions" which are provided by the repository (per eons).  
 The default repository is https://infrastructure.tech.
 
 This means `emi install a_package` will execute the "install" action and provide it with the arguments "a_package".
```

### Comparing `emi-0.0.8/setup.cfg` & `emi-0.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = emi
-version = v0.0.8
+version = v0.0.9
 author = eons
 author_email = support@eons.llc
 description = Eons Modular Installer
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/bin_emi
@@ -18,24 +18,24 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	wheel
+	pytest
+	jsonpickle
 	eons
+	twine
 	sqlalchemy
-	jsonpickle
-	eot
 	build
-	setuptools
-	pytest
+	eot
+	wheel
 	pip
-	twine
+	setuptools
 
 [options.packages.find]
 where = pkg
 
 [options.entry_points]
 console_scripts = 
 	emi = emi:emi
```

