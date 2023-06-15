# Comparing `tmp/threedi-schema-0.217.3.tar.gz` & `tmp/threedi-schema-0.217.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.217.3.tar", last modified: Mon Jun 12 13:31:06 2023, max compression
+gzip compressed data, was "threedi-schema-0.217.4.tar", last modified: Thu Jun 15 11:35:37 2023, max compression
```

## Comparing `threedi-schema-0.217.3.tar` & `threedi-schema-0.217.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.084562 threedi-schema-0.217.3/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.088562 threedi-schema-0.217.3/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.088562 threedi-schema-0.217.3/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.092562 threedi-schema-0.217.3/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.092562 threedi-schema-0.217.3/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.088562 threedi-schema-0.217.3/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:31:05.000000 threedi-schema-0.217.3/threedi_schema.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.378269 threedi-schema-0.217.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-15 11:35:37.378269 threedi-schema-0.217.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-15 11:35:37.378269 threedi-schema-0.217.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.370269 threedi-schema-0.217.4/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.370269 threedi-schema-0.217.4/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.370269 threedi-schema-0.217.4/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.374269 threedi-schema-0.217.4/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.374269 threedi-schema-0.217.4/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.374269 threedi-schema-0.217.4/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.374269 threedi-schema-0.217.4/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.374269 threedi-schema-0.217.4/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-15 11:35:28.000000 threedi-schema-0.217.4/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:37.370269 threedi-schema-0.217.4/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-15 11:35:37.000000 threedi-schema-0.217.4/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-15 11:35:37.000000 threedi-schema-0.217.4/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:35:37.000000 threedi-schema-0.217.4/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 11:35:37.000000 threedi-schema-0.217.4/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:35:37.000000 threedi-schema-0.217.4/threedi_schema.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 11:35:37.000000 threedi-schema-0.217.4/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 11:35:37.000000 threedi-schema-0.217.4/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.217.3/CHANGES.rst` & `threedi-schema-0.217.4/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog of threedi-schema
 ===================================================
 
+0.217.4 (2023-06-15)
+--------------------
+
+- Fix SQLAlchemy engine and connection usage.
+
+- Do not pool connections (solving file permission denied issues on Windows).
+
+
 0.217.3 (2023-06-12)
 --------------------
 
 - Added groundwater 1D2D columns to the views.
 
 
 0.217.2 (2023-05-24)
```

### Comparing `threedi-schema-0.217.3/LICENSE` & `threedi-schema-0.217.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/PKG-INFO` & `threedi-schema-0.217.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.217.3
+Version: 0.217.4
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,22 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.4 (2023-06-15)
+--------------------
+
+- Fix SQLAlchemy engine and connection usage.
+
+- Do not pool connections (solving file permission denied issues on Windows).
+
+
 0.217.3 (2023-06-12)
 --------------------
 
 - Added groundwater 1D2D columns to the views.
 
 
 0.217.2 (2023-05-24)
```

### Comparing `threedi-schema-0.217.3/README.rst` & `threedi-schema-0.217.4/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/setup.py` & `threedi-schema-0.217.4/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/application/schema.py` & `threedi-schema-0.217.4/threedi_schema/application/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     script = ScriptDirectory.from_config(config)
     with EnvironmentContext(config=config, script=script) as env:
         return int(env.get_head_revision())
 
 
 def _upgrade_database(db, revision="head", unsafe=True):
     """Upgrade ThreediDatabase instance"""
-    engine = db.get_engine()
+    engine = db.engine
 
     config = get_alembic_config(engine, unsafe=unsafe)
     alembic_command.upgrade(config, revision)
 
 
 class ModelSchema:
     def __init__(self, threedi_db, declared_models=models.DECLARED_MODELS):
@@ -49,30 +49,30 @@
         self.declared_models = declared_models
 
     def _get_version_old(self):
         """The version of the database using the old 'south' versioning."""
         south_migrationhistory = Table(
             "south_migrationhistory", MetaData(), Column("id", Integer)
         )
-        engine = self.db.get_engine()
+        engine = self.db.engine
         if not self.db.has_table("south_migrationhistory"):
             return
-        with engine.begin() as connection:
+        with engine.connect() as connection:
             query = south_migrationhistory.select().order_by(
                 south_migrationhistory.columns["id"].desc()
             )
             versions = list(connection.execute(query.limit(1)))
             if len(versions) == 1:
                 return versions[0][0]
             else:
                 return None
 
     def get_version(self):
         """Returns the id (integer) of the latest migration"""
