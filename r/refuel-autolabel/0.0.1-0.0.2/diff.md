# Comparing `tmp/refuel-autolabel-0.0.1.tar.gz` & `tmp/refuel-autolabel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-autolabel-0.0.1.tar", last modified: Wed Jun 14 23:24:15 2023, max compression
+gzip compressed data, was "refuel-autolabel-0.0.2.tar", last modified: Thu Jun 15 09:29:43 2023, max compression
```

## Comparing `refuel-autolabel-0.0.1.tar` & `refuel-autolabel-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.512709 refuel-autolabel-0.0.1/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/LICENSE
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8783 2023-06-14 23:24:15.512486 refuel-autolabel-0.0.1/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6774 2023-06-14 23:08:47.000000 refuel-autolabel-0.0.1/README.md
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1922 2023-06-14 06:12:01.000000 refuel-autolabel-0.0.1/pyproject.toml
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-14 23:24:15.512752 refuel-autolabel-0.0.1/setup.cfg
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.499519 refuel-autolabel-0.0.1/src/
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.503670 refuel-autolabel-0.0.1/src/autolabel/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/__init__.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.504625 refuel-autolabel-0.0.1/src/autolabel/cache/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/cache/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.1/src/autolabel/cache/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/cache/sqlalchemy_cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-14 23:08:50.000000 refuel-autolabel-0.0.1/src/autolabel/confidence.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.505348 refuel-autolabel-0.0.1/src/autolabel/configs/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/configs/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1515 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/configs/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5714 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.1/src/autolabel/configs/config.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.506989 refuel-autolabel-0.0.1/src/autolabel/data_models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/data_models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/data_models/annotation.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/data_models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.1/src/autolabel/data_models/cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/data_models/dataset.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/data_models/task.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/data_models/task_run.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.507617 refuel-autolabel-0.0.1/src/autolabel/database/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/database/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      410 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.1/src/autolabel/database/engine.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/database/state_manager.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6592 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/dataset_loader.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.508478 refuel-autolabel-0.0.1/src/autolabel/few_shot/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2429 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/few_shot/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/few_shot/fixed_example_selector.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.1/src/autolabel/few_shot/vector_store.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19394 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/labeler.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.510026 refuel-autolabel-0.0.1/src/autolabel/models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/models/anthropic.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3037 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/models/hf_pipeline.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3768 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.1/src/autolabel/models/openai.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2672 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/models/palm.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3569 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/models/refuel.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4625 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.511512 refuel-autolabel-0.0.1/src/autolabel/tasks/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1160 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.1/src/autolabel/tasks/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3509 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/tasks/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7060 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/tasks/classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7071 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/tasks/entity_matching.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12517 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/tasks/named_entity_recognition.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7160 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/tasks/question_answering.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.1/src/autolabel/tasks/utils.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8888 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.1/src/autolabel/utils.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-14 23:24:15.512214 refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8783 2023-06-14 23:24:15.000000 refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1571 2023-06-14 23:24:15.000000 refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-14 23:24:15.000000 refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      641 2023-06-14 23:24:15.000000 refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/requires.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-14 23:24:15.000000 refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/top_level.txt
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.294209 refuel-autolabel-0.0.2/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/LICENSE
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10292 2023-06-15 09:29:43.293992 refuel-autolabel-0.0.2/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8283 2023-06-15 09:16:31.000000 refuel-autolabel-0.0.2/README.md
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1922 2023-06-15 09:25:59.000000 refuel-autolabel-0.0.2/pyproject.toml
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-15 09:29:43.294283 refuel-autolabel-0.0.2/setup.cfg
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.280100 refuel-autolabel-0.0.2/src/
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.282542 refuel-autolabel-0.0.2/src/autolabel/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/__init__.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.283321 refuel-autolabel-0.0.2/src/autolabel/cache/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/cache/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/cache/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/cache/sqlalchemy_cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.2/src/autolabel/confidence.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.284043 refuel-autolabel-0.0.2/src/autolabel/configs/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/configs/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1515 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/configs/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5880 2023-06-15 01:06:20.000000 refuel-autolabel-0.0.2/src/autolabel/configs/config.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.285882 refuel-autolabel-0.0.2/src/autolabel/data_models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/annotation.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/dataset.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/task.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/task_run.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.286481 refuel-autolabel-0.0.2/src/autolabel/database/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/database/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      410 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/database/engine.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/database/state_manager.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6592 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/dataset_loader.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.287143 refuel-autolabel-0.0.2/src/autolabel/few_shot/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2429 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/few_shot/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/few_shot/fixed_example_selector.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/few_shot/vector_store.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19394 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/labeler.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.291584 refuel-autolabel-0.0.2/src/autolabel/models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/anthropic.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3037 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/hf_pipeline.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3768 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/openai.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3599 2023-06-15 01:29:24.000000 refuel-autolabel-0.0.2/src/autolabel/models/palm.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3569 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/models/refuel.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4625 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/schema.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.292909 refuel-autolabel-0.0.2/src/autolabel/tasks/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1160 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3509 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7060 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/classification.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7071 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/entity_matching.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12517 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/named_entity_recognition.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7160 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/question_answering.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/utils.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8888 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/utils.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.293610 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10292 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1571 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      641 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/requires.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/top_level.txt
```

### Comparing `refuel-autolabel-0.0.1/LICENSE` & `refuel-autolabel-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/PKG-INFO` & `refuel-autolabel-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7265 6675  : 2.1.Name: refu
 00000020: 656c 2d61 7574 6f6c 6162 656c 0a56 6572  el-autolabel.Ver
-00000030: 7369 6f6e 3a20 302e 302e 310a 5375 6d6d  sion: 0.0.1.Summ
+00000030: 7369 6f6e 3a20 302e 302e 320a 5375 6d6d  sion: 0.0.2.Summ
 00000040: 6172 793a 204c 6962 7261 7279 2066 6f72  ary: Library for
 00000050: 204c 4c4d 2070 6f77 6572 6564 206c 6162   LLM powered lab
 00000060: 656c 696e 670a 4175 7468 6f72 2d65 6d61  eling.Author-ema
 00000070: 696c 3a20 2252 6566 7565 6c2e 6169 2220  il: "Refuel.ai" 
 00000080: 3c73 7570 706f 7274 4072 6566 7565 6c2e  <support@refuel.
 00000090: 6169 3e0a 4c69 6365 6e73 653a 204d 4954  ai>.License: MIT
 000000a0: 204c 6963 656e 7365 0a20 2020 2020 2020   License.       
@@ -120,430 +120,525 @@
 00000770: 2061 6e74 6872 6f70 6963 0a50 726f 7669   anthropic.Provi
 00000780: 6465 732d 4578 7472 613a 2068 7567 6769  des-Extra: huggi
 00000790: 6e67 6661 6365 0a50 726f 7669 6465 732d  ngface.Provides-
 000007a0: 4578 7472 613a 2067 6f6f 676c 650a 5072  Extra: google.Pr
 000007b0: 6f76 6964 6573 2d45 7874 7261 3a20 616c  ovides-Extra: al
 000007c0: 6c0a 4c69 6365 6e73 652d 4669 6c65 3a20  l.License-File: 
 000007d0: 4c49 4345 4e53 450a 0a3c 7069 6374 7572  LICENSE..<pictur
