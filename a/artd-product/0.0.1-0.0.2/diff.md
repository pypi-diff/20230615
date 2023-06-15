# Comparing `tmp/artd_product-0.0.1.tar.gz` & `tmp/artd_product-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd_product-0.0.1.tar", last modified: Thu Jun 15 04:19:59 2023, max compression
+gzip compressed data, was "artd_product-0.0.2.tar", last modified: Thu Jun 15 05:45:18 2023, max compression
```

## Comparing `artd_product-0.0.1.tar` & `artd_product-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:59.915942 artd_product-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 04:19:55.000000 artd_product-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-15 04:19:59.915942 artd_product-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 04:19:55.000000 artd_product-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:59.915942 artd_product-0.0.1/artd_product.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-15 04:19:59.000000 artd_product-0.0.1/artd_product.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 04:19:59.000000 artd_product-0.0.1/artd_product.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 04:19:59.000000 artd_product-0.0.1/artd_product.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 04:19:59.000000 artd_product-0.0.1/artd_product.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-06-15 04:19:55.000000 artd_product-0.0.1/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:59.915942 artd_product-0.0.1/product/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:59.915942 artd_product-0.0.1/product/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/data/taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:59.915942 artd_product-0.0.1/product/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:59.915942 artd_product-0.0.1/product/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/management/commands/create_taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:59.915942 artd_product-0.0.1/product/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/migrations/0002_productimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/migrations/0003_alter_rootcategory_options_groupedproduct.py
--rw-r--r--   0 runner    (1001) docker     (123)    16682 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/migrations/0004_alter_productimage_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 04:19:55.000000 artd_product-0.0.1/product/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 04:19:59.915942 artd_product-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-15 04:19:57.000000 artd_product-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 05:45:10.000000 artd_product-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-15 05:45:18.044328 artd_product-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 05:45:10.000000 artd_product-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/data/taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/management/commands/create_taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:10.000000 artd_product-0.0.2/artd_product/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:18.044328 artd_product-0.0.2/artd_product.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:45:18.000000 artd_product-0.0.2/artd_product.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-15 05:45:10.000000 artd_product-0.0.2/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:45:18.044328 artd_product-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-15 05:45:16.000000 artd_product-0.0.2/setup.py
```

### Comparing `artd_product-0.0.1/PKG-INFO` & `artd_product-0.0.2/artd_product.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: artd_product
-Version: 0.0.1
-Summary: A Django app to create Colombian cities
+Name: artd-product
+Version: 0.0.2
+Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
@@ -27,19 +27,19 @@
 
 A Django app to create products.
 
 
 Quick start
 -----------
 
-1. Add "product" to your INSTALLED_APPS setting like this:
+1. Add "artd_product" to your INSTALLED_APPS setting like this:
     
         INSTALLED_APPS = [
             ...
-            'product',
+            'artd_product',
         ]
 
 2. Run ``python manage.py migrate`` to create the polls models.
 
-3. Run ``python manage.py createsuperuser`` to create a superuser.
+3. Run ``python manage.py create_taxes`` to create tax types.
 
 4. Start the development server and visit http://127.0.0.1:8000/admin/
```

### Comparing `artd_product-0.0.1/artd_product.egg-info/PKG-INFO` & `artd_product-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: artd-product
-Version: 0.0.1
-Summary: A Django app to create Colombian cities
+Name: artd_product
+Version: 0.0.2
+Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
@@ -27,19 +27,19 @@
 
 A Django app to create products.
 
 
 Quick start
 -----------
 
-1. Add "product" to your INSTALLED_APPS setting like this:
+1. Add "artd_product" to your INSTALLED_APPS setting like this:
     
         INSTALLED_APPS = [
             ...
-            'product',
+            'artd_product',
         ]
 
 2. Run ``python manage.py migrate`` to create the polls models.
 
