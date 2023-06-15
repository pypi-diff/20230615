# Comparing `tmp/terraform-compliance-1.3.8.tar.gz` & `tmp/terraform-compliance-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/terraform-compliance-1.3.8.tar", last modified: Mon Dec  7 15:48:05 2020, max compression
+gzip compressed data, was "dist/terraform-compliance-1.3.9.tar", last modified: Sun Jan 10 23:48:54 2021, max compression
```

## Comparing `terraform-compliance-1.3.8.tar` & `terraform-compliance-1.3.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/
--rw-r--r--   0 runner    (1001) docker     (116)     7607 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2609 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/override_radish_hookerrors.py
--rw-r--r--   0 runner    (1001) docker     (116)     2632 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/silent_formatter.py
--rw-r--r--   0 runner    (1001) docker     (116)     6695 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/override_radish_step.py
--rw-r--r--   0 runner    (1001) docker     (116)     3162 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/ext_radish_bdd.py
--rw-r--r--   0 runner    (1001) docker     (116)    20303 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/terraform.py
--rw-r--r--   0 runner    (1001) docker     (116)    16383 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/extensions/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)      104 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/common/
--rw-r--r--   0 runner    (1001) docker     (116)     3798 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/bdd_tags.py
--rw-r--r--   0 runner    (1001) docker     (116)    21639 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2376 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/defaults.py
--rw-r--r--   0 runner    (1001) docker     (116)     4498 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (116)     1523 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/readable_dir.py
--rw-r--r--   0 runner    (1001) docker     (116)      673 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/pip_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     3510 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/terraform_files.py
--rw-r--r--   0 runner    (1001) docker     (116)      359 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3582 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/common/readable_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/steps/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/steps/given/
--rw-r--r--   0 runner    (1001) docker     (116)     7506 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/given/i_have_name_section_configured.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/given/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1200 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/security_group_related.py
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/it_must_be_in.py
--rw-r--r--   0 runner    (1001) docker     (116)      470 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/interpolations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1323 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/property_is_enabled.py
--rw-r--r--   0 runner    (1001) docker     (116)     6592 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/its_value_condition_match_the_search_regex.py
--rw-r--r--   0 runner    (1001) docker     (116)    11668 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/it_must_contain_something.py
--rw-r--r--   0 runner    (1001) docker     (116)     1149 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/it_must_have_reference_address_referenced.py
--rw-r--r--   0 runner    (1001) docker     (116)     2570 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/its_value_condition_contain.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/its_value_condition_be_null.py
--rw-r--r--   0 runner    (1001) docker     (116)     2908 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/then/its_key_condition_be_value.py
--rw-r--r--   0 runner    (1001) docker     (116)     1601 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10374 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/steps.py
--rw-r--r--   0 runner    (1001) docker     (116)     4804 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/terrain.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance/steps/when/
--rw-r--r--   0 runner    (1001) docker     (116)     5941 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/when/its_key_is_value.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/when/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4012 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/when/maths.py
--rw-r--r--   0 runner    (1001) docker     (116)    14453 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/terraform_compliance/steps/when/it_contains_something.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/tests/terraform_compliance/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/tests/terraform_compliance/extensions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22981 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/extensions/test_terraform.py
--rw-r--r--   0 runner    (1001) docker     (116)      816 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/extensions/test_ext_radish_bdd.py
--rw-r--r--   0 runner    (1001) docker     (116)    13381 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/extensions/test_security_groups.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/
--rw-r--r--   0 runner    (1001) docker     (116)    10696 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     2519 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/test_readable_plan.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      637 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/test_terraform_files.py
--rw-r--r--   0 runner    (1001) docker     (116)      354 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/test_pip_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)      701 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/test_bdd_tags.py
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/common/test_readable_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/tests/terraform_compliance/steps/
--rw-r--r--   0 runner    (1001) docker     (116)     2494 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/steps/test_its_key_value_step.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    44592 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/steps/test_main_steps.py
--rw-r--r--   0 runner    (1001) docker     (116)      610 2020-12-07 15:47:42.000000 terraform-compliance-1.3.8/tests/terraform_compliance/steps/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)       72 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     3143 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)      184 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/terraform_compliance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5815 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2020-12-07 15:48:05.000000 terraform-compliance-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1865 2020-12-07 15:47:41.000000 terraform-compliance-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1167 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      184 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       72 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     3143 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-10 23:48:53.000000 terraform-compliance-1.3.9/terraform_compliance.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/
+-rw-r--r--   0 runner    (1001) docker     (116)     3162 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/ext_radish_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16383 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22216 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6695 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/override_radish_step.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2609 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/override_radish_hookerrors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2632 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/silent_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance/steps/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance/steps/when/
+-rw-r--r--   0 runner    (1001) docker     (116)    14453 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/when/it_contains_something.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4012 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/when/maths.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5941 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/when/its_key_is_value.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/when/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/
+-rw-r--r--   0 runner    (1001) docker     (116)     2164 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/its_value_condition_be_null.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1200 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/security_group_related.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6592 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/its_value_condition_match_the_search_regex.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1149 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/it_must_have_reference_address_referenced.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1110 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/it_must_be_in.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11668 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/it_must_contain_something.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2908 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/its_key_condition_be_value.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2570 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/its_value_condition_contain.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      470 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/interpolations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1323 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/then/property_is_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10534 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/steps.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4804 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1601 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance/steps/given/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/given/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7835 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/steps/given/i_have_name_section_configured.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/terraform_compliance/common/
+-rw-r--r--   0 runner    (1001) docker     (116)     3798 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/bdd_tags.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4522 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3510 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/terraform_files.py
+-rw-r--r--   0 runner    (1001) docker     (116)      359 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)      673 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/pip_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2376 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3582 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/readable_plan.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21846 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1523 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/common/readable_dir.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7607 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/terraform_compliance/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)      104 2021-01-10 23:48:53.000000 terraform-compliance-1.3.9/terraform_compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1167 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1865 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)       61 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/tests/terraform_compliance/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/tests/terraform_compliance/extensions/
+-rw-r--r--   0 runner    (1001) docker     (116)      816 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/extensions/test_ext_radish_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13381 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/extensions/test_security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25417 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/extensions/test_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/tests/terraform_compliance/steps/
+-rw-r--r--   0 runner    (1001) docker     (116)     2494 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/steps/test_its_key_value_step.py
+-rw-r--r--   0 runner    (1001) docker     (116)    44592 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/steps/test_main_steps.py
+-rw-r--r--   0 runner    (1001) docker     (116)      610 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/steps/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:54.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/
+-rw-r--r--   0 runner    (1001) docker     (116)      354 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/test_pip_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10696 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (116)      637 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/test_terraform_files.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1505 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/test_readable_dir.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2519 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/test_readable_plan.py
+-rw-r--r--   0 runner    (1001) docker     (116)      701 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/test_bdd_tags.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/tests/terraform_compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5815 2021-01-10 23:48:29.000000 terraform-compliance-1.3.9/README.md
```

### Comparing `terraform-compliance-1.3.8/terraform_compliance/main.py` & `terraform-compliance-1.3.9/terraform_compliance/main.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/extensions/override_radish_hookerrors.py` & `terraform-compliance-1.3.9/terraform_compliance/extensions/override_radish_hookerrors.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/extensions/silent_formatter.py` & `terraform-compliance-1.3.9/terraform_compliance/extensions/silent_formatter.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/extensions/override_radish_step.py` & `terraform-compliance-1.3.9/terraform_compliance/extensions/override_radish_step.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/extensions/ext_radish_bdd.py` & `terraform-compliance-1.3.9/terraform_compliance/extensions/ext_radish_bdd.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/extensions/terraform.py` & `terraform-compliance-1.3.9/terraform_compliance/extensions/terraform.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.data = {}
 
         self.providers = {}
 
         self.configuration = dict(resources={}, variables={})
         self.file_type = "plan"
         self.resources_raw = {}
