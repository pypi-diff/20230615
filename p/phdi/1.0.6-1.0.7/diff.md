# Comparing `tmp/phdi-1.0.6.tar.gz` & `tmp/phdi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-1.0.6.tar", max compression
+gzip compressed data, was "phdi-1.0.7.tar", max compression
```

## Comparing `phdi-1.0.6.tar` & `phdi-1.0.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-05-26 21:23:14.238944 phdi-1.0.6/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-05-26 21:23:14.238944 phdi-1.0.6/README.md
--rw-r--r--   0        0        0       22 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     9436 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2776 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3587 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     8834 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5911 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     1948 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     3167 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/core.py
--rw-r--r--   0        0        0    57291 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/link.py
--rw-r--r--   0        0        0    15429 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2752 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11838 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2046 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1820 2023-05-26 21:23:14.714949 phdi-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-06-15 17:43:36.256598 phdi-1.0.7/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-06-15 17:43:36.256598 phdi-1.0.7/README.md
+-rw-r--r--   0        0        0       22 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     9436 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2776 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3640 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     8834 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5992 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     2555 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     3167 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/core.py
+-rw-r--r--   0        0        0    59276 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/link.py
+-rw-r--r--   0        0        0    15429 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2752 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11838 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2046 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1825 2023-06-15 17:43:36.816606 phdi-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    13445 1970-01-01 00:00:00.000000 phdi-1.0.7/PKG-INFO
```

### Comparing `phdi-1.0.6/LICENSE.md` & `phdi-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/README.md` & `phdi-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/cloud/azure.py` & `phdi-1.0.7/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/cloud/core.py` & `phdi-1.0.7/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/cloud/gcp.py` & `phdi-1.0.7/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/containers/base_service.py` & `phdi-1.0.7/phdi/containers/base_service.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/cloud/azure.py` & `phdi-1.0.7/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/conversion/convert.py` & `phdi-1.0.7/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/geospatial/README.md` & `phdi-1.0.7/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/geospatial/census.py` & `phdi-1.0.7/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/geospatial/core.py` & `phdi-1.0.7/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/geospatial/smarty.py` & `phdi-1.0.7/phdi/fhir/geospatial/smarty.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,20 @@
     Implementation of a geocoding client designed to handle FHIR-
     formatted data using the SmartyStreets API.
     Requires an authorization ID as well as an authentication token
     in order to build a street lookup client.
     """
 
     def __init__(
-        self, auth_id: str, auth_token: str, licenses: list[str] = ["us-standard-cloud"]
+        self,
+        smarty_auth_id: str,
+        smarty_auth_token: str,
+        licenses: list[str] = ["us-standard-cloud"],
     ):
-        self.__client = SmartyGeocodeClient(auth_id, auth_token, licenses)
+        self.__client = SmartyGeocodeClient(smarty_auth_id, smarty_auth_token, licenses)
 
     @property
     def geocode_client(self) -> us_street.Client:
         """
         An instance of the underlying Smarty client.
         Allows the FHIR wrapper to access a SmartyStreets-
         specific connection client without instantiating its own
```

### Comparing `phdi-1.0.6/phdi/fhir/harmonization/README.md` & `phdi-1.0.7/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/harmonization/standardization.py` & `phdi-1.0.7/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/linkage/link.py` & `phdi-1.0.7/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/tabulation/tables.py` & `phdi-1.0.7/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/transport/export.py` & `phdi-1.0.7/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/transport/http.py` & `phdi-1.0.7/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/fhir/utils.py` & `phdi-1.0.7/phdi/fhir/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/geospatial/README.md` & `phdi-1.0.7/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/geospatial/census.py` & `phdi-1.0.7/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/geospatial/core.py` & `phdi-1.0.7/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/geospatial/smarty.py` & `phdi-1.0.7/phdi/geospatial/smarty.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,22 @@
     """
     Represents a PHDI-supplied geocoding client using the Smarty API.
     Requires an authorization ID as well as an authentication token
     in order to build a street lookup client.
     """
 
     def __init__(
-        self, auth_id: str, auth_token: str, licenses: list[str] = ["us-standard-cloud"]
+        self,
+        smarty_auth_id: str,
+        smarty_auth_token: str,
+        licenses: list[str] = ["us-standard-cloud"],
     ):
