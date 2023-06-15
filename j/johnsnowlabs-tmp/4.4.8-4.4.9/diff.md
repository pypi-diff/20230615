# Comparing `tmp/johnsnowlabs_tmp-4.4.8.tar.gz` & `tmp/johnsnowlabs_tmp-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs_tmp-4.4.8.tar", last modified: Fri May 26 06:24:33 2023, max compression
+gzip compressed data, was "johnsnowlabs_tmp-4.4.9.tar", last modified: Thu Jun 15 11:10:17 2023, max compression
```

## Comparing `johnsnowlabs_tmp-4.4.8.tar` & `johnsnowlabs_tmp-4.4.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.8/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.8/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9182 2023-05-26 06:23:57.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4528 2023-05-25 02:41:08.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2233 2023-05-26 06:24:30.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-05-21 06:35:03.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2486 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      114 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2045 2023-05-25 05:47:59.000000 johnsnowlabs_tmp-4.4.8/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.337892 johnsnowlabs_tmp-4.4.9/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.9/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-06-15 11:10:17.337892 johnsnowlabs_tmp-4.4.9/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.9/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.333892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.333892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.333892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.333892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-06-13 13:24:37.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.333892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.333892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-06-06 22:37:19.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4755 2023-06-07 00:53:32.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4703 2023-06-07 00:47:56.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4625 2023-06-07 00:48:11.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.333892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31557 2023-06-13 08:46:00.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2202 2023-06-15 11:10:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.337892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-06-14 20:24:15.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.337892 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-15 11:10:17.337892 johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-06-15 11:10:17.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2486 2023-06-15 11:10:17.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-06-15 11:10:17.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-06-15 11:10:17.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-06-15 11:10:17.000000 johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-06-15 11:10:17.337892 johnsnowlabs_tmp-4.4.9/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1904 2023-06-15 11:09:45.000000 johnsnowlabs_tmp-4.4.9/setup.py
```

### Comparing `johnsnowlabs_tmp-4.4.8/LICENSE` & `johnsnowlabs_tmp-4.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/PKG-INFO` & `johnsnowlabs_tmp-4.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs_tmp
-Version: 4.4.8
+Version: 4.4.9
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs_tmp-4.4.8/README.md` & `johnsnowlabs_tmp-4.4.9/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/__init__.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
 
         if cls.has_secret:
             if settings.enforce_versions:
                 url = compat_map[matching_jsl_spark_release][install_type].url.format(
                     secret=secret, lib_version=cls.lib_version.as_str()
                 )
             else:
-                # Read Version from secret
+                # Parse Version from secret
                 url = compat_map[matching_jsl_spark_release][install_type].url.format(
-                    secret=secret, lib_version=secret.split("-")[0]
+                    secret=secret, lib_version=secret.split("-")[0].replace(".PR",'')
                 )
 
         else:
             if settings.enforce_versions:
                 url = compat_map[matching_jsl_spark_release][install_type].url.format(
                     lib_version=cls.lib_version.as_str()
                 )
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/jsl_home.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,16 @@
     aws_key_id: Optional[str] = None,
     fin_license: Optional[str] = None,
     leg_license: Optional[str] = None,
     store_in_jsl_home: bool = True,
     log: bool = True,
 ) -> InstallSuite:
     """Read all info files from JSL home if exists. If not exists, sets up JSL home"""