+        self.type_to_after_unknown_properties = {}
         self.parse_it = parse_it
 
         if parse_it:
             self.cache = Cache()
             self.parse()
 
     def _version_check(self):
@@ -130,25 +131,58 @@
         # Resource Changes ( exists in Plan )
         for finding in self.raw.get('resource_changes', {}):
             resource = deepcopy(finding)
             change = resource.get('change', {})
             actions = change.get('actions', [])
             if actions != ['delete']:
                 resource['values'] = change.get('after', {}) # dict_merge(change.get('after', {}), change.get('after_unknown', {}))
+                self.remember_after_unknown(resource, change.get('after_unknown', {}))
                 if 'change' in resource:
                     del resource['change']
 
                 if self.is_type(resource, 'data'):
                     self.data[resource['address']] = resource
                 else:
                     self.resources[resource['address']] = resource
 
         if self.parse_it:
             self.cache.set('resources', self.resources)
 
+    '''
+    Creates a map of resource type to after_unknown values
+    These can be used in given step "resource that supports x"
+    
+    Note: This function may be extended to capture 'after' values as well. That would require flattening the multi level
+    dictionaries in resource
+    '''
+    def remember_after_unknown(self, resource, after_unknown):
+        # get type
+        resource_type = resource.get('type', '')
+
+        # if resource doesn't have type field, try to extract it from address (ideally, this if never evaluates true)
+        if not resource_type and 'address' in resource and resource['address']:
+            parsed_address = resource.get('address').split('.')
+            if parsed_address != 'module':
+                resource_type = parsed_address[0]
+            elif len(parsed_address) >= 3:
+                resource_type = parsed_address[2]
+            else:
+                return
+
+        # get after_unknown values
+
+        # need to merge because which values are in after_unknown may change from instance to instance
+        # merging rule: if field not in map, add it
+        if resource_type not in self.type_to_after_unknown_properties:
+            self.type_to_after_unknown_properties[resource_type] = after_unknown
+        else:
+            for key, value in after_unknown.items():
+                if key not in self.type_to_after_unknown_properties[resource_type]:
+                    self.type_to_after_unknown_properties[resource_type][key] = value
+
     def _parse_configurations(self):
         '''
         Assigns all configuration related data defined in the terraform plan. This is mostly used for
         resources referencing each other.
 
         :return: none
         '''