-        self.auth_id = auth_id
-        self.auth_token = auth_token
-        creds = StaticCredentials(auth_id, auth_token)
+        self.smarty_auth_id = smarty_auth_id
+        self.smarty_auth_token = smarty_auth_token
+        creds = StaticCredentials(smarty_auth_id, smarty_auth_token)
         self.__client = (
             ClientBuilder(creds).with_licenses(licenses).build_us_street_api_client()
         )
 
     @property
     def client(self) -> us_street.Client:
         """
```

### Comparing `phdi-1.0.6/phdi/harmonization/README.md` & `phdi-1.0.7/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/harmonization/__init__.py` & `phdi-1.0.7/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/harmonization/double_metaphone.py` & `phdi-1.0.7/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/harmonization/hl7.py` & `phdi-1.0.7/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.0.7/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/harmonization/standardization.py` & `phdi-1.0.7/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/harmonization/utils.py` & `phdi-1.0.7/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/linkage/__init__.py` & `phdi-1.0.7/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/linkage/core.py` & `phdi-1.0.7/phdi/linkage/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/linkage/link.py` & `phdi-1.0.7/phdi/linkage/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -396,136 +396,159 @@
         except KeyError:
             raise ValueError(f"Field {block} is not a supported extraction field.")
 
     return block_vals
 
 
 def feature_match_exact(
-    record_i: List, record_j: List, feature_x: int, **kwargs: dict
+    record_i: List,
+    record_j: List,
+    feature_col: str,
+    col_to_idx: dict[str, int],
+    **kwargs: dict,
 ) -> bool:
     """
     Determines whether a single feature in a given pair of records
     constitutes an exact match (perfect equality).
 
     :param record_i: One of the records in the candidate pair to evaluate.
     :param record_j: The second record in the candidate pair.
-    :param feature_x: A number representing the index of the feature to
-      compare for equality.
+    :param feature_col: The name of the column being evaluated (e.g. "city").
+    :param col_to_idx: A dictionary mapping column names to the numeric index
+      in which they occur in order in the data.
     :return: A boolean indicating whether the features are an exact match.
     """
-    return record_i[feature_x] == record_j[feature_x]
+    idx = col_to_idx[feature_col]
+    return record_i[idx] == record_j[idx]
 
 
 def feature_match_four_char(
-    record_i: List, record_j: List, feature_x: int, **kwargs: dict
+    record_i: List,
+    record_j: List,
+    feature_col: str,
+    col_to_idx: dict[str, int],
+    **kwargs: dict,
 ) -> bool:
     """
     Determines whether a string feature in a pair of records exactly matches
     on the first four characters.
 
     :param record_i: One of the records in the candidate pair to evaluate.
     :param record_j: The second record in the candidate pair.
-    :param feature_x: A number representing the index of the feature to
-      compare.
+    :param feature_col: The name of the column being evaluated (e.g. "city").
+    :param col_to_idx: A dictionary mapping column names to the numeric index
+      in which they occur in order in the data.
     :return: A boolean indicating whether the features are a match.
     """
-    first_four_i = record_i[feature_x][: min(4, len(record_i[feature_x]))]
-    first_four_j = record_j[feature_x][: min(4, len(record_j[feature_x]))]
+    idx = col_to_idx[feature_col]
+    first_four_i = record_i[idx][: min(4, len(record_i[idx]))]
+    first_four_j = record_j[idx][: min(4, len(record_j[idx]))]
     return first_four_i == first_four_j
 
 
 def feature_match_fuzzy_string(
-    record_i: List, record_j: List, feature_x: int, **kwargs: dict
+    record_i: List,
+    record_j: List,
+    feature_col: str,
+    col_to_idx: dict[str, int],
+    **kwargs: dict,
 ) -> bool:
     """
     Determines whether two strings in a given pair of records are close
     enough to constitute a partial match. The exact nature of the match
     is determined by the specified string comparison function (see
     harmonization/utils/compare_strings for more details) as well as a
     scoring threshold the comparison must meet or exceed.
 
     :param record_i: One of the records in the candidate pair to evaluate.
     :param record_j: The second record in the candidate pair.
