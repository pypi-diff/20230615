# Comparing `tmp/refuel-autolabel-0.0.2.tar.gz` & `tmp/refuel-autolabel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-autolabel-0.0.2.tar", last modified: Thu Jun 15 09:29:43 2023, max compression
+gzip compressed data, was "refuel-autolabel-0.0.3.tar", last modified: Thu Jun 15 15:35:31 2023, max compression
```

## Comparing `refuel-autolabel-0.0.2.tar` & `refuel-autolabel-0.0.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.294209 refuel-autolabel-0.0.2/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/LICENSE
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10292 2023-06-15 09:29:43.293992 refuel-autolabel-0.0.2/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8283 2023-06-15 09:16:31.000000 refuel-autolabel-0.0.2/README.md
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1922 2023-06-15 09:25:59.000000 refuel-autolabel-0.0.2/pyproject.toml
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-15 09:29:43.294283 refuel-autolabel-0.0.2/setup.cfg
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.280100 refuel-autolabel-0.0.2/src/
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.282542 refuel-autolabel-0.0.2/src/autolabel/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/__init__.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.283321 refuel-autolabel-0.0.2/src/autolabel/cache/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/cache/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/cache/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/cache/sqlalchemy_cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.2/src/autolabel/confidence.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.284043 refuel-autolabel-0.0.2/src/autolabel/configs/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/configs/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1515 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/configs/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5880 2023-06-15 01:06:20.000000 refuel-autolabel-0.0.2/src/autolabel/configs/config.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.285882 refuel-autolabel-0.0.2/src/autolabel/data_models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/annotation.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/dataset.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/task.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/data_models/task_run.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.286481 refuel-autolabel-0.0.2/src/autolabel/database/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/database/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      410 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/database/engine.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/database/state_manager.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6592 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/dataset_loader.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.287143 refuel-autolabel-0.0.2/src/autolabel/few_shot/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2429 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/few_shot/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/few_shot/fixed_example_selector.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/few_shot/vector_store.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19394 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/labeler.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.291584 refuel-autolabel-0.0.2/src/autolabel/models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/anthropic.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3037 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/hf_pipeline.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3768 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.2/src/autolabel/models/openai.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3599 2023-06-15 01:29:24.000000 refuel-autolabel-0.0.2/src/autolabel/models/palm.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3569 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/models/refuel.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4625 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.292909 refuel-autolabel-0.0.2/src/autolabel/tasks/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1160 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3509 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7060 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7071 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/entity_matching.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12517 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/named_entity_recognition.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7160 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/question_answering.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.2/src/autolabel/tasks/utils.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8888 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.2/src/autolabel/utils.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 09:29:43.293610 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    10292 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1571 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      641 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/requires.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-15 09:29:43.000000 refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/top_level.txt
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.643343 refuel-autolabel-0.0.3/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/LICENSE
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-15 15:35:31.642916 refuel-autolabel-0.0.3/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9005 2023-06-15 15:29:16.000000 refuel-autolabel-0.0.3/README.md
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1922 2023-06-15 15:35:08.000000 refuel-autolabel-0.0.3/pyproject.toml
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-15 15:35:31.643404 refuel-autolabel-0.0.3/setup.cfg
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.628712 refuel-autolabel-0.0.3/src/
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.631361 refuel-autolabel-0.0.3/src/autolabel/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/__init__.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.632207 refuel-autolabel-0.0.3/src/autolabel/cache/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/cache/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/cache/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/cache/sqlalchemy_cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.3/src/autolabel/confidence.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.633089 refuel-autolabel-0.0.3/src/autolabel/configs/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/configs/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1515 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/configs/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5880 2023-06-15 01:06:20.000000 refuel-autolabel-0.0.3/src/autolabel/configs/config.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.635318 refuel-autolabel-0.0.3/src/autolabel/data_models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/annotation.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/dataset.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/task.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/task_run.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.635951 refuel-autolabel-0.0.3/src/autolabel/database/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/database/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      410 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/database/engine.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/database/state_manager.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6592 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/dataset_loader.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.636626 refuel-autolabel-0.0.3/src/autolabel/few_shot/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2429 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/few_shot/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/few_shot/fixed_example_selector.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/few_shot/vector_store.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19394 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/labeler.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.638070 refuel-autolabel-0.0.3/src/autolabel/models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/anthropic.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3037 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/hf_pipeline.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3768 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/openai.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3599 2023-06-15 01:29:24.000000 refuel-autolabel-0.0.3/src/autolabel/models/palm.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3569 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/models/refuel.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4625 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/schema.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.641755 refuel-autolabel-0.0.3/src/autolabel/tasks/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1160 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3509 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7060 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/classification.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7071 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/entity_matching.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12517 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/named_entity_recognition.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7160 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/question_answering.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/utils.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8888 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/utils.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.642679 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1571 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      641 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/requires.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/top_level.txt
```

### Comparing `refuel-autolabel-0.0.2/LICENSE` & `refuel-autolabel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/PKG-INFO` & `refuel-autolabel-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for LLM powered labeling
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,17 +38,16 @@
 Provides-Extra: openai
 Provides-Extra: anthropic
 Provides-Extra: huggingface
 Provides-Extra: google
 Provides-Extra: all
 License-File: LICENSE
 