@@ -330,25 +364,26 @@
 
                     # This is where we synchronise constant_value in the configuration section with the resource
                     # for filling up the missing elements that hasn't been defined in the resource due to provider
                     # implementation.
                     target_resource = [t for t in [self.resources.get(resource, {}).get('address')] if t is not None]
                     if not target_resource:
                         target_resource = [k for k in self.resources.keys() if k.startswith(resource)]
-                        if not target_resource:
-                            target_resource = [k for k in self.resources.keys() if k.endswith(resource)]
 
                     for t_r in target_resource:
                         if type(value) is type(self.resources[t_r]['values'].get(key)) and self.resources[t_r]['values'].get(key) != value:
                             if isinstance(value, (list, dict)):
                                 merge_dicts(self.resources[t_r]['values'][key], value)
 
                 if ref_list:
                     ref_type = self.configuration['resources'][resource]['expressions'].get('type', {})
 
+                    if 'references' in ref_type:
+                        ref_type = resource.split('.')[0]
+
                     if not ref_type and not self.is_type(resource, 'data'):
                         resource_type, resource_id = resource.split('.')
                         ref_type = resource_type
 
                     for k, v in ref_list.items():
                         v = flatten_list(v)
 
@@ -389,26 +424,29 @@
 
         if self.file_type == 'plan':
             self._parse_variables()
             self._parse_configurations()
 
         cache_mounted_resources = self.cache.get('mounted_resources') if self.parse_it else None
         cache_raw_resources = self.cache.get('resources_raw') if self.parse_it else None
+        cache_type_to_after_unknown_properties = self.cache.get('type_to_after_unknown_properties') if self.parse_it else None
 
         if cache_mounted_resources and cache_raw_resources:
             # print('Read from cache, instead of re-mounting.')
             self.resources = cache_mounted_resources
             self.resources_raw = cache_raw_resources
+            self.type_to_after_unknown_properties = cache_type_to_after_unknown_properties
         else:
             # print('Building cache for mounted resources at {}'.format(Defaults.cache_dir))
             self._mount_references()
 
             if self.parse_it:
                 self.cache.set('mounted_resources', self.resources)
                 self.cache.set('resources_raw', self.resources_raw)
