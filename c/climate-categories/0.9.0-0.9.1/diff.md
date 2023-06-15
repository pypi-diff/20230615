# Comparing `tmp/climate_categories-0.9.0.tar.gz` & `tmp/climate_categories-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_categories-0.9.0.tar", last modified: Wed Jun 14 16:12:46 2023, max compression
+gzip compressed data, was "climate_categories-0.9.1.tar", last modified: Thu Jun 15 13:50:35 2023, max compression
```

## Comparing `climate_categories-0.9.0.tar` & `climate_categories-0.9.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.835556 climate_categories-0.9.0/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.827556 climate_categories-0.9.0/.github/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.831556 climate_categories-0.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.9.0/.github/ISSUE_TEMPLATE/new_categorization.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.831556 climate_categories-0.9.0/.github/workflows/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.9.0/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-06-13 09:03:12.000000 climate_categories-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.9.0/.readthedocs.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.9.0/.sourcery.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      216 2023-04-26 14:19:11.000000 climate_categories-0.9.0/AUTHORS.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5268 2023-06-14 15:08:21.000000 climate_categories-0.9.0/CHANGELOG.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      696 2023-04-26 14:19:11.000000 climate_categories-0.9.0/LICENSE
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3280 2023-06-14 15:10:21.000000 climate_categories-0.9.0/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9745 2023-06-14 16:12:46.835556 climate_categories-0.9.0/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3460 2023-06-14 16:12:19.000000 climate_categories-0.9.0/README.rst
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.831556 climate_categories-0.9.0/climate_categories/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1978 2023-06-14 15:08:08.000000 climate_categories-0.9.0/climate_categories/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    43254 2023-05-23 15:38:02.000000 climate_categories-0.9.0/climate_categories/_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.9.0/climate_categories/_conversions.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.831556 climate_categories-0.9.0/climate_categories/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.9.0/climate_categories/data/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.9.0/climate_categories/data/BURDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.9.0/climate_categories/data/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.9.0/climate_categories/data/BURDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.9.0/climate_categories/data/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.9.0/climate_categories/data/CRF1999.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013_2021.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013_2022.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/CRF2013_2023.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.9.0/climate_categories/data/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.9.0/climate_categories/data/CRFDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.9.0/climate_categories/data/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.9.0/climate_categories/data/CRFDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.9.0/climate_categories/data/GCB.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/data/GCB.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.9.0/climate_categories/data/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.9.0/climate_categories/data/IPCC1996.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.9.0/climate_categories/data/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.9.0/climate_categories/data/IPCC2006.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.9.0/climate_categories/data/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.9.0/climate_categories/data/IPCC2006_PRIMAP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60468 2023-06-14 15:06:35.000000 climate_categories-0.9.0/climate_categories/data/ISO3.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39499 2023-06-14 15:06:35.000000 climate_categories-0.9.0/climate_categories/data/ISO3.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.9.0/climate_categories/data/RCMIP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.9.0/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.9.0/climate_categories/data/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.9.0/climate_categories/data/gas.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:12:58.000000 climate_categories-0.9.0/climate_categories/py.typed
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.9.0/climate_categories/search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.835556 climate_categories-0.9.0/climate_categories/tests/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.9.0/climate_categories/tests/conftest.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.835556 climate_categories-0.9.0/climate_categories/tests/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.9.0/climate_categories/tests/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.0/climate_categories/tests/data/broken_conversion_not_allowed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.0/climate_categories/tests/data/broken_conversion_not_existing.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/broken_hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/broken_simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.0/climate_categories/tests/data/good_conversion.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/good_conversion_A.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/good_conversion_B.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/good_conversion_aux1.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/good_conversion_aux2.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.0/climate_categories/tests/data/good_conversion_reversed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/data/simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/examples.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21970 2023-05-15 16:28:37.000000 climate_categories-0.9.0/climate_categories/tests/test_climate_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.9.0/climate_categories/tests/test_conversions.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.9.0/climate_categories/tests/test_crf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/test_di.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/test_gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/test_ipcc.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1616 2023-06-14 15:06:35.000000 climate_categories-0.9.0/climate_categories/tests/test_iso3.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/test_overcounting.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.9.0/climate_categories/tests/test_primap.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.9.0/climate_categories/tests/test_rcmip.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.9.0/climate_categories/tests/test_search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.831556 climate_categories-0.9.0/climate_categories.egg-info/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9745 2023-06-14 16:12:46.000000 climate_categories-0.9.0/climate_categories.egg-info/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4157 2023-06-14 16:12:46.000000 climate_categories-0.9.0/climate_categories.egg-info/SOURCES.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-06-14 16:12:46.000000 climate_categories-0.9.0/climate_categories.egg-info/dependency_links.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      307 2023-06-14 16:12:46.000000 climate_categories-0.9.0/climate_categories.egg-info/requires.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-06-14 16:12:46.000000 climate_categories-0.9.0/climate_categories.egg-info/top_level.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.9.0/codecov.yml
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.835556 climate_categories-0.9.0/data_generation/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.9.0/data_generation/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13684 2023-06-14 15:06:35.000000 climate_categories-0.9.0/data_generation/ISO3.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/convert_yaml_to_python.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.9.0/data_generation/utils.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-14 16:12:46.835556 climate_categories-0.9.0/docs/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/api.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/changelog.rst
--rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-05-10 09:47:08.000000 climate_categories-0.9.0/docs/conf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/contributing.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/credits.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8179 2023-05-10 10:01:49.000000 climate_categories-0.9.0/docs/data.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/index.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/installation.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/make.bat
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.9.0/docs/readme.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       21 2023-05-10 09:48:15.000000 climate_categories-0.9.0/docs/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18889 2023-05-15 16:28:37.000000 climate_categories-0.9.0/docs/usage.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.9.0/pyproject.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.9.0/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.9.0/requirements_dev.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1658 2023-06-14 16:12:46.835556 climate_categories-0.9.0/setup.cfg
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.9.0/setup.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-06-14 15:08:08.000000 climate_categories-0.9.0/tbump.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.9.0/tox.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.9.0/update_changelog.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.9.0/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/new_categorization.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.9.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.9.1/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-06-13 09:03:12.000000 climate_categories-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.9.1/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.sourcery.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      216 2023-04-26 14:19:11.000000 climate_categories-0.9.1/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5357 2023-06-15 13:49:02.000000 climate_categories-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      696 2023-04-26 14:19:11.000000 climate_categories-0.9.1/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3280 2023-06-14 15:10:21.000000 climate_categories-0.9.1/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9834 2023-06-15 13:50:35.933570 climate_categories-0.9.1/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3460 2023-06-15 13:50:20.000000 climate_categories-0.9.1/README.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/climate_categories/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1978 2023-06-15 13:48:49.000000 climate_categories-0.9.1/climate_categories/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    43254 2023-05-23 15:38:02.000000 climate_categories-0.9.1/climate_categories/_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.9.1/climate_categories/_conversions.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/climate_categories/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.9.1/climate_categories/data/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.9.1/climate_categories/data/BURDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.9.1/climate_categories/data/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.9.1/climate_categories/data/BURDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.9.1/climate_categories/data/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.9.1/climate_categories/data/CRF1999.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2021.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2022.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2023.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.9.1/climate_categories/data/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.9.1/climate_categories/data/CRFDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.9.1/climate_categories/data/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.9.1/climate_categories/data/CRFDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.9.1/climate_categories/data/GCB.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/data/GCB.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.9.1/climate_categories/data/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.9.1/climate_categories/data/IPCC1996.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    61742 2023-06-15 13:48:28.000000 climate_categories-0.9.1/climate_categories/data/ISO3.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    40093 2023-06-15 13:48:28.000000 climate_categories-0.9.1/climate_categories/data/ISO3.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/RCMIP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.9.1/climate_categories/data/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.9.1/climate_categories/data/gas.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:12:58.000000 climate_categories-0.9.1/climate_categories/py.typed
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.9.1/climate_categories/search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/climate_categories/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.9.1/climate_categories/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/climate_categories/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.9.1/climate_categories/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_conversion_not_allowed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_conversion_not_existing.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_A.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_B.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_aux1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_aux2.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_reversed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21970 2023-05-15 16:28:37.000000 climate_categories-0.9.1/climate_categories/tests/test_climate_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.9.1/climate_categories/tests/test_conversions.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.9.1/climate_categories/tests/test_crf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_di.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_ipcc.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1708 2023-06-15 13:48:28.000000 climate_categories-0.9.1/climate_categories/tests/test_iso3.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_overcounting.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_primap.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/test_rcmip.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.9.1/climate_categories/tests/test_search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/climate_categories.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9834 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4157 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      307 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.9.1/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/data_generation/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.9.1/data_generation/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14792 2023-06-15 13:48:28.000000 climate_categories-0.9.1/data_generation/ISO3.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/convert_yaml_to_python.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-05-10 09:47:08.000000 climate_categories-0.9.1/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/contributing.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8179 2023-05-10 10:01:49.000000 climate_categories-0.9.1/docs/data.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       21 2023-05-10 09:48:15.000000 climate_categories-0.9.1/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18889 2023-05-15 16:28:37.000000 climate_categories-0.9.1/docs/usage.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.9.1/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.9.1/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.9.1/requirements_dev.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1658 2023-06-15 13:50:35.933570 climate_categories-0.9.1/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.9.1/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-06-15 13:48:49.000000 climate_categories-0.9.1/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.9.1/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.9.1/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.9.1/update_citation_info.py
```

### Comparing `climate_categories-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md` & `climate_categories-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md` & `climate_categories-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/.github/ISSUE_TEMPLATE/new_categorization.md` & `climate_categories-0.9.1/.github/ISSUE_TEMPLATE/new_categorization.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/.github/workflows/ci.yml` & `climate_categories-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/.gitignore` & `climate_categories-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/.pre-commit-config.yaml` & `climate_categories-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/CHANGELOG.rst` & `climate_categories-0.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =========
 Changelog
 =========
 