-    :param feature_x: A number representing the index of the feature to
-      compare for a partial match.
+    :param feature_col: The name of the column being evaluated (e.g. "city").
+    :param col_to_idx: A dictionary mapping column names to the numeric index
+      in which they occur in order in the data.
     :param **kwargs: Optionally, a dictionary including specifications for
       the string comparison metric to use, as well as the cutoff score
       beyond which to classify the strings as a partial match.
     :return: A boolean indicating whether the features are a fuzzy match.
     """
+    idx = col_to_idx[feature_col]
+
     # Special case for two empty strings, since we don't want vacuous
     # equality (or in-) to penalize the score
-    if record_i[feature_x] == "" and record_j[feature_x] == "":
+    if record_i[idx] == "" and record_j[idx] == "":
         return True
-    if record_i[feature_x] is None and record_j[feature_x] is None:
+    if record_i[idx] is None and record_j[idx] is None:
         return True
 
     similarity_measure = "JaroWinkler"
     if "similarity_measure" in kwargs:
         similarity_measure = kwargs["similarity_measure"]
     threshold = 0.7
     if "threshold" in kwargs:
         threshold = kwargs["threshold"]
-    score = compare_strings(
-        record_i[feature_x], record_j[feature_x], similarity_measure
-    )
+    score = compare_strings(record_i[idx], record_j[idx], similarity_measure)
     return score >= threshold
 
 
 def feature_match_log_odds_exact(
-    record_i: List, record_j: List, feature_x: int, **kwargs: dict
+    record_i: List,
+    record_j: List,
+    feature_col: str,
+    col_to_idx: dict[str, int],
+    **kwargs: dict,
 ) -> float:
     """
     Determines whether two feature values in two records should earn the full
     log-odds similarity score (i.e. they match exactly) or whether they
     should earn no weight (they differ). Used for fields for which fuzzy
     comparisons are inappropriate, such as sex.
 
     :param record_i: One of the records in the candidate pair to evaluate.
     :param record_j: The second record in the candidate pair.
-    :param feature_x: A number representing the index of the feature to
-      compare for a partial match.
+    :param feature_col: The name of the column being evaluated (e.g. "city").
+    :param col_to_idx: A dictionary mapping column names to the numeric index
+      in which they occur in order in the data.
     :return: A float of the score the feature comparison earned.
     """
-    if "idx_to_col" not in kwargs:
-        raise KeyError("Mapping of indices to column names must be provided.")
     if "log_odds" not in kwargs:
         raise KeyError("Mapping of columns to m/u log-odds must be provided.")
-    col = kwargs["idx_to_col"][feature_x]
-    col_odds = kwargs["log_odds"][col]
-    if record_i[feature_x] == record_j[feature_x]:
+    col_odds = kwargs["log_odds"][feature_col]
+    idx = col_to_idx[feature_col]
+    if record_i[idx] == record_j[idx]:
         return col_odds
     else:
         return 0.0
 
 
 def feature_match_log_odds_fuzzy_compare(
-    record_i: List, record_j: List, feature_x: int, **kwargs: dict
+    record_i: List,
+    record_j: List,
+    feature_col: str,
+    col_to_idx: dict[str, int],
+    **kwargs: dict,
 ) -> float:
     """
     Determines the weighted string-odds similarly score earned by two
     feature values in two records, as a function of the pre-computed
     log-odds weights and the string similarity between the two features.
     This scales the full score that would be earned from a perfect
     match to a degree of partial weight appropriate to how similar the
     two strings are.
 
     :param record_i: One of the records in the candidate pair to evaluate.
     :param record_j: The second record in the candidate pair.
-    :param feature_x: A number representing the index of the feature to
-      compare for a partial match.
+    :param feature_col: The name of the column being evaluated (e.g. "city").
+    :param col_to_idx: A dictionary mapping column names to the numeric index
+      in which they occur in order in the data.
     :return: A float of the score the feature comparison earned.
     """
-    if "idx_to_col" not in kwargs:
-        raise KeyError("Mapping of indices to column names must be provided.")
     if "log_odds" not in kwargs:
         raise KeyError("Mapping of columns to m/u log-odds must be provided.")
-    col = kwargs["idx_to_col"][feature_x]
-    col_odds = kwargs["log_odds"][col]
-    score = compare_strings(record_i[feature_x], record_j[feature_x], "JaroWinkler")
+    col_odds = kwargs["log_odds"][feature_col]
+    idx = col_to_idx[feature_col]
+    score = compare_strings(record_i[idx], record_j[idx], "JaroWinkler")
     return score * col_odds
 
 
 def generate_hash_str(linking_identifier: str, salt_str: str) -> str:
     """
     Generates a hash for a given string of concatenated patient information. The hash
     serves as a "unique" identifier for the patient.