+                self.cache.set('type_to_after_unknown_properties', self.type_to_after_unknown_properties)
 
         self._distribute_providers()
 
         for _, resource in self.resources.items():
             self._expand_resource_tags(resource)
 
     def find_resources_by_type(self, resource_type, match=Match(case_sensitive=False)):
```

### Comparing `terraform-compliance-1.3.8/terraform_compliance/extensions/security_groups.py` & `terraform-compliance-1.3.9/terraform_compliance/extensions/security_groups.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/bdd_tags.py` & `terraform-compliance-1.3.9/terraform_compliance/common/bdd_tags.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/helper.py` & `terraform-compliance-1.3.9/terraform_compliance/common/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,14 +532,26 @@
     return True
 
 def merge_dicts(source, target):
     '''
     successor of dict_merge
     merges two dictionaries or lists into one
     overlapping list/dictionaries are also merged within each other
+   
+    assume target is low priority
+
+    conflicts
+        regular values: higher prio overrides
+        dictionaries: merge conflicting dictionaries
+        lists: higher prio overrides for regular values, merge any matching dictionary/list elements
+            if len(target) > len(source):
+                append the tail to the source
+
+
+    # Confusing and less important comments:
     if isinstance(source, list) and isinstance(target, list):
         # shady, just extend?
         for i, v in enumerate(higher prio):
             if v is dict
                 if lower has dict in the ith element
                     combine them
     if isinstance(source, dict) and isinstance(target, dict):
@@ -561,25 +573,20 @@
         what happens to conflicting dirs?
     if I have two lists
         lists have dictionaries in the same index
             merge those dictionaries
 
         # add remaining values of lower priority to higher priority
         ignore non dict values
-
-    conflicts
-        regular values: higher prio overrides
-        dictionaries: merge conflicting dictionaries
-        lists: higher prio overrides, merge any matching dictionary elements
-
-    assume target is low priority
     '''
     if isinstance(source, list) and isinstance(target, list):
         for i, value in enumerate(target):
-            if isinstance(value, dict) and isinstance(source[i], dict): # what if i not in source?
+            if i >= len(source):
+                source.append(value)
+            elif isinstance(value, dict) and isinstance(source[i], dict):
                 merge_dicts(source[i], target[i])
             elif isinstance(value, list) and isinstance(source[i], list):
                 merge_dicts(source[i], target[i])
 
     if isinstance(source, dict) and isinstance(target, dict):
         for key, value in target.items():
             if key not in source:
```

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/defaults.py` & `terraform-compliance-1.3.9/terraform_compliance/common/defaults.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/error_handling.py` & `terraform-compliance-1.3.9/terraform_compliance/common/error_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,8 @@
     def _fail_step(self, step_id):
         for step in self.step_obj.parent.all_steps:
             if step.id == step_id:
                 step.state = Step.State.FAILED
                 step.failure = WrapperError(self.exception('\r{}'.format(' '*len(self.exception_name))))
 
         if self.message:
-            self.step_obj.failure.traceback = '{}: {}'.format(self.exception_name, '\n'.join(self.message)).replace('\x00', '\\x00') 
+            self.step_obj.failure.traceback = '{}: {}'.format(self.exception_name, '\n'.join(self.message)).replace('\x00', '\\x00').replace('\x08', '\\x08')
```

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/readable_dir.py` & `terraform-compliance-1.3.9/terraform_compliance/common/readable_dir.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/pip_helper.py` & `terraform-compliance-1.3.9/terraform_compliance/common/pip_helper.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/terraform_files.py` & `terraform-compliance-1.3.9/terraform_compliance/common/terraform_files.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/common/readable_plan.py` & `terraform-compliance-1.3.9/terraform_compliance/common/readable_plan.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/given/i_have_name_section_configured.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/given/i_have_name_section_configured.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,17 +68,23 @@
         _step_obj.context.addresses = 'variable'
         _step_obj.context.property_name = 'variable'
         return True
 
     elif name.startswith('resource that supports'):
         filter_property = re.match(r'resource that supports (.*)', name).group(1)
 
