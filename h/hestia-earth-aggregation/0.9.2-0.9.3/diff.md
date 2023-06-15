# Comparing `tmp/hestia-earth-aggregation-0.9.2.tar.gz` & `tmp/hestia-earth-aggregation-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-aggregation-0.9.2.tar", last modified: Mon Aug 15 09:32:25 2022, max compression
+gzip compressed data, was "hestia-earth-aggregation-0.9.3.tar", last modified: Tue Aug 23 08:06:06 2022, max compression
```

## Comparing `hestia-earth-aggregation-0.9.2.tar` & `hestia-earth-aggregation-0.9.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.359598 hestia-earth-aggregation-0.9.2/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1544 2022-08-15 09:32:25.358682 hestia-earth-aggregation-0.9.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1082 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.345847 hestia-earth-aggregation-0.9.2/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.346764 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/
--rw-rw-rw-   0 root         (0) root         (0)     1999 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.348598 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/
--rw-rw-rw-   0 root         (0) root         (0)     2249 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/emission.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/input.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/practice.py
--rw-rw-rw-   0 root         (0) root         (0)      511 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/product.py
--rw-rw-rw-   0 root         (0) root         (0)     8971 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.348598 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/impact_assessment/
--rw-rw-rw-   0 root         (0) root         (0)     1972 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/impact_assessment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/impact_assessment/indicator.py
--rw-rw-rw-   0 root         (0) root         (0)     5467 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/impact_assessment/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.350431 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/
--rw-rw-rw-   0 root         (0) root         (0)      126 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5135 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/countries.py
--rw-rw-rw-   0 root         (0) root         (0)     2809 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/terms.py
--rw-rw-rw-   0 root         (0) root         (0)     5742 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/world.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.352265 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/
--rw-rw-rw-   0 root         (0) root         (0)     4191 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3517 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/combine.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/measurement.py
--rw-rw-rw-   0 root         (0) root         (0)    10851 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     3389 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/site.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/source.py
--rw-rw-rw-   0 root         (0) root         (0)     4387 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/term.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.354098 hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1544 2022-08-15 09:32:25.000000 hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1924 2022-08-15 09:32:25.000000 hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:32:25.000000 hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2022-08-15 09:32:25.000000 hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-08-15 09:32:25.000000 hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-15 09:32:25.359598 hestia-earth-aggregation-0.9.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      996 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.343097 hestia-earth-aggregation-0.9.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.355932 hestia-earth-aggregation-0.9.2/tests/aggregation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.356848 hestia-earth-aggregation-0.9.2/tests/aggregation/cycle/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/cycle/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/cycle/test_practice.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/cycle/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.357765 hestia-earth-aggregation-0.9.2/tests/aggregation/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3465 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/models/test_countries.py
--rw-rw-rw-   0 root         (0) root         (0)     5011 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/models/test_terms.py
--rw-rw-rw-   0 root         (0) root         (0)     3308 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/models/test_world.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/test_aggregation.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/test_cycle.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/test_impact_assesment.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-15 09:32:25.358682 hestia-earth-aggregation-0.9.2/tests/aggregation/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/utils/test_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/utils/test_queries.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/utils/test_source.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2022-08-15 09:32:10.000000 hestia-earth-aggregation-0.9.2/tests/aggregation/utils/test_term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.672292 hestia-earth-aggregation-0.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-08-23 08:06:06.672292 hestia-earth-aggregation-0.9.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.656295 hestia-earth-aggregation-0.9.3/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.657295 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.659294 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/emission.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/input.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/practice.py
+-rw-rw-rw-   0 root         (0) root         (0)      511 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/product.py
+-rw-rw-rw-   0 root         (0) root         (0)     8971 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.660294 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/impact_assessment/
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/impact_assessment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/impact_assessment/indicator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5467 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/impact_assessment/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.662294 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5135 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/countries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/terms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5742 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/world.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.664293 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     4191 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/combine.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/measurement.py
+-rw-rw-rw-   0 root         (0) root         (0)    10894 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     3389 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/site.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/source.py
+-rw-rw-rw-   0 root         (0) root         (0)     4387 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/term.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.666293 hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-08-23 08:06:06.000000 hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1924 2022-08-23 08:06:06.000000 hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 08:06:06.000000 hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2022-08-23 08:06:06.000000 hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-08-23 08:06:06.000000 hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-23 08:06:06.672292 hestia-earth-aggregation-0.9.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      996 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.653295 hestia-earth-aggregation-0.9.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.668293 hestia-earth-aggregation-0.9.3/tests/aggregation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.668293 hestia-earth-aggregation-0.9.3/tests/aggregation/cycle/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/cycle/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/cycle/test_practice.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/cycle/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.670292 hestia-earth-aggregation-0.9.3/tests/aggregation/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3465 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/models/test_countries.py
+-rw-rw-rw-   0 root         (0) root         (0)     5011 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/models/test_terms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/models/test_world.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/test_aggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/test_cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/test_impact_assesment.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 08:06:06.672292 hestia-earth-aggregation-0.9.3/tests/aggregation/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/utils/test_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/utils/test_queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/utils/test_source.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2022-08-23 08:05:50.000000 hestia-earth-aggregation-0.9.3/tests/aggregation/utils/test_term.py
```

### Comparing `hestia-earth-aggregation-0.9.2/LICENSE` & `hestia-earth-aggregation-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/PKG-INFO` & `hestia-earth-aggregation-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-aggregation
-Version: 0.9.2
+Version: 0.9.3
 Summary: Hestia's aggregation engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-aggregation-engine
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-aggregation-0.9.2/README.md` & `hestia-earth-aggregation-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/__init__.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/__init__.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/emission.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/emission.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/practice.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/practice.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/cycle/utils.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/cycle/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/impact_assessment/__init__.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/impact_assessment/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/impact_assessment/indicator.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/impact_assessment/indicator.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/impact_assessment/utils.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/impact_assessment/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/log.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/countries.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/countries.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/terms.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/terms.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/models/world.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/models/world.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/__init__.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/combine.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/combine.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/queries.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,8 +317,9 @@
     }
     results = _run_query(params)
     return results[0].get('endDate') if len(results) > 0 else None
 
 
 def get_time_ranges(node_type: str, country: dict, product_name: str):
     from_date = _earliest_date(node_type, product_name, country)