-
+    if not jsl_home_exist() and not create_jsl_home_if_missing:
+        return InstallSuite.empty()
     license_data: JslSecrets = JslSecrets.build_or_try_find_secrets(
         browser_login=browser_login,
         force_browser=force_browser,
         access_token=access_token,
         local_license_number=local_license_number,
         remote_license_number=remote_license_number,
         secrets_file=secrets_file,
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/auto_install/softwares.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,18 +177,15 @@
     hard_dependencies = {SparkNlpSoftware}
     licensed_dependencies = {SparkHcSoftware, SparkOcrSoftware}
     optional_dependencies = {
         NlpDisplaySoftware
     }  # Todo streamlit,sklearn,plotly, nlp-display
     latest_version = LatestCompatibleProductVersion.nlu.value
     py_module_name = "nlu"
-    # pypi_name = "nlu"
-    pypi_name = "nlu_tmp"
-    # nlu_tmp==
-
+    pypi_name = "nlu"
     install_deps = False
 
     @classmethod
     def get_installed_version_via_import(cls):
         try:
             import nlu
 
@@ -219,15 +216,15 @@
 
     hard_dependencies = {SparkNlpSoftware}
     licensed_dependencies = {SparkHcSoftware, SparkOcrSoftware}
     optional_dependencies = {NlpDisplaySoftware, NluSoftware}
     latest_version = LatestCompatibleProductVersion.jsl_lib.value
     py_module_name = "johnsnowlabs"
     pypi_name = "johnsnowlabs"
-    pypi_name_databricks = "johnsnowlabs_for_databricks_tmp"
+    pypi_name_databricks = "johnsnowlabs_for_databricks"
 
 
 class JslFullSoftware(AbstractSoftwareProduct):
     name = ProductName.jsl_full.value
     logo = ProductLogo.jsl_full.value
     slogan = ProductSlogan.jsl_full.value
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/finance.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/finance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import traceback
 
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_broken_lib
 
 try:
-
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         from sparknlp_jsl.functions import *
         from sparknlp_jsl.training import *
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.base import FeaturesAssembler
         from sparknlp_jsl.annotator.windowed.windowed_sentence import (
             WindowedSentenceModel,
@@ -83,22 +82,23 @@
             DocumentLogRegClassifierApproach,
             RelationExtractionApproach,
             ChunkMergeApproach,
             NerDisambiguator,
             ContextualParserApproach,
             GenericClassifierApproach,
             Router,
-            NerQuestionGenerator,
             Replacer,
-            # NEW
             ContextualParserModel,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             Resolution2Chunk,
             ResolverMerger,
+            NerTemplateRenderModel,
+            AverageEmbeddings,
+            Doc2ChunkInternal,
         )
 
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/legal.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/legal.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,20 +82,22 @@
             DocumentLogRegClassifierApproach,
             RelationExtractionApproach,
             ChunkMergeApproach,
             NerDisambiguator,
             ContextualParserApproach,
             GenericClassifierApproach,
             Router,
-            NerQuestionGenerator,
             AssertionChunkConverter,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             # Resolution2Chunk,
             ResolverMerger,
+            NerTemplateRenderModel,
+            AverageEmbeddings,
+            Doc2ChunkInternal,
         )
         from sparknlp_jsl.modelTracer import ModelTracer
 
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
 
         from sparknlp_jsl import training_log_parser, Deid
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/medical.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/medical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import traceback
+
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.auto_install.softwares import Software
 from johnsnowlabs.utils.env_utils import reverse_compatibility_import
 from johnsnowlabs.utils.print_messages import log_outdated_lib, log_broken_lib
 
 warning_logged = False
 
-
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         from sparknlp_jsl.functions import *
         from sparknlp_jsl.training import *
         from sparknlp_jsl.annotator.windowed.windowed_sentence import (
             WindowedSentenceModel,
         )
@@ -69,15 +69,17 @@
             DocMapperApproach,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             DocumentMLClassifierApproach,
             DocumentMLClassifierModel,
             Resolution2Chunk,
             MedicalQuestionAnswering,
-
+            NerTemplateRenderModel,
+            AverageEmbeddings,
+            Doc2ChunkInternal,
         )
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.base import FeaturesAssembler
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/nlp.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/install_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,23 +100,26 @@
     def py_folder_from_home():
         if os.path.exists(settings.py_info_file):
             return InstallFolder.parse_file(settings.py_info_file)
         return False
 
 
 class InstallSuite(WritableBaseModel):
-    info: RootInfo
+    info: Optional[RootInfo] = None
     secrets: Optional[JslSecrets] = None
     # Py4J Libs
-    nlp: LocalPy4JLib
+    nlp: Optional[LocalPy4JLib] = None
     ocr: Optional[LocalPy4JLib] = None
     hc: Optional[LocalPy4JLib] = None
     # Pure Python Libs
     pure_py_jsl: Optional[LocalPyLib] = None
 
+    @staticmethod
+    def empty():
+        return InstallSuite()
     def get_missing_products(self, nlp, visual, spark_nlp):
         missing = []
         from johnsnowlabs.auto_install.softwares import Software
 
         if self.secrets.OCR_LICENSE and visual:
             if not self.ocr.java_lib or not self.ocr.get_java_path():
                 missing.append(Software.spark_ocr)
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,14 @@
             JslSecrets.store_in_jsl_home_if_new(secrets)
             return secrets
 
         return False
 
     @staticmethod
     def dict_has_jsl_secrets(secret_dict: Dict[str, str]) -> bool:
-
         for key in secret_json_keys:
             if key in secret_dict:
                 return True
         return False
 
     @staticmethod
     def search_env_vars() -> Union["JslSecrets", bool]:
@@ -403,14 +402,22 @@
                 OCR_VERSION=ocr_version,
                 NLP_VERSION=nlp_version,
                 AWS_ACCESS_KEY_ID=aws_access_key_id,
                 AWS_SECRET_ACCESS_KEY=aws_access_key,
                 JSL_LEGAL_LICENSE=leg_license,
                 JSL_FINANCE_LICENSE=fin_license,
             )
+        else:
+            # Check for License json
+            if "JOHNSNOWLABS_LICENSE_JSON" in os.environ:
+                json_dict = json.loads(os.environ["JOHNSNOWLABS_LICENSE_JSON"])
+                if JslSecrets.dict_has_jsl_secrets(json_dict):
+                    print("👌 License detected in Environment Variables")
+                    return JslSecrets.from_json_dict(json_dict)
+
         return False
 
     @staticmethod
     def search_default_locations(license_number=0) -> Union["JslSecrets", bool]:
         """
         Search default google colab folder and current working dir for
         for JSL Secret json file
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/settings.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.4.8"
-raw_version_nlp = "4.4.1"
-# raw_version_nlu = "4.2.0"
-raw_version_nlu = "4.3.0rc3"
+
+raw_version_jsl_lib = "4.4.9"
+raw_version_nlp = "4.4.4"
+raw_version_nlu = "4.2.2"
 
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "4.4.2"
-raw_version_secret_medical = "4.4.2"
+raw_version_medical = "4.4.3"
+raw_version_secret_medical = "4.4.3"
 
-raw_version_secret_ocr = "4.4.1"
-raw_version_ocr = "4.4.1"
+raw_version_secret_ocr = "4.4.2"
+raw_version_ocr = "4.4.2"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
-
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
 
 # Environment
 on_databricks = is_running_in_databricks()
 license_required = env_required_license()
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/enums.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/env_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,12 +117,16 @@
     ):
         return False
     return True
 
 
 def set_py4j_logger_to_error_on_databricks():
     # Only call this when in Databricks
-    import logging
-    from pyspark.sql import SparkSession
-
-    logger = SparkSession.builder.getOrCreate()._jvm.org.apache.log4j
-    logging.getLogger("py4j.java_gateway").setLevel(logging.ERROR)
+    try:
+        if 'SKIP_py4j_DISABLE' in os.environ and os.environ['SKIP_py4j_DISABLE'] == '1':
+            return
+        import logging
+        from pyspark.sql import SparkSession
+        logger = SparkSession.builder.getOrCreate()._jvm.org.apache.log4j
+        logging.getLogger("py4j.java_gateway").setLevel(logging.ERROR)
+    except:
+        pass
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/functional.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/py_process.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs/visual.py` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/PKG-INFO` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs-tmp
-Version: 4.4.8
+Version: 4.4.9
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/SOURCES.txt` & `johnsnowlabs_tmp-4.4.9/johnsnowlabs_tmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.8/setup.py` & `johnsnowlabs_tmp-4.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,43 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 REQUIRED_PKGS = [
-    # f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
+    f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
     f"spark-nlp=={johnsnowlabs.settings.raw_version_nlp}",
     f"nlu=={johnsnowlabs.settings.raw_version_nlu}",
     f"spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}",
     "numpy",
     "dataclasses",
     "requests",
     "databricks-api",
     "pydantic",
     "colorama",
 ]
 
 setup(
     version=johnsnowlabs.settings.raw_version_jsl_lib,
     name="johnsnowlabs_tmp",
-    # name="johnsnowlabs",
+    # name="johnsnowlabs_for_databricks",
     description="The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for "
     "Finance, Legal and Medical domains. Easily scalable to Spark Cluster ",
     long_description=long_description,
     install_requires=REQUIRED_PKGS,
     long_description_content_type="text/markdown",
     url="https://www.johnsnowlabs.com/",
     author="John Snow Labs",
     author_email="christian@johnsnowlabs.com",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
     ],
     keywords="Spark NLP OCR Finance Legal Medical John Snow Labs  ",
     packages=find_packages(exclude=["test*", "tmp*"]),  # exclude=['test']
```