-        with self.db.get_engine().begin() as connection:
+        with self.db.engine.connect() as connection:
             context = MigrationContext.configure(
                 connection, opts={"version_table": constants.VERSION_TABLE_NAME}
             )
             version = context.get_current_revision()
 
         if version is not None:
             return int(version)
```

### Comparing `threedi-schema-0.217.3/threedi_schema/application/threedi_database.py` & `threedi-schema-0.217.4/threedi_schema/application/threedi_database.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from contextlib import contextmanager
 from pathlib import Path
 
 from sqlalchemy import create_engine, event, inspect, text
 from sqlalchemy.engine import Engine
 from sqlalchemy.event import listen
 from sqlalchemy.orm import sessionmaker
+from sqlalchemy.pool import NullPool
 
 from .schema import ModelSchema
 
 __all__ = ["ThreediDatabase"]
 
 
 @event.listens_for(Engine, "connect")
@@ -86,15 +87,23 @@
 
     @property
     def base_path(self):
         return Path(self.path).absolute().parent
 
     def get_engine(self, get_seperate_engine=False):
         if self._engine is None or get_seperate_engine:
-            engine = create_engine("sqlite:///{0}".format(self.path), echo=self.echo)
+            if self.path == "":
+                # Special case in-memory SQLite:
+                # https://docs.sqlalchemy.org/en/20/dialects/sqlite.html#threading-pooling-behavior
+                poolclass = None
+            else:
+                poolclass = NullPool
+            engine = create_engine(
+                "sqlite:///{0}".format(self.path), echo=self.echo, poolclass=poolclass
+            )
             listen(engine, "connect", load_spatialite)
             if get_seperate_engine:
                 return engine
             else:
                 self._engine = engine
 
         return self._engine
```

### Comparing `threedi-schema-0.217.3/threedi_schema/beta_features.py` & `threedi-schema-0.217.4/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/domain/constants.py` & `threedi-schema-0.217.4/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/domain/custom_types.py` & `threedi-schema-0.217.4/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/domain/indexes.py` & `threedi-schema-0.217.4/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/domain/models.py` & `threedi-schema-0.217.4/threedi_schema/domain/models.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/domain/views.py` & `threedi-schema-0.217.4/threedi_schema/domain/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/infrastructure/spatial_index.py` & `threedi-schema-0.217.4/threedi_schema/infrastructure/spatial_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,23 @@
 
     return True
 
 
 def ensure_spatial_indexes(db, models):
     """Ensure presence of spatial indexes for all geometry columns"""
     created = False
-    engine = db.get_engine()
+    engine = db.engine
 
-    with engine.begin() as connection:
-        for model in models:
-            geom_columns = [
-                x for x in model.__table__.columns if isinstance(x.type, Geometry)
-            ]
-            if len(geom_columns) > 1:
-                # Pragmatic fix: spatialindex breaks on multiple geometry columns per table
-                geom_columns = [x for x in geom_columns if x.name == "the_geom"]
-            if geom_columns:
-                created &= _ensure_spatial_index(connection, geom_columns[0])
+    with engine.connect() as connection:
+        with connection.begin():
+            for model in models:
+                geom_columns = [
+                    x for x in model.__table__.columns if isinstance(x.type, Geometry)
+                ]
+                if len(geom_columns) > 1:
+                    # Pragmatic fix: spatialindex breaks on multiple geometry columns per table
+                    geom_columns = [x for x in geom_columns if x.name == "the_geom"]
+                if geom_columns:
+                    created &= _ensure_spatial_index(connection, geom_columns[0])
 
-        if created:
-            connection.execute(text("VACUUM"))
+            if created:
+                connection.execute(text("VACUUM"))
```

### Comparing `threedi-schema-0.217.3/threedi_schema/infrastructure/spatialite_versions.py` & `threedi-schema-0.217.4/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def get_spatialite_version(db):
     with db.session_scope() as session:
         ((lib_version,),) = session.execute(
             text("SELECT spatialite_version()")
         ).fetchall()
 
     # Identify Spatialite version
-    inspector = inspect(db.get_engine())
+    inspector = inspect(db.engine)
     spatial_ref_sys_cols = [x["name"] for x in inspector.get_columns("spatial_ref_sys")]
     if len(spatial_ref_sys_cols) == 0:
         raise ValueError("Not a spatialite file")
 
     if "srs_wkt" in spatial_ref_sys_cols:
         file_version = 3
     else:
```

### Comparing `threedi-schema-0.217.3/threedi_schema/infrastructure/views.py` & `threedi-schema-0.217.4/threedi_schema/infrastructure/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 from sqlalchemy import text
 
 __all__ = ["recreate_views"]
 
 
 def recreate_views(db, file_version, all_views, views_to_delete):
     """Recreate predefined views in a ThreediDatabase instance"""