@@ -586,46 +609,51 @@
         # MPI will be able to find patients if *any* of their names or addresses
         # contains extracted values, so minimally block on the first line
         # if applicable
         field_blocks = extract_blocking_values_from_record(record, blocking_fields)
         data_block = db_client.block_data(field_blocks)
 
         # First row of returned block is column headers
-        # Map idx to column name, not including patient/person IDs
-        idx_to_col = {k: v for k, v in enumerate(data_block[0][2:])}
+        # Map column name to idx, not including patient/person IDs
+        col_to_idx = {v: k for k, v in enumerate(data_block[0][2:])}
         data_block = data_block[1:]
 
         # Blocked fields are returned as LoLoL, but only name / address
         # need to preserve multiple elements, so flatten other fields
         for i in range(len(data_block)):
             blocked_record = data_block[i]
             for j in range(len(blocked_record)):
-                # patient_id, person_id not included in idx->col mapping
+                # patient_id, person_id not included in col->idx mapping
                 if j < 2:
                     continue
-                if idx_to_col[j - 2] != "first_name" and idx_to_col[j - 2] != "address":
+                if col_to_idx["first_name"] != (j - 2) and col_to_idx["address"] != (
+                    j - 2
+                ):
                     while type(blocked_record[j]) == list:
                         # Handle empty list edge case.
                         if len(blocked_record[j]) == 0:
                             blocked_record[j] = ""
                             break
                         blocked_record[j] = blocked_record[j][0]
+                # Name / address come back as lists of one more depth than they should
+                else:
+                    blocked_record[j] = blocked_record[j][0]
 
         clusters = _group_patient_block_by_person(data_block)
 
         # Check if incoming record should belong to one of the person clusters
         kwargs = linkage_pass.get("kwargs", {})
         for person in clusters:
             num_matched_in_cluster = 0.0
             for linked_patient in clusters[person]:
                 is_match = _compare_records(
                     flattened_record,
                     linked_patient,
                     linkage_pass["funcs"],
-                    idx_to_col,
+                    col_to_idx,
                     linkage_pass["matching_rule"],
                     **kwargs,
                 )
                 if is_match:
                     num_matched_in_cluster += 1.0
 
             # Update membership score for this person cluster so that we can
@@ -679,15 +707,16 @@
         raise json.decoder.JSONDecodeError(
             "The specified file is not valid JSON.", e.doc, e.pos
         )
 
 
 def match_within_block(
     block: List[List],
-    feature_funcs: dict[int, Callable],
+    feature_funcs: dict[str, Callable],
+    col_to_idx: dict[str, int],
     match_eval: Callable,
     **kwargs,
 ) -> List[tuple]:
     """
     Performs matching on all candidate pairs of records within a given block
     of data. Actual partitioning of the data should be done outside this
     function, as it compares all possible pairs within the provided partition.
@@ -709,30 +738,33 @@
     comparisons constitute a match according to X.
 
     :param block: A list of records to check for matches. Each record in
       the list is itself a list of features. The first feature of the
       record must be an "id" for the record.
     :param feature_funcs: A dictionary mapping feature indices to functions
       used to evaluate those features for a match.
+    :param col_to_idx: A dictionary mapping column names to the numeric index
+      in which they occur in order in the data.
     :param match_eval: A function for determining whether a given set of
       feature comparisons constitutes a match for linkage.
     :return: A list of 2-tuples of the form (i,j), where i,j give the indices
       in the block of data of records deemed to match.
     """
     match_pairs = []
 
     # Dynamic programming table: order doesn't matter, so only need to
     # check each combo of i,j once
     for i, record_i in enumerate(block):
         for j in range(i + 1, len(block)):
             record_j = block[j]
             feature_comps = [
-                feature_funcs[x](record_i, record_j, x, **kwargs)
-                for x in range(len(record_i))
-                if x in feature_funcs
+                feature_funcs[feature_col](
+                    record_i, record_j, feature_col, col_to_idx, **kwargs
+                )
+                for feature_col in feature_funcs
             ]
 
             # If it's a match, store the result
             is_match = match_eval(feature_comps, **kwargs)
             if is_match:
                 match_pairs.append((i, j))
 