+0.9.1 (2023-06-15)
+------------------
+* Add AOSIS country group to ISO3 categorization.
+
 0.9.0 (2023-06-14)
 ------------------
 * Add ISO3 terminology for countries, areas, and country groups including UNFCCC
   signatories and Annex-I and Non-Annex-I groups and the evolution of the EU over time.
 
 0.8.5 (2023-05-23)
 ------------------
```

### Comparing `climate_categories-0.9.0/CONTRIBUTING.rst` & `climate_categories-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/LICENSE` & `climate_categories-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/Makefile` & `climate_categories-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/PKG-INFO` & `climate_categories-0.9.1/climate_categories.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: climate_categories
-Version: 0.9.0
+Name: climate-categories
+Version: 0.9.1
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -96,22 +96,26 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-14).
-pik-primap/climate_categories: climate_categories Version 0.9.0.
-Zenodo. https://doi.org/10.5281/zenodo.8039308
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-15).
+pik-primap/climate_categories: climate_categories Version 0.9.1.
+Zenodo. https://doi.org/10.5281/zenodo.8043234
 
 =========
 Changelog
 =========
 
+0.9.1 (2023-06-15)
+------------------
+* Add AOSIS country group to ISO3 categorization.
+
 0.9.0 (2023-06-14)
 ------------------
 * Add ISO3 terminology for countries, areas, and country groups including UNFCCC
   signatories and Annex-I and Non-Annex-I groups and the evolution of the EU over time.
 
 0.8.5 (2023-05-23)
 ------------------