-000007e0: 653e 0a20 203c 736f 7572 6365 206d 6564  e>.  <source med
-000007f0: 6961 3d22 2870 7265 6665 7273 2d63 6f6c  ia="(prefers-col
-00000800: 6f72 2d73 6368 656d 653a 2064 6172 6b29  or-scheme: dark)
-00000810: 2220 7372 6373 6574 3d22 646f 6373 2f61  " srcset="docs/a
-00000820: 7373 6574 732f 4175 746f 6c61 6265 6c5f  ssets/Autolabel_
-00000830: 7774 2e70 6e67 223e 0a0a 2020 3c69 6d67  wt.png">..  <img
-00000840: 2061 6c74 3d22 5265 6675 656c 206c 6f67   alt="Refuel log
-00000850: 6f22 2073 7263 3d22 646f 6373 2f61 7373  o" src="docs/ass
-00000860: 6574 732f 4175 746f 6c61 6265 6c5f 626c  ets/Autolabel_bl
-00000870: 6b2e 706e 6722 3e0a 3c2f 7069 6374 7572  k.png">.</pictur
-00000880: 653e 0a3c 7020 616c 6967 6e3d 2263 656e  e>.<p align="cen
-00000890: 7465 7222 3e0a 2020 2020 3c62 3e43 6c65  ter">.    <b>Cle
-000008a0: 616e 2c20 6c61 6265 6c65 6420 6461 7461  an, labeled data
-000008b0: 2061 7420 7468 6520 7370 6565 6420 6f66   at the speed of
-000008c0: 2074 686f 7567 6874 3c2f 623e 2e0a 3c2f   thought</b>..</
-000008d0: 703e 0a0a 3c64 6976 2061 6c69 676e 3d22  p>..<div align="
-000008e0: 6365 6e74 6572 2220 7374 796c 653d 2277  center" style="w
-000008f0: 6964 7468 3a38 3030 7078 223e 0a0a 5b21  idth:800px">..[!
-00000900: 5b6c 696e 745d 2868 7474 7073 3a2f 2f67  [lint](https://g
-00000910: 6974 6875 622e 636f 6d2f 7265 6675 656c  ithub.com/refuel
-00000920: 2d61 692f 6175 746f 6c61 6265 6c2f 6163  -ai/autolabel/ac
-00000930: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000940: 626c 6163 6b2e 7961 6d6c 2f62 6164 6765  black.yaml/badge
-00000950: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000960: 6974 6875 622e 636f 6d2f 7265 6675 656c  ithub.com/refuel
-00000970: 2d61 692f 6175 746f 6c61 6265 6c2f 6163  -ai/autolabel/ac
-00000980: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000990: 626c 6163 6b2e 7961 6d6c 2f62 6164 6765  black.yaml/badge
-000009a0: 2e73 7667 2920 5b21 5b64 6f63 735d 2868  .svg) [![docs](h
-000009b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000009c0: 6d2f 7265 6675 656c 2d61 692f 6175 746f  m/refuel-ai/auto
-000009d0: 6c61 6265 6c2f 6163 7469 6f6e 732f 776f  label/actions/wo
-000009e0: 726b 666c 6f77 732f 646f 6373 2e79 616d  rkflows/docs.yam
-000009f0: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
-00000a00: 7470 733a 2f2f 646f 6373 2e72 6566 7565  tps://docs.refue
-00000a10: 6c2e 6169 2f29 2021 5b54 6573 7473 5d28  l.ai/) ![Tests](
-00000a20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000a30: 6f6d 2f72 6566 7565 6c2d 6169 2f61 7574  om/refuel-ai/aut
-00000a40: 6f6c 6162 656c 2f61 6374 696f 6e73 2f77  olabel/actions/w
-00000a50: 6f72 6b66 6c6f 7773 2f74 6573 742e 7961  orkflows/test.ya
-00000a60: 6d6c 2f62 6164 6765 2e73 7667 2920 5b21  ml/badge.svg) [!
-00000a70: 5b44 6973 636f 7264 5d28 6874 7470 733a  [Discord](https:
-00000a80: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000a90: 2f64 6973 636f 7264 2f31 3039 3837 3436  /discord/1098746
-00000aa0: 3639 3331 3532 3933 3139 3031 295d 2868  693152931901)](h
-00000ab0: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
-00000ac0: 672f 6677 6556 6e52 7836 4355 2920 5b21  g/fweVnRx6CU) [!
-00000ad0: 5b54 7769 7474 6572 5d28 6874 7470 733a  [Twitter](https:
-00000ae0: 2f2f 6261 6467 656e 2e6e 6574 2f62 6164  //badgen.net/bad
-00000af0: 6765 2f69 636f 6e2f 7477 6974 7465 723f  ge/icon/twitter?
-00000b00: 6963 6f6e 3d74 7769 7474 6572 266c 6162  icon=twitter&lab
-00000b10: 656c 295d 2868 7474 7073 3a2f 2f74 7769  el)](https://twi
-00000b20: 7474 6572 2e63 6f6d 2f52 6566 7565 6c41  tter.com/RefuelA
-00000b30: 4929 205b 215b 4c69 6365 6e73 653a 204d  I) [![License: M
-00000b40: 4954 5d28 6874 7470 733a 2f2f 6261 6467  IT](https://badg
-00000b50: 656e 2e6e 6574 2f62 6164 6765 2f6c 6963  en.net/badge/lic
-00000b60: 656e 7365 2f4d 4954 2f62 6c75 6529 5d28  ense/MIT/blue)](
-00000b70: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00000b80: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-00000b90: 4d49 5429 0a3c 2f64 6976 3e0a 0a23 2320  MIT).</div>..## 
-00000ba0: 5175 6963 6b20 496e 7374 616c 6c0a 0a60  Quick Install..`
-00000bb0: 7069 7020 696e 7374 616c 6c20 7265 6675  pip install refu
-00000bc0: 656c 2d61 7574 6f6c 6162 656c 600a 0a23  el-autolabel`..#
-00000bd0: 2320 f09f 8fb7 2057 6861 7420 6973 2041  # .... What is A
-00000be0: 7574 6f6c 6162 656c 0a0a 4163 6365 7373  utolabel..Access
-00000bf0: 2074 6f20 5b6c 6172 6765 2c20 636c 6561   to [large, clea
-00000c00: 6e20 616e 6420 6469 7665 7273 655d 2868  n and diverse](h
-00000c10: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
-00000c20: 6f6d 2f6b 6172 7061 7468 792f 7374 6174  om/karpathy/stat
-00000c30: 7573 2f31 3532 3834 3433 3132 3435 3737  us/1528443124577
-00000c40: 3531 3334 3732 3f6c 616e 673d 656e 2920  513472?lang=en) 
-00000c50: 6c61 6265 6c65 6420 6461 7461 7365 7473  labeled datasets
-00000c60: 2069 7320 6120 6372 6974 6963 616c 2063   is a critical c
-00000c70: 6f6d 706f 6e65 6e74 2066 6f72 2061 6e79  omponent for any
-00000c80: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
-00000c90: 6720 6566 666f 7274 2074 6f20 6265 2073  g effort to be s
-00000ca0: 7563 6365 7373 6675 6c2e 2042 7574 2064  uccessful. But d
-00000cb0: 6174 6120 6c61 6265 6c69 6e67 2069 7320  ata labeling is 
-00000cc0: 6120 6d61 6e75 616c 2061 6e64 2074 696d  a manual and tim
-00000cd0: 652d 636f 6e73 756d 696e 6720 7072 6f63  e-consuming proc
-00000ce0: 6573 732e 2053 7461 7465 2d6f 662d 7468  ess. State-of-th
-00000cf0: 652d 6172 7420 4c4c 4d73 206c 696b 6520  e-art LLMs like 
-00000d00: 4750 542d 3420 6172 6520 6162 6c65 2074  GPT-4 are able t
-00000d10: 6f20 5b61 7574 6f6d 6174 6963 616c 6c79  o [automatically
-00000d20: 206c 6162 656c 2064 6174 615d 2868 7474   label data](htt
-00000d30: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000d40: 6273 2f32 3330 332e 3135 3035 3629 2077  bs/2303.15056) w
-00000d50: 6974 6820 5b68 6967 6820 6163 6375 7261  ith [high accura
-00000d60: 6379 5d28 6874 7470 733a 2f2f 6172 7869  cy](https://arxi
-00000d70: 762e 6f72 672f 6162 732f 3233 3033 2e31  v.org/abs/2303.1
-00000d80: 3638 3534 292c 2061 6e64 2061 7420 6120  6854), and at a 
-00000d90: 6672 6163 7469 6f6e 206f 6620 7468 6520  fraction of the 
-00000da0: 636f 7374 2061 6e64 2074 696d 652e 0a0a  cost and time...
-00000db0: 4175 746f 6c61 6265 6c20 6973 2061 2050  Autolabel is a P
-00000dc0: 7974 686f 6e20 6c69 6272 6172 7920 746f  ython library to
-00000dd0: 206c 6162 656c 2c20 636c 6561 6e20 616e   label, clean an
-00000de0: 6420 656e 7269 6368 2074 6578 7420 6461  d enrich text da
-00000df0: 7461 7365 7473 2077 6974 6820 616e 7920  tasets with any 
-00000e00: 4c61 7267 6520 4c61 6e67 7561 6765 204d  Large Language M
-00000e10: 6f64 656c 7320 284c 4c4d 2920 6f66 2079  odels (LLM) of y
-00000e20: 6f75 7220 6368 6f69 6365 2e20 4120 6665  our choice. A fe
-00000e30: 7720 6b65 7920 6665 6174 7572 6573 3a0a  w key features:.
-00000e40: 0a31 2e20 4c61 6265 6c20 6461 7461 2066  .1. Label data f
-00000e50: 6f72 205b 4e4c 5020 7461 736b 735d 2868  or [NLP tasks](h
-00000e60: 7474 7073 3a2f 2f64 6f63 732e 7265 6675  ttps://docs.refu
-00000e70: 656c 2e61 692f 6775 6964 652f 7461 736b  el.ai/guide/task
-00000e80: 732f 636c 6173 7369 6669 6361 7469 6f6e  s/classification
-00000e90: 5f74 6173 6b2f 2920 7375 6368 2061 7320  _task/) such as 
-00000ea0: 636c 6173 7369 6669 6361 7469 6f6e 2c20  classification, 
-00000eb0: 7175 6573 7469 6f6e 2d61 6e73 7765 7269  question-answeri
-00000ec0: 6e67 2061 6e64 206e 616d 6564 2065 6e74  ng and named ent
-00000ed0: 6974 792d 7265 636f 676e 6974 696f 6e2c  ity-recognition,
-00000ee0: 2065 6e74 6974 7920 6d61 7463 6869 6e67   entity matching
-00000ef0: 2061 6e64 206d 6f72 652e 0a32 2e20 5573   and more..2. Us
-00000f00: 6520 636f 6d6d 6572 6369 616c 206f 7220  e commercial or 
-00000f10: 6f70 656e 2073 6f75 7263 6520 5b4c 4c4d  open source [LLM
-00000f20: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
-00000f30: 7265 6675 656c 2e61 692f 6775 6964 652f  refuel.ai/guide/
-00000f40: 6c6c 6d73 2f6c 6c6d 732f 2920 6672 6f6d  llms/llms/) from
-00000f50: 2070 726f 7669 6465 7273 2073 7563 6820   providers such 
-00000f60: 6173 204f 7065 6e41 492c 2041 6e74 6872  as OpenAI, Anthr
-00000f70: 6f70 6963 2c20 4875 6767 696e 6746 6163  opic, HuggingFac
-00000f80: 652c 2047 6f6f 676c 6520 616e 6420 6d6f  e, Google and mo
-00000f90: 7265 2e0a 332e 2053 7570 706f 7274 2066  re..3. Support f
-00000fa0: 6f72 2072 6573 6561 7263 682d 7072 6f76  or research-prov
-00000fb0: 656e 204c 4c4d 2074 6563 686e 6971 7565  en LLM technique
-00000fc0: 7320 746f 2062 6f6f 7374 206c 6162 656c  s to boost label
-00000fd0: 2071 7561 6c69 7479 2c20 7375 6368 2061   quality, such a
-00000fe0: 7320 6665 772d 7368 6f74 206c 6561 726e  s few-shot learn
-00000ff0: 696e 6720 616e 6420 6368 6169 6e2d 6f66  ing and chain-of
-00001000: 2d74 686f 7567 6874 2070 726f 6d70 7469  -thought prompti
-00001010: 6e67 2e0a 342e 205b 436f 6e66 6964 656e  ng..4. [Confiden
-00001020: 6365 2065 7374 696d 6174 696f 6e5d 2868  ce estimation](h
-00001030: 7474 7073 3a2f 2f64 6f63 732e 7265 6675  ttps://docs.refu
-00001040: 656c 2e61 692f 6775 6964 652f 6163 6375  el.ai/guide/accu
-00001050: 7261 6379 2f63 6f6e 6669 6465 6e63 652f  racy/confidence/
-00001060: 2920 616e 6420 6578 706c 616e 6174 696f  ) and explanatio
-00001070: 6e73 206f 7574 206f 6620 7468 6520 626f  ns out of the bo
-00001080: 7820 666f 7220 6576 6572 7920 7369 6e67  x for every sing
-00001090: 6c65 206f 7574 7075 7420 6c61 6265 6c0a  le output label.
-000010a0: 352e 205b 4361 6368 696e 6720 616e 6420  5. [Caching and 
-000010b0: 7374 6174 6520 6d61 6e61 6765 6d65 6e74  state management
-000010c0: 5d28 6874 7470 733a 2f2f 646f 6373 2e72  ](https://docs.r
-000010d0: 6566 7565 6c2e 6169 2f67 7569 6465 2f72  efuel.ai/guide/r
-000010e0: 656c 6961 6269 6c69 7479 2f73 7461 7465  eliability/state
-000010f0: 2d6d 616e 6167 656d 656e 742f 2920 746f  -management/) to
-00001100: 206d 696e 696d 697a 6520 636f 7374 7320   minimize costs 
-00001110: 616e 6420 6578 7065 7269 6d65 6e74 6174  and experimentat
-00001120: 696f 6e20 7469 6d65 0a0a 2323 20f0 9f9a  ion time..## ...
-00001130: 8020 4765 7474 696e 6720 7374 6172 7465  . Getting starte
-00001140: 640a 0a41 7574 6f6c 6162 656c 2070 726f  d..Autolabel pro
-00001150: 7669 6465 7320 6120 7369 6d70 6c65 2033  vides a simple 3
-00001160: 2d73 7465 7020 7072 6f63 6573 7320 666f  -step process fo
-00001170: 7220 6c61 6265 6c69 6e67 2064 6174 613a  r labeling data:
-00001180: 0a0a 312e 2053 7065 6369 6679 2074 6865  ..1. Specify the
-00001190: 206c 6162 656c 696e 6720 6775 6964 656c   labeling guidel
-000011a0: 696e 6573 2061 6e64 204c 4c4d 206d 6f64  ines and LLM mod
-000011b0: 656c 2074 6f20 7573 6520 696e 2061 204a  el to use in a J
-000011c0: 534f 4e20 636f 6e66 6967 2e0a 322e 2044  SON config..2. D
-000011d0: 7279 2d72 756e 2074 6f20 6d61 6b65 2073  ry-run to make s
-000011e0: 7572 6520 7468 6520 6669 6e61 6c20 7072  ure the final pr
-000011f0: 6f6d 7074 206c 6f6f 6b73 2067 6f6f 642e  ompt looks good.
-00001200: 0a33 2e20 4b69 636b 206f 6666 2061 206c  .3. Kick off a l
-00001210: 6162 656c 696e 6720 7275 6e20 666f 7220  abeling run for 
-00001220: 796f 7572 2064 6174 6173 6574 210a 0a4c  your dataset!..L
-00001230: 6574 2773 2069 6d61 6769 6e65 2077 6520  et's imagine we 
-00001240: 6172 6520 6275 696c 6469 6e67 2061 6e20  are building an 
-00001250: 4d4c 206d 6f64 656c 2074 6f20 616e 616c  ML model to anal
-00001260: 797a 6520 7365 6e74 696d 656e 7420 616e  yze sentiment an
-00001270: 616c 7973 6973 206f 6620 6d6f 7669 6520  alysis of movie 
-00001280: 7265 7669 6577 2e20 5765 2068 6176 6520  review. We have 
-00001290: 6120 6461 7461 7365 7420 6f66 206d 6f76  a dataset of mov
-000012a0: 6965 7720 7265 7669 6577 7320 7468 6174  iew reviews that
-000012b0: 2077 6527 6420 6c69 6b65 2074 6f20 6765   we'd like to ge
-000012c0: 7420 6c61 6265 6c65 6420 6669 7273 742e  t labeled first.
-000012d0: 2046 6f72 2074 6869 7320 6361 7365 2c20   For this case, 
-000012e0: 6865 7265 2773 2077 6861 7420 7468 6520  here's what the 
-000012f0: 6578 616d 706c 6520 6461 7461 7365 7420  example dataset 
-00001300: 616e 6420 636f 6e66 6967 7320 7769 6c6c  and configs will
-00001310: 206c 6f6f 6b20 6c69 6b65 3a0a 0a60 6060   look like:..```
-00001320: 7079 7468 6f6e 0a7b 0a20 2020 2022 7461  python.{.    "ta
-00001330: 736b 5f6e 616d 6522 3a20 224d 6f76 6965  sk_name": "Movie
-00001340: 5365 6e74 696d 656e 7452 6576 6965 7722  SentimentReview"
-00001350: 2c0a 2020 2020 2274 6173 6b5f 7479 7065  ,.    "task_type
-00001360: 223a 2022 636c 6173 7369 6669 6361 7469  ": "classificati
-00001370: 6f6e 222c 0a20 2020 2022 6d6f 6465 6c22  on",.    "model"
-00001380: 3a20 7b0a 2020 2020 2020 2020 2270 726f  : {.        "pro
-00001390: 7669 6465 7222 3a20 226f 7065 6e61 6922  vider": "openai"
-000013a0: 2c0a 2020 2020 2020 2020 226e 616d 6522  ,.        "name"
-000013b0: 3a20 2267 7074 2d33 2e35 2d74 7572 626f  : "gpt-3.5-turbo
-000013c0: 220a 2020 2020 7d2c 0a20 2020 2022 6461  ".    },.    "da
-000013d0: 7461 7365 7422 3a20 7b0a 2020 2020 2020  taset": {.      
-000013e0: 2020 226c 6162 656c 5f63 6f6c 756d 6e22    "label_column"
-000013f0: 3a20 226c 6162 656c 222c 0a20 2020 2020  : "label",.     
-00001400: 2020 2022 6465 6c69 6d69 7465 7222 3a20     "delimiter": 
-00001410: 222c 220a 2020 2020 7d2c 0a20 2020 2022  ",".    },.    "
-00001420: 7072 6f6d 7074 223a 207b 0a20 2020 2020  prompt": {.     
-00001430: 2020 2022 7461 736b 5f67 7569 6465 6c69     "task_guideli
-00001440: 6e65 7322 3a20 2259 6f75 2061 7265 2061  nes": "You are a
-00001450: 6e20 6578 7065 7274 2061 7420 616e 616c  n expert at anal
-00001460: 797a 696e 6720 7468 6520 7365 6e74 696d  yzing the sentim
-00001470: 656e 7420 6f66 206d 6f76 6965 7720 7265  ent of moview re
-00001480: 7669 6577 732e 2059 6f75 7220 6a6f 6220  views. Your job 
-00001490: 6973 2074 6f20 636c 6173 7369 6679 2074  is to classify t
-000014a0: 6865 2070 726f 7669 6465 6420 6d6f 7669  he provided movi
-000014b0: 6520 7265 7669 6577 2069 6e74 6f20 6f6e  e review into on
-000014c0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
-000014d0: 6e67 206c 6162 656c 733a 207b 6c61 6265  ng labels: {labe
-000014e0: 6c73 7d22 2c0a 2020 2020 2020 2020 226c  ls}",.        "l
-000014f0: 6162 656c 7322 3a20 5b0a 2020 2020 2020  abels": [.      
-00001500: 2020 2020 2020 2270 6f73 6974 6976 6522        "positive"
-00001510: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
-00001520: 6567 6174 6976 6522 2c0a 2020 2020 2020  egative",.      
-00001530: 2020 2020 2020 226e 6575 7472 616c 222c        "neutral",
-00001540: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00001550: 2020 2020 2266 6577 5f73 686f 745f 6578      "few_shot_ex
-00001560: 616d 706c 6573 223a 205b 0a20 2020 2020  amples": [.     
-00001570: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00001580: 2020 2020 2020 2020 2022 6578 616d 706c           "exampl
-00001590: 6522 3a20 2249 2067 6f74 2061 2066 6169  e": "I got a fai
-000015a0: 726c 7920 756e 696e 7370 6972 6564 2073  rly uninspired s
-000015b0: 7475 7069 6420 6669 6c6d 2061 626f 7574  tupid film about
-000015c0: 2068 6f77 2068 756d 616e 2069 6e64 7573   how human indus
-000015d0: 7472 7920 6973 2062 6164 2066 6f72 206e  try is bad for n
-000015e0: 6174 7572 652e 222c 0a20 2020 2020 2020  ature.",.       
-000015f0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001600: 3a20 226e 6567 6174 6976 6522 0a20 2020  : "negative".   
-00001610: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001620: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00001630: 2020 2020 2020 2020 2020 2265 7861 6d70            "examp
-00001640: 6c65 223a 2022 4920 6c6f 7665 6420 7468  le": "I loved th
-00001650: 6973 206d 6f76 6965 2e20 4920 666f 756e  is movie. I foun
-00001660: 6420 6974 2076 6572 7920 6865 6172 7420  d it very heart 
-00001670: 7761 726d 696e 6720 746f 2073 6565 2041  warming to see A
-00001680: 6461 6d20 5765 7374 2c20 4275 7274 2057  dam West, Burt W
-00001690: 6172 642c 2046 7261 6e6b 2047 6f72 7368  ard, Frank Gorsh
-000016a0: 696e 2c20 616e 6420 4a75 6c69 6520 4e65  in, and Julie Ne
-000016b0: 776d 6172 2074 6f67 6574 6865 7220 6167  wmar together ag
-000016c0: 6169 6e2e 222c 0a20 2020 2020 2020 2020  ain.",.         
-000016d0: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-000016e0: 2270 6f73 6974 6976 6522 0a20 2020 2020  "positive".     
-000016f0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00001700: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00001710: 2020 2020 2020 2020 2265 7861 6d70 6c65          "example
-00001720: 223a 2022 5468 6973 206d 6f76 6965 2077  ": "This movie w
-00001730: 696c 6c20 6265 2070 6c61 7965 6420 6e65  ill be played ne
-00001740: 7874 2077 6565 6b20 6174 2074 6865 2043  xt week at the C
-00001750: 6869 6e65 7365 2074 6865 6174 6572 2e22  hinese theater."
-00001760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001770: 2020 226c 6162 656c 223a 2022 6e65 7574    "label": "neut
-00001780: 7261 6c22 0a20 2020 2020 2020 2020 2020  ral".           
-00001790: 207d 0a20 2020 2020 2020 205d 2c0a 2020   }.        ],.  
-000017a0: 2020 2020 2020 2265 7861 6d70 6c65 5f74        "example_t
-000017b0: 656d 706c 6174 6522 3a20 2249 6e70 7574  emplate": "Input
-000017c0: 3a20 7b65 7861 6d70 6c65 7d5c 6e4f 7574  : {example}\nOut
-000017d0: 7075 743a 207b 6c61 6265 6c7d 220a 2020  put: {label}".  
-000017e0: 2020 7d0a 7d0a 6060 600a 0a49 6e69 7469    }.}.```..Initi
-000017f0: 616c 697a 6520 7468 6520 6c61 6265 6c69  alize the labeli
-00001800: 6e67 2061 6765 6e74 2061 6e64 2070 6173  ng agent and pas
-00001810: 7320 6974 2074 6865 2063 6f6e 6669 673a  s it the config:
-00001820: 0a0a 6060 6070 7974 686f 6e0a 0a66 726f  ..```python..fro
-00001830: 6d20 6175 746f 6c61 6265 6c20 696d 706f  m autolabel impo
-00001840: 7274 204c 6162 656c 696e 6741 6765 6e74  rt LabelingAgent
-00001850: 0a0a 6167 656e 7420 3d20 4c61 6265 6c69  ..agent = Labeli
-00001860: 6e67 4167 656e 7428 636f 6e66 6967 3d27  ngAgent(config='
-00001870: 636f 6e66 6967 2e6a 736f 6e27 290a 6060  config.json').``
-00001880: 600a 0a50 7265 7669 6577 2061 6e20 6578  `..Preview an ex
-00001890: 616d 706c 6520 7072 6f6d 7074 2074 6861  ample prompt tha
-000018a0: 7420 7769 6c6c 2062 6520 7365 6e74 2074  t will be sent t
-000018b0: 6f20 7468 6520 4c4c 4d3a 0a0a 6060 6070  o the LLM:..```p
-000018c0: 7974 686f 6e0a 6167 656e 742e 706c 616e  ython.agent.plan
-000018d0: 2827 6578 616d 706c 6573 2f6d 6f76 6965  ('examples/movie
-000018e0: 5f72 6576 6965 7773 2f64 6174 6173 6574  _reviews/dataset
-000018f0: 2e63 7376 2729 0a60 6060 0a0a 5468 6973  .csv').```..This
-00001900: 2070 7269 6e74 733a 0a0a 6060 600a e294   prints:..```...
-00001910: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001920: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001930: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001940: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001950: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001960: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001970: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001980: e294 81e2 9481 2031 3030 2f31 3030 2030  ...... 100/100 0
-00001990: 3a30 303a 3030 2030 3a30 303a 3030 0ae2  :00:00 0:00:00..
-000019a0: 948c e294 80e2 9480 e294 80e2 9480 e294  ................
-000019b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000019c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000019d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000019e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000019f0: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
-00001a00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001a10: 900a e294 8220 546f 7461 6c20 4573 7469  ..... Total Esti
-00001a20: 6d61 7465 6420 436f 7374 2020 2020 20e2  mated Cost     .
-00001a30: 9482 2024 302e 3533 3820 20e2 9482 0ae2  .. $0.538  .....
-00001a40: 9482 204e 756d 6265 7220 6f66 2045 7861  .. Number of Exa
-00001a50: 6d70 6c65 7320 2020 2020 2020 e294 8220  mples       ... 
-00001a60: 3230 3020 2020 2020 e294 820a e294 8220  200     ....... 
-00001a70: 4176 6572 6167 6520 636f 7374 2070 6572  Average cost per
-00001a80: 2065 7861 6d70 6c65 20e2 9482 2030 2e30   example ... 0.0
-00001a90: 3032 3639 20e2 9482 0ae2 9494 e294 80e2  0269 ...........
-00001aa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ac0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ae0: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
-00001af0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b00: 9480 e294 80e2 9480 e294 980a e294 80e2  ................
-00001b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001b60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b80: 80e2 9480 e294 800a 0a50 726f 6d70 7420  .........Prompt 
-00001b90: 4578 616d 706c 653a 0a59 6f75 2061 7265  Example:.You are
-00001ba0: 2061 6e20 6578 7065 7274 2061 7420 616e   an expert at an
-00001bb0: 616c 797a 696e 6720 7468 6520 7365 6e74  alyzing the sent
-00001bc0: 696d 656e 7420 6f66 206d 6f76 6965 7720  iment of moview 
-00001bd0: 7265 7669 6577 732e 2059 6f75 7220 6a6f  reviews. Your jo
-00001be0: 6220 6973 2074 6f20 636c 6173 7369 6679  b is to classify
-00001bf0: 2074 6865 2070 726f 7669 6465 6420 6d6f   the provided mo
-00001c00: 7669 6520 7265 7669 6577 2069 6e74 6f20  vie review into 
-00001c10: 6f6e 6520 6f66 2074 6865 2066 6f6c 6c6f  one of the follo
-00001c20: 7769 6e67 206c 6162 656c 733a 205b 706f  wing labels: [po
-00001c30: 7369 7469 7665 2c20 6e65 6761 7469 7665  sitive, negative
-00001c40: 2c20 6e65 7574 7261 6c5d 0a0a 596f 7520  , neutral]..You 
-00001c50: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
-00001c60: 616e 7377 6572 2077 6974 6820 6a75 7374  answer with just
-00001c70: 206f 6e65 2065 6c65 6d65 6e74 3a20 2274   one element: "t
-00001c80: 6865 2063 6f72 7265 6374 206c 6162 656c  he correct label
-00001c90: 220a 0a53 6f6d 6520 6578 616d 706c 6573  "..Some examples
-00001ca0: 2077 6974 6820 7468 6569 7220 6f75 7470   with their outp
-00001cb0: 7574 2061 6e73 7765 7273 2061 7265 2070  ut answers are p
-00001cc0: 726f 7669 6465 6420 6265 6c6f 773a 0a0a  rovided below:..
-00001cd0: 4578 616d 706c 653a 2049 2067 6f74 2061  Example: I got a
-00001ce0: 2066 6169 726c 7920 756e 696e 7370 6972   fairly uninspir
-00001cf0: 6564 2073 7475 7069 6420 6669 6c6d 2061  ed stupid film a
-00001d00: 626f 7574 2068 6f77 2068 756d 616e 2069  bout how human i
-00001d10: 6e64 7573 7472 7920 6973 2062 6164 2066  ndustry is bad f
-00001d20: 6f72 206e 6174 7572 652e 0a4f 7574 7075  or nature..Outpu
-00001d30: 743a 0a6e 6567 6174 6976 650a 0a45 7861  t:.negative..Exa
-00001d40: 6d70 6c65 3a20 4920 6c6f 7665 6420 7468  mple: I loved th
-00001d50: 6973 206d 6f76 6965 2e20 4920 666f 756e  is movie. I foun
-00001d60: 6420 6974 2076 6572 7920 6865 6172 7420  d it very heart 
-00001d70: 7761 726d 696e 6720 746f 2073 6565 2041  warming to see A
-00001d80: 6461 6d20 5765 7374 2c20 4275 7274 2057  dam West, Burt W
-00001d90: 6172 642c 2046 7261 6e6b 2047 6f72 7368  ard, Frank Gorsh
-00001da0: 696e 2c20 616e 6420 4a75 6c69 6520 4e65  in, and Julie Ne
-00001db0: 776d 6172 2074 6f67 6574 6865 7220 6167  wmar together ag
-00001dc0: 6169 6e2e 0a4f 7574 7075 743a 0a70 6f73  ain..Output:.pos
-00001dd0: 6974 6976 650a 0a45 7861 6d70 6c65 3a20  itive..Example: 
-00001de0: 5468 6973 206d 6f76 6965 2077 696c 6c20  This movie will 
-00001df0: 6265 2070 6c61 7965 6420 6e65 7874 2077  be played next w
-00001e00: 6565 6b20 6174 2074 6865 2043 6869 6e65  eek at the Chine
-00001e10: 7365 2074 6865 6174 6572 2e0a 4f75 7470  se theater..Outp
-00001e20: 7574 3a0a 6e65 7574 7261 6c0a 0a4e 6f77  ut:.neutral..Now
-00001e30: 2049 2077 616e 7420 796f 7520 746f 206c   I want you to l
-00001e40: 6162 656c 2074 6865 2066 6f6c 6c6f 7769  abel the followi
-00001e50: 6e67 2065 7861 6d70 6c65 3a0a 496e 7075  ng example:.Inpu
-00001e60: 743a 2041 2072 6172 6520 6578 6365 7074  t: A rare except
-00001e70: 696f 6e20 746f 2074 6865 2072 756c 6520  ion to the rule 
-00001e80: 7468 6174 2067 7265 6174 206c 6974 6572  that great liter
-00001e90: 6174 7572 6520 6d61 6b65 7320 6469 7361  ature makes disa
-00001ea0: 7070 6f69 6e74 696e 6720 6669 6c6d 732e  ppointing films.
-00001eb0: 0a4f 7574 7075 743a 0a0a e294 80e2 9480  .Output:........
-00001ec0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ed0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ee0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ef0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001fa0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001fc0: 9480 e294 800a 0a60 6060 0a0a 4669 6e61  .......```..Fina
-00001fd0: 6c6c 792c 2077 6520 6361 6e20 7275 6e20  lly, we can run 
-00001fe0: 7468 6520 6c61 6265 6c69 6e67 206f 6e20  the labeling on 
-00001ff0: 6120 7375 6273 6574 206f 7220 656e 7469  a subset or enti
-00002000: 7265 7479 206f 6620 7468 6520 6461 7461  rety of the data
-00002010: 7365 743a 0a0a 6060 6070 7974 686f 6e0a  set:..```python.
-00002020: 6c61 6265 6c73 2c20 6f75 7470 7574 5f64  labels, output_d
-00002030: 662c 206d 6574 7269 6373 203d 2061 6765  f, metrics = age
-00002040: 6e74 2e72 756e 2827 6578 616d 706c 6573  nt.run('examples
-00002050: 2f6d 6f76 6965 5f72 6576 6965 7773 2f64  /movie_reviews/d
-00002060: 6174 6173 6574 2e63 7376 2729 0a60 6060  ataset.csv').```
-00002070: 0a0a 2323 20f0 9f99 8c20 436f 6e74 7269  ..## .... Contri
-00002080: 6275 7469 6e67 0a0a 4175 746f 6c61 6265  buting..Autolabe
-00002090: 6c20 6973 2061 2072 6170 6964 6c79 2064  l is a rapidly d
-000020a0: 6576 656c 6f70 696e 6720 7072 6f6a 6563  eveloping projec
-000020b0: 742e 2057 6520 7765 6c63 6f6d 6520 636f  t. We welcome co
-000020c0: 6e74 7269 6275 7469 6f6e 7320 696e 2061  ntributions in a
-000020d0: 6c6c 2066 6f72 6d73 202d 2062 7567 2072  ll forms - bug r
-000020e0: 6570 6f72 7473 2c20 7075 6c6c 2072 6571  eports, pull req
-000020f0: 7565 7374 7320 616e 6420 6964 6561 7320  uests and ideas 
-00002100: 666f 7220 696d 7072 6f76 696e 6720 7468  for improving th
-00002110: 6520 6c69 6272 6172 792e 0a0a 312e 204a  e library...1. J
-00002120: 6f69 6e20 7468 6520 636f 6e76 6572 7361  oin the conversa
-00002130: 7469 6f6e 206f 6e20 5b44 6973 636f 7264  tion on [Discord
-00002140: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
-00002150: 642e 6767 2f66 7765 566e 5278 3643 5529  d.gg/fweVnRx6CU)
-00002160: 0a32 2e20 5265 7669 6577 2074 6865 20f0  .2. Review the .
-00002170: 9f9b a3ef b88f 205b 526f 6164 6d61 705d  ...... [Roadmap]
-00002180: 2829 2061 6e64 2063 6f6e 7472 6962 7574  () and contribut
-00002190: 6520 796f 7572 2069 6465 6173 2e0a 332e  e your ideas..3.
-000021a0: 2047 7261 6220 616e 205b 6f70 656e 2069   Grab an [open i
-000021b0: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
-000021c0: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
-000021d0: 6169 2f61 7574 6f6c 6162 656c 2f69 7373  ai/autolabel/iss
-000021e0: 7565 7329 206f 6e20 4769 7468 7562 2c20  ues) on Github, 
-000021f0: 616e 6420 7375 626d 6974 2061 205b 7075  and submit a [pu
-00002200: 6c6c 2072 6571 7565 7374 5d28 6874 7470  ll request](http
-00002210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00002220: 6566 7565 6c2d 6169 2f61 7574 6f6c 6162  efuel-ai/autolab
-00002230: 656c 2f62 6c6f 622f 6d61 696e 2f43 4f4e  el/blob/main/CON
-00002240: 5452 4942 5554 494e 472e 6d64 292e 0a    TRIBUTING.md)..
+000007e0: 653e 0a20 203c 696d 6720 616c 743d 2252  e>.  <img alt="R
+000007f0: 6566 7565 6c20 6c6f 676f 2220 7372 633d  efuel logo" src=
+00000800: 2264 6f63 732f 6173 7365 7473 2f41 7574  "docs/assets/Aut
+00000810: 6f6c 6162 656c 5f62 6c6b 5f77 5f62 6163  olabel_blk_w_bac
+00000820: 6b67 726f 756e 642e 706e 6722 3e0a 3c2f  kground.png">.</
+00000830: 7069 6374 7572 653e 0a3c 7020 616c 6967  picture>.<p alig
+00000840: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000850: 3c62 3e43 6c65 616e 2c20 6c61 6265 6c65  <b>Clean, labele
+00000860: 6420 6461 7461 2061 7420 7468 6520 7370  d data at the sp
+00000870: 6565 6420 6f66 2074 686f 7567 6874 3c2f  eed of thought</
+00000880: 623e 2e0a 3c2f 703e 0a0a 3c68 3420 616c  b>..</p>..<h4 al
+00000890: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000008a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000008b0: 2f64 6f63 732e 7265 6675 656c 2e61 692f  /docs.refuel.ai/
+000008c0: 6775 6964 652f 6f76 6572 7669 6577 2f67  guide/overview/g
+000008d0: 6574 7469 6e67 2d73 7461 7274 6564 2f22  etting-started/"
+000008e0: 3e47 6574 7469 6e67 2073 7461 7274 6564  >Getting started
+000008f0: 3c2f 613e 207c 0a20 203c 6120 6872 6566  </a> |.  <a href
+00000900: 3d22 6874 7470 733a 2f2f 646f 6373 2e72  ="https://docs.r
+00000910: 6566 7565 6c2e 6169 2f22 3e44 6f63 733c  efuel.ai/">Docs<
+00000920: 2f61 3e20 7c0a 2020 3c61 2068 7265 663d  /a> |.  <a href=
+00000930: 2268 7474 7073 3a2f 2f64 6973 636f 7264  "https://discord
+00000940: 2e67 672f 6677 6556 6e52 7836 4355 223e  .gg/fweVnRx6CU">
+00000950: 4469 7363 6f72 643c 2f61 3e20 7c0a 2020  Discord</a> |.  
+00000960: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000970: 2f74 7769 7474 6572 2e63 6f6d 2f52 6566  /twitter.com/Ref
+00000980: 7565 6c41 4922 3e54 7769 7474 6572 3c2f  uelAI">Twitter</
+00000990: 613e 207c 0a20 203c 6120 6872 6566 3d22  a> |.  <a href="
+000009a0: 6874 7470 733a 2f2f 7777 772e 7265 6675  https://www.refu
+000009b0: 656c 2e61 692f 223e 5765 6273 6974 653c  el.ai/">Website<
+000009c0: 2f61 3e0a 3c2f 6834 3e0a 0a3c 6469 7620  /a>.</h4>..<div 
+000009d0: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
+000009e0: 7479 6c65 3d22 7769 6474 683a 3830 3070  tyle="width:800p
+000009f0: 7822 3e0a 0a5b 215b 6c69 6e74 5d28 6874  x">..[![lint](ht
+00000a00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a10: 2f72 6566 7565 6c2d 6169 2f61 7574 6f6c  /refuel-ai/autol
+00000a20: 6162 656c 2f61 6374 696f 6e73 2f77 6f72  abel/actions/wor
+00000a30: 6b66 6c6f 7773 2f62 6c61 636b 2e79 616d  kflows/black.yam
+00000a40: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
+00000a50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a60: 2f72 6566 7565 6c2d 6169 2f61 7574 6f6c  /refuel-ai/autol
+00000a70: 6162 656c 2f61 6374 696f 6e73 2f77 6f72  abel/actions/wor
+00000a80: 6b66 6c6f 7773 2f62 6c61 636b 2e79 616d  kflows/black.yam
+00000a90: 6c2f 6261 6467 652e 7376 6729 2021 5b54  l/badge.svg) ![T
+00000aa0: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
+00000ab0: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
+00000ac0: 6169 2f61 7574 6f6c 6162 656c 2f61 6374  ai/autolabel/act
+00000ad0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f74  ions/workflows/t
+00000ae0: 6573 742e 7961 6d6c 2f62 6164 6765 2e73  est.yaml/badge.s
+00000af0: 7667 2920 215b 436f 6d6d 6974 2041 6374  vg) ![Commit Act
+00000b00: 6976 6974 795d 2868 7474 7073 3a2f 2f69  ivity](https://i
+00000b10: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000b20: 7468 7562 2f63 6f6d 6d69 742d 6163 7469  thub/commit-acti
+00000b30: 7669 7479 2f6d 2f72 6566 7565 6c2d 6169  vity/m/refuel-ai
+00000b40: 2f61 7574 6f6c 6162 656c 2920 5b21 5b44  /autolabel) [![D
+00000b50: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+00000b60: 696d 672e 7368 6965 6c64 732e 696f 2f64  img.shields.io/d
+00000b70: 6973 636f 7264 2f31 3039 3837 3436 3639  iscord/109874669
+00000b80: 3331 3532 3933 3139 3031 295d 2868 7474  3152931901)](htt
+00000b90: 7073 3a2f 2f64 6973 636f 7264 2e67 672f  ps://discord.gg/
+00000ba0: 6677 6556 6e52 7836 4355 2920 5b21 5b4c  fweVnRx6CU) [![L
+00000bb0: 6963 656e 7365 3a20 4d49 545d 2868 7474  icense: MIT](htt
+00000bc0: 7073 3a2f 2f62 6164 6765 6e2e 6e65 742f  ps://badgen.net/
+00000bd0: 6261 6467 652f 6c69 6365 6e73 652f 4d49  badge/license/MI
+00000be0: 542f 626c 7565 295d 2868 7474 7073 3a2f  T/blue)](https:/
+00000bf0: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
+00000c00: 6c69 6365 6e73 6573 2f4d 4954 290a 3c2f  licenses/MIT).</
+00000c10: 6469 763e 0a0a 2323 20e2 9aa1 2051 7569  div>..## ... Qui
+00000c20: 636b 2049 6e73 7461 6c6c 0a0a 6070 6970  ck Install..`pip
+00000c30: 2069 6e73 7461 6c6c 2072 6566 7565 6c2d   install refuel-
+00000c40: 6175 746f 6c61 6265 6c60 0a0a 2323 20f0  autolabel`..## .
+00000c50: 9f8f b720 5768 6174 2069 7320 4175 746f  ... What is Auto
+00000c60: 6c61 6265 6c0a 0a41 6363 6573 7320 746f  label..Access to
+00000c70: 205b 6c61 7267 652c 2063 6c65 616e 2061   [large, clean a
+00000c80: 6e64 2064 6976 6572 7365 5d28 6874 7470  nd diverse](http
+00000c90: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00000ca0: 6b61 7270 6174 6879 2f73 7461 7475 732f  karpathy/status/
+00000cb0: 3135 3238 3434 3331 3234 3537 3735 3133  1528443124577513
+00000cc0: 3437 323f 6c61 6e67 3d65 6e29 206c 6162  472?lang=en) lab
+00000cd0: 656c 6564 2064 6174 6173 6574 7320 6973  eled datasets is
+00000ce0: 2061 2063 7269 7469 6361 6c20 636f 6d70   a critical comp
+00000cf0: 6f6e 656e 7420 666f 7220 616e 7920 6d61  onent for any ma
+00000d00: 6368 696e 6520 6c65 6172 6e69 6e67 2065  chine learning e
+00000d10: 6666 6f72 7420 746f 2062 6520 7375 6363  ffort to be succ
+00000d20: 6573 7366 756c 2e20 5374 6174 652d 6f66  essful. State-of
+00000d30: 2d74 6865 2d61 7274 204c 4c4d 7320 6c69  -the-art LLMs li
+00000d40: 6b65 2047 5054 2d34 2061 7265 2061 626c  ke GPT-4 are abl
+00000d50: 6520 746f 205b 6175 746f 6d61 7469 6361  e to [automatica
+00000d60: 6c6c 7920 6c61 6265 6c20 6461 7461 5d28  lly label data](
+00000d70: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00000d80: 672f 6162 732f 3233 3033 2e31 3530 3536  g/abs/2303.15056
+00000d90: 2920 7769 7468 205b 6869 6768 2061 6363  ) with [high acc
+00000da0: 7572 6163 795d 2868 7474 7073 3a2f 2f61  uracy](https://a
+00000db0: 7278 6976 2e6f 7267 2f61 6273 2f32 3330  rxiv.org/abs/230
+00000dc0: 332e 3136 3835 3429 2c20 616e 6420 6174  3.16854), and at
+00000dd0: 2061 2066 7261 6374 696f 6e20 6f66 2074   a fraction of t
+00000de0: 6865 2063 6f73 7420 616e 6420 7469 6d65  he cost and time
+00000df0: 2063 6f6d 7061 7265 6420 746f 206d 616e   compared to man
+00000e00: 7561 6c20 6c61 6265 6c69 6e67 2e0a 0a41  ual labeling...A
+00000e10: 7574 6f6c 6162 656c 2069 7320 6120 5079  utolabel is a Py
+00000e20: 7468 6f6e 206c 6962 7261 7279 2074 6f20  thon library to 
+00000e30: 6c61 6265 6c2c 2063 6c65 616e 2061 6e64  label, clean and
+00000e40: 2065 6e72 6963 6820 7465 7874 2064 6174   enrich text dat
+00000e50: 6173 6574 7320 7769 7468 2061 6e79 204c  asets with any L
+00000e60: 6172 6765 204c 616e 6775 6167 6520 4d6f  arge Language Mo
+00000e70: 6465 6c73 2028 4c4c 4d29 206f 6620 796f  dels (LLM) of yo
+00000e80: 7572 2063 686f 6963 652e 0a0a 2323 20f0  ur choice...## .
+00000e90: 9f9a 8020 4765 7474 696e 6720 7374 6172  ... Getting star
+00000ea0: 7465 640a 0a41 7574 6f6c 6162 656c 2070  ted..Autolabel p
+00000eb0: 726f 7669 6465 7320 6120 7369 6d70 6c65  rovides a simple
+00000ec0: 2033 2d73 7465 7020 7072 6f63 6573 7320   3-step process 
+00000ed0: 666f 7220 6c61 6265 6c69 6e67 2064 6174  for labeling dat
+00000ee0: 613a 0a0a 312e 2053 7065 6369 6679 2074  a:..1. Specify t
+00000ef0: 6865 206c 6162 656c 696e 6720 6775 6964  he labeling guid
+00000f00: 656c 696e 6573 2061 6e64 204c 4c4d 206d  elines and LLM m
+00000f10: 6f64 656c 2074 6f20 7573 6520 696e 2061  odel to use in a
+00000f20: 204a 534f 4e20 636f 6e66 6967 2e0a 322e   JSON config..2.
+00000f30: 2044 7279 2d72 756e 2074 6f20 6d61 6b65   Dry-run to make
+00000f40: 2073 7572 6520 7468 6520 6669 6e61 6c20   sure the final 
+00000f50: 7072 6f6d 7074 206c 6f6f 6b73 2067 6f6f  prompt looks goo
+00000f60: 642e 0a33 2e20 4b69 636b 206f 6666 2061  d..3. Kick off a
+00000f70: 206c 6162 656c 696e 6720 7275 6e20 666f   labeling run fo
+00000f80: 7220 796f 7572 2064 6174 6173 6574 210a  r your dataset!.
+00000f90: 0a4c 6574 2773 2069 6d61 6769 6e65 2077  .Let's imagine w
+00000fa0: 6520 6172 6520 6275 696c 6469 6e67 2061  e are building a
+00000fb0: 6e20 4d4c 206d 6f64 656c 2074 6f20 616e  n ML model to an
+00000fc0: 616c 797a 6520 7365 6e74 696d 656e 7420  alyze sentiment 
+00000fd0: 616e 616c 7973 6973 206f 6620 6d6f 7669  analysis of movi
+00000fe0: 6520 7265 7669 6577 2e20 5765 2068 6176  e review. We hav
+00000ff0: 6520 6120 6461 7461 7365 7420 6f66 206d  e a dataset of m
+00001000: 6f76 6965 2072 6576 6965 7773 2074 6861  ovie reviews tha
+00001010: 7420 7765 2764 206c 696b 6520 746f 2067  t we'd like to g
+00001020: 6574 206c 6162 656c 6564 2066 6972 7374  et labeled first
+00001030: 2e20 466f 7220 7468 6973 2063 6173 652c  . For this case,
+00001040: 2068 6572 6527 7320 7768 6174 2074 6865   here's what the
+00001050: 2065 7861 6d70 6c65 2064 6174 6173 6574   example dataset
+00001060: 2061 6e64 2063 6f6e 6669 6773 2077 696c   and configs wil
+00001070: 6c20 6c6f 6f6b 206c 696b 653a 0a0a 6060  l look like:..``
+00001080: 6070 7974 686f 6e0a 7b0a 2020 2020 2274  `python.{.    "t
+00001090: 6173 6b5f 6e61 6d65 223a 2022 4d6f 7669  ask_name": "Movi
+000010a0: 6553 656e 7469 6d65 6e74 5265 7669 6577  eSentimentReview
+000010b0: 222c 0a20 2020 2022 7461 736b 5f74 7970  ",.    "task_typ
+000010c0: 6522 3a20 2263 6c61 7373 6966 6963 6174  e": "classificat
+000010d0: 696f 6e22 2c0a 2020 2020 226d 6f64 656c  ion",.    "model
+000010e0: 223a 207b 0a20 2020 2020 2020 2022 7072  ": {.        "pr
+000010f0: 6f76 6964 6572 223a 2022 6f70 656e 6169  ovider": "openai
+00001100: 222c 0a20 2020 2020 2020 2022 6e61 6d65  ",.        "name
+00001110: 223a 2022 6770 742d 332e 352d 7475 7262  ": "gpt-3.5-turb
+00001120: 6f22 0a20 2020 207d 2c0a 2020 2020 2264  o".    },.    "d
+00001130: 6174 6173 6574 223a 207b 0a20 2020 2020  ataset": {.     
+00001140: 2020 2022 6c61 6265 6c5f 636f 6c75 6d6e     "label_column
+00001150: 223a 2022 6c61 6265 6c22 2c0a 2020 2020  ": "label",.    
+00001160: 2020 2020 2264 656c 696d 6974 6572 223a      "delimiter":
+00001170: 2022 2c22 0a20 2020 207d 2c0a 2020 2020   ",".    },.    
+00001180: 2270 726f 6d70 7422 3a20 7b0a 2020 2020  "prompt": {.    
+00001190: 2020 2020 2274 6173 6b5f 6775 6964 656c      "task_guidel
+000011a0: 696e 6573 223a 2022 596f 7520 6172 6520  ines": "You are 
+000011b0: 616e 2065 7870 6572 7420 6174 2061 6e61  an expert at ana
+000011c0: 6c79 7a69 6e67 2074 6865 2073 656e 7469  lyzing the senti
+000011d0: 6d65 6e74 206f 6620 6d6f 7669 6520 7265  ment of movie re
+000011e0: 7669 6577 732e 2059 6f75 7220 6a6f 6220  views. Your job 
+000011f0: 6973 2074 6f20 636c 6173 7369 6679 2074  is to classify t
+00001200: 6865 2070 726f 7669 6465 6420 6d6f 7669  he provided movi
+00001210: 6520 7265 7669 6577 2069 6e74 6f20 6f6e  e review into on
+00001220: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+00001230: 6e67 206c 6162 656c 733a 207b 6c61 6265  ng labels: {labe
+00001240: 6c73 7d22 2c0a 2020 2020 2020 2020 226c  ls}",.        "l
+00001250: 6162 656c 7322 3a20 5b0a 2020 2020 2020  abels": [.      
+00001260: 2020 2020 2020 2270 6f73 6974 6976 6522        "positive"
+00001270: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00001280: 6567 6174 6976 6522 2c0a 2020 2020 2020  egative",.      
+00001290: 2020 2020 2020 226e 6575 7472 616c 222c        "neutral",
+000012a0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+000012b0: 2020 2020 2266 6577 5f73 686f 745f 6578      "few_shot_ex
+000012c0: 616d 706c 6573 223a 205b 0a20 2020 2020  amples": [.     
+000012d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000012e0: 2020 2020 2020 2020 2022 6578 616d 706c           "exampl
+000012f0: 6522 3a20 2249 2067 6f74 2061 2066 6169  e": "I got a fai
+00001300: 726c 7920 756e 696e 7370 6972 6564 2073  rly uninspired s
+00001310: 7475 7069 6420 6669 6c6d 2061 626f 7574  tupid film about
+00001320: 2068 6f77 2068 756d 616e 2069 6e64 7573   how human indus
+00001330: 7472 7920 6973 2062 6164 2066 6f72 206e  try is bad for n
+00001340: 6174 7572 652e 222c 0a20 2020 2020 2020  ature.",.       
+00001350: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00001360: 3a20 226e 6567 6174 6976 6522 0a20 2020  : "negative".   
+00001370: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00001380: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00001390: 2020 2020 2020 2020 2020 2265 7861 6d70            "examp
+000013a0: 6c65 223a 2022 4920 6c6f 7665 6420 7468  le": "I loved th
+000013b0: 6973 206d 6f76 6965 2e20 4920 666f 756e  is movie. I foun
+000013c0: 6420 6974 2076 6572 7920 6865 6172 7420  d it very heart 
+000013d0: 7761 726d 696e 6720 746f 2073 6565 2041  warming to see A
+000013e0: 6461 6d20 5765 7374 2c20 4275 7274 2057  dam West, Burt W
+000013f0: 6172 642c 2046 7261 6e6b 2047 6f72 7368  ard, Frank Gorsh
+00001400: 696e 2c20 616e 6420 4a75 6c69 6520 4e65  in, and Julie Ne
+00001410: 776d 6172 2074 6f67 6574 6865 7220 6167  wmar together ag
+00001420: 6169 6e2e 222c 0a20 2020 2020 2020 2020  ain.",.         
+00001430: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00001440: 2270 6f73 6974 6976 6522 0a20 2020 2020  "positive".     
+00001450: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001460: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001470: 2020 2020 2020 2020 2265 7861 6d70 6c65          "example
+00001480: 223a 2022 5468 6973 206d 6f76 6965 2077  ": "This movie w
+00001490: 696c 6c20 6265 2070 6c61 7965 6420 6e65  ill be played ne
+000014a0: 7874 2077 6565 6b20 6174 2074 6865 2043  xt week at the C
+000014b0: 6869 6e65 7365 2074 6865 6174 6572 2e22  hinese theater."
+000014c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000014d0: 2020 226c 6162 656c 223a 2022 6e65 7574    "label": "neut
+000014e0: 7261 6c22 0a20 2020 2020 2020 2020 2020  ral".           
+000014f0: 207d 0a20 2020 2020 2020 205d 2c0a 2020   }.        ],.  
+00001500: 2020 2020 2020 2265 7861 6d70 6c65 5f74        "example_t
+00001510: 656d 706c 6174 6522 3a20 2249 6e70 7574  emplate": "Input
+00001520: 3a20 7b65 7861 6d70 6c65 7d5c 6e4f 7574  : {example}\nOut
+00001530: 7075 743a 207b 6c61 6265 6c7d 220a 2020  put: {label}".  
+00001540: 2020 7d0a 7d0a 6060 600a 0a49 6e69 7469    }.}.```..Initi
+00001550: 616c 697a 6520 7468 6520 6c61 6265 6c69  alize the labeli
+00001560: 6e67 2061 6765 6e74 2061 6e64 2070 6173  ng agent and pas
+00001570: 7320 6974 2074 6865 2063 6f6e 6669 673a  s it the config:
+00001580: 0a0a 6060 6070 7974 686f 6e0a 0a66 726f  ..```python..fro
+00001590: 6d20 6175 746f 6c61 6265 6c20 696d 706f  m autolabel impo
+000015a0: 7274 204c 6162 656c 696e 6741 6765 6e74  rt LabelingAgent
+000015b0: 0a0a 6167 656e 7420 3d20 4c61 6265 6c69  ..agent = Labeli
+000015c0: 6e67 4167 656e 7428 636f 6e66 6967 3d27  ngAgent(config='
+000015d0: 636f 6e66 6967 2e6a 736f 6e27 290a 6060  config.json').``
+000015e0: 600a 0a50 7265 7669 6577 2061 6e20 6578  `..Preview an ex
+000015f0: 616d 706c 6520 7072 6f6d 7074 2074 6861  ample prompt tha
+00001600: 7420 7769 6c6c 2062 6520 7365 6e74 2074  t will be sent t
+00001610: 6f20 7468 6520 4c4c 4d3a 0a0a 6060 6070  o the LLM:..```p
+00001620: 7974 686f 6e0a 6167 656e 742e 706c 616e  ython.agent.plan
+00001630: 2827 6461 7461 7365 742e 6373 7627 290a  ('dataset.csv').
+00001640: 6060 600a 0a54 6869 7320 7072 696e 7473  ```..This prints
+00001650: 3a0a 0a60 6060 0ae2 9481 e294 81e2 9481  :..```..........
+00001660: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00001670: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00001680: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00001690: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+000016a0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+000016b0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000016c0: e294 81e2 9481 e294 81e2 9481 e294 8120  ............... 
+000016d0: 3130 302f 3130 3020 303a 3030 3a30 3020  100/100 0:00:00 
+000016e0: 303a 3030 3a30 300a e294 8ce2 9480 e294  0:00:00.........
+000016f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001700: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001710: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001720: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001730: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00001740: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001750: 80e2 9480 e294 80e2 9490 0ae2 9482 2054  .............. T
+00001760: 6f74 616c 2045 7374 696d 6174 6564 2043  otal Estimated C
+00001770: 6f73 7420 2020 2020 e294 8220 2430 2e35  ost     ... $0.5
+00001780: 3338 2020 e294 820a e294 8220 4e75 6d62  38  ....... Numb
+00001790: 6572 206f 6620 4578 616d 706c 6573 2020  er of Examples  
+000017a0: 2020 2020 20e2 9482 2032 3030 2020 2020       ... 200    
+000017b0: 20e2 9482 0ae2 9482 2041 7665 7261 6765   ....... Average
+000017c0: 2063 6f73 7420 7065 7220 6578 616d 706c   cost per exampl
+000017d0: 6520 e294 8220 302e 3030 3236 3920 e294  e ... 0.00269 ..
+000017e0: 820a e294 94e2 9480 e294 80e2 9480 e294  ................
+000017f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001830: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+00001840: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001850: 80e2 9498 0ae2 9480 e294 80e2 9480 e294  ................
+00001860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000018a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000018b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000018c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000018d0: 0a0a 5072 6f6d 7074 2045 7861 6d70 6c65  ..Prompt Example
+000018e0: 3a0a 596f 7520 6172 6520 616e 2065 7870  :.You are an exp
+000018f0: 6572 7420 6174 2061 6e61 6c79 7a69 6e67  ert at analyzing
+00001900: 2074 6865 2073 656e 7469 6d65 6e74 206f   the sentiment o
+00001910: 6620 6d6f 7669 6520 7265 7669 6577 732e  f movie reviews.
+00001920: 2059 6f75 7220 6a6f 6220 6973 2074 6f20   Your job is to 
+00001930: 636c 6173 7369 6679 2074 6865 2070 726f  classify the pro
+00001940: 7669 6465 6420 6d6f 7669 6520 7265 7669  vided movie revi
+00001950: 6577 2069 6e74 6f20 6f6e 6520 6f66 2074  ew into one of t
+00001960: 6865 2066 6f6c 6c6f 7769 6e67 206c 6162  he following lab
+00001970: 656c 733a 205b 706f 7369 7469 7665 2c20  els: [positive, 
+00001980: 6e65 6761 7469 7665 2c20 6e65 7574 7261  negative, neutra
+00001990: 6c5d 0a0a 536f 6d65 2065 7861 6d70 6c65  l]..Some example
+000019a0: 7320 7769 7468 2074 6865 6972 206f 7574  s with their out
+000019b0: 7075 7420 616e 7377 6572 7320 6172 6520  put answers are 
+000019c0: 7072 6f76 6964 6564 2062 656c 6f77 3a0a  provided below:.
+000019d0: 0a45 7861 6d70 6c65 3a20 4920 676f 7420  .Example: I got 
+000019e0: 6120 6661 6972 6c79 2075 6e69 6e73 7069  a fairly uninspi
+000019f0: 7265 6420 7374 7570 6964 2066 696c 6d20  red stupid film 
+00001a00: 6162 6f75 7420 686f 7720 6875 6d61 6e20  about how human 
+00001a10: 696e 6475 7374 7279 2069 7320 6261 6420  industry is bad 
+00001a20: 666f 7220 6e61 7475 7265 2e0a 4f75 7470  for nature..Outp
+00001a30: 7574 3a0a 6e65 6761 7469 7665 0a0a 4578  ut:.negative..Ex
+00001a40: 616d 706c 653a 2049 206c 6f76 6564 2074  ample: I loved t
+00001a50: 6869 7320 6d6f 7669 652e 2049 2066 6f75  his movie. I fou
+00001a60: 6e64 2069 7420 7665 7279 2068 6561 7274  nd it very heart
+00001a70: 2077 6172 6d69 6e67 2074 6f20 7365 6520   warming to see 
+00001a80: 4164 616d 2057 6573 742c 2042 7572 7420  Adam West, Burt 
+00001a90: 5761 7264 2c20 4672 616e 6b20 476f 7273  Ward, Frank Gors
+00001aa0: 6869 6e2c 2061 6e64 204a 756c 6965 204e  hin, and Julie N
+00001ab0: 6577 6d61 7220 746f 6765 7468 6572 2061  ewmar together a
+00001ac0: 6761 696e 2e0a 4f75 7470 7574 3a0a 706f  gain..Output:.po
+00001ad0: 7369 7469 7665 0a0a 4578 616d 706c 653a  sitive..Example:
+00001ae0: 2054 6869 7320 6d6f 7669 6520 7769 6c6c   This movie will
+00001af0: 2062 6520 706c 6179 6564 206e 6578 7420   be played next 
+00001b00: 7765 656b 2061 7420 7468 6520 4368 696e  week at the Chin
+00001b10: 6573 6520 7468 6561 7465 722e 0a4f 7574  ese theater..Out
+00001b20: 7075 743a 0a6e 6575 7472 616c 0a0a 4e6f  put:.neutral..No
+00001b30: 7720 4920 7761 6e74 2079 6f75 2074 6f20  w I want you to 
+00001b40: 6c61 6265 6c20 7468 6520 666f 6c6c 6f77  label the follow
+00001b50: 696e 6720 6578 616d 706c 653a 0a49 6e70  ing example:.Inp
+00001b60: 7574 3a20 4120 7261 7265 2065 7863 6570  ut: A rare excep
+00001b70: 7469 6f6e 2074 6f20 7468 6520 7275 6c65  tion to the rule
+00001b80: 2074 6861 7420 6772 6561 7420 6c69 7465   that great lite
+00001b90: 7261 7475 7265 206d 616b 6573 2064 6973  rature makes dis
+00001ba0: 6170 706f 696e 7469 6e67 2066 696c 6d73  appointing films
+00001bb0: 2e0a 4f75 7470 7574 3a0a 0ae2 9480 e294  ..Output:.......
+00001bc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001bd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001be0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001bf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001ca0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001cb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001cc0: e294 80e2 9480 0a0a 6060 600a 0a46 696e  ........```..Fin
+00001cd0: 616c 6c79 2c20 7765 2063 616e 2072 756e  ally, we can run
+00001ce0: 2074 6865 206c 6162 656c 696e 6720 6f6e   the labeling on
+00001cf0: 2061 2073 7562 7365 7420 6f72 2065 6e74   a subset or ent
+00001d00: 6972 6574 7920 6f66 2074 6865 2064 6174  irety of the dat
+00001d10: 6173 6574 3a0a 0a60 6060 7079 7468 6f6e  aset:..```python
+00001d20: 0a6c 6162 656c 732c 206f 7574 7075 745f  .labels, output_
+00001d30: 6466 2c20 6d65 7472 6963 7320 3d20 6167  df, metrics = ag
+00001d40: 656e 742e 7275 6e28 2764 6174 6173 6574  ent.run('dataset
+00001d50: 2e63 7376 2729 0a60 6060 0a0a 5468 6520  .csv').```..The 
+00001d60: 6f75 7470 7574 2064 6174 6166 7261 6d65  output dataframe
+00001d70: 2063 6f6e 7461 696e 7320 7468 6520 6c61   contains the la
+00001d80: 6265 6c20 636f 6c75 6d6e 3a0a 0a60 6060  bel column:..```
+00001d90: 7079 7468 6f6e 0a6f 7574 7075 745f 6466  python.output_df
+00001da0: 2e68 6561 6428 290a 2020 2020 2020 2020  .head().        
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 2020 2020 7465 7874 2020 2e2e          text  ..
+00001de0: 2e20 4d6f 7669 6553 656e 7469 6d65 6e74  . MovieSentiment
+00001df0: 5265 7669 6577 5f6c 6c6d 5f6c 6162 656c  Review_llm_label
+00001e00: 0a30 2020 4920 7761 7320 7665 7279 2065  .0  I was very e
+00001e10: 7863 6974 6564 2061 626f 7574 2073 6565  xcited about see
+00001e20: 696e 6720 7468 6973 2066 696c 6d2c 2061  ing this film, a
+00001e30: 6e74 2e2e 2e20 202e 2e2e 2020 2020 2020  nt...  ...      
+00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e50: 206e 6567 6174 6976 650a 3120 2053 6572   negative.1  Ser
+00001e60: 756d 2069 7320 6162 6f75 7420 6120 6372  um is about a cr
+00001e70: 617a 7920 646f 6374 6f72 2074 6861 7420  azy doctor that 
+00001e80: 6669 6e64 7320 6120 7365 722e 2e2e 2020  finds a ser...  
+00001e90: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+00001ea0: 2020 2020 2020 2020 2020 6e65 6761 7469            negati
+00001eb0: 7665 0a34 2020 4920 6c6f 7665 6420 7468  ve.4  I loved th
+00001ec0: 6973 206d 6f76 6965 2e20 4920 6b6e 6577  is movie. I knew
+00001ed0: 2069 7420 776f 756c 6420 6265 2063 686f   it would be cho
+00001ee0: 636b 6564 2e2e 2e20 202e 2e2e 2020 2020  cked...  ...    
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2020 2070 6f73 6974 6976 650a 2e2e 2e0a     positive.....
+00001f10: 6060 600a 0a23 2320 4665 6174 7572 6573  ```..## Features
+00001f20: 0a0a 312e 204c 6162 656c 2064 6174 6120  ..1. Label data 
+00001f30: 666f 7220 5b4e 4c50 2074 6173 6b73 5d28  for [NLP tasks](
+00001f40: 6874 7470 733a 2f2f 646f 6373 2e72 6566  https://docs.ref
+00001f50: 7565 6c2e 6169 2f67 7569 6465 2f74 6173  uel.ai/guide/tas
+00001f60: 6b73 2f63 6c61 7373 6966 6963 6174 696f  ks/classificatio
+00001f70: 6e5f 7461 736b 2f29 2073 7563 6820 6173  n_task/) such as
+00001f80: 2063 6c61 7373 6966 6963 6174 696f 6e2c   classification,
+00001f90: 2071 7565 7374 696f 6e2d 616e 7377 6572   question-answer
+00001fa0: 696e 6720 616e 6420 6e61 6d65 6420 656e  ing and named en
+00001fb0: 7469 7479 2d72 6563 6f67 6e69 7469 6f6e  tity-recognition
+00001fc0: 2c20 656e 7469 7479 206d 6174 6368 696e  , entity matchin
+00001fd0: 6720 616e 6420 6d6f 7265 2e0a 322e 2055  g and more..2. U
+00001fe0: 7365 2063 6f6d 6d65 7263 6961 6c20 6f72  se commercial or
+00001ff0: 206f 7065 6e20 736f 7572 6365 205b 4c4c   open source [LL
+00002000: 4d73 5d28 6874 7470 733a 2f2f 646f 6373  Ms](https://docs
+00002010: 2e72 6566 7565 6c2e 6169 2f67 7569 6465  .refuel.ai/guide
+00002020: 2f6c 6c6d 732f 6c6c 6d73 2f29 2066 726f  /llms/llms/) fro
+00002030: 6d20 7072 6f76 6964 6572 7320 7375 6368  m providers such
+00002040: 2061 7320 4f70 656e 4149 2c20 416e 7468   as OpenAI, Anth
+00002050: 726f 7069 632c 2048 7567 6769 6e67 4661  ropic, HuggingFa
+00002060: 6365 2c20 476f 6f67 6c65 2061 6e64 206d  ce, Google and m
+00002070: 6f72 652e 0a33 2e20 5375 7070 6f72 7420  ore..3. Support 
+00002080: 666f 7220 7265 7365 6172 6368 2d70 726f  for research-pro
+00002090: 7665 6e20 4c4c 4d20 7465 6368 6e69 7175  ven LLM techniqu
+000020a0: 6573 2074 6f20 626f 6f73 7420 6c61 6265  es to boost labe
+000020b0: 6c20 7175 616c 6974 792c 2073 7563 6820  l quality, such 
+000020c0: 6173 2066 6577 2d73 686f 7420 6c65 6172  as few-shot lear
+000020d0: 6e69 6e67 2061 6e64 2063 6861 696e 2d6f  ning and chain-o
+000020e0: 662d 7468 6f75 6768 7420 7072 6f6d 7074  f-thought prompt
+000020f0: 696e 672e 0a34 2e20 5b43 6f6e 6669 6465  ing..4. [Confide
+00002100: 6e63 6520 6573 7469 6d61 7469 6f6e 5d28  nce estimation](
+00002110: 6874 7470 733a 2f2f 646f 6373 2e72 6566  https://docs.ref
+00002120: 7565 6c2e 6169 2f67 7569 6465 2f61 6363  uel.ai/guide/acc
+00002130: 7572 6163 792f 636f 6e66 6964 656e 6365  uracy/confidence
+00002140: 2f29 2061 6e64 2065 7870 6c61 6e61 7469  /) and explanati
+00002150: 6f6e 7320 6f75 7420 6f66 2074 6865 2062  ons out of the b
+00002160: 6f78 2066 6f72 2065 7665 7279 2073 696e  ox for every sin
+00002170: 676c 6520 6f75 7470 7574 206c 6162 656c  gle output label
+00002180: 0a35 2e20 5b43 6163 6869 6e67 2061 6e64  .5. [Caching and
+00002190: 2073 7461 7465 206d 616e 6167 656d 656e   state managemen
+000021a0: 745d 2868 7474 7073 3a2f 2f64 6f63 732e  t](https://docs.
+000021b0: 7265 6675 656c 2e61 692f 6775 6964 652f  refuel.ai/guide/
+000021c0: 7265 6c69 6162 696c 6974 792f 7374 6174  reliability/stat
+000021d0: 652d 6d61 6e61 6765 6d65 6e74 2f29 2074  e-management/) t
+000021e0: 6f20 6d69 6e69 6d69 7a65 2063 6f73 7473  o minimize costs
+000021f0: 2061 6e64 2065 7870 6572 696d 656e 7461   and experimenta
+00002200: 7469 6f6e 2074 696d 650a 0a23 2320 f09f  tion time..## ..
+00002210: 9ba0 efb8 8f20 526f 6164 6d61 700a 4f75  ..... Roadmap.Ou
+00002220: 7220 676f 616c 2069 7320 746f 2061 6c6c  r goal is to all
+00002230: 6f77 2075 7365 7273 2074 6f20 6c61 6265  ow users to labe
+00002240: 6c2c 2063 7265 6174 6520 6f72 2065 6e72  l, create or enr
+00002250: 6963 6820 616e 7920 6461 7461 7365 742c  ich any dataset,
+00002260: 2077 6974 6820 616e 7920 4c4c 4d20 2d20   with any LLM - 
+00002270: 6561 7369 6c79 2061 6e64 2071 7569 636b  easily and quick
+00002280: 6c79 2e0a 0a54 6865 7265 2061 7265 2066  ly...There are f
+00002290: 6f75 7220 666f 6375 7320 6172 6561 7320  our focus areas 
+000022a0: 666f 7220 4175 746f 6c61 6265 6c20 666f  for Autolabel fo
+000022b0: 7220 3230 3233 3a0a 0a2a 202a 2a54 6173  r 2023:..* **Tas
+000022c0: 6b73 2a2a 3a20 4164 6420 7375 7070 6f72  ks**: Add suppor
+000022d0: 7420 666f 7220 7461 736b 7320 7375 6368  t for tasks such
+000022e0: 2061 7320 7265 7472 6965 7661 6c2c 2061   as retrieval, a
+000022f0: 7474 7269 6275 7465 2065 6e72 6963 686d  ttribute enrichm
+00002300: 656e 7420 616e 6420 7465 7874 2067 656e  ent and text gen
+00002310: 6572 6174 696f 6e2f 7772 6974 696e 672e  eration/writing.
+00002320: 0a2a 202a 2a4c 4c4d 732a 2a3a 2041 6464  .* **LLMs**: Add
+00002330: 2073 7570 706f 7274 2066 6f72 206d 6f72   support for mor
+00002340: 6520 4c4c 4d73 2c20 6573 7065 6369 616c  e LLMs, especial
+00002350: 6c79 206f 7065 6e20 736f 7572 6365 206d  ly open source m
+00002360: 6f64 656c 7320 6c69 6b65 2046 616c 636f  odels like Falco
+00002370: 6e2c 204d 5054 2061 6e64 2044 6f6c 6c79  n, MPT and Dolly
+00002380: 2061 6e64 2074 6865 2061 6269 6c69 7479   and the ability
+00002390: 2074 6f20 706c 7567 2069 6e20 796f 7572   to plug in your
+000023a0: 206f 776e 204c 4c4d 732e 200a 2a20 576f   own LLMs. .* Wo
+000023b0: 726b 666c 6f77 7320 666f 7220 2a2a 6578  rkflows for **ex
+000023c0: 7065 7269 6d65 6e74 696e 6720 7769 7468  perimenting with
+000023d0: 2079 6f75 7220 6461 7461 7365 7473 2a2a   your datasets**
+000023e0: 206d 6f72 6520 6561 7369 6c79 3a20 4164   more easily: Ad
+000023f0: 6420 7375 7070 6f72 7420 666f 7220 7269  d support for ri
+00002400: 6368 6572 2064 6174 6120 7479 7065 7320  cher data types 
+00002410: 2873 7563 6820 6173 2050 4446 7320 616e  (such as PDFs an
+00002420: 6420 4854 4d4c 2064 6f63 756d 656e 7473  d HTML documents
+00002430: 2920 616e 6420 7468 6520 6162 696c 6974  ) and the abilit
+00002440: 7920 746f 2072 756e 2062 656e 6368 6d61  y to run benchma
+00002450: 726b 696e 6720 6f6e 2079 6f75 7220 6461  rking on your da
+00002460: 7461 2073 6f75 7263 6573 2e0a 2a20 5465  ta sources..* Te
+00002470: 6368 6e69 7175 6573 2074 6f20 2a2a 696d  chniques to **im
+00002480: 7072 6f76 6520 6c61 6265 6c69 6e67 2061  prove labeling a
+00002490: 6363 7572 6163 792a 2a3a 2041 6464 2073  ccuracy**: Add s
+000024a0: 7570 706f 7274 2066 6f72 2061 7574 6f6d  upport for autom
+000024b0: 6174 6963 2070 726f 6d70 7420 696d 7072  atic prompt impr
+000024c0: 6f76 656d 656e 7420 616e 6420 746f 6f6c  ovement and tool
+000024d0: 7320 666f 7220 6265 7474 6572 2065 7272  s for better err
+000024e0: 6f72 2061 6e61 6c79 7369 7320 746f 2069  or analysis to i
+000024f0: 7465 7261 7469 7665 6c79 2069 6d70 726f  teratively impro
+00002500: 7665 204c 4c4d 2070 6572 666f 726d 616e  ve LLM performan
+00002510: 6365 206f 6e20 6469 6666 6572 656e 7420  ce on different 
+00002520: 7461 736b 7320 0a0a 5765 2077 696c 6c20  tasks ..We will 
+00002530: 6265 2072 656c 6561 7369 6e67 2061 206d  be releasing a m
+00002540: 6f72 6520 6465 7461 696c 6564 2072 6f61  ore detailed roa
+00002550: 646d 6170 2073 6f6f 6e2c 2062 7574 2077  dmap soon, but w
+00002560: 6520 6c6f 7665 2073 7567 6765 7374 696f  e love suggestio
+00002570: 6e73 2061 6e64 2063 6f6e 7472 6962 7574  ns and contribut
+00002580: 696f 6e73 2066 726f 6d20 7468 6520 636f  ions from the co
+00002590: 6d6d 756e 6974 792e 2043 6861 7420 7769  mmunity. Chat wi
+000025a0: 7468 2074 6865 2052 6566 7565 6c20 7465  th the Refuel te
+000025b0: 616d 2061 6e64 2041 7574 6f6c 6162 656c  am and Autolabel
+000025c0: 2063 6f6d 6d75 6e69 7479 206f 6e20 5b44   community on [D
+000025d0: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+000025e0: 6469 7363 6f72 642e 6767 2f66 7765 566e  discord.gg/fweVn
+000025f0: 5278 3643 5529 206f 7220 6f70 656e 205b  Rx6CU) or open [
+00002600: 4769 7468 7562 2069 7373 7565 735d 2868  Github issues](h
+00002610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002620: 6d2f 7265 6675 656c 2d61 692f 6175 746f  m/refuel-ai/auto
+00002630: 6c61 6265 6c2f 6973 7375 6573 2920 746f  label/issues) to
+00002640: 2072 6570 6f72 7420 6275 6773 2061 6e64   report bugs and
+00002650: 2072 6571 7565 7374 2066 6561 7475 7265   request feature
+00002660: 732e 0a0a 2323 20f0 9f99 8c20 436f 6e74  s...## .... Cont
+00002670: 7269 6275 7469 6e67 0a0a 4175 746f 6c61  ributing..Autola
+00002680: 6265 6c20 6973 2061 2072 6170 6964 6c79  bel is a rapidly
+00002690: 2064 6576 656c 6f70 696e 6720 7072 6f6a   developing proj
+000026a0: 6563 742e 2057 6520 7765 6c63 6f6d 6520  ect. We welcome 
+000026b0: 636f 6e74 7269 6275 7469 6f6e 7320 696e  contributions in
+000026c0: 2061 6c6c 2066 6f72 6d73 202d 2062 7567   all forms - bug
+000026d0: 2072 6570 6f72 7473 2c20 7075 6c6c 2072   reports, pull r
+000026e0: 6571 7565 7374 7320 616e 6420 6964 6561  equests and idea
+000026f0: 7320 666f 7220 696d 7072 6f76 696e 6720  s for improving 
+00002700: 7468 6520 6c69 6272 6172 792e 0a0a 312e  the library...1.
+00002710: 204a 6f69 6e20 7468 6520 636f 6e76 6572   Join the conver
+00002720: 7361 7469 6f6e 206f 6e20 5b44 6973 636f  sation on [Disco
+00002730: 7264 5d28 6874 7470 733a 2f2f 6469 7363  rd](https://disc
+00002740: 6f72 642e 6767 2f66 7765 566e 5278 3643  ord.gg/fweVnRx6C
+00002750: 5529 0a32 2e20 4f70 656e 2061 6e20 5b69  U).2. Open an [i
+00002760: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
+00002770: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
+00002780: 6169 2f61 7574 6f6c 6162 656c 2f69 7373  ai/autolabel/iss
+00002790: 7565 7329 206f 6e20 4769 7468 7562 2066  ues) on Github f
+000027a0: 6f72 2062 7567 7320 616e 6420 7265 7175  or bugs and requ
+000027b0: 6573 7420 6665 6174 7572 6573 2e0a 332e  est features..3.
+000027c0: 2047 7261 6220 616e 206f 7065 6e20 6973   Grab an open is
+000027d0: 7375 652c 2061 6e64 2073 7562 6d69 7420  sue, and submit 
+000027e0: 6120 5b70 756c 6c20 7265 7175 6573 745d  a [pull request]
+000027f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002800: 636f 6d2f 7265 6675 656c 2d61 692f 6175  com/refuel-ai/au
+00002810: 746f 6c61 6265 6c2f 626c 6f62 2f6d 6169  tolabel/blob/mai
+00002820: 6e2f 434f 4e54 5249 4255 5449 4e47 2e6d  n/CONTRIBUTING.m
+00002830: 6429 2e0a                                d)..
```

### Comparing `refuel-autolabel-0.0.1/README.md` & `refuel-autolabel-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,424 +1,518 @@
-00000000: 3c70 6963 7475 7265 3e0a 2020 3c73 6f75  <picture>.  <sou
-00000010: 7263 6520 6d65 6469 613d 2228 7072 6566  rce media="(pref
-00000020: 6572 732d 636f 6c6f 722d 7363 6865 6d65  ers-color-scheme
-00000030: 3a20 6461 726b 2922 2073 7263 7365 743d  : dark)" srcset=
-00000040: 2264 6f63 732f 6173 7365 7473 2f41 7574  "docs/assets/Aut
-00000050: 6f6c 6162 656c 5f77 742e 706e 6722 3e0a  olabel_wt.png">.
-00000060: 0a20 203c 696d 6720 616c 743d 2252 6566  .  <img alt="Ref
-00000070: 7565 6c20 6c6f 676f 2220 7372 633d 2264  uel logo" src="d
-00000080: 6f63 732f 6173 7365 7473 2f41 7574 6f6c  ocs/assets/Autol
-00000090: 6162 656c 5f62 6c6b 2e70 6e67 223e 0a3c  abel_blk.png">.<
-000000a0: 2f70 6963 7475 7265 3e0a 3c70 2061 6c69  /picture>.<p ali
-000000b0: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
-000000c0: 203c 623e 436c 6561 6e2c 206c 6162 656c   <b>Clean, label
-000000d0: 6564 2064 6174 6120 6174 2074 6865 2073  ed data at the s
-000000e0: 7065 6564 206f 6620 7468 6f75 6768 743c  peed of thought<
-000000f0: 2f62 3e2e 0a3c 2f70 3e0a 0a3c 6469 7620  /b>..</p>..<div 
-00000100: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
-00000110: 7479 6c65 3d22 7769 6474 683a 3830 3070  tyle="width:800p
-00000120: 7822 3e0a 0a5b 215b 6c69 6e74 5d28 6874  x">..[![lint](ht
-00000130: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000140: 2f72 6566 7565 6c2d 6169 2f61 7574 6f6c  /refuel-ai/autol
-00000150: 6162 656c 2f61 6374 696f 6e73 2f77 6f72  abel/actions/wor
-00000160: 6b66 6c6f 7773 2f62 6c61 636b 2e79 616d  kflows/black.yam
-00000170: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
-00000180: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000190: 2f72 6566 7565 6c2d 6169 2f61 7574 6f6c  /refuel-ai/autol
-000001a0: 6162 656c 2f61 6374 696f 6e73 2f77 6f72  abel/actions/wor
-000001b0: 6b66 6c6f 7773 2f62 6c61 636b 2e79 616d  kflows/black.yam
-000001c0: 6c2f 6261 6467 652e 7376 6729 205b 215b  l/badge.svg) [![
-000001d0: 646f 6373 5d28 6874 7470 733a 2f2f 6769  docs](https://gi
-000001e0: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
-000001f0: 6169 2f61 7574 6f6c 6162 656c 2f61 6374  ai/autolabel/act
-00000200: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f64  ions/workflows/d
-00000210: 6f63 732e 7961 6d6c 2f62 6164 6765 2e73  ocs.yaml/badge.s
-00000220: 7667 295d 2868 7474 7073 3a2f 2f64 6f63  vg)](https://doc
-00000230: 732e 7265 6675 656c 2e61 692f 2920 215b  s.refuel.ai/) ![
-00000240: 5465 7374 735d 2868 7474 7073 3a2f 2f67  Tests](https://g
-00000250: 6974 6875 622e 636f 6d2f 7265 6675 656c  ithub.com/refuel
-00000260: 2d61 692f 6175 746f 6c61 6265 6c2f 6163  -ai/autolabel/ac
-00000270: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000280: 7465 7374 2e79 616d 6c2f 6261 6467 652e  test.yaml/badge.
-00000290: 7376 6729 205b 215b 4469 7363 6f72 645d  svg) [![Discord]
-000002a0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000002b0: 656c 6473 2e69 6f2f 6469 7363 6f72 642f  elds.io/discord/
-000002c0: 3130 3938 3734 3636 3933 3135 3239 3331  1098746693152931
-000002d0: 3930 3129 5d28 6874 7470 733a 2f2f 6469  901)](https://di
-000002e0: 7363 6f72 642e 6767 2f66 7765 566e 5278  scord.gg/fweVnRx
-000002f0: 3643 5529 205b 215b 5477 6974 7465 725d  6CU) [![Twitter]
-00000300: 2868 7474 7073 3a2f 2f62 6164 6765 6e2e  (https://badgen.
-00000310: 6e65 742f 6261 6467 652f 6963 6f6e 2f74  net/badge/icon/t
-00000320: 7769 7474 6572 3f69 636f 6e3d 7477 6974  witter?icon=twit
-00000330: 7465 7226 6c61 6265 6c29 5d28 6874 7470  ter&label)](http
-00000340: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
-00000350: 5265 6675 656c 4149 2920 5b21 5b4c 6963  RefuelAI) [![Lic
-00000360: 656e 7365 3a20 4d49 545d 2868 7474 7073  ense: MIT](https
-00000370: 3a2f 2f62 6164 6765 6e2e 6e65 742f 6261  ://badgen.net/ba
-00000380: 6467 652f 6c69 6365 6e73 652f 4d49 542f  dge/license/MIT/
-00000390: 626c 7565 295d 2868 7474 7073 3a2f 2f6f  blue)](https://o
-000003a0: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
-000003b0: 6365 6e73 6573 2f4d 4954 290a 3c2f 6469  censes/MIT).</di
-000003c0: 763e 0a0a 2323 2051 7569 636b 2049 6e73  v>..## Quick Ins
-000003d0: 7461 6c6c 0a0a 6070 6970 2069 6e73 7461  tall..`pip insta
-000003e0: 6c6c 2072 6566 7565 6c2d 6175 746f 6c61  ll refuel-autola
-000003f0: 6265 6c60 0a0a 2323 20f0 9f8f b720 5768  bel`..## .... Wh
-00000400: 6174 2069 7320 4175 746f 6c61 6265 6c0a  at is Autolabel.
-00000410: 0a41 6363 6573 7320 746f 205b 6c61 7267  .Access to [larg
-00000420: 652c 2063 6c65 616e 2061 6e64 2064 6976  e, clean and div
-00000430: 6572 7365 5d28 6874 7470 733a 2f2f 7477  erse](https://tw
-00000440: 6974 7465 722e 636f 6d2f 6b61 7270 6174  itter.com/karpat
-00000450: 6879 2f73 7461 7475 732f 3135 3238 3434  hy/status/152844
-00000460: 3331 3234 3537 3735 3133 3437 323f 6c61  3124577513472?la
-00000470: 6e67 3d65 6e29 206c 6162 656c 6564 2064  ng=en) labeled d
-00000480: 6174 6173 6574 7320 6973 2061 2063 7269  atasets is a cri
-00000490: 7469 6361 6c20 636f 6d70 6f6e 656e 7420  tical component 
-000004a0: 666f 7220 616e 7920 6d61 6368 696e 6520  for any machine 
-000004b0: 6c65 6172 6e69 6e67 2065 6666 6f72 7420  learning effort 
-000004c0: 746f 2062 6520 7375 6363 6573 7366 756c  to be successful
-000004d0: 2e20 4275 7420 6461 7461 206c 6162 656c  . But data label
-000004e0: 696e 6720 6973 2061 206d 616e 7561 6c20  ing is a manual 
-000004f0: 616e 6420 7469 6d65 2d63 6f6e 7375 6d69  and time-consumi
-00000500: 6e67 2070 726f 6365 7373 2e20 5374 6174  ng process. Stat
-00000510: 652d 6f66 2d74 6865 2d61 7274 204c 4c4d  e-of-the-art LLM
-00000520: 7320 6c69 6b65 2047 5054 2d34 2061 7265  s like GPT-4 are
-00000530: 2061 626c 6520 746f 205b 6175 746f 6d61   able to [automa
-00000540: 7469 6361 6c6c 7920 6c61 6265 6c20 6461  tically label da
-00000550: 7461 5d28 6874 7470 733a 2f2f 6172 7869  ta](https://arxi
-00000560: 762e 6f72 672f 6162 732f 3233 3033 2e31  v.org/abs/2303.1
-00000570: 3530 3536 2920 7769 7468 205b 6869 6768  5056) with [high
-00000580: 2061 6363 7572 6163 795d 2868 7474 7073   accuracy](https
-00000590: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-000005a0: 2f32 3330 332e 3136 3835 3429 2c20 616e  /2303.16854), an
-000005b0: 6420 6174 2061 2066 7261 6374 696f 6e20  d at a fraction 
-000005c0: 6f66 2074 6865 2063 6f73 7420 616e 6420  of the cost and 
-000005d0: 7469 6d65 2e0a 0a41 7574 6f6c 6162 656c  time...Autolabel
-000005e0: 2069 7320 6120 5079 7468 6f6e 206c 6962   is a Python lib
-000005f0: 7261 7279 2074 6f20 6c61 6265 6c2c 2063  rary to label, c
-00000600: 6c65 616e 2061 6e64 2065 6e72 6963 6820  lean and enrich 
-00000610: 7465 7874 2064 6174 6173 6574 7320 7769  text datasets wi
-00000620: 7468 2061 6e79 204c 6172 6765 204c 616e  th any Large Lan
-00000630: 6775 6167 6520 4d6f 6465 6c73 2028 4c4c  guage Models (LL
-00000640: 4d29 206f 6620 796f 7572 2063 686f 6963  M) of your choic
-00000650: 652e 2041 2066 6577 206b 6579 2066 6561  e. A few key fea
-00000660: 7475 7265 733a 0a0a 312e 204c 6162 656c  tures:..1. Label
-00000670: 2064 6174 6120 666f 7220 5b4e 4c50 2074   data for [NLP t
-00000680: 6173 6b73 5d28 6874 7470 733a 2f2f 646f  asks](https://do
-00000690: 6373 2e72 6566 7565 6c2e 6169 2f67 7569  cs.refuel.ai/gui
-000006a0: 6465 2f74 6173 6b73 2f63 6c61 7373 6966  de/tasks/classif
-000006b0: 6963 6174 696f 6e5f 7461 736b 2f29 2073  ication_task/) s
-000006c0: 7563 6820 6173 2063 6c61 7373 6966 6963  uch as classific
-000006d0: 6174 696f 6e2c 2071 7565 7374 696f 6e2d  ation, question-
-000006e0: 616e 7377 6572 696e 6720 616e 6420 6e61  answering and na
-000006f0: 6d65 6420 656e 7469 7479 2d72 6563 6f67  med entity-recog
-00000700: 6e69 7469 6f6e 2c20 656e 7469 7479 206d  nition, entity m
-00000710: 6174 6368 696e 6720 616e 6420 6d6f 7265  atching and more
-00000720: 2e0a 322e 2055 7365 2063 6f6d 6d65 7263  ..2. Use commerc
-00000730: 6961 6c20 6f72 206f 7065 6e20 736f 7572  ial or open sour
-00000740: 6365 205b 4c4c 4d73 5d28 6874 7470 733a  ce [LLMs](https:
-00000750: 2f2f 646f 6373 2e72 6566 7565 6c2e 6169  //docs.refuel.ai
-00000760: 2f67 7569 6465 2f6c 6c6d 732f 6c6c 6d73  /guide/llms/llms
-00000770: 2f29 2066 726f 6d20 7072 6f76 6964 6572  /) from provider
-00000780: 7320 7375 6368 2061 7320 4f70 656e 4149  s such as OpenAI
-00000790: 2c20 416e 7468 726f 7069 632c 2048 7567  , Anthropic, Hug
-000007a0: 6769 6e67 4661 6365 2c20 476f 6f67 6c65  gingFace, Google
-000007b0: 2061 6e64 206d 6f72 652e 0a33 2e20 5375   and more..3. Su
-000007c0: 7070 6f72 7420 666f 7220 7265 7365 6172  pport for resear
-000007d0: 6368 2d70 726f 7665 6e20 4c4c 4d20 7465  ch-proven LLM te
-000007e0: 6368 6e69 7175 6573 2074 6f20 626f 6f73  chniques to boos
-000007f0: 7420 6c61 6265 6c20 7175 616c 6974 792c  t label quality,
-00000800: 2073 7563 6820 6173 2066 6577 2d73 686f   such as few-sho
-00000810: 7420 6c65 6172 6e69 6e67 2061 6e64 2063  t learning and c
-00000820: 6861 696e 2d6f 662d 7468 6f75 6768 7420  hain-of-thought 
-00000830: 7072 6f6d 7074 696e 672e 0a34 2e20 5b43  prompting..4. [C
-00000840: 6f6e 6669 6465 6e63 6520 6573 7469 6d61  onfidence estima
-00000850: 7469 6f6e 5d28 6874 7470 733a 2f2f 646f  tion](https://do
-00000860: 6373 2e72 6566 7565 6c2e 6169 2f67 7569  cs.refuel.ai/gui
-00000870: 6465 2f61 6363 7572 6163 792f 636f 6e66  de/accuracy/conf
-00000880: 6964 656e 6365 2f29 2061 6e64 2065 7870  idence/) and exp
-00000890: 6c61 6e61 7469 6f6e 7320 6f75 7420 6f66  lanations out of
-000008a0: 2074 6865 2062 6f78 2066 6f72 2065 7665   the box for eve
-000008b0: 7279 2073 696e 676c 6520 6f75 7470 7574  ry single output
-000008c0: 206c 6162 656c 0a35 2e20 5b43 6163 6869   label.5. [Cachi
-000008d0: 6e67 2061 6e64 2073 7461 7465 206d 616e  ng and state man
-000008e0: 6167 656d 656e 745d 2868 7474 7073 3a2f  agement](https:/
-000008f0: 2f64 6f63 732e 7265 6675 656c 2e61 692f  /docs.refuel.ai/
-00000900: 6775 6964 652f 7265 6c69 6162 696c 6974  guide/reliabilit
-00000910: 792f 7374 6174 652d 6d61 6e61 6765 6d65  y/state-manageme
-00000920: 6e74 2f29 2074 6f20 6d69 6e69 6d69 7a65  nt/) to minimize
-00000930: 2063 6f73 7473 2061 6e64 2065 7870 6572   costs and exper
-00000940: 696d 656e 7461 7469 6f6e 2074 696d 650a  imentation time.
-00000950: 0a23 2320 f09f 9a80 2047 6574 7469 6e67  .## .... Getting
-00000960: 2073 7461 7274 6564 0a0a 4175 746f 6c61   started..Autola
-00000970: 6265 6c20 7072 6f76 6964 6573 2061 2073  bel provides a s
-00000980: 696d 706c 6520 332d 7374 6570 2070 726f  imple 3-step pro
-00000990: 6365 7373 2066 6f72 206c 6162 656c 696e  cess for labelin
-000009a0: 6720 6461 7461 3a0a 0a31 2e20 5370 6563  g data:..1. Spec
-000009b0: 6966 7920 7468 6520 6c61 6265 6c69 6e67  ify the labeling
-000009c0: 2067 7569 6465 6c69 6e65 7320 616e 6420   guidelines and 
-000009d0: 4c4c 4d20 6d6f 6465 6c20 746f 2075 7365  LLM model to use
-000009e0: 2069 6e20 6120 4a53 4f4e 2063 6f6e 6669   in a JSON confi
-000009f0: 672e 0a32 2e20 4472 792d 7275 6e20 746f  g..2. Dry-run to
-00000a00: 206d 616b 6520 7375 7265 2074 6865 2066   make sure the f
-00000a10: 696e 616c 2070 726f 6d70 7420 6c6f 6f6b  inal prompt look
-00000a20: 7320 676f 6f64 2e0a 332e 204b 6963 6b20  s good..3. Kick 
-00000a30: 6f66 6620 6120 6c61 6265 6c69 6e67 2072  off a labeling r
-00000a40: 756e 2066 6f72 2079 6f75 7220 6461 7461  un for your data
-00000a50: 7365 7421 0a0a 4c65 7427 7320 696d 6167  set!..Let's imag
-00000a60: 696e 6520 7765 2061 7265 2062 7569 6c64  ine we are build
-00000a70: 696e 6720 616e 204d 4c20 6d6f 6465 6c20  ing an ML model 
-00000a80: 746f 2061 6e61 6c79 7a65 2073 656e 7469  to analyze senti
-00000a90: 6d65 6e74 2061 6e61 6c79 7369 7320 6f66  ment analysis of
-00000aa0: 206d 6f76 6965 2072 6576 6965 772e 2057   movie review. W
-00000ab0: 6520 6861 7665 2061 2064 6174 6173 6574  e have a dataset
-00000ac0: 206f 6620 6d6f 7669 6577 2072 6576 6965   of moview revie
-00000ad0: 7773 2074 6861 7420 7765 2764 206c 696b  ws that we'd lik
-00000ae0: 6520 746f 2067 6574 206c 6162 656c 6564  e to get labeled
-00000af0: 2066 6972 7374 2e20 466f 7220 7468 6973   first. For this
-00000b00: 2063 6173 652c 2068 6572 6527 7320 7768   case, here's wh
-00000b10: 6174 2074 6865 2065 7861 6d70 6c65 2064  at the example d
-00000b20: 6174 6173 6574 2061 6e64 2063 6f6e 6669  ataset and confi
-00000b30: 6773 2077 696c 6c20 6c6f 6f6b 206c 696b  gs will look lik
-00000b40: 653a 0a0a 6060 6070 7974 686f 6e0a 7b0a  e:..```python.{.
-00000b50: 2020 2020 2274 6173 6b5f 6e61 6d65 223a      "task_name":
-00000b60: 2022 4d6f 7669 6553 656e 7469 6d65 6e74   "MovieSentiment
-00000b70: 5265 7669 6577 222c 0a20 2020 2022 7461  Review",.    "ta
-00000b80: 736b 5f74 7970 6522 3a20 2263 6c61 7373  sk_type": "class
-00000b90: 6966 6963 6174 696f 6e22 2c0a 2020 2020  ification",.    
-00000ba0: 226d 6f64 656c 223a 207b 0a20 2020 2020  "model": {.     
-00000bb0: 2020 2022 7072 6f76 6964 6572 223a 2022     "provider": "
-00000bc0: 6f70 656e 6169 222c 0a20 2020 2020 2020  openai",.       
-00000bd0: 2022 6e61 6d65 223a 2022 6770 742d 332e   "name": "gpt-3.
-00000be0: 352d 7475 7262 6f22 0a20 2020 207d 2c0a  5-turbo".    },.
-00000bf0: 2020 2020 2264 6174 6173 6574 223a 207b      "dataset": {
-00000c00: 0a20 2020 2020 2020 2022 6c61 6265 6c5f  .        "label_
-00000c10: 636f 6c75 6d6e 223a 2022 6c61 6265 6c22  column": "label"
-00000c20: 2c0a 2020 2020 2020 2020 2264 656c 696d  ,.        "delim
-00000c30: 6974 6572 223a 2022 2c22 0a20 2020 207d  iter": ",".    }
-00000c40: 2c0a 2020 2020 2270 726f 6d70 7422 3a20  ,.    "prompt": 
-00000c50: 7b0a 2020 2020 2020 2020 2274 6173 6b5f  {.        "task_
-00000c60: 6775 6964 656c 696e 6573 223a 2022 596f  guidelines": "Yo
-00000c70: 7520 6172 6520 616e 2065 7870 6572 7420  u are an expert 
-00000c80: 6174 2061 6e61 6c79 7a69 6e67 2074 6865  at analyzing the
-00000c90: 2073 656e 7469 6d65 6e74 206f 6620 6d6f   sentiment of mo
-00000ca0: 7669 6577 2072 6576 6965 7773 2e20 596f  view reviews. Yo
-00000cb0: 7572 206a 6f62 2069 7320 746f 2063 6c61  ur job is to cla
-00000cc0: 7373 6966 7920 7468 6520 7072 6f76 6964  ssify the provid
-00000cd0: 6564 206d 6f76 6965 2072 6576 6965 7720  ed movie review 
-00000ce0: 696e 746f 206f 6e65 206f 6620 7468 6520  into one of the 
-00000cf0: 666f 6c6c 6f77 696e 6720 6c61 6265 6c73  following labels
-00000d00: 3a20 7b6c 6162 656c 737d 222c 0a20 2020  : {labels}",.   
-00000d10: 2020 2020 2022 6c61 6265 6c73 223a 205b       "labels": [
-00000d20: 0a20 2020 2020 2020 2020 2020 2022 706f  .            "po
-00000d30: 7369 7469 7665 222c 0a20 2020 2020 2020  sitive",.       
-00000d40: 2020 2020 2022 6e65 6761 7469 7665 222c       "negative",
-00000d50: 0a20 2020 2020 2020 2020 2020 2022 6e65  .            "ne
-00000d60: 7574 7261 6c22 2c0a 2020 2020 2020 2020  utral",.        
-00000d70: 5d2c 0a20 2020 2020 2020 2022 6665 775f  ],.        "few_
-00000d80: 7368 6f74 5f65 7861 6d70 6c65 7322 3a20  shot_examples": 
-00000d90: 5b0a 2020 2020 2020 2020 2020 2020 7b0a  [.            {.
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 2265 7861 6d70 6c65 223a 2022 4920 676f  "example": "I go
-00000dc0: 7420 6120 6661 6972 6c79 2075 6e69 6e73  t a fairly unins
-00000dd0: 7069 7265 6420 7374 7570 6964 2066 696c  pired stupid fil
-00000de0: 6d20 6162 6f75 7420 686f 7720 6875 6d61  m about how huma
-00000df0: 6e20 696e 6475 7374 7279 2069 7320 6261  n industry is ba
-00000e00: 6420 666f 7220 6e61 7475 7265 2e22 2c0a  d for nature.",.
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 226c 6162 656c 223a 2022 6e65 6761 7469  "label": "negati
-00000e30: 7665 220a 2020 2020 2020 2020 2020 2020  ve".            
-00000e40: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
-00000e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e60: 2022 6578 616d 706c 6522 3a20 2249 206c   "example": "I l
-00000e70: 6f76 6564 2074 6869 7320 6d6f 7669 652e  oved this movie.
-00000e80: 2049 2066 6f75 6e64 2069 7420 7665 7279   I found it very
-00000e90: 2068 6561 7274 2077 6172 6d69 6e67 2074   heart warming t
-00000ea0: 6f20 7365 6520 4164 616d 2057 6573 742c  o see Adam West,
-00000eb0: 2042 7572 7420 5761 7264 2c20 4672 616e   Burt Ward, Fran
-00000ec0: 6b20 476f 7273 6869 6e2c 2061 6e64 204a  k Gorshin, and J
-00000ed0: 756c 6965 204e 6577 6d61 7220 746f 6765  ulie Newmar toge
-00000ee0: 7468 6572 2061 6761 696e 2e22 2c0a 2020  ther again.",.  
-00000ef0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00000f00: 6162 656c 223a 2022 706f 7369 7469 7665  abel": "positive
-00000f10: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
-00000f20: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
-00000f30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000f40: 6578 616d 706c 6522 3a20 2254 6869 7320  example": "This 
-00000f50: 6d6f 7669 6520 7769 6c6c 2062 6520 706c  movie will be pl
-00000f60: 6179 6564 206e 6578 7420 7765 656b 2061  ayed next week a
-00000f70: 7420 7468 6520 4368 696e 6573 6520 7468  t the Chinese th
-00000f80: 6561 7465 722e 222c 0a20 2020 2020 2020  eater.",.       
-00000f90: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00000fa0: 3a20 226e 6575 7472 616c 220a 2020 2020  : "neutral".    
-00000fb0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000fc0: 2020 5d2c 0a20 2020 2020 2020 2022 6578    ],.        "ex
-00000fd0: 616d 706c 655f 7465 6d70 6c61 7465 223a  ample_template":
-00000fe0: 2022 496e 7075 743a 207b 6578 616d 706c   "Input: {exampl
-00000ff0: 657d 5c6e 4f75 7470 7574 3a20 7b6c 6162  e}\nOutput: {lab
-00001000: 656c 7d22 0a20 2020 207d 0a7d 0a60 6060  el}".    }.}.```
-00001010: 0a0a 496e 6974 6961 6c69 7a65 2074 6865  ..Initialize the
-00001020: 206c 6162 656c 696e 6720 6167 656e 7420   labeling agent 
-00001030: 616e 6420 7061 7373 2069 7420 7468 6520  and pass it the 
-00001040: 636f 6e66 6967 3a0a 0a60 6060 7079 7468  config:..```pyth
-00001050: 6f6e 0a0a 6672 6f6d 2061 7574 6f6c 6162  on..from autolab
-00001060: 656c 2069 6d70 6f72 7420 4c61 6265 6c69  el import Labeli
-00001070: 6e67 4167 656e 740a 0a61 6765 6e74 203d  ngAgent..agent =
-00001080: 204c 6162 656c 696e 6741 6765 6e74 2863   LabelingAgent(c
-00001090: 6f6e 6669 673d 2763 6f6e 6669 672e 6a73  onfig='config.js
-000010a0: 6f6e 2729 0a60 6060 0a0a 5072 6576 6965  on').```..Previe
-000010b0: 7720 616e 2065 7861 6d70 6c65 2070 726f  w an example pro
-000010c0: 6d70 7420 7468 6174 2077 696c 6c20 6265  mpt that will be
-000010d0: 2073 656e 7420 746f 2074 6865 204c 4c4d   sent to the LLM
-000010e0: 3a0a 0a60 6060 7079 7468 6f6e 0a61 6765  :..```python.age
-000010f0: 6e74 2e70 6c61 6e28 2765 7861 6d70 6c65  nt.plan('example
-00001100: 732f 6d6f 7669 655f 7265 7669 6577 732f  s/movie_reviews/
-00001110: 6461 7461 7365 742e 6373 7627 290a 6060  dataset.csv').``
-00001120: 600a 0a54 6869 7320 7072 696e 7473 3a0a  `..This prints:.
-00001130: 0a60 6060 0ae2 9481 e294 81e2 9481 e294  .```............
-00001140: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001150: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001160: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001170: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001180: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001190: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-000011a0: 81e2 9481 e294 81e2 9481 e294 8120 3130  ............. 10
-000011b0: 302f 3130 3020 303a 3030 3a30 3020 303a  0/100 0:00:00 0:
-000011c0: 3030 3a30 300a e294 8ce2 9480 e294 80e2  00:00...........
-000011d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000011e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000011f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001200: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001210: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
-00001220: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001230: 9480 e294 80e2 9490 0ae2 9482 2054 6f74  ............ Tot
-00001240: 616c 2045 7374 696d 6174 6564 2043 6f73  al Estimated Cos
-00001250: 7420 2020 2020 e294 8220 2430 2e35 3338  t     ... $0.538
-00001260: 2020 e294 820a e294 8220 4e75 6d62 6572    ....... Number
-00001270: 206f 6620 4578 616d 706c 6573 2020 2020   of Examples    
-00001280: 2020 20e2 9482 2032 3030 2020 2020 20e2     ... 200     .
-00001290: 9482 0ae2 9482 2041 7665 7261 6765 2063  ...... Average c
-000012a0: 6f73 7420 7065 7220 6578 616d 706c 6520  ost per example 
-000012b0: e294 8220 302e 3030 3236 3920 e294 820a  ... 0.00269 ....
-000012c0: e294 94e2 9480 e294 80e2 9480 e294 80e2  ................
-000012d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000012e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000012f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001310: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-00001320: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001330: 9498 0ae2 9480 e294 80e2 9480 e294 80e2  ................
-00001340: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001350: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001360: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001370: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001380: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001390: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000013a0: 9480 e294 80e2 9480 e294 80e2 9480 0a0a  ................
-000013b0: 5072 6f6d 7074 2045 7861 6d70 6c65 3a0a  Prompt Example:.
-000013c0: 596f 7520 6172 6520 616e 2065 7870 6572  You are an exper
-000013d0: 7420 6174 2061 6e61 6c79 7a69 6e67 2074  t at analyzing t
-000013e0: 6865 2073 656e 7469 6d65 6e74 206f 6620  he sentiment of 
-000013f0: 6d6f 7669 6577 2072 6576 6965 7773 2e20  moview reviews. 
-00001400: 596f 7572 206a 6f62 2069 7320 746f 2063  Your job is to c
-00001410: 6c61 7373 6966 7920 7468 6520 7072 6f76  lassify the prov
-00001420: 6964 6564 206d 6f76 6965 2072 6576 6965  ided movie revie
-00001430: 7720 696e 746f 206f 6e65 206f 6620 7468  w into one of th
-00001440: 6520 666f 6c6c 6f77 696e 6720 6c61 6265  e following labe
-00001450: 6c73 3a20 5b70 6f73 6974 6976 652c 206e  ls: [positive, n
-00001460: 6567 6174 6976 652c 206e 6575 7472 616c  egative, neutral
-00001470: 5d0a 0a59 6f75 2077 696c 6c20 7265 7475  ]..You will retu
-00001480: 726e 2074 6865 2061 6e73 7765 7220 7769  rn the answer wi
-00001490: 7468 206a 7573 7420 6f6e 6520 656c 656d  th just one elem
-000014a0: 656e 743a 2022 7468 6520 636f 7272 6563  ent: "the correc
-000014b0: 7420 6c61 6265 6c22 0a0a 536f 6d65 2065  t label"..Some e
-000014c0: 7861 6d70 6c65 7320 7769 7468 2074 6865  xamples with the
-000014d0: 6972 206f 7574 7075 7420 616e 7377 6572  ir output answer
-000014e0: 7320 6172 6520 7072 6f76 6964 6564 2062  s are provided b
-000014f0: 656c 6f77 3a0a 0a45 7861 6d70 6c65 3a20  elow:..Example: 
-00001500: 4920 676f 7420 6120 6661 6972 6c79 2075  I got a fairly u
-00001510: 6e69 6e73 7069 7265 6420 7374 7570 6964  ninspired stupid
-00001520: 2066 696c 6d20 6162 6f75 7420 686f 7720   film about how 
-00001530: 6875 6d61 6e20 696e 6475 7374 7279 2069  human industry i
-00001540: 7320 6261 6420 666f 7220 6e61 7475 7265  s bad for nature
-00001550: 2e0a 4f75 7470 7574 3a0a 6e65 6761 7469  ..Output:.negati
-00001560: 7665 0a0a 4578 616d 706c 653a 2049 206c  ve..Example: I l
-00001570: 6f76 6564 2074 6869 7320 6d6f 7669 652e  oved this movie.
-00001580: 2049 2066 6f75 6e64 2069 7420 7665 7279   I found it very
-00001590: 2068 6561 7274 2077 6172 6d69 6e67 2074   heart warming t
-000015a0: 6f20 7365 6520 4164 616d 2057 6573 742c  o see Adam West,
-000015b0: 2042 7572 7420 5761 7264 2c20 4672 616e   Burt Ward, Fran
-000015c0: 6b20 476f 7273 6869 6e2c 2061 6e64 204a  k Gorshin, and J
-000015d0: 756c 6965 204e 6577 6d61 7220 746f 6765  ulie Newmar toge
-000015e0: 7468 6572 2061 6761 696e 2e0a 4f75 7470  ther again..Outp
-000015f0: 7574 3a0a 706f 7369 7469 7665 0a0a 4578  ut:.positive..Ex
-00001600: 616d 706c 653a 2054 6869 7320 6d6f 7669  ample: This movi
-00001610: 6520 7769 6c6c 2062 6520 706c 6179 6564  e will be played
-00001620: 206e 6578 7420 7765 656b 2061 7420 7468   next week at th
-00001630: 6520 4368 696e 6573 6520 7468 6561 7465  e Chinese theate
-00001640: 722e 0a4f 7574 7075 743a 0a6e 6575 7472  r..Output:.neutr
-00001650: 616c 0a0a 4e6f 7720 4920 7761 6e74 2079  al..Now I want y
-00001660: 6f75 2074 6f20 6c61 6265 6c20 7468 6520  ou to label the 
-00001670: 666f 6c6c 6f77 696e 6720 6578 616d 706c  following exampl
-00001680: 653a 0a49 6e70 7574 3a20 4120 7261 7265  e:.Input: A rare
-00001690: 2065 7863 6570 7469 6f6e 2074 6f20 7468   exception to th
-000016a0: 6520 7275 6c65 2074 6861 7420 6772 6561  e rule that grea
-000016b0: 7420 6c69 7465 7261 7475 7265 206d 616b  t literature mak
-000016c0: 6573 2064 6973 6170 706f 696e 7469 6e67  es disappointing
-000016d0: 2066 696c 6d73 2e0a 4f75 7470 7574 3a0a   films..Output:.
-000016e0: 0ae2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000016f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001700: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001710: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001720: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001730: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001740: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001750: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001760: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001770: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001780: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001790: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000017a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000017b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000017c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000017d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000017e0: e294 80e2 9480 e294 80e2 9480 0a0a 6060  ..............``
-000017f0: 600a 0a46 696e 616c 6c79 2c20 7765 2063  `..Finally, we c
-00001800: 616e 2072 756e 2074 6865 206c 6162 656c  an run the label
-00001810: 696e 6720 6f6e 2061 2073 7562 7365 7420  ing on a subset 
-00001820: 6f72 2065 6e74 6972 6574 7920 6f66 2074  or entirety of t
-00001830: 6865 2064 6174 6173 6574 3a0a 0a60 6060  he dataset:..```
-00001840: 7079 7468 6f6e 0a6c 6162 656c 732c 206f  python.labels, o
-00001850: 7574 7075 745f 6466 2c20 6d65 7472 6963  utput_df, metric
-00001860: 7320 3d20 6167 656e 742e 7275 6e28 2765  s = agent.run('e
-00001870: 7861 6d70 6c65 732f 6d6f 7669 655f 7265  xamples/movie_re
-00001880: 7669 6577 732f 6461 7461 7365 742e 6373  views/dataset.cs
-00001890: 7627 290a 6060 600a 0a23 2320 f09f 998c  v').```..## ....
-000018a0: 2043 6f6e 7472 6962 7574 696e 670a 0a41   Contributing..A
-000018b0: 7574 6f6c 6162 656c 2069 7320 6120 7261  utolabel is a ra
-000018c0: 7069 646c 7920 6465 7665 6c6f 7069 6e67  pidly developing
-000018d0: 2070 726f 6a65 6374 2e20 5765 2077 656c   project. We wel
-000018e0: 636f 6d65 2063 6f6e 7472 6962 7574 696f  come contributio
-000018f0: 6e73 2069 6e20 616c 6c20 666f 726d 7320  ns in all forms 
-00001900: 2d20 6275 6720 7265 706f 7274 732c 2070  - bug reports, p
-00001910: 756c 6c20 7265 7175 6573 7473 2061 6e64  ull requests and
-00001920: 2069 6465 6173 2066 6f72 2069 6d70 726f   ideas for impro
-00001930: 7669 6e67 2074 6865 206c 6962 7261 7279  ving the library
-00001940: 2e0a 0a31 2e20 4a6f 696e 2074 6865 2063  ...1. Join the c
-00001950: 6f6e 7665 7273 6174 696f 6e20 6f6e 205b  onversation on [
-00001960: 4469 7363 6f72 645d 2868 7474 7073 3a2f  Discord](https:/
-00001970: 2f64 6973 636f 7264 2e67 672f 6677 6556  /discord.gg/fweV
-00001980: 6e52 7836 4355 290a 322e 2052 6576 6965  nRx6CU).2. Revie
-00001990: 7720 7468 6520 f09f 9ba3 efb8 8f20 5b52  w the ....... [R
-000019a0: 6f61 646d 6170 5d28 2920 616e 6420 636f  oadmap]() and co
-000019b0: 6e74 7269 6275 7465 2079 6f75 7220 6964  ntribute your id
-000019c0: 6561 732e 0a33 2e20 4772 6162 2061 6e20  eas..3. Grab an 
-000019d0: 5b6f 7065 6e20 6973 7375 655d 2868 7474  [open issue](htt
-000019e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000019f0: 7265 6675 656c 2d61 692f 6175 746f 6c61  refuel-ai/autola
-00001a00: 6265 6c2f 6973 7375 6573 2920 6f6e 2047  bel/issues) on G
-00001a10: 6974 6875 622c 2061 6e64 2073 7562 6d69  ithub, and submi
-00001a20: 7420 6120 5b70 756c 6c20 7265 7175 6573  t a [pull reques
-00001a30: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00001a40: 622e 636f 6d2f 7265 6675 656c 2d61 692f  b.com/refuel-ai/
-00001a50: 6175 746f 6c61 6265 6c2f 626c 6f62 2f6d  autolabel/blob/m
-00001a60: 6169 6e2f 434f 4e54 5249 4255 5449 4e47  ain/CONTRIBUTING
-00001a70: 2e6d 6429 2e0a                           .md)..
+00000000: 3c70 6963 7475 7265 3e0a 2020 3c69 6d67  <picture>.  <img
+00000010: 2061 6c74 3d22 5265 6675 656c 206c 6f67   alt="Refuel log
+00000020: 6f22 2073 7263 3d22 646f 6373 2f61 7373  o" src="docs/ass
+00000030: 6574 732f 4175 746f 6c61 6265 6c5f 626c  ets/Autolabel_bl
+00000040: 6b5f 775f 6261 636b 6772 6f75 6e64 2e70  k_w_background.p
+00000050: 6e67 223e 0a3c 2f70 6963 7475 7265 3e0a  ng">.</picture>.
+00000060: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000070: 223e 0a20 2020 203c 623e 436c 6561 6e2c  ">.    <b>Clean,
+00000080: 206c 6162 656c 6564 2064 6174 6120 6174   labeled data at
+00000090: 2074 6865 2073 7065 6564 206f 6620 7468   the speed of th
+000000a0: 6f75 6768 743c 2f62 3e2e 0a3c 2f70 3e0a  ought</b>..</p>.
+000000b0: 0a3c 6834 2061 6c69 676e 3d22 6365 6e74  .<h4 align="cent
+000000c0: 6572 223e 0a20 203c 6120 6872 6566 3d22  er">.  <a href="
+000000d0: 6874 7470 733a 2f2f 646f 6373 2e72 6566  https://docs.ref
+000000e0: 7565 6c2e 6169 2f67 7569 6465 2f6f 7665  uel.ai/guide/ove
+000000f0: 7276 6965 772f 6765 7474 696e 672d 7374  rview/getting-st
+00000100: 6172 7465 642f 223e 4765 7474 696e 6720  arted/">Getting 
+00000110: 7374 6172 7465 643c 2f61 3e20 7c0a 2020  started</a> |.  
+00000120: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000130: 2f64 6f63 732e 7265 6675 656c 2e61 692f  /docs.refuel.ai/
+00000140: 223e 446f 6373 3c2f 613e 207c 0a20 203c  ">Docs</a> |.  <
+00000150: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000160: 6469 7363 6f72 642e 6767 2f66 7765 566e  discord.gg/fweVn
+00000170: 5278 3643 5522 3e44 6973 636f 7264 3c2f  Rx6CU">Discord</
+00000180: 613e 207c 0a20 203c 6120 6872 6566 3d22  a> |.  <a href="
+00000190: 6874 7470 733a 2f2f 7477 6974 7465 722e  https://twitter.
+000001a0: 636f 6d2f 5265 6675 656c 4149 223e 5477  com/RefuelAI">Tw
+000001b0: 6974 7465 723c 2f61 3e20 7c0a 2020 3c61  itter</a> |.  <a
+000001c0: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
+000001d0: 7777 2e72 6566 7565 6c2e 6169 2f22 3e57  ww.refuel.ai/">W
+000001e0: 6562 7369 7465 3c2f 613e 0a3c 2f68 343e  ebsite</a>.</h4>
+000001f0: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000200: 6e74 6572 2220 7374 796c 653d 2277 6964  nter" style="wid
+00000210: 7468 3a38 3030 7078 223e 0a0a 5b21 5b6c  th:800px">..[![l
+00000220: 696e 745d 2868 7474 7073 3a2f 2f67 6974  int](https://git
+00000230: 6875 622e 636f 6d2f 7265 6675 656c 2d61  hub.com/refuel-a
+00000240: 692f 6175 746f 6c61 6265 6c2f 6163 7469  i/autolabel/acti
+00000250: 6f6e 732f 776f 726b 666c 6f77 732f 626c  ons/workflows/bl
+00000260: 6163 6b2e 7961 6d6c 2f62 6164 6765 2e73  ack.yaml/badge.s
+00000270: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000280: 6875 622e 636f 6d2f 7265 6675 656c 2d61  hub.com/refuel-a
+00000290: 692f 6175 746f 6c61 6265 6c2f 6163 7469  i/autolabel/acti
+000002a0: 6f6e 732f 776f 726b 666c 6f77 732f 626c  ons/workflows/bl
+000002b0: 6163 6b2e 7961 6d6c 2f62 6164 6765 2e73  ack.yaml/badge.s
+000002c0: 7667 2920 215b 5465 7374 735d 2868 7474  vg) ![Tests](htt
+000002d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000002e0: 7265 6675 656c 2d61 692f 6175 746f 6c61  refuel-ai/autola
+000002f0: 6265 6c2f 6163 7469 6f6e 732f 776f 726b  bel/actions/work
+00000300: 666c 6f77 732f 7465 7374 2e79 616d 6c2f  flows/test.yaml/
+00000310: 6261 6467 652e 7376 6729 2021 5b43 6f6d  badge.svg) ![Com
+00000320: 6d69 7420 4163 7469 7669 7479 5d28 6874  mit Activity](ht
+00000330: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000340: 732e 696f 2f67 6974 6875 622f 636f 6d6d  s.io/github/comm
+00000350: 6974 2d61 6374 6976 6974 792f 6d2f 7265  it-activity/m/re
+00000360: 6675 656c 2d61 692f 6175 746f 6c61 6265  fuel-ai/autolabe
+00000370: 6c29 205b 215b 4469 7363 6f72 645d 2868  l) [![Discord](h
+00000380: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000390: 6473 2e69 6f2f 6469 7363 6f72 642f 3130  ds.io/discord/10
+000003a0: 3938 3734 3636 3933 3135 3239 3331 3930  9874669315293190
+000003b0: 3129 5d28 6874 7470 733a 2f2f 6469 7363  1)](https://disc
+000003c0: 6f72 642e 6767 2f66 7765 566e 5278 3643  ord.gg/fweVnRx6C
+000003d0: 5529 205b 215b 4c69 6365 6e73 653a 204d  U) [![License: M
+000003e0: 4954 5d28 6874 7470 733a 2f2f 6261 6467  IT](https://badg
+000003f0: 656e 2e6e 6574 2f62 6164 6765 2f6c 6963  en.net/badge/lic
+00000400: 656e 7365 2f4d 4954 2f62 6c75 6529 5d28  ense/MIT/blue)](
+00000410: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00000420: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
+00000430: 4d49 5429 0a3c 2f64 6976 3e0a 0a23 2320  MIT).</div>..## 
+00000440: e29a a120 5175 6963 6b20 496e 7374 616c  ... Quick Instal
+00000450: 6c0a 0a60 7069 7020 696e 7374 616c 6c20  l..`pip install 
+00000460: 7265 6675 656c 2d61 7574 6f6c 6162 656c  refuel-autolabel
+00000470: 600a 0a23 2320 f09f 8fb7 2057 6861 7420  `..## .... What 
+00000480: 6973 2041 7574 6f6c 6162 656c 0a0a 4163  is Autolabel..Ac
+00000490: 6365 7373 2074 6f20 5b6c 6172 6765 2c20  cess to [large, 
+000004a0: 636c 6561 6e20 616e 6420 6469 7665 7273  clean and divers
+000004b0: 655d 2868 7474 7073 3a2f 2f74 7769 7474  e](https://twitt
+000004c0: 6572 2e63 6f6d 2f6b 6172 7061 7468 792f  er.com/karpathy/
+000004d0: 7374 6174 7573 2f31 3532 3834 3433 3132  status/152844312
+000004e0: 3435 3737 3531 3334 3732 3f6c 616e 673d  4577513472?lang=
+000004f0: 656e 2920 6c61 6265 6c65 6420 6461 7461  en) labeled data
+00000500: 7365 7473 2069 7320 6120 6372 6974 6963  sets is a critic
+00000510: 616c 2063 6f6d 706f 6e65 6e74 2066 6f72  al component for
+00000520: 2061 6e79 206d 6163 6869 6e65 206c 6561   any machine lea
+00000530: 726e 696e 6720 6566 666f 7274 2074 6f20  rning effort to 
+00000540: 6265 2073 7563 6365 7373 6675 6c2e 2053  be successful. S
+00000550: 7461 7465 2d6f 662d 7468 652d 6172 7420  tate-of-the-art 
+00000560: 4c4c 4d73 206c 696b 6520 4750 542d 3420  LLMs like GPT-4 
+00000570: 6172 6520 6162 6c65 2074 6f20 5b61 7574  are able to [aut
+00000580: 6f6d 6174 6963 616c 6c79 206c 6162 656c  omatically label
+00000590: 2064 6174 615d 2868 7474 7073 3a2f 2f61   data](https://a
+000005a0: 7278 6976 2e6f 7267 2f61 6273 2f32 3330  rxiv.org/abs/230
+000005b0: 332e 3135 3035 3629 2077 6974 6820 5b68  3.15056) with [h
+000005c0: 6967 6820 6163 6375 7261 6379 5d28 6874  igh accuracy](ht
+000005d0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+000005e0: 6162 732f 3233 3033 2e31 3638 3534 292c  abs/2303.16854),
+000005f0: 2061 6e64 2061 7420 6120 6672 6163 7469   and at a fracti
+00000600: 6f6e 206f 6620 7468 6520 636f 7374 2061  on of the cost a
+00000610: 6e64 2074 696d 6520 636f 6d70 6172 6564  nd time compared
+00000620: 2074 6f20 6d61 6e75 616c 206c 6162 656c   to manual label
+00000630: 696e 672e 0a0a 4175 746f 6c61 6265 6c20  ing...Autolabel 
+00000640: 6973 2061 2050 7974 686f 6e20 6c69 6272  is a Python libr
+00000650: 6172 7920 746f 206c 6162 656c 2c20 636c  ary to label, cl
+00000660: 6561 6e20 616e 6420 656e 7269 6368 2074  ean and enrich t
+00000670: 6578 7420 6461 7461 7365 7473 2077 6974  ext datasets wit
+00000680: 6820 616e 7920 4c61 7267 6520 4c61 6e67  h any Large Lang
+00000690: 7561 6765 204d 6f64 656c 7320 284c 4c4d  uage Models (LLM
+000006a0: 2920 6f66 2079 6f75 7220 6368 6f69 6365  ) of your choice
+000006b0: 2e0a 0a23 2320 f09f 9a80 2047 6574 7469  ...## .... Getti
+000006c0: 6e67 2073 7461 7274 6564 0a0a 4175 746f  ng started..Auto
+000006d0: 6c61 6265 6c20 7072 6f76 6964 6573 2061  label provides a
+000006e0: 2073 696d 706c 6520 332d 7374 6570 2070   simple 3-step p
+000006f0: 726f 6365 7373 2066 6f72 206c 6162 656c  rocess for label
+00000700: 696e 6720 6461 7461 3a0a 0a31 2e20 5370  ing data:..1. Sp
+00000710: 6563 6966 7920 7468 6520 6c61 6265 6c69  ecify the labeli
+00000720: 6e67 2067 7569 6465 6c69 6e65 7320 616e  ng guidelines an
+00000730: 6420 4c4c 4d20 6d6f 6465 6c20 746f 2075  d LLM model to u
+00000740: 7365 2069 6e20 6120 4a53 4f4e 2063 6f6e  se in a JSON con
+00000750: 6669 672e 0a32 2e20 4472 792d 7275 6e20  fig..2. Dry-run 
+00000760: 746f 206d 616b 6520 7375 7265 2074 6865  to make sure the
+00000770: 2066 696e 616c 2070 726f 6d70 7420 6c6f   final prompt lo
+00000780: 6f6b 7320 676f 6f64 2e0a 332e 204b 6963  oks good..3. Kic
+00000790: 6b20 6f66 6620 6120 6c61 6265 6c69 6e67  k off a labeling
+000007a0: 2072 756e 2066 6f72 2079 6f75 7220 6461   run for your da
+000007b0: 7461 7365 7421 0a0a 4c65 7427 7320 696d  taset!..Let's im
+000007c0: 6167 696e 6520 7765 2061 7265 2062 7569  agine we are bui
+000007d0: 6c64 696e 6720 616e 204d 4c20 6d6f 6465  lding an ML mode
+000007e0: 6c20 746f 2061 6e61 6c79 7a65 2073 656e  l to analyze sen
+000007f0: 7469 6d65 6e74 2061 6e61 6c79 7369 7320  timent analysis 
+00000800: 6f66 206d 6f76 6965 2072 6576 6965 772e  of movie review.
+00000810: 2057 6520 6861 7665 2061 2064 6174 6173   We have a datas
+00000820: 6574 206f 6620 6d6f 7669 6520 7265 7669  et of movie revi
+00000830: 6577 7320 7468 6174 2077 6527 6420 6c69  ews that we'd li
+00000840: 6b65 2074 6f20 6765 7420 6c61 6265 6c65  ke to get labele
+00000850: 6420 6669 7273 742e 2046 6f72 2074 6869  d first. For thi
+00000860: 7320 6361 7365 2c20 6865 7265 2773 2077  s case, here's w
+00000870: 6861 7420 7468 6520 6578 616d 706c 6520  hat the example 
+00000880: 6461 7461 7365 7420 616e 6420 636f 6e66  dataset and conf
+00000890: 6967 7320 7769 6c6c 206c 6f6f 6b20 6c69  igs will look li
+000008a0: 6b65 3a0a 0a60 6060 7079 7468 6f6e 0a7b  ke:..```python.{
+000008b0: 0a20 2020 2022 7461 736b 5f6e 616d 6522  .    "task_name"
+000008c0: 3a20 224d 6f76 6965 5365 6e74 696d 656e  : "MovieSentimen
+000008d0: 7452 6576 6965 7722 2c0a 2020 2020 2274  tReview",.    "t
+000008e0: 6173 6b5f 7479 7065 223a 2022 636c 6173  ask_type": "clas
+000008f0: 7369 6669 6361 7469 6f6e 222c 0a20 2020  sification",.   
+00000900: 2022 6d6f 6465 6c22 3a20 7b0a 2020 2020   "model": {.    
+00000910: 2020 2020 2270 726f 7669 6465 7222 3a20      "provider": 
+00000920: 226f 7065 6e61 6922 2c0a 2020 2020 2020  "openai",.      
+00000930: 2020 226e 616d 6522 3a20 2267 7074 2d33    "name": "gpt-3
+00000940: 2e35 2d74 7572 626f 220a 2020 2020 7d2c  .5-turbo".    },
+00000950: 0a20 2020 2022 6461 7461 7365 7422 3a20  .    "dataset": 
+00000960: 7b0a 2020 2020 2020 2020 226c 6162 656c  {.        "label
+00000970: 5f63 6f6c 756d 6e22 3a20 226c 6162 656c  _column": "label
+00000980: 222c 0a20 2020 2020 2020 2022 6465 6c69  ",.        "deli
+00000990: 6d69 7465 7222 3a20 222c 220a 2020 2020  miter": ",".    
+000009a0: 7d2c 0a20 2020 2022 7072 6f6d 7074 223a  },.    "prompt":
+000009b0: 207b 0a20 2020 2020 2020 2022 7461 736b   {.        "task
+000009c0: 5f67 7569 6465 6c69 6e65 7322 3a20 2259  _guidelines": "Y
+000009d0: 6f75 2061 7265 2061 6e20 6578 7065 7274  ou are an expert
+000009e0: 2061 7420 616e 616c 797a 696e 6720 7468   at analyzing th
+000009f0: 6520 7365 6e74 696d 656e 7420 6f66 206d  e sentiment of m
+00000a00: 6f76 6965 2072 6576 6965 7773 2e20 596f  ovie reviews. Yo
+00000a10: 7572 206a 6f62 2069 7320 746f 2063 6c61  ur job is to cla
+00000a20: 7373 6966 7920 7468 6520 7072 6f76 6964  ssify the provid
+00000a30: 6564 206d 6f76 6965 2072 6576 6965 7720  ed movie review 
+00000a40: 696e 746f 206f 6e65 206f 6620 7468 6520  into one of the 
+00000a50: 666f 6c6c 6f77 696e 6720 6c61 6265 6c73  following labels
+00000a60: 3a20 7b6c 6162 656c 737d 222c 0a20 2020  : {labels}",.   
+00000a70: 2020 2020 2022 6c61 6265 6c73 223a 205b       "labels": [
+00000a80: 0a20 2020 2020 2020 2020 2020 2022 706f  .            "po
+00000a90: 7369 7469 7665 222c 0a20 2020 2020 2020  sitive",.       
+00000aa0: 2020 2020 2022 6e65 6761 7469 7665 222c       "negative",
+00000ab0: 0a20 2020 2020 2020 2020 2020 2022 6e65  .            "ne
+00000ac0: 7574 7261 6c22 2c0a 2020 2020 2020 2020  utral",.        
+00000ad0: 5d2c 0a20 2020 2020 2020 2022 6665 775f  ],.        "few_
+00000ae0: 7368 6f74 5f65 7861 6d70 6c65 7322 3a20  shot_examples": 
+00000af0: 5b0a 2020 2020 2020 2020 2020 2020 7b0a  [.            {.
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b10: 2265 7861 6d70 6c65 223a 2022 4920 676f  "example": "I go
+00000b20: 7420 6120 6661 6972 6c79 2075 6e69 6e73  t a fairly unins
+00000b30: 7069 7265 6420 7374 7570 6964 2066 696c  pired stupid fil
+00000b40: 6d20 6162 6f75 7420 686f 7720 6875 6d61  m about how huma
+00000b50: 6e20 696e 6475 7374 7279 2069 7320 6261  n industry is ba
+00000b60: 6420 666f 7220 6e61 7475 7265 2e22 2c0a  d for nature.",.
+00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b80: 226c 6162 656c 223a 2022 6e65 6761 7469  "label": "negati
+00000b90: 7665 220a 2020 2020 2020 2020 2020 2020  ve".            
+00000ba0: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
+00000bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000bc0: 2022 6578 616d 706c 6522 3a20 2249 206c   "example": "I l
+00000bd0: 6f76 6564 2074 6869 7320 6d6f 7669 652e  oved this movie.
+00000be0: 2049 2066 6f75 6e64 2069 7420 7665 7279   I found it very
+00000bf0: 2068 6561 7274 2077 6172 6d69 6e67 2074   heart warming t
+00000c00: 6f20 7365 6520 4164 616d 2057 6573 742c  o see Adam West,
+00000c10: 2042 7572 7420 5761 7264 2c20 4672 616e   Burt Ward, Fran
+00000c20: 6b20 476f 7273 6869 6e2c 2061 6e64 204a  k Gorshin, and J
+00000c30: 756c 6965 204e 6577 6d61 7220 746f 6765  ulie Newmar toge
+00000c40: 7468 6572 2061 6761 696e 2e22 2c0a 2020  ther again.",.  
+00000c50: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00000c60: 6162 656c 223a 2022 706f 7369 7469 7665  abel": "positive
+00000c70: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
+00000c80: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000ca0: 6578 616d 706c 6522 3a20 2254 6869 7320  example": "This 
+00000cb0: 6d6f 7669 6520 7769 6c6c 2062 6520 706c  movie will be pl
+00000cc0: 6179 6564 206e 6578 7420 7765 656b 2061  ayed next week a
+00000cd0: 7420 7468 6520 4368 696e 6573 6520 7468  t the Chinese th
+00000ce0: 6561 7465 722e 222c 0a20 2020 2020 2020  eater.",.       
+00000cf0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00000d00: 3a20 226e 6575 7472 616c 220a 2020 2020  : "neutral".    
+00000d10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000d20: 2020 5d2c 0a20 2020 2020 2020 2022 6578    ],.        "ex
+00000d30: 616d 706c 655f 7465 6d70 6c61 7465 223a  ample_template":
+00000d40: 2022 496e 7075 743a 207b 6578 616d 706c   "Input: {exampl
+00000d50: 657d 5c6e 4f75 7470 7574 3a20 7b6c 6162  e}\nOutput: {lab
+00000d60: 656c 7d22 0a20 2020 207d 0a7d 0a60 6060  el}".    }.}.```
+00000d70: 0a0a 496e 6974 6961 6c69 7a65 2074 6865  ..Initialize the
+00000d80: 206c 6162 656c 696e 6720 6167 656e 7420   labeling agent 
+00000d90: 616e 6420 7061 7373 2069 7420 7468 6520  and pass it the 
+00000da0: 636f 6e66 6967 3a0a 0a60 6060 7079 7468  config:..```pyth
+00000db0: 6f6e 0a0a 6672 6f6d 2061 7574 6f6c 6162  on..from autolab
+00000dc0: 656c 2069 6d70 6f72 7420 4c61 6265 6c69  el import Labeli
+00000dd0: 6e67 4167 656e 740a 0a61 6765 6e74 203d  ngAgent..agent =
+00000de0: 204c 6162 656c 696e 6741 6765 6e74 2863   LabelingAgent(c
+00000df0: 6f6e 6669 673d 2763 6f6e 6669 672e 6a73  onfig='config.js
+00000e00: 6f6e 2729 0a60 6060 0a0a 5072 6576 6965  on').```..Previe
+00000e10: 7720 616e 2065 7861 6d70 6c65 2070 726f  w an example pro
+00000e20: 6d70 7420 7468 6174 2077 696c 6c20 6265  mpt that will be
+00000e30: 2073 656e 7420 746f 2074 6865 204c 4c4d   sent to the LLM
+00000e40: 3a0a 0a60 6060 7079 7468 6f6e 0a61 6765  :..```python.age
+00000e50: 6e74 2e70 6c61 6e28 2764 6174 6173 6574  nt.plan('dataset
+00000e60: 2e63 7376 2729 0a60 6060 0a0a 5468 6973  .csv').```..This
+00000e70: 2070 7269 6e74 733a 0a0a 6060 600a e294   prints:..```...
+00000e80: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00000e90: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00000ea0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00000eb0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00000ec0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00000ed0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00000ee0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00000ef0: e294 81e2 9481 2031 3030 2f31 3030 2030  ...... 100/100 0
+00000f00: 3a30 303a 3030 2030 3a30 303a 3030 0ae2  :00:00 0:00:00..
+00000f10: 948c e294 80e2 9480 e294 80e2 9480 e294  ................
+00000f20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000f30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000f40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000f50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000f60: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00000f70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000f80: 900a e294 8220 546f 7461 6c20 4573 7469  ..... Total Esti
+00000f90: 6d61 7465 6420 436f 7374 2020 2020 20e2  mated Cost     .
+00000fa0: 9482 2024 302e 3533 3820 20e2 9482 0ae2  .. $0.538  .....
+00000fb0: 9482 204e 756d 6265 7220 6f66 2045 7861  .. Number of Exa
+00000fc0: 6d70 6c65 7320 2020 2020 2020 e294 8220  mples       ... 
+00000fd0: 3230 3020 2020 2020 e294 820a e294 8220  200     ....... 
+00000fe0: 4176 6572 6167 6520 636f 7374 2070 6572  Average cost per
+00000ff0: 2065 7861 6d70 6c65 20e2 9482 2030 2e30   example ... 0.0
+00001000: 3032 3639 20e2 9482 0ae2 9494 e294 80e2  0269 ...........
+00001010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001050: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+00001060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001070: 9480 e294 80e2 9480 e294 980a e294 80e2  ................
+00001080: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000010a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000010b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000010c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000010d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000010e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000010f0: 80e2 9480 e294 800a 0a50 726f 6d70 7420  .........Prompt 
+00001100: 4578 616d 706c 653a 0a59 6f75 2061 7265  Example:.You are
+00001110: 2061 6e20 6578 7065 7274 2061 7420 616e   an expert at an
+00001120: 616c 797a 696e 6720 7468 6520 7365 6e74  alyzing the sent
+00001130: 696d 656e 7420 6f66 206d 6f76 6965 2072  iment of movie r
+00001140: 6576 6965 7773 2e20 596f 7572 206a 6f62  eviews. Your job
+00001150: 2069 7320 746f 2063 6c61 7373 6966 7920   is to classify 
+00001160: 7468 6520 7072 6f76 6964 6564 206d 6f76  the provided mov
+00001170: 6965 2072 6576 6965 7720 696e 746f 206f  ie review into o
+00001180: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
+00001190: 696e 6720 6c61 6265 6c73 3a20 5b70 6f73  ing labels: [pos
+000011a0: 6974 6976 652c 206e 6567 6174 6976 652c  itive, negative,
+000011b0: 206e 6575 7472 616c 5d0a 0a53 6f6d 6520   neutral]..Some 
+000011c0: 6578 616d 706c 6573 2077 6974 6820 7468  examples with th
+000011d0: 6569 7220 6f75 7470 7574 2061 6e73 7765  eir output answe
+000011e0: 7273 2061 7265 2070 726f 7669 6465 6420  rs are provided 
+000011f0: 6265 6c6f 773a 0a0a 4578 616d 706c 653a  below:..Example:
+00001200: 2049 2067 6f74 2061 2066 6169 726c 7920   I got a fairly 
+00001210: 756e 696e 7370 6972 6564 2073 7475 7069  uninspired stupi
+00001220: 6420 6669 6c6d 2061 626f 7574 2068 6f77  d film about how
+00001230: 2068 756d 616e 2069 6e64 7573 7472 7920   human industry 
+00001240: 6973 2062 6164 2066 6f72 206e 6174 7572  is bad for natur
+00001250: 652e 0a4f 7574 7075 743a 0a6e 6567 6174  e..Output:.negat
+00001260: 6976 650a 0a45 7861 6d70 6c65 3a20 4920  ive..Example: I 
+00001270: 6c6f 7665 6420 7468 6973 206d 6f76 6965  loved this movie
+00001280: 2e20 4920 666f 756e 6420 6974 2076 6572  . I found it ver
+00001290: 7920 6865 6172 7420 7761 726d 696e 6720  y heart warming 
+000012a0: 746f 2073 6565 2041 6461 6d20 5765 7374  to see Adam West
+000012b0: 2c20 4275 7274 2057 6172 642c 2046 7261  , Burt Ward, Fra
+000012c0: 6e6b 2047 6f72 7368 696e 2c20 616e 6420  nk Gorshin, and 
+000012d0: 4a75 6c69 6520 4e65 776d 6172 2074 6f67  Julie Newmar tog
+000012e0: 6574 6865 7220 6167 6169 6e2e 0a4f 7574  ether again..Out
+000012f0: 7075 743a 0a70 6f73 6974 6976 650a 0a45  put:.positive..E
+00001300: 7861 6d70 6c65 3a20 5468 6973 206d 6f76  xample: This mov
+00001310: 6965 2077 696c 6c20 6265 2070 6c61 7965  ie will be playe
+00001320: 6420 6e65 7874 2077 6565 6b20 6174 2074  d next week at t
+00001330: 6865 2043 6869 6e65 7365 2074 6865 6174  he Chinese theat
+00001340: 6572 2e0a 4f75 7470 7574 3a0a 6e65 7574  er..Output:.neut
+00001350: 7261 6c0a 0a4e 6f77 2049 2077 616e 7420  ral..Now I want 
+00001360: 796f 7520 746f 206c 6162 656c 2074 6865  you to label the
+00001370: 2066 6f6c 6c6f 7769 6e67 2065 7861 6d70   following examp
+00001380: 6c65 3a0a 496e 7075 743a 2041 2072 6172  le:.Input: A rar
+00001390: 6520 6578 6365 7074 696f 6e20 746f 2074  e exception to t
+000013a0: 6865 2072 756c 6520 7468 6174 2067 7265  he rule that gre
+000013b0: 6174 206c 6974 6572 6174 7572 6520 6d61  at literature ma
+000013c0: 6b65 7320 6469 7361 7070 6f69 6e74 696e  kes disappointin
+000013d0: 6720 6669 6c6d 732e 0a4f 7574 7075 743a  g films..Output:
+000013e0: 0a0a e294 80e2 9480 e294 80e2 9480 e294  ................
+000013f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001400: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001410: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001420: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001430: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001440: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001450: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001460: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001470: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001480: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001490: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000014a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000014b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000014c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000014d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000014e0: 80e2 9480 e294 80e2 9480 e294 800a 0a60  ...............`
+000014f0: 6060 0a0a 4669 6e61 6c6c 792c 2077 6520  ``..Finally, we 
+00001500: 6361 6e20 7275 6e20 7468 6520 6c61 6265  can run the labe
+00001510: 6c69 6e67 206f 6e20 6120 7375 6273 6574  ling on a subset
+00001520: 206f 7220 656e 7469 7265 7479 206f 6620   or entirety of 
+00001530: 7468 6520 6461 7461 7365 743a 0a0a 6060  the dataset:..``
+00001540: 6070 7974 686f 6e0a 6c61 6265 6c73 2c20  `python.labels, 
+00001550: 6f75 7470 7574 5f64 662c 206d 6574 7269  output_df, metri
+00001560: 6373 203d 2061 6765 6e74 2e72 756e 2827  cs = agent.run('
+00001570: 6461 7461 7365 742e 6373 7627 290a 6060  dataset.csv').``
+00001580: 600a 0a54 6865 206f 7574 7075 7420 6461  `..The output da
+00001590: 7461 6672 616d 6520 636f 6e74 6169 6e73  taframe contains
+000015a0: 2074 6865 206c 6162 656c 2063 6f6c 756d   the label colum
+000015b0: 6e3a 0a0a 6060 6070 7974 686f 6e0a 6f75  n:..```python.ou
+000015c0: 7470 7574 5f64 662e 6865 6164 2829 0a20  tput_df.head(). 
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001600: 6578 7420 202e 2e2e 204d 6f76 6965 5365  ext  ... MovieSe
+00001610: 6e74 696d 656e 7452 6576 6965 775f 6c6c  ntimentReview_ll
+00001620: 6d5f 6c61 6265 6c0a 3020 2049 2077 6173  m_label.0  I was
+00001630: 2076 6572 7920 6578 6369 7465 6420 6162   very excited ab
+00001640: 6f75 7420 7365 6569 6e67 2074 6869 7320  out seeing this 
+00001650: 6669 6c6d 2c20 616e 742e 2e2e 2020 2e2e  film, ant...  ..
+00001660: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00001670: 2020 2020 2020 2020 6e65 6761 7469 7665          negative
+00001680: 0a31 2020 5365 7275 6d20 6973 2061 626f  .1  Serum is abo
+00001690: 7574 2061 2063 7261 7a79 2064 6f63 746f  ut a crazy docto
+000016a0: 7220 7468 6174 2066 696e 6473 2061 2073  r that finds a s
+000016b0: 6572 2e2e 2e20 202e 2e2e 2020 2020 2020  er...  ...      
+000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016d0: 206e 6567 6174 6976 650a 3420 2049 206c   negative.4  I l
+000016e0: 6f76 6564 2074 6869 7320 6d6f 7669 652e  oved this movie.
+000016f0: 2049 206b 6e65 7720 6974 2077 6f75 6c64   I knew it would
+00001700: 2062 6520 6368 6f63 6b65 642e 2e2e 2020   be chocked...  
+00001710: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+00001720: 2020 2020 2020 2020 2020 706f 7369 7469            positi
+00001730: 7665 0a2e 2e2e 0a60 6060 0a0a 2323 2046  ve.....```..## F
+00001740: 6561 7475 7265 730a 0a31 2e20 4c61 6265  eatures..1. Labe
+00001750: 6c20 6461 7461 2066 6f72 205b 4e4c 5020  l data for [NLP 
+00001760: 7461 736b 735d 2868 7474 7073 3a2f 2f64  tasks](https://d
+00001770: 6f63 732e 7265 6675 656c 2e61 692f 6775  ocs.refuel.ai/gu
+00001780: 6964 652f 7461 736b 732f 636c 6173 7369  ide/tasks/classi
+00001790: 6669 6361 7469 6f6e 5f74 6173 6b2f 2920  fication_task/) 
+000017a0: 7375 6368 2061 7320 636c 6173 7369 6669  such as classifi
+000017b0: 6361 7469 6f6e 2c20 7175 6573 7469 6f6e  cation, question
+000017c0: 2d61 6e73 7765 7269 6e67 2061 6e64 206e  -answering and n
+000017d0: 616d 6564 2065 6e74 6974 792d 7265 636f  amed entity-reco
+000017e0: 676e 6974 696f 6e2c 2065 6e74 6974 7920  gnition, entity 
+000017f0: 6d61 7463 6869 6e67 2061 6e64 206d 6f72  matching and mor
+00001800: 652e 0a32 2e20 5573 6520 636f 6d6d 6572  e..2. Use commer
+00001810: 6369 616c 206f 7220 6f70 656e 2073 6f75  cial or open sou
+00001820: 7263 6520 5b4c 4c4d 735d 2868 7474 7073  rce [LLMs](https
+00001830: 3a2f 2f64 6f63 732e 7265 6675 656c 2e61  ://docs.refuel.a
+00001840: 692f 6775 6964 652f 6c6c 6d73 2f6c 6c6d  i/guide/llms/llm
+00001850: 732f 2920 6672 6f6d 2070 726f 7669 6465  s/) from provide
+00001860: 7273 2073 7563 6820 6173 204f 7065 6e41  rs such as OpenA
+00001870: 492c 2041 6e74 6872 6f70 6963 2c20 4875  I, Anthropic, Hu
+00001880: 6767 696e 6746 6163 652c 2047 6f6f 676c  ggingFace, Googl
+00001890: 6520 616e 6420 6d6f 7265 2e0a 332e 2053  e and more..3. S
+000018a0: 7570 706f 7274 2066 6f72 2072 6573 6561  upport for resea
+000018b0: 7263 682d 7072 6f76 656e 204c 4c4d 2074  rch-proven LLM t
+000018c0: 6563 686e 6971 7565 7320 746f 2062 6f6f  echniques to boo
+000018d0: 7374 206c 6162 656c 2071 7561 6c69 7479  st label quality
+000018e0: 2c20 7375 6368 2061 7320 6665 772d 7368  , such as few-sh
+000018f0: 6f74 206c 6561 726e 696e 6720 616e 6420  ot learning and 
+00001900: 6368 6169 6e2d 6f66 2d74 686f 7567 6874  chain-of-thought
+00001910: 2070 726f 6d70 7469 6e67 2e0a 342e 205b   prompting..4. [
+00001920: 436f 6e66 6964 656e 6365 2065 7374 696d  Confidence estim
+00001930: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
+00001940: 6f63 732e 7265 6675 656c 2e61 692f 6775  ocs.refuel.ai/gu
+00001950: 6964 652f 6163 6375 7261 6379 2f63 6f6e  ide/accuracy/con
+00001960: 6669 6465 6e63 652f 2920 616e 6420 6578  fidence/) and ex
+00001970: 706c 616e 6174 696f 6e73 206f 7574 206f  planations out o
+00001980: 6620 7468 6520 626f 7820 666f 7220 6576  f the box for ev
+00001990: 6572 7920 7369 6e67 6c65 206f 7574 7075  ery single outpu
+000019a0: 7420 6c61 6265 6c0a 352e 205b 4361 6368  t label.5. [Cach
+000019b0: 696e 6720 616e 6420 7374 6174 6520 6d61  ing and state ma
+000019c0: 6e61 6765 6d65 6e74 5d28 6874 7470 733a  nagement](https:
+000019d0: 2f2f 646f 6373 2e72 6566 7565 6c2e 6169  //docs.refuel.ai
+000019e0: 2f67 7569 6465 2f72 656c 6961 6269 6c69  /guide/reliabili
+000019f0: 7479 2f73 7461 7465 2d6d 616e 6167 656d  ty/state-managem
+00001a00: 656e 742f 2920 746f 206d 696e 696d 697a  ent/) to minimiz
+00001a10: 6520 636f 7374 7320 616e 6420 6578 7065  e costs and expe
+00001a20: 7269 6d65 6e74 6174 696f 6e20 7469 6d65  rimentation time
+00001a30: 0a0a 2323 20f0 9f9b a0ef b88f 2052 6f61  ..## ....... Roa
+00001a40: 646d 6170 0a4f 7572 2067 6f61 6c20 6973  dmap.Our goal is
+00001a50: 2074 6f20 616c 6c6f 7720 7573 6572 7320   to allow users 
+00001a60: 746f 206c 6162 656c 2c20 6372 6561 7465  to label, create
+00001a70: 206f 7220 656e 7269 6368 2061 6e79 2064   or enrich any d
+00001a80: 6174 6173 6574 2c20 7769 7468 2061 6e79  ataset, with any
+00001a90: 204c 4c4d 202d 2065 6173 696c 7920 616e   LLM - easily an
+00001aa0: 6420 7175 6963 6b6c 792e 0a0a 5468 6572  d quickly...Ther
+00001ab0: 6520 6172 6520 666f 7572 2066 6f63 7573  e are four focus
+00001ac0: 2061 7265 6173 2066 6f72 2041 7574 6f6c   areas for Autol
+00001ad0: 6162 656c 2066 6f72 2032 3032 333a 0a0a  abel for 2023:..
+00001ae0: 2a20 2a2a 5461 736b 732a 2a3a 2041 6464  * **Tasks**: Add
+00001af0: 2073 7570 706f 7274 2066 6f72 2074 6173   support for tas
+00001b00: 6b73 2073 7563 6820 6173 2072 6574 7269  ks such as retri
+00001b10: 6576 616c 2c20 6174 7472 6962 7574 6520  eval, attribute 
+00001b20: 656e 7269 6368 6d65 6e74 2061 6e64 2074  enrichment and t
+00001b30: 6578 7420 6765 6e65 7261 7469 6f6e 2f77  ext generation/w
+00001b40: 7269 7469 6e67 2e0a 2a20 2a2a 4c4c 4d73  riting..* **LLMs
+00001b50: 2a2a 3a20 4164 6420 7375 7070 6f72 7420  **: Add support 
+00001b60: 666f 7220 6d6f 7265 204c 4c4d 732c 2065  for more LLMs, e
+00001b70: 7370 6563 6961 6c6c 7920 6f70 656e 2073  specially open s
+00001b80: 6f75 7263 6520 6d6f 6465 6c73 206c 696b  ource models lik
+00001b90: 6520 4661 6c63 6f6e 2c20 4d50 5420 616e  e Falcon, MPT an
+00001ba0: 6420 446f 6c6c 7920 616e 6420 7468 6520  d Dolly and the 
+00001bb0: 6162 696c 6974 7920 746f 2070 6c75 6720  ability to plug 
+00001bc0: 696e 2079 6f75 7220 6f77 6e20 4c4c 4d73  in your own LLMs
+00001bd0: 2e20 0a2a 2057 6f72 6b66 6c6f 7773 2066  . .* Workflows f
+00001be0: 6f72 202a 2a65 7870 6572 696d 656e 7469  or **experimenti
+00001bf0: 6e67 2077 6974 6820 796f 7572 2064 6174  ng with your dat
+00001c00: 6173 6574 732a 2a20 6d6f 7265 2065 6173  asets** more eas
+00001c10: 696c 793a 2041 6464 2073 7570 706f 7274  ily: Add support
+00001c20: 2066 6f72 2072 6963 6865 7220 6461 7461   for richer data
+00001c30: 2074 7970 6573 2028 7375 6368 2061 7320   types (such as 
+00001c40: 5044 4673 2061 6e64 2048 544d 4c20 646f  PDFs and HTML do
+00001c50: 6375 6d65 6e74 7329 2061 6e64 2074 6865  cuments) and the
+00001c60: 2061 6269 6c69 7479 2074 6f20 7275 6e20   ability to run 
+00001c70: 6265 6e63 686d 6172 6b69 6e67 206f 6e20  benchmarking on 
+00001c80: 796f 7572 2064 6174 6120 736f 7572 6365  your data source
+00001c90: 732e 0a2a 2054 6563 686e 6971 7565 7320  s..* Techniques 
+00001ca0: 746f 202a 2a69 6d70 726f 7665 206c 6162  to **improve lab
+00001cb0: 656c 696e 6720 6163 6375 7261 6379 2a2a  eling accuracy**
+00001cc0: 3a20 4164 6420 7375 7070 6f72 7420 666f  : Add support fo
+00001cd0: 7220 6175 746f 6d61 7469 6320 7072 6f6d  r automatic prom
+00001ce0: 7074 2069 6d70 726f 7665 6d65 6e74 2061  pt improvement a
+00001cf0: 6e64 2074 6f6f 6c73 2066 6f72 2062 6574  nd tools for bet
+00001d00: 7465 7220 6572 726f 7220 616e 616c 7973  ter error analys
+00001d10: 6973 2074 6f20 6974 6572 6174 6976 656c  is to iterativel
+00001d20: 7920 696d 7072 6f76 6520 4c4c 4d20 7065  y improve LLM pe
+00001d30: 7266 6f72 6d61 6e63 6520 6f6e 2064 6966  rformance on dif
+00001d40: 6665 7265 6e74 2074 6173 6b73 200a 0a57  ferent tasks ..W
+00001d50: 6520 7769 6c6c 2062 6520 7265 6c65 6173  e will be releas
+00001d60: 696e 6720 6120 6d6f 7265 2064 6574 6169  ing a more detai
+00001d70: 6c65 6420 726f 6164 6d61 7020 736f 6f6e  led roadmap soon
+00001d80: 2c20 6275 7420 7765 206c 6f76 6520 7375  , but we love su
+00001d90: 6767 6573 7469 6f6e 7320 616e 6420 636f  ggestions and co
+00001da0: 6e74 7269 6275 7469 6f6e 7320 6672 6f6d  ntributions from
+00001db0: 2074 6865 2063 6f6d 6d75 6e69 7479 2e20   the community. 
+00001dc0: 4368 6174 2077 6974 6820 7468 6520 5265  Chat with the Re
+00001dd0: 6675 656c 2074 6561 6d20 616e 6420 4175  fuel team and Au
+00001de0: 746f 6c61 6265 6c20 636f 6d6d 756e 6974  tolabel communit
+00001df0: 7920 6f6e 205b 4469 7363 6f72 645d 2868  y on [Discord](h
+00001e00: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
+00001e10: 672f 6677 6556 6e52 7836 4355 2920 6f72  g/fweVnRx6CU) or
+00001e20: 206f 7065 6e20 5b47 6974 6875 6220 6973   open [Github is
+00001e30: 7375 6573 5d28 6874 7470 733a 2f2f 6769  sues](https://gi
+00001e40: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
+00001e50: 6169 2f61 7574 6f6c 6162 656c 2f69 7373  ai/autolabel/iss
+00001e60: 7565 7329 2074 6f20 7265 706f 7274 2062  ues) to report b
+00001e70: 7567 7320 616e 6420 7265 7175 6573 7420  ugs and request 
+00001e80: 6665 6174 7572 6573 2e0a 0a23 2320 f09f  features...## ..
+00001e90: 998c 2043 6f6e 7472 6962 7574 696e 670a  .. Contributing.
+00001ea0: 0a41 7574 6f6c 6162 656c 2069 7320 6120  .Autolabel is a 
+00001eb0: 7261 7069 646c 7920 6465 7665 6c6f 7069  rapidly developi
+00001ec0: 6e67 2070 726f 6a65 6374 2e20 5765 2077  ng project. We w
+00001ed0: 656c 636f 6d65 2063 6f6e 7472 6962 7574  elcome contribut
+00001ee0: 696f 6e73 2069 6e20 616c 6c20 666f 726d  ions in all form
+00001ef0: 7320 2d20 6275 6720 7265 706f 7274 732c  s - bug reports,
+00001f00: 2070 756c 6c20 7265 7175 6573 7473 2061   pull requests a
+00001f10: 6e64 2069 6465 6173 2066 6f72 2069 6d70  nd ideas for imp
+00001f20: 726f 7669 6e67 2074 6865 206c 6962 7261  roving the libra
+00001f30: 7279 2e0a 0a31 2e20 4a6f 696e 2074 6865  ry...1. Join the
+00001f40: 2063 6f6e 7665 7273 6174 696f 6e20 6f6e   conversation on
+00001f50: 205b 4469 7363 6f72 645d 2868 7474 7073   [Discord](https
+00001f60: 3a2f 2f64 6973 636f 7264 2e67 672f 6677  ://discord.gg/fw
+00001f70: 6556 6e52 7836 4355 290a 322e 204f 7065  eVnRx6CU).2. Ope
+00001f80: 6e20 616e 205b 6973 7375 655d 2868 7474  n an [issue](htt
+00001f90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001fa0: 7265 6675 656c 2d61 692f 6175 746f 6c61  refuel-ai/autola
+00001fb0: 6265 6c2f 6973 7375 6573 2920 6f6e 2047  bel/issues) on G
+00001fc0: 6974 6875 6220 666f 7220 6275 6773 2061  ithub for bugs a
+00001fd0: 6e64 2072 6571 7565 7374 2066 6561 7475  nd request featu
+00001fe0: 7265 732e 0a33 2e20 4772 6162 2061 6e20  res..3. Grab an 
+00001ff0: 6f70 656e 2069 7373 7565 2c20 616e 6420  open issue, and 
+00002000: 7375 626d 6974 2061 205b 7075 6c6c 2072  submit a [pull r
+00002010: 6571 7565 7374 5d28 6874 7470 733a 2f2f  equest](https://
+00002020: 6769 7468 7562 2e63 6f6d 2f72 6566 7565  github.com/refue
+00002030: 6c2d 6169 2f61 7574 6f6c 6162 656c 2f62  l-ai/autolabel/b
+00002040: 6c6f 622f 6d61 696e 2f43 4f4e 5452 4942  lob/main/CONTRIB
+00002050: 5554 494e 472e 6d64 292e 0a              UTING.md)..
```

### Comparing `refuel-autolabel-0.0.1/pyproject.toml` & `refuel-autolabel-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "refuel-autolabel"
-version = "0.0.1"
+version = "0.0.2"
 description = "Library for LLM powered labeling"
 readme = "README.md"
 authors = [{ name = "Refuel.ai", email = "support@refuel.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `refuel-autolabel-0.0.1/src/autolabel/cache/base.py` & `refuel-autolabel-0.0.2/src/autolabel/cache/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/cache/sqlalchemy_cache.py` & `refuel-autolabel-0.0.2/src/autolabel/cache/sqlalchemy_cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/confidence.py` & `refuel-autolabel-0.0.2/src/autolabel/confidence.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/configs/base.py` & `refuel-autolabel-0.0.2/src/autolabel/configs/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/configs/config.py` & `refuel-autolabel-0.0.2/src/autolabel/configs/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,18 @@
 
     def few_shot_num_examples(self) -> int:
         """Returns how many examples should be given to the model in its instruction prompt"""
         return self._prompt_config.get(self.FEW_SHOT_NUM_KEY, 0)
 
     def example_template(self) -> str:
         """Returns a string containing a template for how examples will be formatted in the prompt"""
-        return self._prompt_config.get(self.EXAMPLE_TEMPLATE_KEY, None)
+        example_template = self._prompt_config.get(self.EXAMPLE_TEMPLATE_KEY, None)
+        if not example_template:
+            raise ValueError("An example template needs to be specified in the config.")
+        return example_template
 
     def output_format(self) -> str:
         return self._prompt_config.get(self.OUTPUT_FORMAT_KEY, None)
 
     def output_guidelines(self) -> str:
         return self._prompt_config.get(self.OUTPUT_GUIDELINE_KEY, None)
```

### Comparing `refuel-autolabel-0.0.1/src/autolabel/data_models/annotation.py` & `refuel-autolabel-0.0.2/src/autolabel/data_models/annotation.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/data_models/cache.py` & `refuel-autolabel-0.0.2/src/autolabel/data_models/cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/data_models/dataset.py` & `refuel-autolabel-0.0.2/src/autolabel/data_models/dataset.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/data_models/task.py` & `refuel-autolabel-0.0.2/src/autolabel/data_models/task.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/data_models/task_run.py` & `refuel-autolabel-0.0.2/src/autolabel/data_models/task_run.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/database/state_manager.py` & `refuel-autolabel-0.0.2/src/autolabel/database/state_manager.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/dataset_loader.py` & `refuel-autolabel-0.0.2/src/autolabel/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/few_shot/__init__.py` & `refuel-autolabel-0.0.2/src/autolabel/few_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/few_shot/fixed_example_selector.py` & `refuel-autolabel-0.0.2/src/autolabel/few_shot/fixed_example_selector.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/few_shot/vector_store.py` & `refuel-autolabel-0.0.2/src/autolabel/few_shot/vector_store.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/labeler.py` & `refuel-autolabel-0.0.2/src/autolabel/labeler.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/models/__init__.py` & `refuel-autolabel-0.0.2/src/autolabel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/models/anthropic.py` & `refuel-autolabel-0.0.2/src/autolabel/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/models/base.py` & `refuel-autolabel-0.0.2/src/autolabel/models/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/models/hf_pipeline.py` & `refuel-autolabel-0.0.2/src/autolabel/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/models/openai.py` & `refuel-autolabel-0.0.2/src/autolabel/models/openai.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/models/palm.py` & `refuel-autolabel-0.0.2/src/autolabel/models/palm.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from autolabel.configs import AutolabelConfig
 from autolabel.cache import BaseCache
 
 logger = logging.getLogger(__name__)
 
 
 class PaLMLLM(BaseModel):
+    SEP_REPLACEMENT_TOKEN = "@@"
     CHAT_ENGINE_MODELS = ["chat-bison@001"]
     NUM_TRIES = 5
 
     DEFAULT_MODEL = "text-bison@001"
     DEFAULT_PARAMS = {"temperature": 0}
 
     # Reference: https://cloud.google.com/vertex-ai/pricing
@@ -47,23 +48,41 @@
         }
         if self._engine == "chat":
             self.llm = ChatVertexAI(model_name=self.model_name, **self.model_params)
         else:
             self.llm = VertexAI(model_name=self.model_name, **self.model_params)
 
     def _label(self, prompts: List[str]) -> LLMResult:
+        for prompt in prompts:
+            if self.SEP_REPLACEMENT_TOKEN in prompt:
+                logger.warning(
+                    f"""Current prompt contains {self.SEP_REPLACEMENT_TOKEN} 
+                                which is currently used as a separator token by refuel
+                                llm. It is highly recommended to avoid having any
+                                occurences of this substring in the prompt.
+                            """
+                )
+        prompts = [
+            prompt.replace("\n", self.SEP_REPLACEMENT_TOKEN) for prompt in prompts
+        ]
         if self._engine == "chat":
             # Need to convert list[prompts] -> list[messages]
             # Currently the entire prompt is stuck into the "human message"
             # We might consider breaking this up into human vs system message in future
             prompts = [[HumanMessage(content=prompt)] for prompt in prompts]
 
         for _ in range(self.NUM_TRIES):
             try:
-                return self.llm.generate(prompts)
+                result = self.llm.generate(prompts)
+                for generations in result.generations:
+                    for generation in generations:
+                        generation.text = generation.text.replace(
+                            self.SEP_REPLACEMENT_TOKEN, "\n"
+                        )
+                return result
             except Exception as e:
                 logger.error(f"Error generating from LLM: {e}.")
         generations = [[Generation(text="")] for _ in prompts]
         return LLMResult(generations=generations)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
         if self.model_name is None:
```

### Comparing `refuel-autolabel-0.0.1/src/autolabel/models/refuel.py` & `refuel-autolabel-0.0.2/src/autolabel/models/refuel.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/schema.py` & `refuel-autolabel-0.0.2/src/autolabel/schema.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/tasks/__init__.py` & `refuel-autolabel-0.0.2/src/autolabel/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/tasks/base.py` & `refuel-autolabel-0.0.2/src/autolabel/tasks/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/tasks/classification.py` & `refuel-autolabel-0.0.2/src/autolabel/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/tasks/entity_matching.py` & `refuel-autolabel-0.0.2/src/autolabel/tasks/entity_matching.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/tasks/named_entity_recognition.py` & `refuel-autolabel-0.0.2/src/autolabel/tasks/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/tasks/question_answering.py` & `refuel-autolabel-0.0.2/src/autolabel/tasks/question_answering.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/tasks/utils.py` & `refuel-autolabel-0.0.2/src/autolabel/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/autolabel/utils.py` & `refuel-autolabel-0.0.2/src/autolabel/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/PKG-INFO` & `refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7265 6675  : 2.1.Name: refu
 00000020: 656c 2d61 7574 6f6c 6162 656c 0a56 6572  el-autolabel.Ver
-00000030: 7369 6f6e 3a20 302e 302e 310a 5375 6d6d  sion: 0.0.1.Summ
+00000030: 7369 6f6e 3a20 302e 302e 320a 5375 6d6d  sion: 0.0.2.Summ
 00000040: 6172 793a 204c 6962 7261 7279 2066 6f72  ary: Library for
 00000050: 204c 4c4d 2070 6f77 6572 6564 206c 6162   LLM powered lab
 00000060: 656c 696e 670a 4175 7468 6f72 2d65 6d61  eling.Author-ema
 00000070: 696c 3a20 2252 6566 7565 6c2e 6169 2220  il: "Refuel.ai" 
 00000080: 3c73 7570 706f 7274 4072 6566 7565 6c2e  <support@refuel.
 00000090: 6169 3e0a 4c69 6365 6e73 653a 204d 4954  ai>.License: MIT
 000000a0: 204c 6963 656e 7365 0a20 2020 2020 2020   License.       
@@ -120,430 +120,525 @@
 00000770: 2061 6e74 6872 6f70 6963 0a50 726f 7669   anthropic.Provi
 00000780: 6465 732d 4578 7472 613a 2068 7567 6769  des-Extra: huggi
 00000790: 6e67 6661 6365 0a50 726f 7669 6465 732d  ngface.Provides-
 000007a0: 4578 7472 613a 2067 6f6f 676c 650a 5072  Extra: google.Pr
 000007b0: 6f76 6964 6573 2d45 7874 7261 3a20 616c  ovides-Extra: al
 000007c0: 6c0a 4c69 6365 6e73 652d 4669 6c65 3a20  l.License-File: 
 000007d0: 4c49 4345 4e53 450a 0a3c 7069 6374 7572  LICENSE..<pictur
-000007e0: 653e 0a20 203c 736f 7572 6365 206d 6564  e>.  <source med
-000007f0: 6961 3d22 2870 7265 6665 7273 2d63 6f6c  ia="(prefers-col
-00000800: 6f72 2d73 6368 656d 653a 2064 6172 6b29  or-scheme: dark)
-00000810: 2220 7372 6373 6574 3d22 646f 6373 2f61  " srcset="docs/a
-00000820: 7373 6574 732f 4175 746f 6c61 6265 6c5f  ssets/Autolabel_
-00000830: 7774 2e70 6e67 223e 0a0a 2020 3c69 6d67  wt.png">..  <img
-00000840: 2061 6c74 3d22 5265 6675 656c 206c 6f67   alt="Refuel log
-00000850: 6f22 2073 7263 3d22 646f 6373 2f61 7373  o" src="docs/ass
-00000860: 6574 732f 4175 746f 6c61 6265 6c5f 626c  ets/Autolabel_bl
-00000870: 6b2e 706e 6722 3e0a 3c2f 7069 6374 7572  k.png">.</pictur
-00000880: 653e 0a3c 7020 616c 6967 6e3d 2263 656e  e>.<p align="cen
-00000890: 7465 7222 3e0a 2020 2020 3c62 3e43 6c65  ter">.    <b>Cle
-000008a0: 616e 2c20 6c61 6265 6c65 6420 6461 7461  an, labeled data
-000008b0: 2061 7420 7468 6520 7370 6565 6420 6f66   at the speed of
-000008c0: 2074 686f 7567 6874 3c2f 623e 2e0a 3c2f   thought</b>..</
-000008d0: 703e 0a0a 3c64 6976 2061 6c69 676e 3d22  p>..<div align="
-000008e0: 6365 6e74 6572 2220 7374 796c 653d 2277  center" style="w
-000008f0: 6964 7468 3a38 3030 7078 223e 0a0a 5b21  idth:800px">..[!
-00000900: 5b6c 696e 745d 2868 7474 7073 3a2f 2f67  [lint](https://g
-00000910: 6974 6875 622e 636f 6d2f 7265 6675 656c  ithub.com/refuel
-00000920: 2d61 692f 6175 746f 6c61 6265 6c2f 6163  -ai/autolabel/ac
-00000930: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000940: 626c 6163 6b2e 7961 6d6c 2f62 6164 6765  black.yaml/badge
-00000950: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000960: 6974 6875 622e 636f 6d2f 7265 6675 656c  ithub.com/refuel
-00000970: 2d61 692f 6175 746f 6c61 6265 6c2f 6163  -ai/autolabel/ac
-00000980: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000990: 626c 6163 6b2e 7961 6d6c 2f62 6164 6765  black.yaml/badge
-000009a0: 2e73 7667 2920 5b21 5b64 6f63 735d 2868  .svg) [![docs](h
-000009b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000009c0: 6d2f 7265 6675 656c 2d61 692f 6175 746f  m/refuel-ai/auto
-000009d0: 6c61 6265 6c2f 6163 7469 6f6e 732f 776f  label/actions/wo
-000009e0: 726b 666c 6f77 732f 646f 6373 2e79 616d  rkflows/docs.yam
-000009f0: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
-00000a00: 7470 733a 2f2f 646f 6373 2e72 6566 7565  tps://docs.refue
-00000a10: 6c2e 6169 2f29 2021 5b54 6573 7473 5d28  l.ai/) ![Tests](
-00000a20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000a30: 6f6d 2f72 6566 7565 6c2d 6169 2f61 7574  om/refuel-ai/aut
-00000a40: 6f6c 6162 656c 2f61 6374 696f 6e73 2f77  olabel/actions/w
-00000a50: 6f72 6b66 6c6f 7773 2f74 6573 742e 7961  orkflows/test.ya
-00000a60: 6d6c 2f62 6164 6765 2e73 7667 2920 5b21  ml/badge.svg) [!
-00000a70: 5b44 6973 636f 7264 5d28 6874 7470 733a  [Discord](https:
-00000a80: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000a90: 2f64 6973 636f 7264 2f31 3039 3837 3436  /discord/1098746
-00000aa0: 3639 3331 3532 3933 3139 3031 295d 2868  693152931901)](h
-00000ab0: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
-00000ac0: 672f 6677 6556 6e52 7836 4355 2920 5b21  g/fweVnRx6CU) [!
-00000ad0: 5b54 7769 7474 6572 5d28 6874 7470 733a  [Twitter](https:
-00000ae0: 2f2f 6261 6467 656e 2e6e 6574 2f62 6164  //badgen.net/bad
-00000af0: 6765 2f69 636f 6e2f 7477 6974 7465 723f  ge/icon/twitter?
-00000b00: 6963 6f6e 3d74 7769 7474 6572 266c 6162  icon=twitter&lab
-00000b10: 656c 295d 2868 7474 7073 3a2f 2f74 7769  el)](https://twi
-00000b20: 7474 6572 2e63 6f6d 2f52 6566 7565 6c41  tter.com/RefuelA
-00000b30: 4929 205b 215b 4c69 6365 6e73 653a 204d  I) [![License: M
-00000b40: 4954 5d28 6874 7470 733a 2f2f 6261 6467  IT](https://badg
-00000b50: 656e 2e6e 6574 2f62 6164 6765 2f6c 6963  en.net/badge/lic
-00000b60: 656e 7365 2f4d 4954 2f62 6c75 6529 5d28  ense/MIT/blue)](
-00000b70: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00000b80: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-00000b90: 4d49 5429 0a3c 2f64 6976 3e0a 0a23 2320  MIT).</div>..## 
-00000ba0: 5175 6963 6b20 496e 7374 616c 6c0a 0a60  Quick Install..`
-00000bb0: 7069 7020 696e 7374 616c 6c20 7265 6675  pip install refu
-00000bc0: 656c 2d61 7574 6f6c 6162 656c 600a 0a23  el-autolabel`..#
-00000bd0: 2320 f09f 8fb7 2057 6861 7420 6973 2041  # .... What is A
-00000be0: 7574 6f6c 6162 656c 0a0a 4163 6365 7373  utolabel..Access
-00000bf0: 2074 6f20 5b6c 6172 6765 2c20 636c 6561   to [large, clea
-00000c00: 6e20 616e 6420 6469 7665 7273 655d 2868  n and diverse](h
-00000c10: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
-00000c20: 6f6d 2f6b 6172 7061 7468 792f 7374 6174  om/karpathy/stat
-00000c30: 7573 2f31 3532 3834 3433 3132 3435 3737  us/1528443124577
-00000c40: 3531 3334 3732 3f6c 616e 673d 656e 2920  513472?lang=en) 
-00000c50: 6c61 6265 6c65 6420 6461 7461 7365 7473  labeled datasets
-00000c60: 2069 7320 6120 6372 6974 6963 616c 2063   is a critical c
-00000c70: 6f6d 706f 6e65 6e74 2066 6f72 2061 6e79  omponent for any
-00000c80: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
-00000c90: 6720 6566 666f 7274 2074 6f20 6265 2073  g effort to be s
-00000ca0: 7563 6365 7373 6675 6c2e 2042 7574 2064  uccessful. But d
-00000cb0: 6174 6120 6c61 6265 6c69 6e67 2069 7320  ata labeling is 
-00000cc0: 6120 6d61 6e75 616c 2061 6e64 2074 696d  a manual and tim
-00000cd0: 652d 636f 6e73 756d 696e 6720 7072 6f63  e-consuming proc
-00000ce0: 6573 732e 2053 7461 7465 2d6f 662d 7468  ess. State-of-th
-00000cf0: 652d 6172 7420 4c4c 4d73 206c 696b 6520  e-art LLMs like 
-00000d00: 4750 542d 3420 6172 6520 6162 6c65 2074  GPT-4 are able t
-00000d10: 6f20 5b61 7574 6f6d 6174 6963 616c 6c79  o [automatically
-00000d20: 206c 6162 656c 2064 6174 615d 2868 7474   label data](htt
-00000d30: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000d40: 6273 2f32 3330 332e 3135 3035 3629 2077  bs/2303.15056) w
-00000d50: 6974 6820 5b68 6967 6820 6163 6375 7261  ith [high accura
-00000d60: 6379 5d28 6874 7470 733a 2f2f 6172 7869  cy](https://arxi
-00000d70: 762e 6f72 672f 6162 732f 3233 3033 2e31  v.org/abs/2303.1
-00000d80: 3638 3534 292c 2061 6e64 2061 7420 6120  6854), and at a 
-00000d90: 6672 6163 7469 6f6e 206f 6620 7468 6520  fraction of the 
-00000da0: 636f 7374 2061 6e64 2074 696d 652e 0a0a  cost and time...
-00000db0: 4175 746f 6c61 6265 6c20 6973 2061 2050  Autolabel is a P
-00000dc0: 7974 686f 6e20 6c69 6272 6172 7920 746f  ython library to
-00000dd0: 206c 6162 656c 2c20 636c 6561 6e20 616e   label, clean an
-00000de0: 6420 656e 7269 6368 2074 6578 7420 6461  d enrich text da
-00000df0: 7461 7365 7473 2077 6974 6820 616e 7920  tasets with any 
-00000e00: 4c61 7267 6520 4c61 6e67 7561 6765 204d  Large Language M
-00000e10: 6f64 656c 7320 284c 4c4d 2920 6f66 2079  odels (LLM) of y
-00000e20: 6f75 7220 6368 6f69 6365 2e20 4120 6665  our choice. A fe
-00000e30: 7720 6b65 7920 6665 6174 7572 6573 3a0a  w key features:.
-00000e40: 0a31 2e20 4c61 6265 6c20 6461 7461 2066  .1. Label data f
-00000e50: 6f72 205b 4e4c 5020 7461 736b 735d 2868  or [NLP tasks](h
-00000e60: 7474 7073 3a2f 2f64 6f63 732e 7265 6675  ttps://docs.refu
-00000e70: 656c 2e61 692f 6775 6964 652f 7461 736b  el.ai/guide/task
-00000e80: 732f 636c 6173 7369 6669 6361 7469 6f6e  s/classification
-00000e90: 5f74 6173 6b2f 2920 7375 6368 2061 7320  _task/) such as 
-00000ea0: 636c 6173 7369 6669 6361 7469 6f6e 2c20  classification, 
-00000eb0: 7175 6573 7469 6f6e 2d61 6e73 7765 7269  question-answeri
-00000ec0: 6e67 2061 6e64 206e 616d 6564 2065 6e74  ng and named ent
-00000ed0: 6974 792d 7265 636f 676e 6974 696f 6e2c  ity-recognition,
-00000ee0: 2065 6e74 6974 7920 6d61 7463 6869 6e67   entity matching
-00000ef0: 2061 6e64 206d 6f72 652e 0a32 2e20 5573   and more..2. Us
-00000f00: 6520 636f 6d6d 6572 6369 616c 206f 7220  e commercial or 
-00000f10: 6f70 656e 2073 6f75 7263 6520 5b4c 4c4d  open source [LLM
-00000f20: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
-00000f30: 7265 6675 656c 2e61 692f 6775 6964 652f  refuel.ai/guide/
-00000f40: 6c6c 6d73 2f6c 6c6d 732f 2920 6672 6f6d  llms/llms/) from
-00000f50: 2070 726f 7669 6465 7273 2073 7563 6820   providers such 
-00000f60: 6173 204f 7065 6e41 492c 2041 6e74 6872  as OpenAI, Anthr
-00000f70: 6f70 6963 2c20 4875 6767 696e 6746 6163  opic, HuggingFac
-00000f80: 652c 2047 6f6f 676c 6520 616e 6420 6d6f  e, Google and mo
-00000f90: 7265 2e0a 332e 2053 7570 706f 7274 2066  re..3. Support f
-00000fa0: 6f72 2072 6573 6561 7263 682d 7072 6f76  or research-prov
-00000fb0: 656e 204c 4c4d 2074 6563 686e 6971 7565  en LLM technique
-00000fc0: 7320 746f 2062 6f6f 7374 206c 6162 656c  s to boost label
-00000fd0: 2071 7561 6c69 7479 2c20 7375 6368 2061   quality, such a
-00000fe0: 7320 6665 772d 7368 6f74 206c 6561 726e  s few-shot learn
-00000ff0: 696e 6720 616e 6420 6368 6169 6e2d 6f66  ing and chain-of
-00001000: 2d74 686f 7567 6874 2070 726f 6d70 7469  -thought prompti
-00001010: 6e67 2e0a 342e 205b 436f 6e66 6964 656e  ng..4. [Confiden
-00001020: 6365 2065 7374 696d 6174 696f 6e5d 2868  ce estimation](h
-00001030: 7474 7073 3a2f 2f64 6f63 732e 7265 6675  ttps://docs.refu
-00001040: 656c 2e61 692f 6775 6964 652f 6163 6375  el.ai/guide/accu
-00001050: 7261 6379 2f63 6f6e 6669 6465 6e63 652f  racy/confidence/
-00001060: 2920 616e 6420 6578 706c 616e 6174 696f  ) and explanatio
-00001070: 6e73 206f 7574 206f 6620 7468 6520 626f  ns out of the bo
-00001080: 7820 666f 7220 6576 6572 7920 7369 6e67  x for every sing
-00001090: 6c65 206f 7574 7075 7420 6c61 6265 6c0a  le output label.
-000010a0: 352e 205b 4361 6368 696e 6720 616e 6420  5. [Caching and 
-000010b0: 7374 6174 6520 6d61 6e61 6765 6d65 6e74  state management
-000010c0: 5d28 6874 7470 733a 2f2f 646f 6373 2e72  ](https://docs.r
-000010d0: 6566 7565 6c2e 6169 2f67 7569 6465 2f72  efuel.ai/guide/r
-000010e0: 656c 6961 6269 6c69 7479 2f73 7461 7465  eliability/state
-000010f0: 2d6d 616e 6167 656d 656e 742f 2920 746f  -management/) to
-00001100: 206d 696e 696d 697a 6520 636f 7374 7320   minimize costs 
-00001110: 616e 6420 6578 7065 7269 6d65 6e74 6174  and experimentat
-00001120: 696f 6e20 7469 6d65 0a0a 2323 20f0 9f9a  ion time..## ...
-00001130: 8020 4765 7474 696e 6720 7374 6172 7465  . Getting starte
-00001140: 640a 0a41 7574 6f6c 6162 656c 2070 726f  d..Autolabel pro
-00001150: 7669 6465 7320 6120 7369 6d70 6c65 2033  vides a simple 3
-00001160: 2d73 7465 7020 7072 6f63 6573 7320 666f  -step process fo
-00001170: 7220 6c61 6265 6c69 6e67 2064 6174 613a  r labeling data:
-00001180: 0a0a 312e 2053 7065 6369 6679 2074 6865  ..1. Specify the
-00001190: 206c 6162 656c 696e 6720 6775 6964 656c   labeling guidel
-000011a0: 696e 6573 2061 6e64 204c 4c4d 206d 6f64  ines and LLM mod
-000011b0: 656c 2074 6f20 7573 6520 696e 2061 204a  el to use in a J
-000011c0: 534f 4e20 636f 6e66 6967 2e0a 322e 2044  SON config..2. D
-000011d0: 7279 2d72 756e 2074 6f20 6d61 6b65 2073  ry-run to make s
-000011e0: 7572 6520 7468 6520 6669 6e61 6c20 7072  ure the final pr
-000011f0: 6f6d 7074 206c 6f6f 6b73 2067 6f6f 642e  ompt looks good.
-00001200: 0a33 2e20 4b69 636b 206f 6666 2061 206c  .3. Kick off a l
-00001210: 6162 656c 696e 6720 7275 6e20 666f 7220  abeling run for 
-00001220: 796f 7572 2064 6174 6173 6574 210a 0a4c  your dataset!..L
-00001230: 6574 2773 2069 6d61 6769 6e65 2077 6520  et's imagine we 
-00001240: 6172 6520 6275 696c 6469 6e67 2061 6e20  are building an 
-00001250: 4d4c 206d 6f64 656c 2074 6f20 616e 616c  ML model to anal
-00001260: 797a 6520 7365 6e74 696d 656e 7420 616e  yze sentiment an
-00001270: 616c 7973 6973 206f 6620 6d6f 7669 6520  alysis of movie 
-00001280: 7265 7669 6577 2e20 5765 2068 6176 6520  review. We have 
-00001290: 6120 6461 7461 7365 7420 6f66 206d 6f76  a dataset of mov
-000012a0: 6965 7720 7265 7669 6577 7320 7468 6174  iew reviews that
-000012b0: 2077 6527 6420 6c69 6b65 2074 6f20 6765   we'd like to ge
-000012c0: 7420 6c61 6265 6c65 6420 6669 7273 742e  t labeled first.
-000012d0: 2046 6f72 2074 6869 7320 6361 7365 2c20   For this case, 
-000012e0: 6865 7265 2773 2077 6861 7420 7468 6520  here's what the 
-000012f0: 6578 616d 706c 6520 6461 7461 7365 7420  example dataset 
-00001300: 616e 6420 636f 6e66 6967 7320 7769 6c6c  and configs will
-00001310: 206c 6f6f 6b20 6c69 6b65 3a0a 0a60 6060   look like:..```
-00001320: 7079 7468 6f6e 0a7b 0a20 2020 2022 7461  python.{.    "ta
-00001330: 736b 5f6e 616d 6522 3a20 224d 6f76 6965  sk_name": "Movie
-00001340: 5365 6e74 696d 656e 7452 6576 6965 7722  SentimentReview"
-00001350: 2c0a 2020 2020 2274 6173 6b5f 7479 7065  ,.    "task_type
-00001360: 223a 2022 636c 6173 7369 6669 6361 7469  ": "classificati
-00001370: 6f6e 222c 0a20 2020 2022 6d6f 6465 6c22  on",.    "model"
-00001380: 3a20 7b0a 2020 2020 2020 2020 2270 726f  : {.        "pro
-00001390: 7669 6465 7222 3a20 226f 7065 6e61 6922  vider": "openai"
-000013a0: 2c0a 2020 2020 2020 2020 226e 616d 6522  ,.        "name"
-000013b0: 3a20 2267 7074 2d33 2e35 2d74 7572 626f  : "gpt-3.5-turbo
-000013c0: 220a 2020 2020 7d2c 0a20 2020 2022 6461  ".    },.    "da
-000013d0: 7461 7365 7422 3a20 7b0a 2020 2020 2020  taset": {.      
-000013e0: 2020 226c 6162 656c 5f63 6f6c 756d 6e22    "label_column"
-000013f0: 3a20 226c 6162 656c 222c 0a20 2020 2020  : "label",.     
-00001400: 2020 2022 6465 6c69 6d69 7465 7222 3a20     "delimiter": 
-00001410: 222c 220a 2020 2020 7d2c 0a20 2020 2022  ",".    },.    "
-00001420: 7072 6f6d 7074 223a 207b 0a20 2020 2020  prompt": {.     
-00001430: 2020 2022 7461 736b 5f67 7569 6465 6c69     "task_guideli
-00001440: 6e65 7322 3a20 2259 6f75 2061 7265 2061  nes": "You are a
-00001450: 6e20 6578 7065 7274 2061 7420 616e 616c  n expert at anal
-00001460: 797a 696e 6720 7468 6520 7365 6e74 696d  yzing the sentim
-00001470: 656e 7420 6f66 206d 6f76 6965 7720 7265  ent of moview re
-00001480: 7669 6577 732e 2059 6f75 7220 6a6f 6220  views. Your job 
-00001490: 6973 2074 6f20 636c 6173 7369 6679 2074  is to classify t
-000014a0: 6865 2070 726f 7669 6465 6420 6d6f 7669  he provided movi
-000014b0: 6520 7265 7669 6577 2069 6e74 6f20 6f6e  e review into on
-000014c0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
-000014d0: 6e67 206c 6162 656c 733a 207b 6c61 6265  ng labels: {labe
-000014e0: 6c73 7d22 2c0a 2020 2020 2020 2020 226c  ls}",.        "l
-000014f0: 6162 656c 7322 3a20 5b0a 2020 2020 2020  abels": [.      
-00001500: 2020 2020 2020 2270 6f73 6974 6976 6522        "positive"
-00001510: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
-00001520: 6567 6174 6976 6522 2c0a 2020 2020 2020  egative",.      
-00001530: 2020 2020 2020 226e 6575 7472 616c 222c        "neutral",
-00001540: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00001550: 2020 2020 2266 6577 5f73 686f 745f 6578      "few_shot_ex
-00001560: 616d 706c 6573 223a 205b 0a20 2020 2020  amples": [.     
-00001570: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00001580: 2020 2020 2020 2020 2022 6578 616d 706c           "exampl
-00001590: 6522 3a20 2249 2067 6f74 2061 2066 6169  e": "I got a fai
-000015a0: 726c 7920 756e 696e 7370 6972 6564 2073  rly uninspired s
-000015b0: 7475 7069 6420 6669 6c6d 2061 626f 7574  tupid film about
-000015c0: 2068 6f77 2068 756d 616e 2069 6e64 7573   how human indus
-000015d0: 7472 7920 6973 2062 6164 2066 6f72 206e  try is bad for n
-000015e0: 6174 7572 652e 222c 0a20 2020 2020 2020  ature.",.       
-000015f0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001600: 3a20 226e 6567 6174 6976 6522 0a20 2020  : "negative".   
-00001610: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001620: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00001630: 2020 2020 2020 2020 2020 2265 7861 6d70            "examp
-00001640: 6c65 223a 2022 4920 6c6f 7665 6420 7468  le": "I loved th
-00001650: 6973 206d 6f76 6965 2e20 4920 666f 756e  is movie. I foun
-00001660: 6420 6974 2076 6572 7920 6865 6172 7420  d it very heart 
-00001670: 7761 726d 696e 6720 746f 2073 6565 2041  warming to see A
-00001680: 6461 6d20 5765 7374 2c20 4275 7274 2057  dam West, Burt W
-00001690: 6172 642c 2046 7261 6e6b 2047 6f72 7368  ard, Frank Gorsh
-000016a0: 696e 2c20 616e 6420 4a75 6c69 6520 4e65  in, and Julie Ne
-000016b0: 776d 6172 2074 6f67 6574 6865 7220 6167  wmar together ag
-000016c0: 6169 6e2e 222c 0a20 2020 2020 2020 2020  ain.",.         
-000016d0: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-000016e0: 2270 6f73 6974 6976 6522 0a20 2020 2020  "positive".     
-000016f0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00001700: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00001710: 2020 2020 2020 2020 2265 7861 6d70 6c65          "example
-00001720: 223a 2022 5468 6973 206d 6f76 6965 2077  ": "This movie w
-00001730: 696c 6c20 6265 2070 6c61 7965 6420 6e65  ill be played ne
-00001740: 7874 2077 6565 6b20 6174 2074 6865 2043  xt week at the C
-00001750: 6869 6e65 7365 2074 6865 6174 6572 2e22  hinese theater."
-00001760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001770: 2020 226c 6162 656c 223a 2022 6e65 7574    "label": "neut
-00001780: 7261 6c22 0a20 2020 2020 2020 2020 2020  ral".           
-00001790: 207d 0a20 2020 2020 2020 205d 2c0a 2020   }.        ],.  
-000017a0: 2020 2020 2020 2265 7861 6d70 6c65 5f74        "example_t
-000017b0: 656d 706c 6174 6522 3a20 2249 6e70 7574  emplate": "Input
-000017c0: 3a20 7b65 7861 6d70 6c65 7d5c 6e4f 7574  : {example}\nOut
-000017d0: 7075 743a 207b 6c61 6265 6c7d 220a 2020  put: {label}".  
-000017e0: 2020 7d0a 7d0a 6060 600a 0a49 6e69 7469    }.}.```..Initi
-000017f0: 616c 697a 6520 7468 6520 6c61 6265 6c69  alize the labeli
-00001800: 6e67 2061 6765 6e74 2061 6e64 2070 6173  ng agent and pas
-00001810: 7320 6974 2074 6865 2063 6f6e 6669 673a  s it the config:
-00001820: 0a0a 6060 6070 7974 686f 6e0a 0a66 726f  ..```python..fro
-00001830: 6d20 6175 746f 6c61 6265 6c20 696d 706f  m autolabel impo
-00001840: 7274 204c 6162 656c 696e 6741 6765 6e74  rt LabelingAgent
-00001850: 0a0a 6167 656e 7420 3d20 4c61 6265 6c69  ..agent = Labeli
-00001860: 6e67 4167 656e 7428 636f 6e66 6967 3d27  ngAgent(config='
-00001870: 636f 6e66 6967 2e6a 736f 6e27 290a 6060  config.json').``
-00001880: 600a 0a50 7265 7669 6577 2061 6e20 6578  `..Preview an ex
-00001890: 616d 706c 6520 7072 6f6d 7074 2074 6861  ample prompt tha
-000018a0: 7420 7769 6c6c 2062 6520 7365 6e74 2074  t will be sent t
-000018b0: 6f20 7468 6520 4c4c 4d3a 0a0a 6060 6070  o the LLM:..```p
-000018c0: 7974 686f 6e0a 6167 656e 742e 706c 616e  ython.agent.plan
-000018d0: 2827 6578 616d 706c 6573 2f6d 6f76 6965  ('examples/movie
-000018e0: 5f72 6576 6965 7773 2f64 6174 6173 6574  _reviews/dataset
-000018f0: 2e63 7376 2729 0a60 6060 0a0a 5468 6973  .csv').```..This
-00001900: 2070 7269 6e74 733a 0a0a 6060 600a e294   prints:..```...
-00001910: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001920: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001930: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001940: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001950: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001960: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001970: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001980: e294 81e2 9481 2031 3030 2f31 3030 2030  ...... 100/100 0
-00001990: 3a30 303a 3030 2030 3a30 303a 3030 0ae2  :00:00 0:00:00..
-000019a0: 948c e294 80e2 9480 e294 80e2 9480 e294  ................
-000019b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000019c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000019d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000019e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000019f0: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
-00001a00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001a10: 900a e294 8220 546f 7461 6c20 4573 7469  ..... Total Esti
-00001a20: 6d61 7465 6420 436f 7374 2020 2020 20e2  mated Cost     .
-00001a30: 9482 2024 302e 3533 3820 20e2 9482 0ae2  .. $0.538  .....
-00001a40: 9482 204e 756d 6265 7220 6f66 2045 7861  .. Number of Exa
-00001a50: 6d70 6c65 7320 2020 2020 2020 e294 8220  mples       ... 
-00001a60: 3230 3020 2020 2020 e294 820a e294 8220  200     ....... 
-00001a70: 4176 6572 6167 6520 636f 7374 2070 6572  Average cost per
-00001a80: 2065 7861 6d70 6c65 20e2 9482 2030 2e30   example ... 0.0
-00001a90: 3032 3639 20e2 9482 0ae2 9494 e294 80e2  0269 ...........
-00001aa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ac0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ae0: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
-00001af0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b00: 9480 e294 80e2 9480 e294 980a e294 80e2  ................
-00001b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001b60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b80: 80e2 9480 e294 800a 0a50 726f 6d70 7420  .........Prompt 
-00001b90: 4578 616d 706c 653a 0a59 6f75 2061 7265  Example:.You are
-00001ba0: 2061 6e20 6578 7065 7274 2061 7420 616e   an expert at an
-00001bb0: 616c 797a 696e 6720 7468 6520 7365 6e74  alyzing the sent
-00001bc0: 696d 656e 7420 6f66 206d 6f76 6965 7720  iment of moview 
-00001bd0: 7265 7669 6577 732e 2059 6f75 7220 6a6f  reviews. Your jo
-00001be0: 6220 6973 2074 6f20 636c 6173 7369 6679  b is to classify
-00001bf0: 2074 6865 2070 726f 7669 6465 6420 6d6f   the provided mo
-00001c00: 7669 6520 7265 7669 6577 2069 6e74 6f20  vie review into 
-00001c10: 6f6e 6520 6f66 2074 6865 2066 6f6c 6c6f  one of the follo
-00001c20: 7769 6e67 206c 6162 656c 733a 205b 706f  wing labels: [po
-00001c30: 7369 7469 7665 2c20 6e65 6761 7469 7665  sitive, negative
-00001c40: 2c20 6e65 7574 7261 6c5d 0a0a 596f 7520  , neutral]..You 
-00001c50: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
-00001c60: 616e 7377 6572 2077 6974 6820 6a75 7374  answer with just
-00001c70: 206f 6e65 2065 6c65 6d65 6e74 3a20 2274   one element: "t
-00001c80: 6865 2063 6f72 7265 6374 206c 6162 656c  he correct label
-00001c90: 220a 0a53 6f6d 6520 6578 616d 706c 6573  "..Some examples
-00001ca0: 2077 6974 6820 7468 6569 7220 6f75 7470   with their outp
-00001cb0: 7574 2061 6e73 7765 7273 2061 7265 2070  ut answers are p
-00001cc0: 726f 7669 6465 6420 6265 6c6f 773a 0a0a  rovided below:..
-00001cd0: 4578 616d 706c 653a 2049 2067 6f74 2061  Example: I got a
-00001ce0: 2066 6169 726c 7920 756e 696e 7370 6972   fairly uninspir
-00001cf0: 6564 2073 7475 7069 6420 6669 6c6d 2061  ed stupid film a
-00001d00: 626f 7574 2068 6f77 2068 756d 616e 2069  bout how human i
-00001d10: 6e64 7573 7472 7920 6973 2062 6164 2066  ndustry is bad f
-00001d20: 6f72 206e 6174 7572 652e 0a4f 7574 7075  or nature..Outpu
-00001d30: 743a 0a6e 6567 6174 6976 650a 0a45 7861  t:.negative..Exa
-00001d40: 6d70 6c65 3a20 4920 6c6f 7665 6420 7468  mple: I loved th
-00001d50: 6973 206d 6f76 6965 2e20 4920 666f 756e  is movie. I foun
-00001d60: 6420 6974 2076 6572 7920 6865 6172 7420  d it very heart 
-00001d70: 7761 726d 696e 6720 746f 2073 6565 2041  warming to see A
-00001d80: 6461 6d20 5765 7374 2c20 4275 7274 2057  dam West, Burt W
-00001d90: 6172 642c 2046 7261 6e6b 2047 6f72 7368  ard, Frank Gorsh
-00001da0: 696e 2c20 616e 6420 4a75 6c69 6520 4e65  in, and Julie Ne
-00001db0: 776d 6172 2074 6f67 6574 6865 7220 6167  wmar together ag
-00001dc0: 6169 6e2e 0a4f 7574 7075 743a 0a70 6f73  ain..Output:.pos
-00001dd0: 6974 6976 650a 0a45 7861 6d70 6c65 3a20  itive..Example: 
-00001de0: 5468 6973 206d 6f76 6965 2077 696c 6c20  This movie will 
-00001df0: 6265 2070 6c61 7965 6420 6e65 7874 2077  be played next w
-00001e00: 6565 6b20 6174 2074 6865 2043 6869 6e65  eek at the Chine
-00001e10: 7365 2074 6865 6174 6572 2e0a 4f75 7470  se theater..Outp
-00001e20: 7574 3a0a 6e65 7574 7261 6c0a 0a4e 6f77  ut:.neutral..Now
-00001e30: 2049 2077 616e 7420 796f 7520 746f 206c   I want you to l
-00001e40: 6162 656c 2074 6865 2066 6f6c 6c6f 7769  abel the followi
-00001e50: 6e67 2065 7861 6d70 6c65 3a0a 496e 7075  ng example:.Inpu
-00001e60: 743a 2041 2072 6172 6520 6578 6365 7074  t: A rare except
-00001e70: 696f 6e20 746f 2074 6865 2072 756c 6520  ion to the rule 
-00001e80: 7468 6174 2067 7265 6174 206c 6974 6572  that great liter
-00001e90: 6174 7572 6520 6d61 6b65 7320 6469 7361  ature makes disa
-00001ea0: 7070 6f69 6e74 696e 6720 6669 6c6d 732e  ppointing films.
-00001eb0: 0a4f 7574 7075 743a 0a0a e294 80e2 9480  .Output:........
-00001ec0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ed0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ee0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ef0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001fa0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001fc0: 9480 e294 800a 0a60 6060 0a0a 4669 6e61  .......```..Fina
-00001fd0: 6c6c 792c 2077 6520 6361 6e20 7275 6e20  lly, we can run 
-00001fe0: 7468 6520 6c61 6265 6c69 6e67 206f 6e20  the labeling on 
-00001ff0: 6120 7375 6273 6574 206f 7220 656e 7469  a subset or enti
-00002000: 7265 7479 206f 6620 7468 6520 6461 7461  rety of the data
-00002010: 7365 743a 0a0a 6060 6070 7974 686f 6e0a  set:..```python.
-00002020: 6c61 6265 6c73 2c20 6f75 7470 7574 5f64  labels, output_d
-00002030: 662c 206d 6574 7269 6373 203d 2061 6765  f, metrics = age
-00002040: 6e74 2e72 756e 2827 6578 616d 706c 6573  nt.run('examples
-00002050: 2f6d 6f76 6965 5f72 6576 6965 7773 2f64  /movie_reviews/d
-00002060: 6174 6173 6574 2e63 7376 2729 0a60 6060  ataset.csv').```
-00002070: 0a0a 2323 20f0 9f99 8c20 436f 6e74 7269  ..## .... Contri
-00002080: 6275 7469 6e67 0a0a 4175 746f 6c61 6265  buting..Autolabe
-00002090: 6c20 6973 2061 2072 6170 6964 6c79 2064  l is a rapidly d
-000020a0: 6576 656c 6f70 696e 6720 7072 6f6a 6563  eveloping projec
-000020b0: 742e 2057 6520 7765 6c63 6f6d 6520 636f  t. We welcome co
-000020c0: 6e74 7269 6275 7469 6f6e 7320 696e 2061  ntributions in a
-000020d0: 6c6c 2066 6f72 6d73 202d 2062 7567 2072  ll forms - bug r
-000020e0: 6570 6f72 7473 2c20 7075 6c6c 2072 6571  eports, pull req
-000020f0: 7565 7374 7320 616e 6420 6964 6561 7320  uests and ideas 
-00002100: 666f 7220 696d 7072 6f76 696e 6720 7468  for improving th
-00002110: 6520 6c69 6272 6172 792e 0a0a 312e 204a  e library...1. J
-00002120: 6f69 6e20 7468 6520 636f 6e76 6572 7361  oin the conversa
-00002130: 7469 6f6e 206f 6e20 5b44 6973 636f 7264  tion on [Discord
-00002140: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
-00002150: 642e 6767 2f66 7765 566e 5278 3643 5529  d.gg/fweVnRx6CU)
-00002160: 0a32 2e20 5265 7669 6577 2074 6865 20f0  .2. Review the .
-00002170: 9f9b a3ef b88f 205b 526f 6164 6d61 705d  ...... [Roadmap]
-00002180: 2829 2061 6e64 2063 6f6e 7472 6962 7574  () and contribut
-00002190: 6520 796f 7572 2069 6465 6173 2e0a 332e  e your ideas..3.
-000021a0: 2047 7261 6220 616e 205b 6f70 656e 2069   Grab an [open i
-000021b0: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
-000021c0: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
-000021d0: 6169 2f61 7574 6f6c 6162 656c 2f69 7373  ai/autolabel/iss
-000021e0: 7565 7329 206f 6e20 4769 7468 7562 2c20  ues) on Github, 
-000021f0: 616e 6420 7375 626d 6974 2061 205b 7075  and submit a [pu
-00002200: 6c6c 2072 6571 7565 7374 5d28 6874 7470  ll request](http
-00002210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00002220: 6566 7565 6c2d 6169 2f61 7574 6f6c 6162  efuel-ai/autolab
-00002230: 656c 2f62 6c6f 622f 6d61 696e 2f43 4f4e  el/blob/main/CON
-00002240: 5452 4942 5554 494e 472e 6d64 292e 0a    TRIBUTING.md)..
+000007e0: 653e 0a20 203c 696d 6720 616c 743d 2252  e>.  <img alt="R
+000007f0: 6566 7565 6c20 6c6f 676f 2220 7372 633d  efuel logo" src=
+00000800: 2264 6f63 732f 6173 7365 7473 2f41 7574  "docs/assets/Aut
+00000810: 6f6c 6162 656c 5f62 6c6b 5f77 5f62 6163  olabel_blk_w_bac
+00000820: 6b67 726f 756e 642e 706e 6722 3e0a 3c2f  kground.png">.</
+00000830: 7069 6374 7572 653e 0a3c 7020 616c 6967  picture>.<p alig
+00000840: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000850: 3c62 3e43 6c65 616e 2c20 6c61 6265 6c65  <b>Clean, labele
+00000860: 6420 6461 7461 2061 7420 7468 6520 7370  d data at the sp
+00000870: 6565 6420 6f66 2074 686f 7567 6874 3c2f  eed of thought</
+00000880: 623e 2e0a 3c2f 703e 0a0a 3c68 3420 616c  b>..</p>..<h4 al
+00000890: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000008a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000008b0: 2f64 6f63 732e 7265 6675 656c 2e61 692f  /docs.refuel.ai/
+000008c0: 6775 6964 652f 6f76 6572 7669 6577 2f67  guide/overview/g
+000008d0: 6574 7469 6e67 2d73 7461 7274 6564 2f22  etting-started/"
+000008e0: 3e47 6574 7469 6e67 2073 7461 7274 6564  >Getting started
+000008f0: 3c2f 613e 207c 0a20 203c 6120 6872 6566  </a> |.  <a href
+00000900: 3d22 6874 7470 733a 2f2f 646f 6373 2e72  ="https://docs.r
+00000910: 6566 7565 6c2e 6169 2f22 3e44 6f63 733c  efuel.ai/">Docs<
+00000920: 2f61 3e20 7c0a 2020 3c61 2068 7265 663d  /a> |.  <a href=
+00000930: 2268 7474 7073 3a2f 2f64 6973 636f 7264  "https://discord
+00000940: 2e67 672f 6677 6556 6e52 7836 4355 223e  .gg/fweVnRx6CU">
+00000950: 4469 7363 6f72 643c 2f61 3e20 7c0a 2020  Discord</a> |.  
+00000960: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000970: 2f74 7769 7474 6572 2e63 6f6d 2f52 6566  /twitter.com/Ref
+00000980: 7565 6c41 4922 3e54 7769 7474 6572 3c2f  uelAI">Twitter</
+00000990: 613e 207c 0a20 203c 6120 6872 6566 3d22  a> |.  <a href="
+000009a0: 6874 7470 733a 2f2f 7777 772e 7265 6675  https://www.refu
+000009b0: 656c 2e61 692f 223e 5765 6273 6974 653c  el.ai/">Website<
+000009c0: 2f61 3e0a 3c2f 6834 3e0a 0a3c 6469 7620  /a>.</h4>..<div 
+000009d0: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
+000009e0: 7479 6c65 3d22 7769 6474 683a 3830 3070  tyle="width:800p
+000009f0: 7822 3e0a 0a5b 215b 6c69 6e74 5d28 6874  x">..[![lint](ht
+00000a00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a10: 2f72 6566 7565 6c2d 6169 2f61 7574 6f6c  /refuel-ai/autol
+00000a20: 6162 656c 2f61 6374 696f 6e73 2f77 6f72  abel/actions/wor
+00000a30: 6b66 6c6f 7773 2f62 6c61 636b 2e79 616d  kflows/black.yam
+00000a40: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
+00000a50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a60: 2f72 6566 7565 6c2d 6169 2f61 7574 6f6c  /refuel-ai/autol
+00000a70: 6162 656c 2f61 6374 696f 6e73 2f77 6f72  abel/actions/wor
+00000a80: 6b66 6c6f 7773 2f62 6c61 636b 2e79 616d  kflows/black.yam
+00000a90: 6c2f 6261 6467 652e 7376 6729 2021 5b54  l/badge.svg) ![T
+00000aa0: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
+00000ab0: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
+00000ac0: 6169 2f61 7574 6f6c 6162 656c 2f61 6374  ai/autolabel/act
+00000ad0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f74  ions/workflows/t
+00000ae0: 6573 742e 7961 6d6c 2f62 6164 6765 2e73  est.yaml/badge.s
+00000af0: 7667 2920 215b 436f 6d6d 6974 2041 6374  vg) ![Commit Act
+00000b00: 6976 6974 795d 2868 7474 7073 3a2f 2f69  ivity](https://i
+00000b10: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000b20: 7468 7562 2f63 6f6d 6d69 742d 6163 7469  thub/commit-acti
+00000b30: 7669 7479 2f6d 2f72 6566 7565 6c2d 6169  vity/m/refuel-ai
+00000b40: 2f61 7574 6f6c 6162 656c 2920 5b21 5b44  /autolabel) [![D
+00000b50: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+00000b60: 696d 672e 7368 6965 6c64 732e 696f 2f64  img.shields.io/d
+00000b70: 6973 636f 7264 2f31 3039 3837 3436 3639  iscord/109874669
+00000b80: 3331 3532 3933 3139 3031 295d 2868 7474  3152931901)](htt
+00000b90: 7073 3a2f 2f64 6973 636f 7264 2e67 672f  ps://discord.gg/
+00000ba0: 6677 6556 6e52 7836 4355 2920 5b21 5b4c  fweVnRx6CU) [![L
+00000bb0: 6963 656e 7365 3a20 4d49 545d 2868 7474  icense: MIT](htt
+00000bc0: 7073 3a2f 2f62 6164 6765 6e2e 6e65 742f  ps://badgen.net/
+00000bd0: 6261 6467 652f 6c69 6365 6e73 652f 4d49  badge/license/MI
+00000be0: 542f 626c 7565 295d 2868 7474 7073 3a2f  T/blue)](https:/
+00000bf0: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
+00000c00: 6c69 6365 6e73 6573 2f4d 4954 290a 3c2f  licenses/MIT).</
+00000c10: 6469 763e 0a0a 2323 20e2 9aa1 2051 7569  div>..## ... Qui
+00000c20: 636b 2049 6e73 7461 6c6c 0a0a 6070 6970  ck Install..`pip
+00000c30: 2069 6e73 7461 6c6c 2072 6566 7565 6c2d   install refuel-
+00000c40: 6175 746f 6c61 6265 6c60 0a0a 2323 20f0  autolabel`..## .
+00000c50: 9f8f b720 5768 6174 2069 7320 4175 746f  ... What is Auto
+00000c60: 6c61 6265 6c0a 0a41 6363 6573 7320 746f  label..Access to
+00000c70: 205b 6c61 7267 652c 2063 6c65 616e 2061   [large, clean a
+00000c80: 6e64 2064 6976 6572 7365 5d28 6874 7470  nd diverse](http
+00000c90: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00000ca0: 6b61 7270 6174 6879 2f73 7461 7475 732f  karpathy/status/
+00000cb0: 3135 3238 3434 3331 3234 3537 3735 3133  1528443124577513
+00000cc0: 3437 323f 6c61 6e67 3d65 6e29 206c 6162  472?lang=en) lab
+00000cd0: 656c 6564 2064 6174 6173 6574 7320 6973  eled datasets is
+00000ce0: 2061 2063 7269 7469 6361 6c20 636f 6d70   a critical comp
+00000cf0: 6f6e 656e 7420 666f 7220 616e 7920 6d61  onent for any ma
+00000d00: 6368 696e 6520 6c65 6172 6e69 6e67 2065  chine learning e
+00000d10: 6666 6f72 7420 746f 2062 6520 7375 6363  ffort to be succ
+00000d20: 6573 7366 756c 2e20 5374 6174 652d 6f66  essful. State-of
+00000d30: 2d74 6865 2d61 7274 204c 4c4d 7320 6c69  -the-art LLMs li
+00000d40: 6b65 2047 5054 2d34 2061 7265 2061 626c  ke GPT-4 are abl
+00000d50: 6520 746f 205b 6175 746f 6d61 7469 6361  e to [automatica
+00000d60: 6c6c 7920 6c61 6265 6c20 6461 7461 5d28  lly label data](
+00000d70: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00000d80: 672f 6162 732f 3233 3033 2e31 3530 3536  g/abs/2303.15056
+00000d90: 2920 7769 7468 205b 6869 6768 2061 6363  ) with [high acc
+00000da0: 7572 6163 795d 2868 7474 7073 3a2f 2f61  uracy](https://a
+00000db0: 7278 6976 2e6f 7267 2f61 6273 2f32 3330  rxiv.org/abs/230
+00000dc0: 332e 3136 3835 3429 2c20 616e 6420 6174  3.16854), and at
+00000dd0: 2061 2066 7261 6374 696f 6e20 6f66 2074   a fraction of t
+00000de0: 6865 2063 6f73 7420 616e 6420 7469 6d65  he cost and time
+00000df0: 2063 6f6d 7061 7265 6420 746f 206d 616e   compared to man
+00000e00: 7561 6c20 6c61 6265 6c69 6e67 2e0a 0a41  ual labeling...A
+00000e10: 7574 6f6c 6162 656c 2069 7320 6120 5079  utolabel is a Py
+00000e20: 7468 6f6e 206c 6962 7261 7279 2074 6f20  thon library to 
+00000e30: 6c61 6265 6c2c 2063 6c65 616e 2061 6e64  label, clean and
+00000e40: 2065 6e72 6963 6820 7465 7874 2064 6174   enrich text dat
+00000e50: 6173 6574 7320 7769 7468 2061 6e79 204c  asets with any L
+00000e60: 6172 6765 204c 616e 6775 6167 6520 4d6f  arge Language Mo
+00000e70: 6465 6c73 2028 4c4c 4d29 206f 6620 796f  dels (LLM) of yo
+00000e80: 7572 2063 686f 6963 652e 0a0a 2323 20f0  ur choice...## .
+00000e90: 9f9a 8020 4765 7474 696e 6720 7374 6172  ... Getting star
+00000ea0: 7465 640a 0a41 7574 6f6c 6162 656c 2070  ted..Autolabel p
+00000eb0: 726f 7669 6465 7320 6120 7369 6d70 6c65  rovides a simple
+00000ec0: 2033 2d73 7465 7020 7072 6f63 6573 7320   3-step process 
+00000ed0: 666f 7220 6c61 6265 6c69 6e67 2064 6174  for labeling dat
+00000ee0: 613a 0a0a 312e 2053 7065 6369 6679 2074  a:..1. Specify t
+00000ef0: 6865 206c 6162 656c 696e 6720 6775 6964  he labeling guid
+00000f00: 656c 696e 6573 2061 6e64 204c 4c4d 206d  elines and LLM m
+00000f10: 6f64 656c 2074 6f20 7573 6520 696e 2061  odel to use in a
+00000f20: 204a 534f 4e20 636f 6e66 6967 2e0a 322e   JSON config..2.
+00000f30: 2044 7279 2d72 756e 2074 6f20 6d61 6b65   Dry-run to make
+00000f40: 2073 7572 6520 7468 6520 6669 6e61 6c20   sure the final 
+00000f50: 7072 6f6d 7074 206c 6f6f 6b73 2067 6f6f  prompt looks goo
+00000f60: 642e 0a33 2e20 4b69 636b 206f 6666 2061  d..3. Kick off a
+00000f70: 206c 6162 656c 696e 6720 7275 6e20 666f   labeling run fo
+00000f80: 7220 796f 7572 2064 6174 6173 6574 210a  r your dataset!.
+00000f90: 0a4c 6574 2773 2069 6d61 6769 6e65 2077  .Let's imagine w
+00000fa0: 6520 6172 6520 6275 696c 6469 6e67 2061  e are building a
+00000fb0: 6e20 4d4c 206d 6f64 656c 2074 6f20 616e  n ML model to an
+00000fc0: 616c 797a 6520 7365 6e74 696d 656e 7420  alyze sentiment 
+00000fd0: 616e 616c 7973 6973 206f 6620 6d6f 7669  analysis of movi
+00000fe0: 6520 7265 7669 6577 2e20 5765 2068 6176  e review. We hav
+00000ff0: 6520 6120 6461 7461 7365 7420 6f66 206d  e a dataset of m
+00001000: 6f76 6965 2072 6576 6965 7773 2074 6861  ovie reviews tha
+00001010: 7420 7765 2764 206c 696b 6520 746f 2067  t we'd like to g
+00001020: 6574 206c 6162 656c 6564 2066 6972 7374  et labeled first
+00001030: 2e20 466f 7220 7468 6973 2063 6173 652c  . For this case,
+00001040: 2068 6572 6527 7320 7768 6174 2074 6865   here's what the
+00001050: 2065 7861 6d70 6c65 2064 6174 6173 6574   example dataset
+00001060: 2061 6e64 2063 6f6e 6669 6773 2077 696c   and configs wil
+00001070: 6c20 6c6f 6f6b 206c 696b 653a 0a0a 6060  l look like:..``
+00001080: 6070 7974 686f 6e0a 7b0a 2020 2020 2274  `python.{.    "t
+00001090: 6173 6b5f 6e61 6d65 223a 2022 4d6f 7669  ask_name": "Movi
+000010a0: 6553 656e 7469 6d65 6e74 5265 7669 6577  eSentimentReview
+000010b0: 222c 0a20 2020 2022 7461 736b 5f74 7970  ",.    "task_typ
+000010c0: 6522 3a20 2263 6c61 7373 6966 6963 6174  e": "classificat
+000010d0: 696f 6e22 2c0a 2020 2020 226d 6f64 656c  ion",.    "model
+000010e0: 223a 207b 0a20 2020 2020 2020 2022 7072  ": {.        "pr
+000010f0: 6f76 6964 6572 223a 2022 6f70 656e 6169  ovider": "openai
+00001100: 222c 0a20 2020 2020 2020 2022 6e61 6d65  ",.        "name
+00001110: 223a 2022 6770 742d 332e 352d 7475 7262  ": "gpt-3.5-turb
+00001120: 6f22 0a20 2020 207d 2c0a 2020 2020 2264  o".    },.    "d
+00001130: 6174 6173 6574 223a 207b 0a20 2020 2020  ataset": {.     
+00001140: 2020 2022 6c61 6265 6c5f 636f 6c75 6d6e     "label_column
+00001150: 223a 2022 6c61 6265 6c22 2c0a 2020 2020  ": "label",.    
+00001160: 2020 2020 2264 656c 696d 6974 6572 223a      "delimiter":
+00001170: 2022 2c22 0a20 2020 207d 2c0a 2020 2020   ",".    },.    
+00001180: 2270 726f 6d70 7422 3a20 7b0a 2020 2020  "prompt": {.    
+00001190: 2020 2020 2274 6173 6b5f 6775 6964 656c      "task_guidel
+000011a0: 696e 6573 223a 2022 596f 7520 6172 6520  ines": "You are 
+000011b0: 616e 2065 7870 6572 7420 6174 2061 6e61  an expert at ana
+000011c0: 6c79 7a69 6e67 2074 6865 2073 656e 7469  lyzing the senti
+000011d0: 6d65 6e74 206f 6620 6d6f 7669 6520 7265  ment of movie re
+000011e0: 7669 6577 732e 2059 6f75 7220 6a6f 6220  views. Your job 
+000011f0: 6973 2074 6f20 636c 6173 7369 6679 2074  is to classify t
+00001200: 6865 2070 726f 7669 6465 6420 6d6f 7669  he provided movi
+00001210: 6520 7265 7669 6577 2069 6e74 6f20 6f6e  e review into on
+00001220: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+00001230: 6e67 206c 6162 656c 733a 207b 6c61 6265  ng labels: {labe
+00001240: 6c73 7d22 2c0a 2020 2020 2020 2020 226c  ls}",.        "l
+00001250: 6162 656c 7322 3a20 5b0a 2020 2020 2020  abels": [.      
+00001260: 2020 2020 2020 2270 6f73 6974 6976 6522        "positive"
+00001270: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00001280: 6567 6174 6976 6522 2c0a 2020 2020 2020  egative",.      
+00001290: 2020 2020 2020 226e 6575 7472 616c 222c        "neutral",
+000012a0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+000012b0: 2020 2020 2266 6577 5f73 686f 745f 6578      "few_shot_ex
+000012c0: 616d 706c 6573 223a 205b 0a20 2020 2020  amples": [.     
+000012d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000012e0: 2020 2020 2020 2020 2022 6578 616d 706c           "exampl
+000012f0: 6522 3a20 2249 2067 6f74 2061 2066 6169  e": "I got a fai
+00001300: 726c 7920 756e 696e 7370 6972 6564 2073  rly uninspired s
+00001310: 7475 7069 6420 6669 6c6d 2061 626f 7574  tupid film about
+00001320: 2068 6f77 2068 756d 616e 2069 6e64 7573   how human indus
+00001330: 7472 7920 6973 2062 6164 2066 6f72 206e  try is bad for n
+00001340: 6174 7572 652e 222c 0a20 2020 2020 2020  ature.",.       
+00001350: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00001360: 3a20 226e 6567 6174 6976 6522 0a20 2020  : "negative".   
+00001370: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00001380: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00001390: 2020 2020 2020 2020 2020 2265 7861 6d70            "examp
+000013a0: 6c65 223a 2022 4920 6c6f 7665 6420 7468  le": "I loved th
+000013b0: 6973 206d 6f76 6965 2e20 4920 666f 756e  is movie. I foun
+000013c0: 6420 6974 2076 6572 7920 6865 6172 7420  d it very heart 
+000013d0: 7761 726d 696e 6720 746f 2073 6565 2041  warming to see A
+000013e0: 6461 6d20 5765 7374 2c20 4275 7274 2057  dam West, Burt W
+000013f0: 6172 642c 2046 7261 6e6b 2047 6f72 7368  ard, Frank Gorsh
+00001400: 696e 2c20 616e 6420 4a75 6c69 6520 4e65  in, and Julie Ne
+00001410: 776d 6172 2074 6f67 6574 6865 7220 6167  wmar together ag
+00001420: 6169 6e2e 222c 0a20 2020 2020 2020 2020  ain.",.         
+00001430: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00001440: 2270 6f73 6974 6976 6522 0a20 2020 2020  "positive".     
+00001450: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001460: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001470: 2020 2020 2020 2020 2265 7861 6d70 6c65          "example
+00001480: 223a 2022 5468 6973 206d 6f76 6965 2077  ": "This movie w
+00001490: 696c 6c20 6265 2070 6c61 7965 6420 6e65  ill be played ne
+000014a0: 7874 2077 6565 6b20 6174 2074 6865 2043  xt week at the C
+000014b0: 6869 6e65 7365 2074 6865 6174 6572 2e22  hinese theater."
+000014c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000014d0: 2020 226c 6162 656c 223a 2022 6e65 7574    "label": "neut
+000014e0: 7261 6c22 0a20 2020 2020 2020 2020 2020  ral".           
+000014f0: 207d 0a20 2020 2020 2020 205d 2c0a 2020   }.        ],.  
+00001500: 2020 2020 2020 2265 7861 6d70 6c65 5f74        "example_t
+00001510: 656d 706c 6174 6522 3a20 2249 6e70 7574  emplate": "Input
+00001520: 3a20 7b65 7861 6d70 6c65 7d5c 6e4f 7574  : {example}\nOut
+00001530: 7075 743a 207b 6c61 6265 6c7d 220a 2020  put: {label}".  
+00001540: 2020 7d0a 7d0a 6060 600a 0a49 6e69 7469    }.}.```..Initi
+00001550: 616c 697a 6520 7468 6520 6c61 6265 6c69  alize the labeli
+00001560: 6e67 2061 6765 6e74 2061 6e64 2070 6173  ng agent and pas
+00001570: 7320 6974 2074 6865 2063 6f6e 6669 673a  s it the config:
+00001580: 0a0a 6060 6070 7974 686f 6e0a 0a66 726f  ..```python..fro
+00001590: 6d20 6175 746f 6c61 6265 6c20 696d 706f  m autolabel impo
+000015a0: 7274 204c 6162 656c 696e 6741 6765 6e74  rt LabelingAgent
+000015b0: 0a0a 6167 656e 7420 3d20 4c61 6265 6c69  ..agent = Labeli
+000015c0: 6e67 4167 656e 7428 636f 6e66 6967 3d27  ngAgent(config='
+000015d0: 636f 6e66 6967 2e6a 736f 6e27 290a 6060  config.json').``
+000015e0: 600a 0a50 7265 7669 6577 2061 6e20 6578  `..Preview an ex
+000015f0: 616d 706c 6520 7072 6f6d 7074 2074 6861  ample prompt tha
+00001600: 7420 7769 6c6c 2062 6520 7365 6e74 2074  t will be sent t
+00001610: 6f20 7468 6520 4c4c 4d3a 0a0a 6060 6070  o the LLM:..```p
+00001620: 7974 686f 6e0a 6167 656e 742e 706c 616e  ython.agent.plan
+00001630: 2827 6461 7461 7365 742e 6373 7627 290a  ('dataset.csv').
+00001640: 6060 600a 0a54 6869 7320 7072 696e 7473  ```..This prints
+00001650: 3a0a 0a60 6060 0ae2 9481 e294 81e2 9481  :..```..........
+00001660: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00001670: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00001680: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00001690: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+000016a0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+000016b0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000016c0: e294 81e2 9481 e294 81e2 9481 e294 8120  ............... 
+000016d0: 3130 302f 3130 3020 303a 3030 3a30 3020  100/100 0:00:00 
+000016e0: 303a 3030 3a30 300a e294 8ce2 9480 e294  0:00:00.........
+000016f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001700: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001710: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001720: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001730: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00001740: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001750: 80e2 9480 e294 80e2 9490 0ae2 9482 2054  .............. T
+00001760: 6f74 616c 2045 7374 696d 6174 6564 2043  otal Estimated C
+00001770: 6f73 7420 2020 2020 e294 8220 2430 2e35  ost     ... $0.5
+00001780: 3338 2020 e294 820a e294 8220 4e75 6d62  38  ....... Numb
+00001790: 6572 206f 6620 4578 616d 706c 6573 2020  er of Examples  
+000017a0: 2020 2020 20e2 9482 2032 3030 2020 2020       ... 200    
+000017b0: 20e2 9482 0ae2 9482 2041 7665 7261 6765   ....... Average
+000017c0: 2063 6f73 7420 7065 7220 6578 616d 706c   cost per exampl
+000017d0: 6520 e294 8220 302e 3030 3236 3920 e294  e ... 0.00269 ..
+000017e0: 820a e294 94e2 9480 e294 80e2 9480 e294  ................
+000017f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001830: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+00001840: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001850: 80e2 9498 0ae2 9480 e294 80e2 9480 e294  ................
+00001860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000018a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000018b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000018c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000018d0: 0a0a 5072 6f6d 7074 2045 7861 6d70 6c65  ..Prompt Example
+000018e0: 3a0a 596f 7520 6172 6520 616e 2065 7870  :.You are an exp
+000018f0: 6572 7420 6174 2061 6e61 6c79 7a69 6e67  ert at analyzing
+00001900: 2074 6865 2073 656e 7469 6d65 6e74 206f   the sentiment o
+00001910: 6620 6d6f 7669 6520 7265 7669 6577 732e  f movie reviews.
+00001920: 2059 6f75 7220 6a6f 6220 6973 2074 6f20   Your job is to 
+00001930: 636c 6173 7369 6679 2074 6865 2070 726f  classify the pro
+00001940: 7669 6465 6420 6d6f 7669 6520 7265 7669  vided movie revi
+00001950: 6577 2069 6e74 6f20 6f6e 6520 6f66 2074  ew into one of t
+00001960: 6865 2066 6f6c 6c6f 7769 6e67 206c 6162  he following lab
+00001970: 656c 733a 205b 706f 7369 7469 7665 2c20  els: [positive, 
+00001980: 6e65 6761 7469 7665 2c20 6e65 7574 7261  negative, neutra
+00001990: 6c5d 0a0a 536f 6d65 2065 7861 6d70 6c65  l]..Some example
+000019a0: 7320 7769 7468 2074 6865 6972 206f 7574  s with their out
+000019b0: 7075 7420 616e 7377 6572 7320 6172 6520  put answers are 
+000019c0: 7072 6f76 6964 6564 2062 656c 6f77 3a0a  provided below:.
+000019d0: 0a45 7861 6d70 6c65 3a20 4920 676f 7420  .Example: I got 
+000019e0: 6120 6661 6972 6c79 2075 6e69 6e73 7069  a fairly uninspi
+000019f0: 7265 6420 7374 7570 6964 2066 696c 6d20  red stupid film 
+00001a00: 6162 6f75 7420 686f 7720 6875 6d61 6e20  about how human 
+00001a10: 696e 6475 7374 7279 2069 7320 6261 6420  industry is bad 
+00001a20: 666f 7220 6e61 7475 7265 2e0a 4f75 7470  for nature..Outp
+00001a30: 7574 3a0a 6e65 6761 7469 7665 0a0a 4578  ut:.negative..Ex
+00001a40: 616d 706c 653a 2049 206c 6f76 6564 2074  ample: I loved t
+00001a50: 6869 7320 6d6f 7669 652e 2049 2066 6f75  his movie. I fou
+00001a60: 6e64 2069 7420 7665 7279 2068 6561 7274  nd it very heart
+00001a70: 2077 6172 6d69 6e67 2074 6f20 7365 6520   warming to see 
+00001a80: 4164 616d 2057 6573 742c 2042 7572 7420  Adam West, Burt 
+00001a90: 5761 7264 2c20 4672 616e 6b20 476f 7273  Ward, Frank Gors
+00001aa0: 6869 6e2c 2061 6e64 204a 756c 6965 204e  hin, and Julie N
+00001ab0: 6577 6d61 7220 746f 6765 7468 6572 2061  ewmar together a
+00001ac0: 6761 696e 2e0a 4f75 7470 7574 3a0a 706f  gain..Output:.po
+00001ad0: 7369 7469 7665 0a0a 4578 616d 706c 653a  sitive..Example:
+00001ae0: 2054 6869 7320 6d6f 7669 6520 7769 6c6c   This movie will
+00001af0: 2062 6520 706c 6179 6564 206e 6578 7420   be played next 
+00001b00: 7765 656b 2061 7420 7468 6520 4368 696e  week at the Chin
+00001b10: 6573 6520 7468 6561 7465 722e 0a4f 7574  ese theater..Out
+00001b20: 7075 743a 0a6e 6575 7472 616c 0a0a 4e6f  put:.neutral..No
+00001b30: 7720 4920 7761 6e74 2079 6f75 2074 6f20  w I want you to 
+00001b40: 6c61 6265 6c20 7468 6520 666f 6c6c 6f77  label the follow
+00001b50: 696e 6720 6578 616d 706c 653a 0a49 6e70  ing example:.Inp
+00001b60: 7574 3a20 4120 7261 7265 2065 7863 6570  ut: A rare excep
+00001b70: 7469 6f6e 2074 6f20 7468 6520 7275 6c65  tion to the rule
+00001b80: 2074 6861 7420 6772 6561 7420 6c69 7465   that great lite
+00001b90: 7261 7475 7265 206d 616b 6573 2064 6973  rature makes dis
+00001ba0: 6170 706f 696e 7469 6e67 2066 696c 6d73  appointing films
+00001bb0: 2e0a 4f75 7470 7574 3a0a 0ae2 9480 e294  ..Output:.......
+00001bc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001bd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001be0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001bf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001ca0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001cb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001cc0: e294 80e2 9480 0a0a 6060 600a 0a46 696e  ........```..Fin
+00001cd0: 616c 6c79 2c20 7765 2063 616e 2072 756e  ally, we can run
+00001ce0: 2074 6865 206c 6162 656c 696e 6720 6f6e   the labeling on
+00001cf0: 2061 2073 7562 7365 7420 6f72 2065 6e74   a subset or ent
+00001d00: 6972 6574 7920 6f66 2074 6865 2064 6174  irety of the dat
+00001d10: 6173 6574 3a0a 0a60 6060 7079 7468 6f6e  aset:..```python
+00001d20: 0a6c 6162 656c 732c 206f 7574 7075 745f  .labels, output_
+00001d30: 6466 2c20 6d65 7472 6963 7320 3d20 6167  df, metrics = ag
+00001d40: 656e 742e 7275 6e28 2764 6174 6173 6574  ent.run('dataset
+00001d50: 2e63 7376 2729 0a60 6060 0a0a 5468 6520  .csv').```..The 
+00001d60: 6f75 7470 7574 2064 6174 6166 7261 6d65  output dataframe
+00001d70: 2063 6f6e 7461 696e 7320 7468 6520 6c61   contains the la
+00001d80: 6265 6c20 636f 6c75 6d6e 3a0a 0a60 6060  bel column:..```
+00001d90: 7079 7468 6f6e 0a6f 7574 7075 745f 6466  python.output_df
+00001da0: 2e68 6561 6428 290a 2020 2020 2020 2020  .head().        
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 2020 2020 7465 7874 2020 2e2e          text  ..
+00001de0: 2e20 4d6f 7669 6553 656e 7469 6d65 6e74  . MovieSentiment
+00001df0: 5265 7669 6577 5f6c 6c6d 5f6c 6162 656c  Review_llm_label
+00001e00: 0a30 2020 4920 7761 7320 7665 7279 2065  .0  I was very e
+00001e10: 7863 6974 6564 2061 626f 7574 2073 6565  xcited about see
+00001e20: 696e 6720 7468 6973 2066 696c 6d2c 2061  ing this film, a
+00001e30: 6e74 2e2e 2e20 202e 2e2e 2020 2020 2020  nt...  ...      
+00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e50: 206e 6567 6174 6976 650a 3120 2053 6572   negative.1  Ser
+00001e60: 756d 2069 7320 6162 6f75 7420 6120 6372  um is about a cr
+00001e70: 617a 7920 646f 6374 6f72 2074 6861 7420  azy doctor that 
+00001e80: 6669 6e64 7320 6120 7365 722e 2e2e 2020  finds a ser...  
+00001e90: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+00001ea0: 2020 2020 2020 2020 2020 6e65 6761 7469            negati
+00001eb0: 7665 0a34 2020 4920 6c6f 7665 6420 7468  ve.4  I loved th
+00001ec0: 6973 206d 6f76 6965 2e20 4920 6b6e 6577  is movie. I knew
+00001ed0: 2069 7420 776f 756c 6420 6265 2063 686f   it would be cho
+00001ee0: 636b 6564 2e2e 2e20 202e 2e2e 2020 2020  cked...  ...    
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2020 2070 6f73 6974 6976 650a 2e2e 2e0a     positive.....
+00001f10: 6060 600a 0a23 2320 4665 6174 7572 6573  ```..## Features
+00001f20: 0a0a 312e 204c 6162 656c 2064 6174 6120  ..1. Label data 
+00001f30: 666f 7220 5b4e 4c50 2074 6173 6b73 5d28  for [NLP tasks](
+00001f40: 6874 7470 733a 2f2f 646f 6373 2e72 6566  https://docs.ref
+00001f50: 7565 6c2e 6169 2f67 7569 6465 2f74 6173  uel.ai/guide/tas
+00001f60: 6b73 2f63 6c61 7373 6966 6963 6174 696f  ks/classificatio
+00001f70: 6e5f 7461 736b 2f29 2073 7563 6820 6173  n_task/) such as
+00001f80: 2063 6c61 7373 6966 6963 6174 696f 6e2c   classification,
+00001f90: 2071 7565 7374 696f 6e2d 616e 7377 6572   question-answer
+00001fa0: 696e 6720 616e 6420 6e61 6d65 6420 656e  ing and named en
+00001fb0: 7469 7479 2d72 6563 6f67 6e69 7469 6f6e  tity-recognition
+00001fc0: 2c20 656e 7469 7479 206d 6174 6368 696e  , entity matchin
+00001fd0: 6720 616e 6420 6d6f 7265 2e0a 322e 2055  g and more..2. U
+00001fe0: 7365 2063 6f6d 6d65 7263 6961 6c20 6f72  se commercial or
+00001ff0: 206f 7065 6e20 736f 7572 6365 205b 4c4c   open source [LL
+00002000: 4d73 5d28 6874 7470 733a 2f2f 646f 6373  Ms](https://docs
+00002010: 2e72 6566 7565 6c2e 6169 2f67 7569 6465  .refuel.ai/guide
+00002020: 2f6c 6c6d 732f 6c6c 6d73 2f29 2066 726f  /llms/llms/) fro
+00002030: 6d20 7072 6f76 6964 6572 7320 7375 6368  m providers such
+00002040: 2061 7320 4f70 656e 4149 2c20 416e 7468   as OpenAI, Anth
+00002050: 726f 7069 632c 2048 7567 6769 6e67 4661  ropic, HuggingFa
+00002060: 6365 2c20 476f 6f67 6c65 2061 6e64 206d  ce, Google and m
+00002070: 6f72 652e 0a33 2e20 5375 7070 6f72 7420  ore..3. Support 
+00002080: 666f 7220 7265 7365 6172 6368 2d70 726f  for research-pro
+00002090: 7665 6e20 4c4c 4d20 7465 6368 6e69 7175  ven LLM techniqu
+000020a0: 6573 2074 6f20 626f 6f73 7420 6c61 6265  es to boost labe
+000020b0: 6c20 7175 616c 6974 792c 2073 7563 6820  l quality, such 
+000020c0: 6173 2066 6577 2d73 686f 7420 6c65 6172  as few-shot lear
+000020d0: 6e69 6e67 2061 6e64 2063 6861 696e 2d6f  ning and chain-o
+000020e0: 662d 7468 6f75 6768 7420 7072 6f6d 7074  f-thought prompt
+000020f0: 696e 672e 0a34 2e20 5b43 6f6e 6669 6465  ing..4. [Confide
+00002100: 6e63 6520 6573 7469 6d61 7469 6f6e 5d28  nce estimation](
+00002110: 6874 7470 733a 2f2f 646f 6373 2e72 6566  https://docs.ref
+00002120: 7565 6c2e 6169 2f67 7569 6465 2f61 6363  uel.ai/guide/acc
+00002130: 7572 6163 792f 636f 6e66 6964 656e 6365  uracy/confidence
+00002140: 2f29 2061 6e64 2065 7870 6c61 6e61 7469  /) and explanati
+00002150: 6f6e 7320 6f75 7420 6f66 2074 6865 2062  ons out of the b
+00002160: 6f78 2066 6f72 2065 7665 7279 2073 696e  ox for every sin
+00002170: 676c 6520 6f75 7470 7574 206c 6162 656c  gle output label
+00002180: 0a35 2e20 5b43 6163 6869 6e67 2061 6e64  .5. [Caching and
+00002190: 2073 7461 7465 206d 616e 6167 656d 656e   state managemen
+000021a0: 745d 2868 7474 7073 3a2f 2f64 6f63 732e  t](https://docs.
+000021b0: 7265 6675 656c 2e61 692f 6775 6964 652f  refuel.ai/guide/
+000021c0: 7265 6c69 6162 696c 6974 792f 7374 6174  reliability/stat
+000021d0: 652d 6d61 6e61 6765 6d65 6e74 2f29 2074  e-management/) t
+000021e0: 6f20 6d69 6e69 6d69 7a65 2063 6f73 7473  o minimize costs
+000021f0: 2061 6e64 2065 7870 6572 696d 656e 7461   and experimenta
+00002200: 7469 6f6e 2074 696d 650a 0a23 2320 f09f  tion time..## ..
+00002210: 9ba0 efb8 8f20 526f 6164 6d61 700a 4f75  ..... Roadmap.Ou
+00002220: 7220 676f 616c 2069 7320 746f 2061 6c6c  r goal is to all
+00002230: 6f77 2075 7365 7273 2074 6f20 6c61 6265  ow users to labe
+00002240: 6c2c 2063 7265 6174 6520 6f72 2065 6e72  l, create or enr
+00002250: 6963 6820 616e 7920 6461 7461 7365 742c  ich any dataset,
+00002260: 2077 6974 6820 616e 7920 4c4c 4d20 2d20   with any LLM - 
+00002270: 6561 7369 6c79 2061 6e64 2071 7569 636b  easily and quick
+00002280: 6c79 2e0a 0a54 6865 7265 2061 7265 2066  ly...There are f
+00002290: 6f75 7220 666f 6375 7320 6172 6561 7320  our focus areas 
+000022a0: 666f 7220 4175 746f 6c61 6265 6c20 666f  for Autolabel fo
+000022b0: 7220 3230 3233 3a0a 0a2a 202a 2a54 6173  r 2023:..* **Tas
+000022c0: 6b73 2a2a 3a20 4164 6420 7375 7070 6f72  ks**: Add suppor
+000022d0: 7420 666f 7220 7461 736b 7320 7375 6368  t for tasks such
+000022e0: 2061 7320 7265 7472 6965 7661 6c2c 2061   as retrieval, a
+000022f0: 7474 7269 6275 7465 2065 6e72 6963 686d  ttribute enrichm
+00002300: 656e 7420 616e 6420 7465 7874 2067 656e  ent and text gen
+00002310: 6572 6174 696f 6e2f 7772 6974 696e 672e  eration/writing.
+00002320: 0a2a 202a 2a4c 4c4d 732a 2a3a 2041 6464  .* **LLMs**: Add
+00002330: 2073 7570 706f 7274 2066 6f72 206d 6f72   support for mor
+00002340: 6520 4c4c 4d73 2c20 6573 7065 6369 616c  e LLMs, especial
+00002350: 6c79 206f 7065 6e20 736f 7572 6365 206d  ly open source m
+00002360: 6f64 656c 7320 6c69 6b65 2046 616c 636f  odels like Falco
+00002370: 6e2c 204d 5054 2061 6e64 2044 6f6c 6c79  n, MPT and Dolly
+00002380: 2061 6e64 2074 6865 2061 6269 6c69 7479   and the ability
+00002390: 2074 6f20 706c 7567 2069 6e20 796f 7572   to plug in your
+000023a0: 206f 776e 204c 4c4d 732e 200a 2a20 576f   own LLMs. .* Wo
+000023b0: 726b 666c 6f77 7320 666f 7220 2a2a 6578  rkflows for **ex
+000023c0: 7065 7269 6d65 6e74 696e 6720 7769 7468  perimenting with
+000023d0: 2079 6f75 7220 6461 7461 7365 7473 2a2a   your datasets**
+000023e0: 206d 6f72 6520 6561 7369 6c79 3a20 4164   more easily: Ad
+000023f0: 6420 7375 7070 6f72 7420 666f 7220 7269  d support for ri
+00002400: 6368 6572 2064 6174 6120 7479 7065 7320  cher data types 
+00002410: 2873 7563 6820 6173 2050 4446 7320 616e  (such as PDFs an
+00002420: 6420 4854 4d4c 2064 6f63 756d 656e 7473  d HTML documents
+00002430: 2920 616e 6420 7468 6520 6162 696c 6974  ) and the abilit
+00002440: 7920 746f 2072 756e 2062 656e 6368 6d61  y to run benchma
+00002450: 726b 696e 6720 6f6e 2079 6f75 7220 6461  rking on your da
+00002460: 7461 2073 6f75 7263 6573 2e0a 2a20 5465  ta sources..* Te
+00002470: 6368 6e69 7175 6573 2074 6f20 2a2a 696d  chniques to **im
+00002480: 7072 6f76 6520 6c61 6265 6c69 6e67 2061  prove labeling a
+00002490: 6363 7572 6163 792a 2a3a 2041 6464 2073  ccuracy**: Add s
+000024a0: 7570 706f 7274 2066 6f72 2061 7574 6f6d  upport for autom
+000024b0: 6174 6963 2070 726f 6d70 7420 696d 7072  atic prompt impr
+000024c0: 6f76 656d 656e 7420 616e 6420 746f 6f6c  ovement and tool
+000024d0: 7320 666f 7220 6265 7474 6572 2065 7272  s for better err
+000024e0: 6f72 2061 6e61 6c79 7369 7320 746f 2069  or analysis to i
+000024f0: 7465 7261 7469 7665 6c79 2069 6d70 726f  teratively impro
+00002500: 7665 204c 4c4d 2070 6572 666f 726d 616e  ve LLM performan
+00002510: 6365 206f 6e20 6469 6666 6572 656e 7420  ce on different 
+00002520: 7461 736b 7320 0a0a 5765 2077 696c 6c20  tasks ..We will 
+00002530: 6265 2072 656c 6561 7369 6e67 2061 206d  be releasing a m
+00002540: 6f72 6520 6465 7461 696c 6564 2072 6f61  ore detailed roa
+00002550: 646d 6170 2073 6f6f 6e2c 2062 7574 2077  dmap soon, but w
+00002560: 6520 6c6f 7665 2073 7567 6765 7374 696f  e love suggestio
+00002570: 6e73 2061 6e64 2063 6f6e 7472 6962 7574  ns and contribut
+00002580: 696f 6e73 2066 726f 6d20 7468 6520 636f  ions from the co
+00002590: 6d6d 756e 6974 792e 2043 6861 7420 7769  mmunity. Chat wi
+000025a0: 7468 2074 6865 2052 6566 7565 6c20 7465  th the Refuel te
+000025b0: 616d 2061 6e64 2041 7574 6f6c 6162 656c  am and Autolabel
+000025c0: 2063 6f6d 6d75 6e69 7479 206f 6e20 5b44   community on [D
+000025d0: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+000025e0: 6469 7363 6f72 642e 6767 2f66 7765 566e  discord.gg/fweVn
+000025f0: 5278 3643 5529 206f 7220 6f70 656e 205b  Rx6CU) or open [
+00002600: 4769 7468 7562 2069 7373 7565 735d 2868  Github issues](h
+00002610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002620: 6d2f 7265 6675 656c 2d61 692f 6175 746f  m/refuel-ai/auto
+00002630: 6c61 6265 6c2f 6973 7375 6573 2920 746f  label/issues) to
+00002640: 2072 6570 6f72 7420 6275 6773 2061 6e64   report bugs and
+00002650: 2072 6571 7565 7374 2066 6561 7475 7265   request feature
+00002660: 732e 0a0a 2323 20f0 9f99 8c20 436f 6e74  s...## .... Cont
+00002670: 7269 6275 7469 6e67 0a0a 4175 746f 6c61  ributing..Autola
+00002680: 6265 6c20 6973 2061 2072 6170 6964 6c79  bel is a rapidly
+00002690: 2064 6576 656c 6f70 696e 6720 7072 6f6a   developing proj
+000026a0: 6563 742e 2057 6520 7765 6c63 6f6d 6520  ect. We welcome 
+000026b0: 636f 6e74 7269 6275 7469 6f6e 7320 696e  contributions in
+000026c0: 2061 6c6c 2066 6f72 6d73 202d 2062 7567   all forms - bug
+000026d0: 2072 6570 6f72 7473 2c20 7075 6c6c 2072   reports, pull r
+000026e0: 6571 7565 7374 7320 616e 6420 6964 6561  equests and idea
+000026f0: 7320 666f 7220 696d 7072 6f76 696e 6720  s for improving 
+00002700: 7468 6520 6c69 6272 6172 792e 0a0a 312e  the library...1.
+00002710: 204a 6f69 6e20 7468 6520 636f 6e76 6572   Join the conver
+00002720: 7361 7469 6f6e 206f 6e20 5b44 6973 636f  sation on [Disco
+00002730: 7264 5d28 6874 7470 733a 2f2f 6469 7363  rd](https://disc
+00002740: 6f72 642e 6767 2f66 7765 566e 5278 3643  ord.gg/fweVnRx6C
+00002750: 5529 0a32 2e20 4f70 656e 2061 6e20 5b69  U).2. Open an [i
+00002760: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
+00002770: 7468 7562 2e63 6f6d 2f72 6566 7565 6c2d  thub.com/refuel-
+00002780: 6169 2f61 7574 6f6c 6162 656c 2f69 7373  ai/autolabel/iss
+00002790: 7565 7329 206f 6e20 4769 7468 7562 2066  ues) on Github f
+000027a0: 6f72 2062 7567 7320 616e 6420 7265 7175  or bugs and requ
+000027b0: 6573 7420 6665 6174 7572 6573 2e0a 332e  est features..3.
+000027c0: 2047 7261 6220 616e 206f 7065 6e20 6973   Grab an open is
+000027d0: 7375 652c 2061 6e64 2073 7562 6d69 7420  sue, and submit 
+000027e0: 6120 5b70 756c 6c20 7265 7175 6573 745d  a [pull request]
+000027f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002800: 636f 6d2f 7265 6675 656c 2d61 692f 6175  com/refuel-ai/au
+00002810: 746f 6c61 6265 6c2f 626c 6f62 2f6d 6169  tolabel/blob/mai
+00002820: 6e2f 434f 4e54 5249 4255 5449 4e47 2e6d  n/CONTRIBUTING.m
+00002830: 6429 2e0a                                d)..
```

### Comparing `refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/SOURCES.txt` & `refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.1/src/refuel_autolabel.egg-info/requires.txt` & `refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/requires.txt`

 * *Files identical despite different names*