@@ -742,15 +774,15 @@
 # @TODO: Make the data parameter into a list of lists once we finish up
 # statistical evaluation--alternatively, allow the function to accept both
 # data types, but either way, LoL needs to be in there since that's our
 # primary data type to use here.
 def perform_linkage_pass(
     data: pd.DataFrame,
     blocks: List,
-    feature_funcs: dict[int, Callable],
+    feature_funcs: dict[str, Callable],
     matching_rule: Callable,
     cluster_ratio: Union[float, None] = None,
     **kwargs,
 ) -> dict:
     """
     Performs a partial run of a linkage algorithm using a single rule.
     Each rule in an algorithm is associated with its own pass through the
@@ -766,28 +798,33 @@
       feature comparisons constitutes a match for linkage.
     :param cluster_ratio: An optional parameter indicating, if using the
       algorithm in cluster mode, the required membership percentage a record
       must score with an existing cluster in order to join.
     :return: A dictionary mapping each block found in the pass to the matches
       discovered within that block.
     """
+    # Retrieve indices of columns
+    cols = list(data.columns.values)
+    col_to_idx = dict(zip(cols, range(len(cols))))
+
     blocked_data = block_data(data, blocks)
     matches = {}
     for block in blocked_data:
         if cluster_ratio:
             matches_in_block = _match_within_block_cluster_ratio(
                 blocked_data[block],
                 cluster_ratio,
                 feature_funcs,
+                col_to_idx,
                 matching_rule,
                 **kwargs,
             )
         else:
             matches_in_block = match_within_block(
-                blocked_data[block], feature_funcs, matching_rule, **kwargs
+                blocked_data[block], feature_funcs, col_to_idx, matching_rule, **kwargs
             )
         matches_in_block = _map_matches_to_record_ids(
             matches_in_block, blocked_data[block], cluster_ratio is not None
         )
         matches[block] = matches_in_block
     return matches
 