```

### Comparing `climate_categories-0.9.0/README.rst` & `climate_categories-0.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,10 +72,10 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-14).
-pik-primap/climate_categories: climate_categories Version 0.9.0.
-Zenodo. https://doi.org/10.5281/zenodo.8039308
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-15).
+pik-primap/climate_categories: climate_categories Version 0.9.1.
+Zenodo. https://doi.org/10.5281/zenodo.8043234
```

### Comparing `climate_categories-0.9.0/climate_categories/__init__.py` & `climate_categories-0.9.1/climate_categories/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Access to all categorizations is provided directly at the module level, using the
 names of categorizations. To access the example categorization `Excat`, simply use
 `climate_categories.Excat` .
 """
 
 __author__ = """Mika Pflüger"""
 __email__ = "mika.pflueger@climate-resource.com"
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 import importlib
 import importlib.resources
 
 from . import (
     search,
 )
```

### Comparing `climate_categories-0.9.0/climate_categories/_categories.py` & `climate_categories-0.9.1/climate_categories/_categories.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/_conversions.py` & `climate_categories-0.9.1/climate_categories/_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/BURDI.py` & `climate_categories-0.9.1/climate_categories/data/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/BURDI.yaml` & `climate_categories-0.9.1/climate_categories/data/BURDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/BURDI_class.py` & `climate_categories-0.9.1/climate_categories/data/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/BURDI_class.yaml` & `climate_categories-0.9.1/climate_categories/data/BURDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF1999.py` & `climate_categories-0.9.1/climate_categories/data/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF1999.yaml` & `climate_categories-0.9.1/climate_categories/data/CRF1999.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013.py` & `climate_categories-0.9.1/climate_categories/data/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013.yaml` & `climate_categories-0.9.1/climate_categories/data/CRF2013.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013_2021.py` & `climate_categories-0.9.1/climate_categories/data/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013_2021.yaml` & `climate_categories-0.9.1/climate_categories/data/CRF2013_2021.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013_2022.py` & `climate_categories-0.9.1/climate_categories/data/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013_2022.yaml` & `climate_categories-0.9.1/climate_categories/data/CRF2013_2022.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013_2023.py` & `climate_categories-0.9.1/climate_categories/data/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRF2013_2023.yaml` & `climate_categories-0.9.1/climate_categories/data/CRF2013_2023.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRFDI.py` & `climate_categories-0.9.1/climate_categories/data/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRFDI.yaml` & `climate_categories-0.9.1/climate_categories/data/CRFDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRFDI_class.py` & `climate_categories-0.9.1/climate_categories/data/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/CRFDI_class.yaml` & `climate_categories-0.9.1/climate_categories/data/CRFDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/GCB.py` & `climate_categories-0.9.1/climate_categories/data/GCB.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/GCB.yaml` & `climate_categories-0.9.1/climate_categories/data/GCB.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/IPCC1996.py` & `climate_categories-0.9.1/climate_categories/data/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/IPCC1996.yaml` & `climate_categories-0.9.1/climate_categories/data/IPCC1996.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/IPCC2006.py` & `climate_categories-0.9.1/climate_categories/data/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/IPCC2006.yaml` & `climate_categories-0.9.1/climate_categories/data/IPCC2006.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/IPCC2006_PRIMAP.py` & `climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/IPCC2006_PRIMAP.yaml` & `climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/ISO3.py` & `climate_categories-0.9.1/climate_categories/data/ISO3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Do not edit this file. It was auto-generated from the
 # corresponding YAML file.
 spec = {
     "name": "ISO3",
     "title": "ISO 3166-1 countries with climate-relevant groupings",
     "comment": "Countries, regions, and other areas. Also includes information on groups like being included in Annex I of the UN Framework Convention on Climate Change.",
-    "references": "ISO 3166, https://www.iso.org/iso-3166-country-codes.html; iso-codes package, https://salsa.debian.org/iso-codes-team/iso-codes; UNFCCC Parties & Observers, https://unfccc.int/parties-observers; EU members, https://ec.europa.eu/eurostat/statistics-explained/; G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20; OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htmindex.php?title=Glossary:EU_enlargements ",
+    "references": "ISO 3166, https://www.iso.org/iso-3166-country-codes.html; iso-codes package, https://salsa.debian.org/iso-codes-team/iso-codes; UNFCCC Parties & Observers, https://unfccc.int/parties-observers; EU members, https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements; G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20; OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm; AOSIS members, https://www.aosis.org/about/member-states/",
     "institution": "UN",
     "hierarchical": True,
     "last_update": "2023-04-27",
     "version": "2023-04-27",
     "total_sum": False,
     "canonical_top_level_category": "World",
     "categories": {
@@ -1708,14 +1708,60 @@
             ],
         },
         "UNFCCC": {
             "title": "Parties to the UNFCCC",
             "comment": "Parties to the UN Framework Convention on Climate Change.",
             "children": [["Annex-I", "Non-Annex-I"]],
         },
+        "AOSIS": {
+            "title": "Alliance of Small Island States",
+            "children": [
+                [
+                    "ATG",
+                    "BHS",
+                    "BLZ",
+                    "BRB",
+                    "COK",
+                    "COM",
+                    "CPV",
+                    "CUB",
+                    "DMA",
+                    "DOM",
+                    "FJI",
+                    "FSM",
+                    "GNB",
+                    "GRD",
+                    "GUY",
+                    "HTI",
+                    "JAM",
+                    "KIR",
+                    "KNA",
+                    "LCA",
+                    "MDV",
+                    "MHL",
+                    "MUS",
+                    "NIU",
+                    "NRU",
+                    "PLW",
+                    "PNG",
+                    "SGP",
+                    "SLB",
+                    "STP",
+                    "SUR",
+                    "SYC",
+                    "TLS",
+                    "TON",
+                    "TTO",
+                    "TUV",
+                    "VCT",
+                    "VUT",
+                    "WSM",
+                ]
+            ],
+        },
         "G7": {
             "title": "Group of Seven",
             "children": [["CAN", "DEU", "EU_2020", "FRA", "GBR", "ITA", "JPN", "USA"]],
         },
         "G8": {
             "title": "Group of Eight",
             "children": [
```

### Comparing `climate_categories-0.9.0/climate_categories/data/ISO3.yaml` & `climate_categories-0.9.1/climate_categories/data/ISO3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 name: ISO3
 title: ISO 3166-1 countries with climate-relevant groupings
 comment: Countries, regions, and other areas. Also includes information on groups
   like being included in Annex I of the UN Framework Convention on Climate Change.
-references: 'ISO 3166, https://www.iso.org/iso-3166-country-codes.html; iso-codes
-  package, https://salsa.debian.org/iso-codes-team/iso-codes; UNFCCC Parties & Observers,
-  https://unfccc.int/parties-observers; EU members, https://ec.europa.eu/eurostat/statistics-explained/;
+references: ISO 3166, https://www.iso.org/iso-3166-country-codes.html; iso-codes package,
+  https://salsa.debian.org/iso-codes-team/iso-codes; UNFCCC Parties & Observers, https://unfccc.int/parties-observers;
+  EU members,
+  https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements;
   G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20;
-  OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htmindex.php?title=Glossary:EU_enlargements '
+  OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm;
+  AOSIS members, https://www.aosis.org/about/member-states/
 institution: UN
 hierarchical: true
 last_update: '2023-04-27'
 version: '2023-04-27'
 total_sum: false
 canonical_top_level_category: World
 categories:
@@ -2281,14 +2283,56 @@
       - ZWE
   UNFCCC:
     title: Parties to the UNFCCC
     comment: Parties to the UN Framework Convention on Climate Change.
     children:
     - - Annex-I
       - Non-Annex-I
+  AOSIS:
+    title: Alliance of Small Island States
+    children:
+    - - ATG
+      - BHS
+      - BLZ
+      - BRB
+      - COK
+      - COM
+      - CPV
+      - CUB
+      - DMA
+      - DOM
+      - FJI
+      - FSM
+      - GNB
+      - GRD
+      - GUY
+      - HTI
+      - JAM
+      - KIR
+      - KNA
+      - LCA
+      - MDV
+      - MHL
+      - MUS
+      - NIU
+      - NRU
+      - PLW
+      - PNG
+      - SGP
+      - SLB
+      - STP
+      - SUR
+      - SYC
+      - TLS
+      - TON
+      - TTO
+      - TUV
+      - VCT
+      - VUT
+      - WSM
   G7:
     title: Group of Seven
     children:
     - - CAN
       - DEU
       - EU_2020
       - FRA
```

### Comparing `climate_categories-0.9.0/climate_categories/data/RCMIP.py` & `climate_categories-0.9.1/climate_categories/data/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/RCMIP.yaml` & `climate_categories-0.9.1/climate_categories/data/RCMIP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/conversion.IPCC1996.IPCC2006.csv` & `climate_categories-0.9.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/gas.py` & `climate_categories-0.9.1/climate_categories/data/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/data/gas.yaml` & `climate_categories-0.9.1/climate_categories/data/gas.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/conftest.py` & `climate_categories-0.9.1/climate_categories/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/data/broken_hierarchical_categorization.yaml` & `climate_categories-0.9.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/data/broken_simple_categorization.yaml` & `climate_categories-0.9.1/climate_categories/tests/data/broken_simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/data/good_conversion_A.yaml` & `climate_categories-0.9.1/climate_categories/tests/data/good_conversion_A.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/data/hierarchical_categorization.yaml` & `climate_categories-0.9.1/climate_categories/tests/data/hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/data/simple_categorization.yaml` & `climate_categories-0.9.1/climate_categories/tests/data/simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/examples.py` & `climate_categories-0.9.1/climate_categories/tests/examples.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_climate_categories.py` & `climate_categories-0.9.1/climate_categories/tests/test_climate_categories.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_conversions.py` & `climate_categories-0.9.1/climate_categories/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_crf.py` & `climate_categories-0.9.1/climate_categories/tests/test_crf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_di.py` & `climate_categories-0.9.1/climate_categories/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_ipcc.py` & `climate_categories-0.9.1/climate_categories/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_iso3.py` & `climate_categories-0.9.1/climate_categories/tests/test_iso3.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,7 +38,11 @@
     assert len(climate_categories.ISO3["G8"].children[0]) == 9
     # in the G20, the EU is enumerated
     assert len(climate_categories.ISO3["G20"].children[0]) == 20
 
 
 def test_oecd():
     assert len(climate_categories.ISO3["OECD"].leaf_children[0]) == 38
+
+
+def test_aosis():
+    assert len(climate_categories.ISO3["AOSIS"].leaf_children[0]) == 39
```

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_overcounting.py` & `climate_categories-0.9.1/climate_categories/tests/test_overcounting.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_primap.py` & `climate_categories-0.9.1/climate_categories/tests/test_primap.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories/tests/test_search.py` & `climate_categories-0.9.1/climate_categories/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/climate_categories.egg-info/PKG-INFO` & `climate_categories-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: climate-categories
-Version: 0.9.0
+Name: climate_categories
+Version: 0.9.1
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -96,22 +96,26 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-14).
-pik-primap/climate_categories: climate_categories Version 0.9.0.
-Zenodo. https://doi.org/10.5281/zenodo.8039308
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-15).
+pik-primap/climate_categories: climate_categories Version 0.9.1.
+Zenodo. https://doi.org/10.5281/zenodo.8043234
 
 =========
 Changelog
 =========
 
+0.9.1 (2023-06-15)
+------------------
+* Add AOSIS country group to ISO3 categorization.
+
 0.9.0 (2023-06-14)
 ------------------
 * Add ISO3 terminology for countries, areas, and country groups including UNFCCC
   signatories and Annex-I and Non-Annex-I groups and the evolution of the EU over time.
 
 0.8.5 (2023-05-23)
 ------------------
```

### Comparing `climate_categories-0.9.0/climate_categories.egg-info/SOURCES.txt` & `climate_categories-0.9.1/climate_categories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/BURDI.py` & `climate_categories-0.9.1/data_generation/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/BURDI_class.py` & `climate_categories-0.9.1/data_generation/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/CRF1999.py` & `climate_categories-0.9.1/data_generation/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/CRF2013.py` & `climate_categories-0.9.1/data_generation/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/CRF2013_2021.py` & `climate_categories-0.9.1/data_generation/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/CRF2013_2022.py` & `climate_categories-0.9.1/data_generation/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/CRF2013_2023.py` & `climate_categories-0.9.1/data_generation/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/CRFDI.py` & `climate_categories-0.9.1/data_generation/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/CRFDI_class.py` & `climate_categories-0.9.1/data_generation/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/IPCC1996.py` & `climate_categories-0.9.1/data_generation/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/IPCC2006.py` & `climate_categories-0.9.1/data_generation/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/IPCC2006_PRIMAP.py` & `climate_categories-0.9.1/data_generation/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/ISO3.py` & `climate_categories-0.9.1/data_generation/ISO3.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,45 +23,95 @@
         "title": "The world",
         "alternative_codes": ["EARTH", "Earth", "WORLD"],
         "children": [list(categories.keys())],
     }
     categories = add_eu_categories(categories)
     categories = add_unfccc_categories(categories)
     categories = add_unfccc_names(categories)
+    categories = add_aosis(categories)
     categories = add_g7g20(categories)
     categories = add_oecd(categories)
     categories = add_historical_names(categories)
 
     spec = {
         "name": "ISO3",
         "title": "ISO 3166-1 countries with climate-relevant groupings",
         "comment": "Countries, regions, and other areas. Also includes information on "
         "groups like being included in Annex I of the UN Framework Convention on "
         "Climate Change.",
-        "references": "ISO 3166, https://www.iso.org/iso-3166-country-codes.html; "
-        "iso-codes package, https://salsa.debian.org/iso-codes-team/iso-codes; "
-        "UNFCCC Parties & Observers, https://unfccc.int/parties-observers; "
-        "EU members, https://ec.europa.eu/eurostat/statistics-explained/; "
-        "G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/"
-        "g7-und-g20; "
-        "OECD members, https://www.oecd.org/about/document/"
-        "ratification-oecd-convention.htm"
-        "index.php?title=Glossary:EU_enlargements ",
+        "references": """ISO 3166, https://www.iso.org/iso-3166-country-codes.html;
+iso-codes package, https://salsa.debian.org/iso-codes-team/iso-codes;
+UNFCCC Parties & Observers, https://unfccc.int/parties-observers;
+EU members,
+https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements;
+G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20;
+OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm;
+AOSIS members, https://www.aosis.org/about/member-states/""",
         "institution": "UN",
         "last_update": "2023-04-27",
         "hierarchical": True,
         "version": "2023-04-27",
         "total_sum": False,
         "categories": categories,
         "canonical_top_level_category": "WORLD",
     }
 
     return climate_categories.HierarchicalCategorization.from_spec(spec)
 
 
