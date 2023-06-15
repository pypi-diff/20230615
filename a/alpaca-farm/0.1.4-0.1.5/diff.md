# Comparing `tmp/alpaca_farm-0.1.4.tar.gz` & `tmp/alpaca_farm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_farm-0.1.4.tar", last modified: Mon Jun 12 23:54:25 2023, max compression
+gzip compressed data, was "alpaca_farm-0.1.5.tar", last modified: Thu Jun 15 04:33:44 2023, max compression
```

## Comparing `alpaca_farm-0.1.4.tar` & `alpaca_farm-0.1.5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.426278 alpaca_farm-0.1.4/
--rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.4/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.4/MANIFEST.in
--rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-12 23:54:25.426096 alpaca_farm-0.1.4/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)    16695 2023-06-12 23:53:35.000000 alpaca_farm-0.1.4/README.md
--rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-12 23:54:25.426314 alpaca_farm-0.1.4/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)     2524 2023-06-11 20:30:56.000000 alpaca_farm-0.1.4/setup.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.405768 alpaca_farm-0.1.4/src/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.411159 alpaca_farm-0.1.4/src/alpaca_farm/
--rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-12 23:53:35.000000 alpaca_farm-0.1.4/src/alpaca_farm/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/accelerate_patch.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.413518 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/
--rw-r--r--   0 xuechenli   (501) staff       (20)      635 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1894 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/analysis.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.406126 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.421022 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6969 2023-06-11 02:31:44.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.421504 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      481 2023-06-11 02:31:44.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.421777 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/test/
--rw-r--r--   0 xuechenli   (501) staff       (20)      426 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     4951 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/decoders.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4763 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/eval.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    28834 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/pairwise_annotators.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11404 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-12 18:21:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/common.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/constants.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1565 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/data_postprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    21184 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/data_preprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4527 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/data_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/distributed_utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.422832 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/apex_patch.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/tensor_ops.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.423385 alpaca_farm-0.1.4/src/alpaca_farm/inference/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/inference/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.4/src/alpaca_farm/inference/decode.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/inference/score.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/logging.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.424015 alpaca_farm-0.1.4/src/alpaca_farm/models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.4/src/alpaca_farm/models/reward_model.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/models/rl_models.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11542 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/openai_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/reward_modeling_trainer.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.425280 alpaca_farm-0.1.4/src/alpaca_farm/rl/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/kl_controller.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    22890 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/quark_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7932 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/quark_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13749 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/rl_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/trainer_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/types.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     6767 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.411897 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     4356 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      295 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/top_level.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.425848 alpaca_farm-0.1.4/tests/
--rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/tests/test_flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/tests/test_flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/tests/test_torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      581 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/tests/test_utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.005156 alpaca_farm-0.1.5/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.5/LICENSE
+-rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.5/MANIFEST.in
+-rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-15 04:33:44.004931 alpaca_farm-0.1.5/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16695 2023-06-12 23:53:35.000000 alpaca_farm-0.1.5/README.md
+-rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-15 04:33:44.005191 alpaca_farm-0.1.5/setup.cfg
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2524 2023-06-11 20:30:56.000000 alpaca_farm-0.1.5/setup.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.987712 alpaca_farm-0.1.5/src/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.992692 alpaca_farm-0.1.5/src/alpaca_farm/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-15 04:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/accelerate_patch.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.994807 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      672 2023-06-15 04:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1894 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/analysis.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.988075 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.999859 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6969 2023-06-11 02:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.000369 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      481 2023-06-11 02:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.000668 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/test/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      426 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4951 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/decoders.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4692 2023-06-15 04:31:44.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/eval.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    28861 2023-06-13 06:34:11.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/pairwise_annotators.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11404 2023-06-15 04:30:13.000000 alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-12 18:21:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/common.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/constants.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1565 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/data_postprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21184 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/data_preprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4527 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/data_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/distributed_utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.001488 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/apex_patch.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/flash_models/tensor_ops.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.002061 alpaca_farm-0.1.5/src/alpaca_farm/inference/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/inference/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.5/src/alpaca_farm/inference/decode.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/inference/score.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/logging.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.002637 alpaca_farm-0.1.5/src/alpaca_farm/models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.5/src/alpaca_farm/models/reward_model.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/models/rl_models.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11542 2023-06-11 22:43:54.000000 alpaca_farm-0.1.5/src/alpaca_farm/openai_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/reward_modeling_trainer.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.003999 alpaca_farm-0.1.5/src/alpaca_farm/rl/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/kl_controller.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    22890 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7932 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13749 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/rl/rl_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/torch_ops.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/src/alpaca_farm/trainer_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-06-11 22:43:54.000000 alpaca_farm-0.1.5/src/alpaca_farm/types.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6767 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/src/alpaca_farm/utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:43.993331 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4356 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/SOURCES.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/dependency_links.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      295 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/requires.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-15 04:33:43.000000 alpaca_farm-0.1.5/src/alpaca_farm.egg-info/top_level.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-15 04:33:44.004732 alpaca_farm-0.1.5/tests/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/tests/test_flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/tests/test_flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.5/tests/test_torch_ops.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      581 2023-06-12 23:52:33.000000 alpaca_farm-0.1.5/tests/test_utils.py
```

### Comparing `alpaca_farm-0.1.4/LICENSE` & `alpaca_farm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/PKG-INFO` & `alpaca_farm-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_farm
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `alpaca_farm-0.1.4/README.md` & `alpaca_farm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/setup.py` & `alpaca_farm-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/__init__.py` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.4"
+from .eval import alpaca_leaderboard
+from .pairwise_annotators import PairwiseAutoAnnotator
```

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/accelerate_patch.py` & `alpaca_farm-0.1.5/src/alpaca_farm/accelerate_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/__init__.py` & `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from .eval import *
-from .pairwise_annotators import *
```

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/analysis.py` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/analysis.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/decoders.py` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/decoders.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/eval.py` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import json
 import logging
 from typing import Union
 
 import datasets
 import pandas as pd
 
-from alpaca_farm import constants
-from alpaca_farm.auto_annotations import PairwiseAutoAnnotator
-from alpaca_farm.auto_annotations.analysis import head2head_to_metrics
-
+from .. import constants
+from . import analysis, pairwise_annotators
 from . import utils as ann_utils
 
 __all__ = ["alpaca_leaderboard"]
 
 PRECOMPUTED_LEADERBOARD = {
     "annotators/annotator_pool_v0/configs.yaml": {
         # Internal codename: rlhf_llama_7b_regen_v7_3ep_v12_ckpt_20
@@ -129,17 +127,17 @@
 
     if len(all_outputs) != 805:
         logging.warning(
             f"""You gave {len(all_outputs)} outputs, but there are 805 examples in Alpaca Eval.
         We are computing the metrics on all examples you gave."""
         )
 
-    annotator = PairwiseAutoAnnotator(annotators_config=annotators_config, **kwargs)
+    annotator = pairwise_annotators.PairwiseAutoAnnotator(annotators_config=annotators_config, **kwargs)
     annotated = annotator.annotate_head2head(outputs_1=outputs_baseline, outputs_2=all_outputs)
-    all_metrics[name] = head2head_to_metrics(preferences=[a["preference"] for a in annotated])
+    all_metrics[name] = analysis.head2head_to_metrics(preferences=[a["preference"] for a in annotated])
 
     df_results = pd.DataFrame(all_metrics).T.sort_values(by="win_rate", ascending=False)
 
     if is_print_metrics:
         print(df_results.to_string(float_format="%.2f"))
     else:
         return df_results
```

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/pairwise_annotators.py` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/pairwise_annotators.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
 import logging
 import os
 import re
 from pathlib import Path
 from typing import Any, Callable, Optional, Sequence, Union
 
 import datasets
@@ -393,15 +394,15 @@
         return {
             name: SinglePairwiseAutoAnnotator(**annotator_config)
             for name, annotator_config in annotators_config.items()
         }
 
     def _annotate(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
         """Annotate the examples."""
-        curr_decoding_kwargs = self.decoding_kwargs
+        curr_decoding_kwargs = copy.deepcopy(self.decoding_kwargs)
         curr_decoding_kwargs.update(decoding_kwargs)
 
         df_annotated = df_to_annotate
         for annotator in self.annotators.keys():
             # only annotate examples that have not been annotated yet
             curr_idcs = (df_annotated["annotator"] == annotator) & df_annotated["preference"].isna()
```

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/auto_annotations/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/common.py` & `alpaca_farm-0.1.5/src/alpaca_farm/common.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/constants.py` & `alpaca_farm-0.1.5/src/alpaca_farm/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/data_postprocessor.py` & `alpaca_farm-0.1.5/src/alpaca_farm/data_postprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/data_preprocessor.py` & `alpaca_farm-0.1.5/src/alpaca_farm/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/data_utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/distributed_utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/__init__.py` & `alpaca_farm-0.1.5/src/alpaca_farm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/apex_patch.py` & `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/apex_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_llama.py` & `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_opt.py` & `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/tensor_ops.py` & `alpaca_farm-0.1.5/src/alpaca_farm/flash_models/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/inference/__init__.py` & `alpaca_farm-0.1.5/src/alpaca_farm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/inference/decode.py` & `alpaca_farm-0.1.5/src/alpaca_farm/inference/decode.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/inference/score.py` & `alpaca_farm-0.1.5/src/alpaca_farm/inference/score.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/logging.py` & `alpaca_farm-0.1.5/src/alpaca_farm/logging.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/models/__init__.py` & `alpaca_farm-0.1.5/src/alpaca_farm/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/models/reward_model.py` & `alpaca_farm-0.1.5/src/alpaca_farm/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/models/rl_models.py` & `alpaca_farm-0.1.5/src/alpaca_farm/models/rl_models.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/openai_utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/openai_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/reward_modeling_trainer.py` & `alpaca_farm-0.1.5/src/alpaca_farm/reward_modeling_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/rl/__init__.py` & `alpaca_farm-0.1.5/src/alpaca_farm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = "0.1.5"
```

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/rl/kl_controller.py` & `alpaca_farm-0.1.5/src/alpaca_farm/rl/kl_controller.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_trainer.py` & `alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/rl/ppo_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/rl/quark_trainer.py` & `alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/rl/quark_utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/rl/quark_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/rl/rl_trainer.py` & `alpaca_farm-0.1.5/src/alpaca_farm/rl/rl_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/torch_ops.py` & `alpaca_farm-0.1.5/src/alpaca_farm/torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/trainer_utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/types.py` & `alpaca_farm-0.1.5/src/alpaca_farm/types.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm/utils.py` & `alpaca_farm-0.1.5/src/alpaca_farm/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm.egg-info/PKG-INFO` & `alpaca_farm-0.1.5/src/alpaca_farm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-farm
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `alpaca_farm-0.1.4/src/alpaca_farm.egg-info/SOURCES.txt` & `alpaca_farm-0.1.5/src/alpaca_farm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/tests/test_flash_llama.py` & `alpaca_farm-0.1.5/tests/test_flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/tests/test_flash_opt.py` & `alpaca_farm-0.1.5/tests/test_flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/tests/test_torch_ops.py` & `alpaca_farm-0.1.5/tests/test_torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.4/tests/test_utils.py` & `alpaca_farm-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*