-    engine = db.get_engine()
+    engine = db.engine
 
-    with engine.begin() as connection:
-        for name, view in all_views.items():
-            connection.execute(text(f"DROP VIEW IF EXISTS {name}"))
-            connection.execute(
-                text(f"DELETE FROM views_geometry_columns WHERE view_name = '{name}'")
-            )
-            connection.execute(text(f"CREATE VIEW {name} AS {view['definition']}"))
-            if file_version == 3:
+    with engine.connect() as connection:
+        with connection.begin():
+            for name, view in all_views.items():
+                connection.execute(text(f"DROP VIEW IF EXISTS {name}"))
                 connection.execute(
                     text(
-                        f"INSERT INTO views_geometry_columns (view_name, view_geometry,view_rowid,f_table_name,f_geometry_column) VALUES('{name}', '{view['view_geometry']}', '{view['view_rowid']}', '{view['f_table_name']}', '{view['f_geometry_column']}')"
+                        f"DELETE FROM views_geometry_columns WHERE view_name = '{name}'"
                     )
                 )
-            else:
+                connection.execute(text(f"CREATE VIEW {name} AS {view['definition']}"))
+                if file_version == 3:
+                    connection.execute(
+                        text(
+                            f"INSERT INTO views_geometry_columns (view_name, view_geometry,view_rowid,f_table_name,f_geometry_column) VALUES('{name}', '{view['view_geometry']}', '{view['view_rowid']}', '{view['f_table_name']}', '{view['f_geometry_column']}')"
+                        )
+                    )
+                else:
+                    connection.execute(
+                        text(
+                            f"INSERT INTO views_geometry_columns (view_name, view_geometry,view_rowid,f_table_name,f_geometry_column,read_only) VALUES('{name}', '{view['view_geometry']}', '{view['view_rowid']}', '{view['f_table_name']}', '{view['f_geometry_column']}', 0)"
+                        )
+                    )
+            for name in views_to_delete:
+                connection.execute(text(f"DROP VIEW IF EXISTS {name}"))
                 connection.execute(
                     text(
-                        f"INSERT INTO views_geometry_columns (view_name, view_geometry,view_rowid,f_table_name,f_geometry_column,read_only) VALUES('{name}', '{view['view_geometry']}', '{view['view_rowid']}', '{view['f_table_name']}', '{view['f_geometry_column']}', 0)"
+                        f"DELETE FROM views_geometry_columns WHERE view_name = '{name}'"
                     )
                 )
-        for name in views_to_delete:
-            connection.execute(text(f"DROP VIEW IF EXISTS {name}"))
-            connection.execute(
-                text(f"DELETE FROM views_geometry_columns WHERE view_name = '{name}'")
-            )
```

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/env.py` & `threedi-schema-0.217.4/threedi_schema/migrations/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     Note: SQLite does not (completely) support transactions, so, backup the
     SQLite before running migrations.
     """
     unsafe = config.attributes.get("unsafe")
     
     engine = config.attributes.get("engine")
     if engine is None:
-        engine = ThreediDatabase(get_url()).get_engine()
+        engine = ThreediDatabase(get_url()).engine
     
 
-    with engine.begin() as connection:
+    with engine.connect() as connection:
         if unsafe:
             # Speed up by journalling in memory; in case of a crash the database
             # will likely go corrupt.
             # NB: This setting is scoped to this connection.
             connection.execute(text("PRAGMA journal_mode = MEMORY"))
 
         context.configure(
```

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0200_initial.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi-schema-0.217.4/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/scripts.py` & `threedi-schema-0.217.4/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/tests/conftest.py` & `threedi-schema-0.217.4/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/tests/test_migration_213.py` & `threedi-schema-0.217.4/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema/tests/test_schema.py` & `threedi-schema-0.217.4/threedi_schema/tests/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
 
 @pytest.fixture
 def south_migration_table(in_memory_sqlite):
     south_migrationhistory = Table(
         "south_migrationhistory", MetaData(), Column("id", Integer)
     )
-    engine = in_memory_sqlite.get_engine()
+    engine = in_memory_sqlite.engine
     south_migrationhistory.create(engine)
     return south_migrationhistory
 
 
 @pytest.fixture
 def alembic_version_table(in_memory_sqlite):
     alembic_version = Table(
         constants.VERSION_TABLE_NAME,
         MetaData(),
         Column("version_num", String(32), nullable=False),
     )