@@ -908,20 +945,23 @@
 
     :param config_file: A `pathlib.Path` string pointing to a JSON file
       that describes the algorithm to decode.
     :return: A list of dictionaries whose values can be passed to the
       various parts of linkage pass function.
     """
     try:
-        algo_config = json.load(open(config_file))
-        # Need to convert function keys back to column indices, since
-        # JSON serializes dict keys as strings
-        for rl_pass in algo_config.get("algorithm"):
-            rl_pass["funcs"] = {int(col): f for (col, f) in rl_pass["funcs"].items()}
-        return algo_config.get("algorithm", [])
+        with open(config_file) as f:
+            algo_config = json.load(f)
+            # Need to convert function keys back to column indices, since
+            # JSON serializes dict keys as strings
+            for rl_pass in algo_config.get("algorithm"):
+                rl_pass["funcs"] = {
+                    int(col): f for (col, f) in rl_pass["funcs"].items()
+                }
+            return algo_config.get("algorithm", [])
     except FileNotFoundError:
         raise FileNotFoundError(f"No file exists at path {config_file}.")
     except json.decoder.JSONDecodeError as e:
         raise json.decoder.JSONDecodeError(
             "The specified file is not valid JSON.", e.doc, e.pos
         )
 
@@ -1087,123 +1127,140 @@
 
 
 def _eval_record_in_cluster(
     block: List[List],
     i: int,
     cluster: set,
     cluster_ratio: float,
-    feature_funcs: dict[int, Callable],
+    feature_funcs: dict[str, Callable],
+    col_to_idx: dict[str, int],
     match_eval: Callable,
     **kwargs,
 ):
     """
     A helper function used to evaluate whether a given incoming record
     satisfies the matching proportion threshold of an existing cluster,
     and therefore would belong to the cluster.
     """
     record_i = block[i]
     num_matched = 0.0
     for j in cluster:
         record_j = block[j]
         feature_comps = [
-            feature_funcs[x](record_i, record_j, x, **kwargs)
-            for x in range(len(record_i))
-            if x in feature_funcs
+            feature_funcs[feature_col](
+                record_i, record_j, feature_col, col_to_idx, **kwargs
+            )
+            for feature_col in feature_funcs
         ]
 
         is_match = match_eval(feature_comps)
         if is_match:
             num_matched += 1.0
     if (num_matched / len(cluster)) >= cluster_ratio:
         return True
     return False
 
 
 def _compare_records(
     record: List,
     mpi_patient: List,
     feature_funcs: dict,
-    idx_to_col: dict,
+    col_to_idx: dict[str, int],
     matching_rule: callable,
     **kwargs,
 ) -> bool:
     """
     Helper method that compares the flattened form of an incoming new
     patient record to the flattened form of a patient record pulled
     from the MPI.
     """
     # Format is patient_id, person_id, alphabetical list of FHIR keys
     # Don't use the first two ID cols when linking
     feature_comps = [
         _compare_records_field_helper(
-            record[2:], mpi_patient[2:], x, idx_to_col, feature_funcs, **kwargs
+            record[2:],
+            mpi_patient[2:],
+            feature_col,
+            col_to_idx,
+            feature_funcs,
+            **kwargs,
         )
-        for x in feature_funcs
+        for feature_col in feature_funcs
     ]
     is_match = matching_rule(feature_comps, **kwargs)
     return is_match
 
 
 def _compare_records_field_helper(
     record: List,
     mpi_patient: List,
-    idx: int,
-    idx_to_col: dict,
+    feature_col: str,
+    col_to_idx: dict[str, int],
     feature_funcs: dict,
     **kwargs,
 ) -> bool:
-    if idx_to_col[idx] == "first_name":
-        return _compare_name_elements(record, mpi_patient, feature_funcs, idx, **kwargs)
-    elif idx_to_col[idx] == "address":
+    if feature_col == "first_name":
+        return _compare_name_elements(
+            record, mpi_patient, feature_funcs, feature_col, col_to_idx, **kwargs
+        )
+    elif feature_col == "address":
         return _compare_address_elements(
-            record, mpi_patient, feature_funcs, idx, **kwargs
+            record, mpi_patient, feature_funcs, feature_col, col_to_idx, **kwargs
         )
     else:
-        return feature_funcs[idx](record, mpi_patient, idx, **kwargs)
+        return feature_funcs[feature_col](
+            record, mpi_patient, feature_col, col_to_idx, **kwargs
+        )
 
 
 def _compare_address_elements(
     record: List,
     mpi_patient: List,
-    feature_func: dict,
-    x,
+    feature_funcs: dict,
+    feature_col: str,
+    col_to_idx: dict[str, int],
     **kwargs,
 ) -> bool:
     """
     Helper method that compares all elements from the flattened form of an incoming
     new patient record to all elements of the flattened patient record pulled from
     the MPI.
     """
     feature_comp = False
-    for r in record[2:][x]:
-        for m in mpi_patient[2:][x]:
-            feature_comp = feature_func[x]([r], [m], 0, **kwargs)
-            if feature_comp is True:
+    idx = col_to_idx[feature_col]
+    for r in record[idx]:
+        for m in mpi_patient[idx]:
+            feature_comp = feature_funcs[feature_col](
+                [r], [m], feature_col, {feature_col: 0}, **kwargs
+            )
+            if feature_comp:
                 break
         break
     return feature_comp
 
 
 def _compare_name_elements(
     record: List,
     mpi_patient: List,
-    feature_func: dict,
-    x,
+    feature_funcs: dict,
+    feature_col: str,
+    col_to_idx: dict[str, int],
     **kwargs,
 ) -> bool:
     """
     Helper method that compares all elements from the flattened form of an incoming
     new patient record's name(s) to all elements of the flattened
     patient's name(s) pulled from the MPI.
     """
-
-    feature_comp = feature_func[x](
-        [" ".join(n for n in record[2:][x])],
-        [" ".join(n for n in mpi_patient[2:][x])],
-        0,
+    idx = col_to_idx[feature_col]
+    feature_comp = feature_funcs[feature_col](
+        [" ".join(n for n in record[idx])],
+        [" ".join(n for n in mpi_patient[idx])],
+        feature_col,
+        {feature_col: 0},
         **kwargs,
     )
     return feature_comp
 
 
 def _condense_extract_address_from_resource(resource: dict):
     """
@@ -1307,15 +1364,16 @@
             matched_records.append((id_i, id_j))
     return matched_records
 
 
 def _match_within_block_cluster_ratio(
     block: List[List],
     cluster_ratio: float,
-    feature_funcs: dict[int, Callable],
+    feature_funcs: dict[str, Callable],
+    col_to_idx: dict[str, int],
     match_eval: Callable,
     **kwargs,
 ) -> List[set]:
     """
     A matching function for statistically testing the impact of membership
     ratio to the quality of clusters formed. This function behaves similarly
     to `match_within_block`, except that rather than identifying all pairwise
@@ -1330,14 +1388,16 @@
       the list is itself a list of features. The first feature of the
       record must be an "id" for the record.
     :param cluster_ratio: A float giving the proportion of records in an
       existing cluster that a new incoming record must match in order
       to qualify for membership in the cluster.
     :param feature_funcs: A dictionary mapping feature indices to functions
       used to evaluate those features for a match.
+    :param col_to_idx: A dictionary mapping column names to the numeric index
+      in which they occur in order in the data.
     :param match_eval: A function for determining whether a given set of
       feature comparisons constitutes a match for linkage.
     :return: A list of 2-tuples of the form (i,j), where i,j give the indices
       in the block of data of records deemed to match.
     """
     clusters = []
     for i in range(len(block)):