+def add_aosis(categories):
+    categories["AOSIS"] = {
+        "title": "Alliance of Small Island States",
+        "children": [
+            [
+                "ATG",
+                "BHS",
+                "BRB",
+                "BLZ",
+                "CUB",
+                "DMA",
+                "DOM",
+                "GRD",
+                "GUY",
+                "HTI",
+                "JAM",
+                "KNA",
+                "LCA",
+                "VCT",
+                "SUR",
+                "TTO",
+                "COK",
+                "FSM",
+                "FJI",
+                "KIR",
+                "NRU",
+                "NIU",
+                "PLW",
+                "PNG",
+                "MHL",
+                "WSM",
+                "SLB",
+                "TON",
+                "TUV",
+                "VUT",
+                "CPV",
+                "COM",
+                "GNB",
+                "MDV",
+                "MUS",
+                "STP",
+                "SYC",
+                "SGP",
+                "TLS",
+            ]
+        ],
+    }
+    return categories
+
+
 def add_historical_names(categories):
     categories["TUR"]["info"]["historical_names"] = ["Turkey"]
     return categories
 
 
 def add_oecd(categories):
     categories["OECD"] = {
```

### Comparing `climate_categories-0.9.0/data_generation/RCMIP.py` & `climate_categories-0.9.1/data_generation/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/gas.py` & `climate_categories-0.9.1/data_generation/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/data_generation/utils.py` & `climate_categories-0.9.1/data_generation/utils.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/docs/Makefile` & `climate_categories-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/docs/conf.py` & `climate_categories-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/docs/data.rst` & `climate_categories-0.9.1/docs/data.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/docs/installation.rst` & `climate_categories-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/docs/make.bat` & `climate_categories-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/docs/usage.ipynb` & `climate_categories-0.9.1/docs/usage.ipynb`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/setup.cfg` & `climate_categories-0.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climate_categories
-version = 0.9.0
+version = 0.9.1
 author = Mika Pflüger
 author_email = mika.pflueger@climate-resource.com
 description = Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/climate_categories
 project_urls =
```

### Comparing `climate_categories-0.9.0/tbump.toml` & `climate_categories-0.9.1/tbump.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/climate_categories/"
 
 [version]
-current = "0.9.0"
+current = "0.9.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `climate_categories-0.9.0/update_changelog.py` & `climate_categories-0.9.1/update_changelog.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.0/update_citation_info.py` & `climate_categories-0.9.1/update_citation_info.py`

 * *Files identical despite different names*