-    engine = in_memory_sqlite.get_engine()
+    engine = in_memory_sqlite.engine
     alembic_version.create(engine)
     return alembic_version
 
 
 def test_get_schema_version():
     """The current version in the library. We start counting at 200."""
     # this will catch future mistakes of setting non-integer revisions
@@ -51,17 +51,18 @@
     schema_checker = ModelSchema(in_memory_sqlite)
     migration_id = schema_checker.get_version()
     assert migration_id is None
 
 
 def test_get_version_south(in_memory_sqlite, south_migration_table):
     """Get the version of a sqlite with a South version table"""
-    with in_memory_sqlite.get_engine().begin() as connection:
-        for v in (42, 43):
-            connection.execute(south_migration_table.insert().values(id=v))
+    with in_memory_sqlite.engine.connect() as connection:
+        with connection.begin():
+            for v in (42, 43):
+                connection.execute(south_migration_table.insert().values(id=v))
 
     schema_checker = ModelSchema(in_memory_sqlite)
     migration_id = schema_checker.get_version()
     assert migration_id == 43
 
 
 def test_get_version_empty_alembic(in_memory_sqlite, alembic_version_table):
@@ -69,16 +70,19 @@
     schema_checker = ModelSchema(in_memory_sqlite)
     migration_id = schema_checker.get_version()
     assert migration_id is None
 
 
 def test_get_version_alembic(in_memory_sqlite, alembic_version_table):
     """Get the version of a sqlite with an alembic version table"""
-    with in_memory_sqlite.get_engine().begin() as connection:
-        connection.execute(alembic_version_table.insert().values(version_num="0201"))
+    with in_memory_sqlite.engine.connect() as connection:
+        with connection.begin():
+            connection.execute(
+                alembic_version_table.insert().values(version_num="0201")
+            )
 
     schema_checker = ModelSchema(in_memory_sqlite)
     migration_id = schema_checker.get_version()
     assert migration_id == 201
 
 
 def test_validate_schema(sqlite_latest):
@@ -196,35 +200,36 @@
     schema = ModelSchema(oldest_sqlite)
     schema.upgrade(backup=False, upgrade_spatialite_version=True)
 
     _, file_version_after = get_spatialite_version(oldest_sqlite)
     assert file_version_after == 4
 
     # the spatial indexes are there
-    with oldest_sqlite.get_engine().begin() as connection:
+    with oldest_sqlite.engine.connect() as connection:
         check_result = connection.execute(
             text("SELECT CheckSpatialIndex('v2_connection_nodes', 'the_geom')")
         ).scalar()
 
     assert check_result == 1
 
 
 def test_set_spatial_indexes(in_memory_sqlite):
-    engine = in_memory_sqlite.get_engine()
+    engine = in_memory_sqlite.engine
 
     schema = ModelSchema(in_memory_sqlite)
     schema.upgrade(backup=False)
 
-    with engine.begin() as connection:
-        connection.execute(
-            text("SELECT DisableSpatialIndex('v2_connection_nodes', 'the_geom')")
-        ).scalar()
-        connection.execute(text("DROP TABLE idx_v2_connection_nodes_the_geom"))
+    with engine.connect() as connection:
+        with connection.begin():
+            connection.execute(
+                text("SELECT DisableSpatialIndex('v2_connection_nodes', 'the_geom')")
+            ).scalar()
+            connection.execute(text("DROP TABLE idx_v2_connection_nodes_the_geom"))
 
     schema.set_spatial_indexes()
 
-    with engine.begin() as connection:
+    with engine.connect() as connection:
         check_result = connection.execute(
             text("SELECT CheckSpatialIndex('v2_connection_nodes', 'the_geom')")
         ).scalar()
 
     assert check_result == 1
```

### Comparing `threedi-schema-0.217.3/threedi_schema/tests/test_spatalite_versions.py` & `threedi-schema-0.217.4/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.3/threedi_schema.egg-info/PKG-INFO` & `threedi-schema-0.217.4/threedi_schema.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.217.3
+Version: 0.217.4
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,22 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.4 (2023-06-15)
+--------------------
+
+- Fix SQLAlchemy engine and connection usage.
+
+- Do not pool connections (solving file permission denied issues on Windows).
+
+
 0.217.3 (2023-06-12)
 --------------------
 
 - Added groundwater 1D2D columns to the views.
 
 
 0.217.2 (2023-05-24)
```

### Comparing `threedi-schema-0.217.3/threedi_schema.egg-info/SOURCES.txt` & `threedi-schema-0.217.4/threedi_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