@@ -1346,15 +1406,22 @@
             clusters.append({i})
             continue
         found_master_cluster = False
 
         # Iterate through clusters to find one that we match with
         for cluster in clusters:
             belongs = _eval_record_in_cluster(
-                block, i, cluster, cluster_ratio, feature_funcs, match_eval, **kwargs
+                block,
+                i,
+                cluster,
+                cluster_ratio,
+                feature_funcs,
+                col_to_idx,
+                match_eval,
+                **kwargs,
             )
             if belongs:
                 found_master_cluster = True
                 cluster.add(i)
                 break
 
         # Create a new singleton if no other cluster qualified
```

### Comparing `phdi-1.0.6/phdi/linkage/postgres.py` & `phdi-1.0.7/phdi/linkage/postgres.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/linkage/seed.py` & `phdi-1.0.7/phdi/linkage/seed.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/tabulation/tables.py` & `phdi-1.0.7/phdi/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/tabulation/validation_schema.json` & `phdi-1.0.7/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/transport/http.py` & `phdi-1.0.7/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/validation/__init__.py` & `phdi-1.0.7/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/validation/validation.py` & `phdi-1.0.7/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/phdi/validation/xml_utils.py` & `phdi-1.0.7/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.6/pyproject.toml` & `phdi-1.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "phdi"
-version = "v1.0.6"
+version = "v1.0.7"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>", "Nick Clyde <nclyde@skylight.digital", "Dan Paseltiner <dan@skylight.digital>", "Brady Fausett <brady@skylight.digital>", "Marcelle Goggins <marcelle@skylight.digital", "Nick Bristow <nick@skylight.digital>", "Bryan Britten <bryan@skylight.digital>", "Emma Stephenson <emma@skylight.digital>" , "Gordon Farrell <gordon@skylight.digital>", "Robert Mitchell <rmitchell@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11.3"
 smartystreets-python-sdk = "^4.10.6"
-pydantic = "^1.9.0"
-fastapi = "^0.95.0"
+pydantic = "^1.10.9"
+fastapi = "^0.96.0"
 httpx = "^0.23.3"
 hl7 = "^0.4.5"
 azure-identity = "^1.10.0"
 azure-storage-blob = "^12.12.0"
 polling = "^0.3.2"
 phonenumbers = "^8.12.48"
 pycountry = "^22.3.5"
 PyYAML = "^6.0"
-pyarrow = "^8.0.0"
+pyarrow = "^12.0.0"
 pandas = "^1.4.2"
 coverage = "^6.4.1"
 fhirpathpy = "^0.1.0"
 google-auth = "^2.10.0"
 google-cloud-storage = "^2.5.0"
 jsonschema = "4.16.0"
 rapidfuzz = "^2.13.6"
```

### Comparing `phdi-1.0.6/PKG-INFO` & `phdi-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 1.0.6
+Version: 1.0.7
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
 Requires-Dist: azure-storage-blob (>=12.12.0,<13.0.0)
 Requires-Dist: coverage (>=6.4.1,<7.0.0)
 Requires-Dist: detect-delimiter (>=0.1.1,<0.2.0)
 Requires-Dist: faker (>=18.4.0,<19.0.0)
-Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: fhirpathpy (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth (>=2.10.0,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0)
 Requires-Dist: hl7 (>=0.4.5,<0.5.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: jsonschema (==4.16.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: phonenumbers (>=8.12.48,<9.0.0)
 Requires-Dist: polling (>=0.3.2,<0.4.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
-Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: rapidfuzz (>=2.13.6,<3.0.0)
 Requires-Dist: smartystreets-python-sdk (>=4.10.6,<5.0.0)
 Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Project-URL: Documentation, https://cdcgov.github.io/phdi
 Project-URL: Repository, https://github.com/CDCgov/phdi
 Description-Content-Type: text/markdown
```