-        resource_types_supports_tags = find_root_by_key(_terraform_config.config.terraform.resources_raw,
+        resource_types_supports_tags = set(find_root_by_key(_terraform_config.config.terraform.resources_raw,
                                                         filter_property,
-                                                        return_key='type')
+                                                        return_key='type'))
+
+        # look for after_unknown values in case they were omitted
+        for resource_type, after_unknown_properties in _terraform_config.config.terraform.type_to_after_unknown_properties.items():
+            if filter_property in after_unknown_properties:
+                resource_types_supports_tags.add(resource_type)
+
         resource_list = []
         for resource_type in resource_types_supports_tags:
             # Issue-168: Mounted resources causes problem on recursive searching for resources that supports tags
             #            We are removing all mounted resources here for future steps, since we don't need them for
             #            tags checking.
             found_resources = remove_mounted_resources(_terraform_config.config.terraform.find_resources_by_type(resource_type, match))
             found_resources = transform_asg_style_tags(found_resources)
```

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/security_group_related.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/security_group_related.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/it_must_be_in.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/it_must_be_in.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/property_is_enabled.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/property_is_enabled.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/its_value_condition_match_the_search_regex.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/its_value_condition_match_the_search_regex.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/it_must_contain_something.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/it_must_contain_something.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/it_must_have_reference_address_referenced.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/it_must_have_reference_address_referenced.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/its_value_condition_contain.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/its_value_condition_contain.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/its_value_condition_be_null.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/its_value_condition_be_null.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/then/its_key_condition_be_value.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/then/its_key_condition_be_value.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/__init__.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/steps.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from terraform_compliance.steps.then.its_value_condition_contain import its_value_condition_contain
 from terraform_compliance.steps.then.it_must_have_reference_address_referenced import it_must_have_reference_address_referenced
 from terraform_compliance.steps.then.its_key_condition_be_value import its_key_condition_be_value
 from terraform_compliance.steps.then.interpolations import i_flatten_everything_found
 from terraform_compliance.steps.then.it_must_be_in import it_must_be_in
 from terraform_compliance.steps.then.its_value_condition_be_null import its_value_condition_be_null
 
+# {name} is checked for startswith("resource that supports "). The @given decorator for that documented case is not needed
 @given(u'I have {name:ANY} defined')
 @given(u'I have {name:ANY} {type_name:SECTION} configured')
 def wrapper(_step_obj, name, type_name='resource', _terraform_config=world):
     return i_have_name_section_configured(_step_obj, name, type_name, _terraform_config)
 
 
 @when(u'its {key:PROPERTY} is {value:PROPERTY}')
@@ -124,14 +125,15 @@
 @then(u'they must not contain {something:PROPERTY_COMPAT}')
 @then(u'it must not have {something:PROPERTY_COMPAT}')
 @then(u'they must not have {something:PROPERTY_COMPAT}')
 def wrapper(_step_obj, something, inherited_values=Null):
     return it_must_not_contain_something(_step_obj, something, inherited_values=Null)
 
 
+@then(u'{something:ANY} is enabled')
 @then(u'{something:ANY} is be enabled')
 @then(u'{something:ANY} must be enabled')
 def wrapper(_step_obj, something):
     return property_is_enabled(_step_obj, something)
 
 
 @when(u'I {action_type:PROPERTY} it')
```

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/terrain.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/terrain.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/when/its_key_is_value.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/when/its_key_is_value.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/when/maths.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/when/maths.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance/steps/when/it_contains_something.py` & `terraform-compliance-1.3.9/terraform_compliance/steps/when/it_contains_something.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/extensions/test_terraform.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/extensions/test_terraform.py`

 * *Files 8% similar despite different names*

```diff
@@ -590,7 +590,61 @@
             }
         }
         obj._expand_resource_tags(obj.resources['provider_resource_id'])
         obj._expand_resource_tags(obj.resources['other-provider_other_resource_id'])
         self.assertTrue('tags' not in obj.resources['other-provider_other_resource_id']['values'])
         self.assertEqual(value, obj.resources['provider_resource_id']['values']['tags'][0])
 