-<picture>
-  <img alt="Refuel logo" src="docs/assets/Autolabel_blk_w_background.png">
-</picture>
+<img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
+
 <p align="center">
     <b>Clean, labeled data at the speed of thought</b>.
 </p>
 
 <h4 align="center">
   <a href="https://docs.refuel.ai/guide/overview/getting-started/">Getting started</a> |
   <a href="https://docs.refuel.ai/">Docs</a> |
@@ -192,14 +191,24 @@
 
 1. Label data for [NLP tasks](https://docs.refuel.ai/guide/tasks/classification_task/) such as classification, question-answering and named entity-recognition, entity matching and more.
 2. Use commercial or open source [LLMs](https://docs.refuel.ai/guide/llms/llms/) from providers such as OpenAI, Anthropic, HuggingFace, Google and more.
 3. Support for research-proven LLM techniques to boost label quality, such as few-shot learning and chain-of-thought prompting.
 4. [Confidence estimation](https://docs.refuel.ai/guide/accuracy/confidence/) and explanations out of the box for every single output label
 5. [Caching and state management](https://docs.refuel.ai/guide/reliability/state-management/) to minimize costs and experimentation time
 
+## Access to Refuel hosted LLMs
+
+Refuel provides access to hosted open source LLMs for labeling, and for estimating confidence This is helpful, because you can calibrate a confidence threshold for your labeling task, and then route less confident labels to humans, while you still get the benefits of auto-labeling for the confident examples.
+
+In order to use Refuel hosted LLMs, you can [request access here](https://refuel-ai.typeform.com/llm-access).
+
+## Benchmark
+
+Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-technical-report) to learn more about the performance of various LLMs, and human annoators, on label quality, turnaround time and cost.
+
 ## 🛠️ Roadmap
 Our goal is to allow users to label, create or enrich any dataset, with any LLM - easily and quickly.
 
 There are four focus areas for Autolabel for 2023:
 
 * **Tasks**: Add support for tasks such as retrieval, attribute enrichment and text generation/writing.
 * **LLMs**: Add support for more LLMs, especially open source models like Falcon, MPT and Dolly and the ability to plug in your own LLMs.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.2 Summary: Library
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.3 Summary: Library
 for LLM powered labeling Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -18,15 +18,15 @@
 autolabel Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
 Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
-File: LICENSE  [Refuel logo]
+File: LICENSE [Refuel logo]
                  Clean, labeled data at the speed of thought.
          *** Getting_started | Docs | Discord | Twitter | Website ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
@@ -93,28 +93,37 @@
 source [LLMs](https://docs.refuel.ai/guide/llms/llms/) from providers such as
 OpenAI, Anthropic, HuggingFace, Google and more. 3. Support for research-proven
 LLM techniques to boost label quality, such as few-shot learning and chain-of-
 thought prompting. 4. [Confidence estimation](https://docs.refuel.ai/guide/
 accuracy/confidence/) and explanations out of the box for every single output
 label 5. [Caching and state management](https://docs.refuel.ai/guide/
 reliability/state-management/) to minimize costs and experimentation time ##
-ð ï¸ Roadmap Our goal is to allow users to label, create or enrich any
-dataset, with any LLM - easily and quickly. There are four focus areas for
-Autolabel for 2023: * **Tasks**: Add support for tasks such as retrieval,
-attribute enrichment and text generation/writing. * **LLMs**: Add support for
-more LLMs, especially open source models like Falcon, MPT and Dolly and the
-ability to plug in your own LLMs. * Workflows for **experimenting with your
-datasets** more easily: Add support for richer data types (such as PDFs and
-HTML documents) and the ability to run benchmarking on your data sources. *
-Techniques to **improve labeling accuracy**: Add support for automatic prompt
-improvement and tools for better error analysis to iteratively improve LLM
-performance on different tasks We will be releasing a more detailed roadmap
-soon, but we love suggestions and contributions from the community. Chat with
-the Refuel team and Autolabel community on [Discord](https://discord.gg/
-fweVnRx6CU) or open [Github issues](https://github.com/refuel-ai/autolabel/
-issues) to report bugs and request features. ## ð Contributing Autolabel is
-a rapidly developing project. We welcome contributions in all forms - bug
-reports, pull requests and ideas for improving the library. 1. Join the
-conversation on [Discord](https://discord.gg/fweVnRx6CU) 2. Open an [issue]
-(https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request
-features. 3. Grab an open issue, and submit a [pull request](https://
-github.com/refuel-ai/autolabel/blob/main/CONTRIBUTING.md).
+Access to Refuel hosted LLMs Refuel provides access to hosted open source LLMs
+for labeling, and for estimating confidence This is helpful, because you can
+calibrate a confidence threshold for your labeling task, and then route less
+confident labels to humans, while you still get the benefits of auto-labeling
+for the confident examples. In order to use Refuel hosted LLMs, you can
+[request access here](https://refuel-ai.typeform.com/llm-access). ## Benchmark
+Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-
+technical-report) to learn more about the performance of various LLMs, and
+human annoators, on label quality, turnaround time and cost. ## ð ï¸ Roadmap
+Our goal is to allow users to label, create or enrich any dataset, with any LLM
+- easily and quickly. There are four focus areas for Autolabel for 2023: *
+**Tasks**: Add support for tasks such as retrieval, attribute enrichment and
+text generation/writing. * **LLMs**: Add support for more LLMs, especially open
+source models like Falcon, MPT and Dolly and the ability to plug in your own
+LLMs. * Workflows for **experimenting with your datasets** more easily: Add
+support for richer data types (such as PDFs and HTML documents) and the ability
+to run benchmarking on your data sources. * Techniques to **improve labeling
+accuracy**: Add support for automatic prompt improvement and tools for better
+error analysis to iteratively improve LLM performance on different tasks We
+will be releasing a more detailed roadmap soon, but we love suggestions and
+contributions from the community. Chat with the Refuel team and Autolabel
+community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues]
+(https://github.com/refuel-ai/autolabel/issues) to report bugs and request
+features. ## ð Contributing Autolabel is a rapidly developing project. We
+welcome contributions in all forms - bug reports, pull requests and ideas for
+improving the library. 1. Join the conversation on [Discord](https://
+discord.gg/fweVnRx6CU) 2. Open an [issue](https://github.com/refuel-ai/
+autolabel/issues) on Github for bugs and request features. 3. Grab an open
+issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/
+main/CONTRIBUTING.md).
```

### Comparing `refuel-autolabel-0.0.2/README.md` & `refuel-autolabel-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-<picture>
-  <img alt="Refuel logo" src="docs/assets/Autolabel_blk_w_background.png">
-</picture>
+<img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
+
 <p align="center">
     <b>Clean, labeled data at the speed of thought</b>.
 </p>
 
 <h4 align="center">
   <a href="https://docs.refuel.ai/guide/overview/getting-started/">Getting started</a> |
   <a href="https://docs.refuel.ai/">Docs</a> |
@@ -148,14 +147,24 @@
 
 1. Label data for [NLP tasks](https://docs.refuel.ai/guide/tasks/classification_task/) such as classification, question-answering and named entity-recognition, entity matching and more.
 2. Use commercial or open source [LLMs](https://docs.refuel.ai/guide/llms/llms/) from providers such as OpenAI, Anthropic, HuggingFace, Google and more.
 3. Support for research-proven LLM techniques to boost label quality, such as few-shot learning and chain-of-thought prompting.
 4. [Confidence estimation](https://docs.refuel.ai/guide/accuracy/confidence/) and explanations out of the box for every single output label
 5. [Caching and state management](https://docs.refuel.ai/guide/reliability/state-management/) to minimize costs and experimentation time
 
+## Access to Refuel hosted LLMs
+
+Refuel provides access to hosted open source LLMs for labeling, and for estimating confidence This is helpful, because you can calibrate a confidence threshold for your labeling task, and then route less confident labels to humans, while you still get the benefits of auto-labeling for the confident examples.
+
+In order to use Refuel hosted LLMs, you can [request access here](https://refuel-ai.typeform.com/llm-access).
+
+## Benchmark
+
+Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-technical-report) to learn more about the performance of various LLMs, and human annoators, on label quality, turnaround time and cost.
+
 ## 🛠️ Roadmap
 Our goal is to allow users to label, create or enrich any dataset, with any LLM - easily and quickly.
 
 There are four focus areas for Autolabel for 2023:
 
 * **Tasks**: Add support for tasks such as retrieval, attribute enrichment and text generation/writing.
 * **LLMs**: Add support for more LLMs, especially open source models like Falcon, MPT and Dolly and the ability to plug in your own LLMs.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
- [Refuel logo]
+[Refuel logo]
                  Clean, labeled data at the speed of thought.
          *** Getting_started | Docs | Discord | Twitter | Website ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
@@ -69,28 +69,37 @@
 source [LLMs](https://docs.refuel.ai/guide/llms/llms/) from providers such as
 OpenAI, Anthropic, HuggingFace, Google and more. 3. Support for research-proven
 LLM techniques to boost label quality, such as few-shot learning and chain-of-
 thought prompting. 4. [Confidence estimation](https://docs.refuel.ai/guide/
 accuracy/confidence/) and explanations out of the box for every single output
 label 5. [Caching and state management](https://docs.refuel.ai/guide/
 reliability/state-management/) to minimize costs and experimentation time ##
-ð ï¸ Roadmap Our goal is to allow users to label, create or enrich any
-dataset, with any LLM - easily and quickly. There are four focus areas for
-Autolabel for 2023: * **Tasks**: Add support for tasks such as retrieval,
-attribute enrichment and text generation/writing. * **LLMs**: Add support for
-more LLMs, especially open source models like Falcon, MPT and Dolly and the
-ability to plug in your own LLMs. * Workflows for **experimenting with your
-datasets** more easily: Add support for richer data types (such as PDFs and
-HTML documents) and the ability to run benchmarking on your data sources. *
-Techniques to **improve labeling accuracy**: Add support for automatic prompt
-improvement and tools for better error analysis to iteratively improve LLM
-performance on different tasks We will be releasing a more detailed roadmap
-soon, but we love suggestions and contributions from the community. Chat with
-the Refuel team and Autolabel community on [Discord](https://discord.gg/
-fweVnRx6CU) or open [Github issues](https://github.com/refuel-ai/autolabel/
-issues) to report bugs and request features. ## ð Contributing Autolabel is
-a rapidly developing project. We welcome contributions in all forms - bug
-reports, pull requests and ideas for improving the library. 1. Join the
-conversation on [Discord](https://discord.gg/fweVnRx6CU) 2. Open an [issue]
-(https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request
-features. 3. Grab an open issue, and submit a [pull request](https://
-github.com/refuel-ai/autolabel/blob/main/CONTRIBUTING.md).
+Access to Refuel hosted LLMs Refuel provides access to hosted open source LLMs
+for labeling, and for estimating confidence This is helpful, because you can
+calibrate a confidence threshold for your labeling task, and then route less
+confident labels to humans, while you still get the benefits of auto-labeling
+for the confident examples. In order to use Refuel hosted LLMs, you can
+[request access here](https://refuel-ai.typeform.com/llm-access). ## Benchmark
+Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-
+technical-report) to learn more about the performance of various LLMs, and
+human annoators, on label quality, turnaround time and cost. ## ð ï¸ Roadmap
+Our goal is to allow users to label, create or enrich any dataset, with any LLM
+- easily and quickly. There are four focus areas for Autolabel for 2023: *
+**Tasks**: Add support for tasks such as retrieval, attribute enrichment and
+text generation/writing. * **LLMs**: Add support for more LLMs, especially open
+source models like Falcon, MPT and Dolly and the ability to plug in your own
+LLMs. * Workflows for **experimenting with your datasets** more easily: Add
+support for richer data types (such as PDFs and HTML documents) and the ability
+to run benchmarking on your data sources. * Techniques to **improve labeling
+accuracy**: Add support for automatic prompt improvement and tools for better
+error analysis to iteratively improve LLM performance on different tasks We
+will be releasing a more detailed roadmap soon, but we love suggestions and
+contributions from the community. Chat with the Refuel team and Autolabel
+community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues]
+(https://github.com/refuel-ai/autolabel/issues) to report bugs and request
+features. ## ð Contributing Autolabel is a rapidly developing project. We
+welcome contributions in all forms - bug reports, pull requests and ideas for
+improving the library. 1. Join the conversation on [Discord](https://
+discord.gg/fweVnRx6CU) 2. Open an [issue](https://github.com/refuel-ai/
+autolabel/issues) on Github for bugs and request features. 3. Grab an open
+issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/
+main/CONTRIBUTING.md).
```

### Comparing `refuel-autolabel-0.0.2/pyproject.toml` & `refuel-autolabel-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "refuel-autolabel"
-version = "0.0.2"
+version = "0.0.3"
 description = "Library for LLM powered labeling"
 readme = "README.md"
 authors = [{ name = "Refuel.ai", email = "support@refuel.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `refuel-autolabel-0.0.2/src/autolabel/cache/base.py` & `refuel-autolabel-0.0.3/src/autolabel/cache/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/cache/sqlalchemy_cache.py` & `refuel-autolabel-0.0.3/src/autolabel/cache/sqlalchemy_cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/confidence.py` & `refuel-autolabel-0.0.3/src/autolabel/confidence.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/configs/base.py` & `refuel-autolabel-0.0.3/src/autolabel/configs/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/configs/config.py` & `refuel-autolabel-0.0.3/src/autolabel/configs/config.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/data_models/annotation.py` & `refuel-autolabel-0.0.3/src/autolabel/data_models/annotation.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/data_models/cache.py` & `refuel-autolabel-0.0.3/src/autolabel/data_models/cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/data_models/dataset.py` & `refuel-autolabel-0.0.3/src/autolabel/data_models/dataset.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/data_models/task.py` & `refuel-autolabel-0.0.3/src/autolabel/data_models/task.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/data_models/task_run.py` & `refuel-autolabel-0.0.3/src/autolabel/data_models/task_run.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/database/state_manager.py` & `refuel-autolabel-0.0.3/src/autolabel/database/state_manager.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/dataset_loader.py` & `refuel-autolabel-0.0.3/src/autolabel/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/few_shot/__init__.py` & `refuel-autolabel-0.0.3/src/autolabel/few_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/few_shot/fixed_example_selector.py` & `refuel-autolabel-0.0.3/src/autolabel/few_shot/fixed_example_selector.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/few_shot/vector_store.py` & `refuel-autolabel-0.0.3/src/autolabel/few_shot/vector_store.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/labeler.py` & `refuel-autolabel-0.0.3/src/autolabel/labeler.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/models/__init__.py` & `refuel-autolabel-0.0.3/src/autolabel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/models/anthropic.py` & `refuel-autolabel-0.0.3/src/autolabel/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/models/base.py` & `refuel-autolabel-0.0.3/src/autolabel/models/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/models/hf_pipeline.py` & `refuel-autolabel-0.0.3/src/autolabel/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/models/openai.py` & `refuel-autolabel-0.0.3/src/autolabel/models/openai.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/models/palm.py` & `refuel-autolabel-0.0.3/src/autolabel/models/palm.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/models/refuel.py` & `refuel-autolabel-0.0.3/src/autolabel/models/refuel.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/schema.py` & `refuel-autolabel-0.0.3/src/autolabel/schema.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/tasks/__init__.py` & `refuel-autolabel-0.0.3/src/autolabel/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/tasks/base.py` & `refuel-autolabel-0.0.3/src/autolabel/tasks/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/tasks/classification.py` & `refuel-autolabel-0.0.3/src/autolabel/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/tasks/entity_matching.py` & `refuel-autolabel-0.0.3/src/autolabel/tasks/entity_matching.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/tasks/named_entity_recognition.py` & `refuel-autolabel-0.0.3/src/autolabel/tasks/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/tasks/question_answering.py` & `refuel-autolabel-0.0.3/src/autolabel/tasks/question_answering.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/tasks/utils.py` & `refuel-autolabel-0.0.3/src/autolabel/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/autolabel/utils.py` & `refuel-autolabel-0.0.3/src/autolabel/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/PKG-INFO` & `refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for LLM powered labeling
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,17 +38,16 @@
 Provides-Extra: openai
 Provides-Extra: anthropic
 Provides-Extra: huggingface
 Provides-Extra: google
 Provides-Extra: all
 License-File: LICENSE
 
-<picture>
-  <img alt="Refuel logo" src="docs/assets/Autolabel_blk_w_background.png">
-</picture>
+<img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
+
 <p align="center">
     <b>Clean, labeled data at the speed of thought</b>.
 </p>
 
 <h4 align="center">
   <a href="https://docs.refuel.ai/guide/overview/getting-started/">Getting started</a> |
   <a href="https://docs.refuel.ai/">Docs</a> |
@@ -192,14 +191,24 @@
 
 1. Label data for [NLP tasks](https://docs.refuel.ai/guide/tasks/classification_task/) such as classification, question-answering and named entity-recognition, entity matching and more.
 2. Use commercial or open source [LLMs](https://docs.refuel.ai/guide/llms/llms/) from providers such as OpenAI, Anthropic, HuggingFace, Google and more.
 3. Support for research-proven LLM techniques to boost label quality, such as few-shot learning and chain-of-thought prompting.
 4. [Confidence estimation](https://docs.refuel.ai/guide/accuracy/confidence/) and explanations out of the box for every single output label
 5. [Caching and state management](https://docs.refuel.ai/guide/reliability/state-management/) to minimize costs and experimentation time
 
+## Access to Refuel hosted LLMs
+
+Refuel provides access to hosted open source LLMs for labeling, and for estimating confidence This is helpful, because you can calibrate a confidence threshold for your labeling task, and then route less confident labels to humans, while you still get the benefits of auto-labeling for the confident examples.
+
+In order to use Refuel hosted LLMs, you can [request access here](https://refuel-ai.typeform.com/llm-access).
+
+## Benchmark
+
+Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-technical-report) to learn more about the performance of various LLMs, and human annoators, on label quality, turnaround time and cost.
+
 ## 🛠️ Roadmap
 Our goal is to allow users to label, create or enrich any dataset, with any LLM - easily and quickly.
 
 There are four focus areas for Autolabel for 2023:
 
 * **Tasks**: Add support for tasks such as retrieval, attribute enrichment and text generation/writing.
 * **LLMs**: Add support for more LLMs, especially open source models like Falcon, MPT and Dolly and the ability to plug in your own LLMs.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.2 Summary: Library
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.3 Summary: Library
 for LLM powered labeling Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -18,15 +18,15 @@
 autolabel Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
 Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
-File: LICENSE  [Refuel logo]
+File: LICENSE [Refuel logo]
                  Clean, labeled data at the speed of thought.
          *** Getting_started | Docs | Discord | Twitter | Website ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
@@ -93,28 +93,37 @@
 source [LLMs](https://docs.refuel.ai/guide/llms/llms/) from providers such as
 OpenAI, Anthropic, HuggingFace, Google and more. 3. Support for research-proven
 LLM techniques to boost label quality, such as few-shot learning and chain-of-
 thought prompting. 4. [Confidence estimation](https://docs.refuel.ai/guide/
 accuracy/confidence/) and explanations out of the box for every single output
 label 5. [Caching and state management](https://docs.refuel.ai/guide/
 reliability/state-management/) to minimize costs and experimentation time ##
-ð ï¸ Roadmap Our goal is to allow users to label, create or enrich any
-dataset, with any LLM - easily and quickly. There are four focus areas for
-Autolabel for 2023: * **Tasks**: Add support for tasks such as retrieval,
-attribute enrichment and text generation/writing. * **LLMs**: Add support for
-more LLMs, especially open source models like Falcon, MPT and Dolly and the
-ability to plug in your own LLMs. * Workflows for **experimenting with your
-datasets** more easily: Add support for richer data types (such as PDFs and
-HTML documents) and the ability to run benchmarking on your data sources. *
-Techniques to **improve labeling accuracy**: Add support for automatic prompt
-improvement and tools for better error analysis to iteratively improve LLM
-performance on different tasks We will be releasing a more detailed roadmap
-soon, but we love suggestions and contributions from the community. Chat with
-the Refuel team and Autolabel community on [Discord](https://discord.gg/
-fweVnRx6CU) or open [Github issues](https://github.com/refuel-ai/autolabel/
-issues) to report bugs and request features. ## ð Contributing Autolabel is
-a rapidly developing project. We welcome contributions in all forms - bug
-reports, pull requests and ideas for improving the library. 1. Join the
-conversation on [Discord](https://discord.gg/fweVnRx6CU) 2. Open an [issue]
-(https://github.com/refuel-ai/autolabel/issues) on Github for bugs and request
-features. 3. Grab an open issue, and submit a [pull request](https://
-github.com/refuel-ai/autolabel/blob/main/CONTRIBUTING.md).
+Access to Refuel hosted LLMs Refuel provides access to hosted open source LLMs
+for labeling, and for estimating confidence This is helpful, because you can
+calibrate a confidence threshold for your labeling task, and then route less
+confident labels to humans, while you still get the benefits of auto-labeling
+for the confident examples. In order to use Refuel hosted LLMs, you can
+[request access here](https://refuel-ai.typeform.com/llm-access). ## Benchmark
+Check out our [technical report](https://www.refuel.ai/blog-posts/llm-labeling-
+technical-report) to learn more about the performance of various LLMs, and
+human annoators, on label quality, turnaround time and cost. ## ð ï¸ Roadmap
+Our goal is to allow users to label, create or enrich any dataset, with any LLM
+- easily and quickly. There are four focus areas for Autolabel for 2023: *
+**Tasks**: Add support for tasks such as retrieval, attribute enrichment and
+text generation/writing. * **LLMs**: Add support for more LLMs, especially open
+source models like Falcon, MPT and Dolly and the ability to plug in your own
+LLMs. * Workflows for **experimenting with your datasets** more easily: Add
+support for richer data types (such as PDFs and HTML documents) and the ability
+to run benchmarking on your data sources. * Techniques to **improve labeling
+accuracy**: Add support for automatic prompt improvement and tools for better
+error analysis to iteratively improve LLM performance on different tasks We
+will be releasing a more detailed roadmap soon, but we love suggestions and
+contributions from the community. Chat with the Refuel team and Autolabel
+community on [Discord](https://discord.gg/fweVnRx6CU) or open [Github issues]
+(https://github.com/refuel-ai/autolabel/issues) to report bugs and request
+features. ## ð Contributing Autolabel is a rapidly developing project. We
+welcome contributions in all forms - bug reports, pull requests and ideas for
+improving the library. 1. Join the conversation on [Discord](https://
+discord.gg/fweVnRx6CU) 2. Open an [issue](https://github.com/refuel-ai/
+autolabel/issues) on Github for bugs and request features. 3. Grab an open
+issue, and submit a [pull request](https://github.com/refuel-ai/autolabel/blob/
+main/CONTRIBUTING.md).
```

### Comparing `refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/SOURCES.txt` & `refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.2/src/refuel_autolabel.egg-info/requires.txt` & `refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/requires.txt`

 * *Files identical despite different names*