-    return _get_time_ranges(from_date, _latest_date(node_type, product_name, country)) if from_date else []
+    to_date = _latest_date(node_type, product_name, country) if from_date else None
+    return _get_time_ranges(from_date, to_date) if to_date else []
```

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/site.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/site.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/source.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/source.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth/aggregation/utils/term.py` & `hestia-earth-aggregation-0.9.3/hestia_earth/aggregation/utils/term.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/PKG-INFO` & `hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-aggregation
-Version: 0.9.2
+Version: 0.9.3
 Summary: Hestia's aggregation engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-aggregation-engine
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-aggregation-0.9.2/hestia_earth_aggregation.egg-info/SOURCES.txt` & `hestia-earth-aggregation-0.9.3/hestia_earth_aggregation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/setup.py` & `hestia-earth-aggregation-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/cycle/test_practice.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/cycle/test_practice.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/models/test_countries.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/models/test_countries.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/models/test_terms.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/models/test_terms.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/models/test_world.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/models/test_world.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/test_aggregation.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/test_cycle.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/test_cycle.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/test_impact_assesment.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/test_impact_assesment.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/test_utils.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/test_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/utils/test_combine.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/utils/test_combine.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/utils/test_queries.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/utils/test_queries.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-aggregation-0.9.2/tests/aggregation/utils/test_term.py` & `hestia-earth-aggregation-0.9.3/tests/aggregation/utils/test_term.py`

 * *Files identical despite different names*