+    @patch.object(TerraformParser, '_read_file', return_value={})
+    def test_remember_after_unknown_simple(self, *args):
+        obj = TerraformParser('somefile', parse_it=False)
+        resource = {
+            'type': 'resource_type',
+        }
+
+        after_unknown_values = {'property_{}'.format(i): i for i in range(10)}
+        obj.remember_after_unknown(resource, after_unknown_values)
+
+        self.assertTrue(resource['type'] in obj.type_to_after_unknown_properties)
+
+        for key in after_unknown_values:
+            mapped_after_unknown_value = obj.type_to_after_unknown_properties[resource['type']][key]
+            self.assertEqual(mapped_after_unknown_value, after_unknown_values[key])
+    
+    @patch.object(TerraformParser, '_read_file', return_value={})
+    def test_remember_after_unknown(self, *args):
+        obj = TerraformParser('somefile', parse_it=False)
+
+        # test parameters (not all combinations will cover all properties for all types)
+        len_resources = 20
+        len_properties = 20
+        len_types = 3
+
+        # create resources that falls into specific types
+        resources = {
+            'resource_{}'.format(i): {'type': 'type_{}'.format(i % len_types)} for i in range(len_resources)
+        }
+        
+        # create after_unknown for each.
+        # resource will have varying after_unknown values despite belonging the same type
+        resource_to_after_unknown_values = {}
+        for j, resource in enumerate(resources):
+            if j < 3:
+                resource_to_after_unknown_values[resource] = {}
+            else:
+                resource_to_after_unknown_values[resource] = {'property_{}'.format(i): i for i in range(j % 2, len_properties, 2)}
+
+        # check if all after_unknown values are accumulated correctly per each resource type
+        for resource_name, resource in resources.items():
+            obj.remember_after_unknown(resource, resource_to_after_unknown_values[resource_name])
+
+
+        for i in range(len_types):
+            t = 'type_{}'.format(i)
+
+            self.assertTrue(t in obj.type_to_after_unknown_properties)
+
+            for property_value in range(len_properties):
+                property_key = 'property_{}'.format(property_value)
+
+                mapped_after_unknown_value = obj.type_to_after_unknown_properties[t][property_key]
+                self.assertEqual(mapped_after_unknown_value, property_value)
```

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/extensions/test_ext_radish_bdd.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/extensions/test_ext_radish_bdd.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/extensions/test_security_groups.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/extensions/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/common/test_helper.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/common/test_helper.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/common/test_readable_plan.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/common/test_readable_plan.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/common/test_terraform_files.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/common/test_terraform_files.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/common/test_bdd_tags.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/common/test_bdd_tags.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/common/test_readable_dir.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/common/test_readable_dir.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/steps/test_its_key_value_step.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/steps/test_its_key_value_step.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/steps/test_main_steps.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/steps/test_main_steps.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/tests/terraform_compliance/steps/test_types.py` & `terraform-compliance-1.3.9/tests/terraform_compliance/steps/test_types.py`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance.egg-info/SOURCES.txt` & `terraform-compliance-1.3.9/terraform_compliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/terraform_compliance.egg-info/PKG-INFO` & `terraform-compliance-1.3.9/terraform_compliance.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: terraform-compliance
-Version: 1.3.8
+Version: 1.3.9
 Summary: BDD test framework for terraform
 Home-page: https://github.com/eerkunt/terraform-compliance
 Author: Emre Erkunt
 Author-email: emre.erkunt@gmail.com
 License: MIT
 Description: 
         BDD test framework for terraform
```

### Comparing `terraform-compliance-1.3.8/README.md` & `terraform-compliance-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `terraform-compliance-1.3.8/PKG-INFO` & `terraform-compliance-1.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: terraform-compliance
-Version: 1.3.8
+Version: 1.3.9
 Summary: BDD test framework for terraform
 Home-page: https://github.com/eerkunt/terraform-compliance
 Author: Emre Erkunt
 Author-email: emre.erkunt@gmail.com
 License: MIT
 Description: 
         BDD test framework for terraform
```

### Comparing `terraform-compliance-1.3.8/setup.py` & `terraform-compliance-1.3.9/setup.py`

 * *Files identical despite different names*

