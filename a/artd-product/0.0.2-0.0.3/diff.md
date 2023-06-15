# Comparing `tmp/artd_product-0.0.2.tar.gz` & `tmp/artd-product-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd_product-0.0.2.tar", last modified: Thu Jun 15 05:45:18 2023, max compression
+gzip compressed data, was "artd-product-0.0.3.tar", last modified: Thu Jun 15 13:32:51 2023, max compression
```

## Comparing `artd_product-0.0.2.tar` & `artd-product-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 05:45:10.000000 artd_product-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-15 05:45:18.044328 artd_product-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 05:45:10.000000 artd_product-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/data/taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/management/commands/create_taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-15 05:45:10.000000 artd_product-0.0.2/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:45:18.044328 artd_product-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-15 05:45:16.000000 artd_product-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-15 13:32:47.000000 artd-product-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 13:32:47.000000 artd-product-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 13:32:51.366399 artd-product-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 13:32:47.000000 artd-product-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.362399 artd-product-0.0.3/artd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/data/taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.362399 artd-product-0.0.3/artd_product/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/management/commands/create_taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/migrations/0002_alter_product_special_price_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:32:51.366399 artd-product-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 13:32:49.000000 artd-product-0.0.3/setup.py
```

### Comparing `artd_product-0.0.2/PKG-INFO` & `artd-product-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: artd_product
-Version: 0.0.2
+Name: artd-product
+Version: 0.0.3
 Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 =================
 Products
 =================
 
 A Django app to create products.
```

### Comparing `artd_product-0.0.2/artd_product/migrations/0001_initial.py` & `artd-product-0.0.3/artd_product/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd_product-0.0.2/artd_product.egg-info/PKG-INFO` & `artd-product-0.0.3/artd_product.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-product
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 =================
 Products
 =================
 
 A Django app to create products.
```

### Comparing `artd_product-0.0.2/setup.py` & `artd-product-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
-    name="artd_product",
-    version="0.0.2",
+    name="artd-product",
+    version="0.0.3",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to administrate products",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
-    packages=find_packages(
-        "artd_product",
-        "artd_product.*",
-    ),
+    packages=find_packages(),
     keywords=["pypi", "cicd", "python"],
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
```