-3. Run ``python manage.py createsuperuser`` to create a superuser.
+3. Run ``python manage.py create_taxes`` to create tax types.
 
 4. Start the development server and visit http://127.0.0.1:8000/admin/
```

### Comparing `artd_product-0.0.1/manage.py` & `artd_product-0.0.2/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Django's command-line utility for administrative tasks."""
 import os
 import sys
 
 
 def main():
     """Run administrative tasks."""
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "artd_product.settings")
+    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "artd.settings")
     try:
         from django.core.management import execute_from_command_line
     except ImportError as exc:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
```

### Comparing `artd_product-0.0.1/product/migrations/0004_alter_productimage_options_and_more.py` & `artd_product-0.0.2/artd_product/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,497 +1,593 @@
-# Generated by Django 4.2.2 on 2023-06-15 04:03
+# Generated by Django 4.2.2 on 2023-06-15 05:20
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-    dependencies = [
-        ("product", "0003_alter_rootcategory_options_groupedproduct"),
-    ]
+    initial = True
+
+    dependencies = []
 
     operations = [
-        migrations.AlterModelOptions(
-            name="productimage",
+        migrations.CreateModel(
+            name="Brand",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("status", models.BooleanField(default=True, verbose_name="status")),
+                (
+                    "url_key",
+                    models.CharField(
+                        help_text="Enter the url key of the search engine",
+                        max_length=250,
+                        verbose_name="Url key",
+                    ),
+                ),
+                (
+                    "meta_title",
+                    models.CharField(
+                        help_text="Enter the meta title of the search engine",
+                        max_length=250,
+                        verbose_name="Meta title",
+                    ),
+                ),
+                (
+                    "meta_description",
+                    models.CharField(
+                        help_text="Enter the meta description of the search engine",
+                        max_length=250,
+                        verbose_name="Meta description",
+                    ),
+                ),
+                (
+                    "meta_keywords",
+                    models.CharField(
+                        help_text="Enter the meta keywords of the search engine",
+                        max_length=250,
+                        verbose_name="Meta keywords",
+                    ),
+                ),
+                (
+                    "name",
+                    models.CharField(
+                        help_text="Enter the name of the brand",
+                        max_length=250,
+                        verbose_name="Name",
+                    ),
+                ),
+            ],
             options={
-                "verbose_name": "Product Image",
-                "verbose_name_plural": "Product Images",
+                "verbose_name": "Brand",
+                "verbose_name_plural": "Brands",
+            },
+        ),
+        migrations.CreateModel(
+            name="Category",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("status", models.BooleanField(default=True, verbose_name="status")),
+                (
+                    "url_key",
+                    models.CharField(
+                        help_text="Enter the url key of the search engine",
+                        max_length=250,
+                        verbose_name="Url key",
+                    ),
+                ),
+                (
+                    "meta_title",
+                    models.CharField(
+                        help_text="Enter the meta title of the search engine",
+                        max_length=250,
+                        verbose_name="Meta title",
+                    ),
+                ),
+                (
+                    "meta_description",
+                    models.CharField(
+                        help_text="Enter the meta description of the search engine",
+                        max_length=250,
+                        verbose_name="Meta description",
+                    ),
+                ),
+                (
+                    "meta_keywords",
+                    models.CharField(
+                        help_text="Enter the meta keywords of the search engine",
+                        max_length=250,
+                        verbose_name="Meta keywords",
+                    ),
+                ),
+                (
+                    "name",
+                    models.CharField(
+                        help_text="Enter the name of the category",
+                        max_length=250,
+                        verbose_name="Name",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "Category",
+                "verbose_name_plural": "Categories",
+            },
+        ),
+        migrations.CreateModel(
+            name="Product",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("status", models.BooleanField(default=True, verbose_name="status")),
+                (
+                    "url_key",
+                    models.CharField(
+                        help_text="Enter the url key of the search engine",
+                        max_length=250,
+                        verbose_name="Url key",
+                    ),
+                ),
+                (
+                    "meta_title",
+                    models.CharField(
+                        help_text="Enter the meta title of the search engine",
+                        max_length=250,
+                        verbose_name="Meta title",
+                    ),
+                ),
+                (
+                    "meta_description",
+                    models.CharField(
+                        help_text="Enter the meta description of the search engine",
+                        max_length=250,
+                        verbose_name="Meta description",
+                    ),
+                ),
+                (
+                    "meta_keywords",
+                    models.CharField(
+                        help_text="Enter the meta keywords of the search engine",
+                        max_length=250,
+                        verbose_name="Meta keywords",
+                    ),
+                ),
+                (
+                    "name",
+                    models.CharField(
+                        help_text="Enter the name of the product",
+                        max_length=250,
+                        verbose_name="Name",
+                    ),
+                ),
+                (
+                    "sku",
+                    models.CharField(
+                        help_text="Enter the sku of the product",
+                        max_length=250,
+                        verbose_name="Sku",
+                    ),
+                ),
+                (
+                    "description",
+                    models.TextField(
+                        help_text="Enter the description of the product",
+                        verbose_name="Description",
+                    ),
+                ),
+                (
+                    "short_description",
+                    models.TextField(
+                        help_text="Enter the short description of the product",
+                        verbose_name="Short description",
+                    ),
+                ),
+                (
+                    "price",
+                    models.DecimalField(
+                        decimal_places=2,
+                        help_text="Enter the price of the product",
+                        max_digits=10,
+                        verbose_name="Price",
+                    ),
+                ),
+                (
+                    "special_price",
+                    models.DecimalField(
+                        decimal_places=2,
+                        help_text="Enter the special price of the product",
+                        max_digits=10,
+                        verbose_name="Special price",
+                    ),
+                ),
+                (
+                    "special_price_from",
+                    models.DateTimeField(
+                        help_text="Enter the special price from of the product",
+                        verbose_name="Special price from",
+                    ),
+                ),
+                (
+                    "special_price_to",
+                    models.DateTimeField(
+                        help_text="Enter the special price to of the product",
+                        verbose_name="Special price to",
+                    ),
+                ),
+                (
+                    "stock",
+                    models.IntegerField(
+                        help_text="Enter the stock of the product", verbose_name="Stock"
+                    ),
+                ),
+                (
+                    "weight",
+                    models.DecimalField(
+                        decimal_places=2,
+                        default=0.0,
+                        help_text="Enter the weight of the product",
+                        max_digits=10,
+                        verbose_name="Weight",
+                    ),
+                ),
+                (
+                    "unit_of_measure",
+                    models.CharField(
+                        choices=[
+                            ("kg", "Kilogram"),
+                            ("g", "Gram"),
+                            ("l", "Liter"),
+                            ("ml", "Milliliter"),
+                            ("m", "Meter"),
+                            ("cm", "Centimeter"),
+                            ("mm", "Millimeter"),
+                            ("in", "Inch"),
+                            ("ft", "Foot"),
+                            ("yd", "Yard"),
+                            ("mi", "Mile"),
+                            ("oz", "Ounce"),
+                            ("lb", "Pound"),
+                            ("st", "Stone"),
+                            ("t", "Ton"),
+                            ("gal", "Gallon"),
+                            ("pt", "Pint"),
+                            ("qt", "Quart"),
+                            ("cup", "Cup"),
+                            ("pc", "Piece"),
+                            ("set", "Set"),
+                            ("pair", "Pair"),
+                            ("doz", "Dozen"),
+                            ("box", "Box"),
+                            ("pack", "Pack"),
+                            ("roll", "Roll"),
+                            ("bag", "Bag"),
+                            ("bottle", "Bottle"),
+                            ("tube", "Tube"),
+                            ("can", "Can"),
+                            ("jar", "Jar"),
+                            ("case", "Case"),
+                            ("other", "Other"),
+                        ],
+                        default="kg",
+                        help_text="Select the unit of measure of the product",
+                        max_length=250,
+                        verbose_name="Unit of measure",
+                    ),
+                ),
+                (
+                    "measure",
+                    models.DecimalField(
+                        decimal_places=2,
+                        default=0.0,
+                        help_text="Enter the measure of the product",
+                        max_digits=10,
+                        verbose_name="Measure",
+                    ),
+                ),
+                (
+                    "brand",
+                    models.ForeignKey(
+                        help_text="Select the brand",
+                        on_delete=django.db.models.deletion.CASCADE,
+                        to="artd_product.brand",
+                        verbose_name="brand",
+                    ),
+                ),
+                (
+                    "categories",
+                    models.ManyToManyField(
+                        help_text="Select the category",
+                        to="artd_product.category",
+                        verbose_name="Category",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "Product",
+                "verbose_name_plural": "Products",
             },
         ),
-        migrations.AlterModelOptions(
-            name="rootcategory",
+        migrations.CreateModel(
+            name="RootCategory",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("status", models.BooleanField(default=True, verbose_name="status")),
+                (
+                    "url_key",
+                    models.CharField(
+                        help_text="Enter the url key of the search engine",
+                        max_length=250,
+                        verbose_name="Url key",
+                    ),
+                ),
+                (
+                    "meta_title",
+                    models.CharField(
+                        help_text="Enter the meta title of the search engine",
+                        max_length=250,
+                        verbose_name="Meta title",
+                    ),
+                ),
+                (
+                    "meta_description",
+                    models.CharField(
+                        help_text="Enter the meta description of the search engine",
+                        max_length=250,
+                        verbose_name="Meta description",
+                    ),
+                ),
+                (
+                    "meta_keywords",
+                    models.CharField(
+                        help_text="Enter the meta keywords of the search engine",
+                        max_length=250,
+                        verbose_name="Meta keywords",
+                    ),
+                ),
+                (
+                    "name",
+                    models.CharField(
+                        help_text="Enter the name of the root category",
+                        max_length=250,
+                        verbose_name="Name",
+                    ),
+                ),
+            ],
             options={
                 "verbose_name": "Root Category",
                 "verbose_name_plural": "Root Categories",
             },
         ),
-        migrations.AddField(
-            model_name="product",
-            name="measure",
-            field=models.DecimalField(
-                decimal_places=2,
-                default=0.0,
-                help_text="Enter the measure of the product",
-                max_digits=10,
-                verbose_name="Measure",
-            ),
+        migrations.CreateModel(
+            name="Tax",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("status", models.BooleanField(default=True, verbose_name="status")),
+                (
+                    "name",
+                    models.CharField(
+                        help_text="Enter the name of the tax",
+                        max_length=250,
+                        verbose_name="Name",
+                    ),
+                ),
+                (
+                    "percentage",
+                    models.DecimalField(
+                        decimal_places=2,
+                        help_text="Enter the percentage of the tax",
+                        max_digits=5,
+                        verbose_name="Percentage",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "Tax",
+                "verbose_name_plural": "Taxes",
+            },
         ),
-        migrations.AddField(
-            model_name="product",
-            name="unit_of_measure",
-            field=models.CharField(
-                choices=[
-                    ("kg", "Kilogram"),
-                    ("g", "Gram"),
-                    ("l", "Liter"),
-                    ("ml", "Milliliter"),
-                    ("m", "Meter"),
-                    ("cm", "Centimeter"),
-                    ("mm", "Millimeter"),
-                    ("in", "Inch"),
-                    ("ft", "Foot"),
-                    ("yd", "Yard"),
-                    ("mi", "Mile"),
-                    ("oz", "Ounce"),
-                    ("lb", "Pound"),
-                    ("st", "Stone"),
-                    ("t", "Ton"),
-                    ("gal", "Gallon"),
-                    ("pt", "Pint"),
-                    ("qt", "Quart"),
-                    ("cup", "Cup"),
-                    ("pc", "Piece"),
-                    ("set", "Set"),
-                    ("pair", "Pair"),
-                    ("doz", "Dozen"),
-                    ("box", "Box"),
-                    ("pack", "Pack"),
-                    ("roll", "Roll"),
-                    ("bag", "Bag"),
-                    ("bottle", "Bottle"),
-                    ("tube", "Tube"),
-                    ("can", "Can"),
-                    ("jar", "Jar"),
-                    ("case", "Case"),
-                    ("other", "Other"),
-                ],
-                default="kg",
-                help_text="Select the unit of measure of the product",
-                max_length=250,
-                verbose_name="Unit of measure",
-            ),
+        migrations.CreateModel(
+            name="ProductImage",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("status", models.BooleanField(default=True, verbose_name="status")),
+                (
+                    "image",
+                    models.ImageField(
+                        help_text="Select the image",
+                        upload_to="product/images/",
+                        verbose_name="Image",
+                    ),
+                ),
+                (
+                    "alt",
+                    models.CharField(
+                        help_text="Enter the alt of the image",
+                        max_length=250,
+                        verbose_name="Alt",
+                    ),
+                ),
+                (
+                    "product",
+                    models.ForeignKey(
+                        help_text="Select the product",
+                        on_delete=django.db.models.deletion.CASCADE,
+                        to="artd_product.product",
+                        verbose_name="Product",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "Product Image",
+                "verbose_name_plural": "Product Images",
+            },
         ),
         migrations.AddField(
             model_name="product",
-            name="weight",
-            field=models.DecimalField(
-                decimal_places=2,
-                default=0.0,
-                help_text="Enter the weight of the product",
-                max_digits=10,
-                verbose_name="Weight",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="brand",
-            name="meta_description",
-            field=models.CharField(
-                help_text="Enter the meta description of the search engine",
-                max_length=250,
-                verbose_name="Meta description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="brand",
-            name="meta_keywords",
-            field=models.CharField(
-                help_text="Enter the meta keywords of the search engine",
-                max_length=250,
-                verbose_name="Meta keywords",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="brand",
-            name="meta_title",
-            field=models.CharField(
-                help_text="Enter the meta title of the search engine",
-                max_length=250,
-                verbose_name="Meta title",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="brand",
-            name="name",
-            field=models.CharField(
-                help_text="Enter the name of the brand",
-                max_length=250,
-                verbose_name="Name",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="brand",
-            name="url_key",
-            field=models.CharField(
-                help_text="Enter the url key of the search engine",
-                max_length=250,
-                verbose_name="Url key",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="category",
-            name="meta_description",
-            field=models.CharField(
-                help_text="Enter the meta description of the search engine",
-                max_length=250,
-                verbose_name="Meta description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="category",
-            name="meta_keywords",
-            field=models.CharField(
-                help_text="Enter the meta keywords of the search engine",
-                max_length=250,
-                verbose_name="Meta keywords",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="category",
-            name="meta_title",
-            field=models.CharField(
-                help_text="Enter the meta title of the search engine",
-                max_length=250,
-                verbose_name="Meta title",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="category",
-            name="name",
-            field=models.CharField(
-                help_text="Enter the name of the category",
-                max_length=250,
-                verbose_name="Name",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="category",
-            name="parent",
-            field=models.ForeignKey(
-                help_text="Select the root category",
-                on_delete=django.db.models.deletion.CASCADE,
-                to="product.rootcategory",
-                verbose_name="Root category",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="category",
-            name="url_key",
-            field=models.CharField(
-                help_text="Enter the url key of the search engine",
-                max_length=250,
-                verbose_name="Url key",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="description",
-            field=models.TextField(
-                help_text="Enter the description of the grouped product",
-                verbose_name="Description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="meta_description",
-            field=models.CharField(
-                help_text="Enter the meta description of the search engine",
-                max_length=250,
-                verbose_name="Meta description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="meta_keywords",
-            field=models.CharField(
-                help_text="Enter the meta keywords of the search engine",
-                max_length=250,
-                verbose_name="Meta keywords",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="meta_title",
-            field=models.CharField(
-                help_text="Enter the meta title of the search engine",
-                max_length=250,
-                verbose_name="Meta title",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="name",
-            field=models.CharField(
-                help_text="Enter the name of the grouped product",
-                max_length=250,
-                verbose_name="Name",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="products",
-            field=models.ManyToManyField(
-                help_text="Select the product",
-                to="product.product",
-                verbose_name="Product",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="short_description",
-            field=models.TextField(
-                help_text="Enter the short description of the grouped product",
-                verbose_name="Short_description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="sku",
-            field=models.CharField(
-                help_text="Enter the sku of the grouped product",
-                max_length=250,
-                verbose_name="Sku",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="groupedproduct",
-            name="url_key",
-            field=models.CharField(
-                help_text="Enter the url key of the search engine",
-                max_length=250,
-                verbose_name="Url key",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="categories",
-            field=models.ManyToManyField(
-                help_text="Select the category",
-                to="product.category",
-                verbose_name="Category",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="description",
-            field=models.TextField(
-                help_text="Enter the description of the product",
-                verbose_name="Description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="meta_description",
-            field=models.CharField(
-                help_text="Enter the meta description of the search engine",
-                max_length=250,
-                verbose_name="Meta description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="meta_keywords",
-            field=models.CharField(
-                help_text="Enter the meta keywords of the search engine",
-                max_length=250,
-                verbose_name="Meta keywords",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="meta_title",
-            field=models.CharField(
-                help_text="Enter the meta title of the search engine",
-                max_length=250,
-                verbose_name="Meta title",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="name",
-            field=models.CharField(
-                help_text="Enter the name of the product",
-                max_length=250,
-                verbose_name="Name",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="price",
-            field=models.DecimalField(
-                decimal_places=2,
-                help_text="Enter the price of the product",
-                max_digits=10,
-                verbose_name="Price",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="short_description",
-            field=models.TextField(
-                help_text="Enter the short description of the product",
-                verbose_name="Short description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="sku",
-            field=models.CharField(
-                help_text="Enter the sku of the product",
-                max_length=250,
-                verbose_name="Sku",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="special_price",
-            field=models.DecimalField(
-                decimal_places=2,
-                help_text="Enter the special price of the product",
-                max_digits=10,
-                verbose_name="Special price",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="special_price_from",
-            field=models.DateTimeField(
-                help_text="Enter the special price from of the product",
-                verbose_name="Special price from",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="special_price_to",
-            field=models.DateTimeField(
-                help_text="Enter the special price to of the product",
-                verbose_name="Special price to",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
-            name="stock",
-            field=models.IntegerField(
-                help_text="Enter the stock of the product", verbose_name="Stock"
-            ),
-        ),
-        migrations.AlterField(
-            model_name="product",
             name="tax",
             field=models.ForeignKey(
                 help_text="Select the tax",
                 on_delete=django.db.models.deletion.CASCADE,
-                to="product.tax",
+                to="artd_product.tax",
                 verbose_name="Tax",
             ),
         ),
-        migrations.AlterField(
-            model_name="product",
-            name="url_key",
-            field=models.CharField(
-                help_text="Enter the url key of the search engine",
-                max_length=250,
-                verbose_name="Url key",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="productimage",
-            name="alt",
-            field=models.CharField(
-                help_text="Enter the alt of the image",
-                max_length=250,
-                verbose_name="Alt",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="productimage",
-            name="image",
-            field=models.ImageField(
-                help_text="Select the image",
-                upload_to="product/images/",
-                verbose_name="Image",
-            ),
+        migrations.CreateModel(
+            name="GroupedProduct",
+            fields=[
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("status", models.BooleanField(default=True, verbose_name="status")),
+                (
+                    "url_key",
+                    models.CharField(
+                        help_text="Enter the url key of the search engine",
+                        max_length=250,
+                        verbose_name="Url key",
+                    ),
+                ),
+                (
+                    "meta_title",
+                    models.CharField(
+                        help_text="Enter the meta title of the search engine",
+                        max_length=250,
+                        verbose_name="Meta title",
+                    ),
+                ),
+                (
+                    "meta_description",
+                    models.CharField(
+                        help_text="Enter the meta description of the search engine",
+                        max_length=250,
+                        verbose_name="Meta description",
+                    ),
+                ),
+                (
+                    "meta_keywords",
+                    models.CharField(
+                        help_text="Enter the meta keywords of the search engine",
+                        max_length=250,
+                        verbose_name="Meta keywords",
+                    ),
+                ),
+                (
+                    "name",
+                    models.CharField(
+                        help_text="Enter the name of the grouped product",
+                        max_length=250,
+                        verbose_name="Name",
+                    ),
+                ),
+                (
+                    "sku",
+                    models.CharField(
+                        help_text="Enter the sku of the grouped product",
+                        max_length=250,
+                        verbose_name="Sku",
+                    ),
+                ),
+                (
+                    "description",
+                    models.TextField(
+                        help_text="Enter the description of the grouped product",
+                        verbose_name="Description",
+                    ),
+                ),
+                (
+                    "short_description",
+                    models.TextField(
+                        help_text="Enter the short description of the grouped product",
+                        verbose_name="Short_description",
+                    ),
+                ),
+                (
+                    "products",
+                    models.ManyToManyField(
+                        help_text="Select the product",
+                        to="artd_product.product",
+                        verbose_name="Product",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "Grouped Product",
+                "verbose_name_plural": "Grouped Products",
+            },
         ),
-        migrations.AlterField(
-            model_name="productimage",
-            name="product",
+        migrations.AddField(
+            model_name="category",
+            name="parent",
             field=models.ForeignKey(
-                help_text="Select the product",
+                help_text="Select the root category",
                 on_delete=django.db.models.deletion.CASCADE,
-                to="product.product",
-                verbose_name="Product",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="rootcategory",
-            name="meta_description",
-            field=models.CharField(
-                help_text="Enter the meta description of the search engine",
-                max_length=250,
-                verbose_name="Meta description",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="rootcategory",
-            name="meta_keywords",
-            field=models.CharField(
-                help_text="Enter the meta keywords of the search engine",
-                max_length=250,
-                verbose_name="Meta keywords",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="rootcategory",
-            name="meta_title",
-            field=models.CharField(
-                help_text="Enter the meta title of the search engine",
-                max_length=250,
-                verbose_name="Meta title",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="rootcategory",
-            name="name",
-            field=models.CharField(
-                help_text="Enter the name of the root category",
-                max_length=250,
-                verbose_name="Name",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="rootcategory",
-            name="url_key",
-            field=models.CharField(
-                help_text="Enter the url key of the search engine",
-                max_length=250,
-                verbose_name="Url key",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="tax",
-            name="name",
-            field=models.CharField(
-                help_text="Enter the name of the tax",
-                max_length=250,
-                verbose_name="Name",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="tax",
-            name="percentage",
-            field=models.DecimalField(
-                decimal_places=2,
-                help_text="Enter the percentage of the tax",
-                max_digits=5,
-                verbose_name="Percentage",
+                to="artd_product.rootcategory",
+                verbose_name="Root category",
             ),
         ),
     ]
```

### Comparing `artd_product-0.0.1/setup.py` & `artd_product-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd_product",
-    version="0.0.1",
+    version="0.0.2",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
-    description="A Django app to create Colombian cities",
+    description="A Django app to administrate products",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
     packages=find_packages(
-        include=[
-            "pillow",
-        ]
+        "artd_product",
+        "artd_product.*",
     ),
     keywords=["pypi", "cicd", "python"],
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
```

