# Comparing `tmp/jury-2.2.3.tar.gz` & `tmp/jury-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jury-2.2.3.tar", last modified: Mon Dec 26 14:31:08 2022, max compression
+gzip compressed data, was "jury-2.2.4.tar", last modified: Thu Jun 15 09:25:06 2023, max compression
```

## Comparing `jury-2.2.3.tar` & `jury-2.2.4.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.812338 jury-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2022-12-26 14:30:58.000000 jury-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14475 2022-12-26 14:31:08.812338 jury-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13378 2022-12-26 14:30:58.000000 jury-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-12-26 14:30:58.000000 jury-2.2.3/jury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3178 2022-12-26 14:30:58.000000 jury-2.2.3/jury/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2227 2022-12-26 14:30:58.000000 jury-2.2.3/jury/collator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8247 2022-12-26 14:30:58.000000 jury-2.2.3/jury/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      301 2022-12-26 14:30:58.000000 jury-2.2.3/jury/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/_core/
--rw-r--r--   0 runner    (1001) docker     (122)      538 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5761 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/_core/auto.py
--rw-r--r--   0 runner    (1001) docker     (122)     4140 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/_core/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (122)    23361 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/_core/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2279 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/accuracy/
--rw-r--r--   0 runner    (1001) docker     (122)       52 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/accuracy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/accuracy/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)     5524 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/accuracy/accuracy_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4642 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/accuracy/accuracy_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/bartscore/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bartscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bartscore/bartscore.py
--rw-r--r--   0 runner    (1001) docker     (122)    11740 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bartscore/bartscore_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/bertscore/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bertscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bertscore/bertscore.py
--rw-r--r--   0 runner    (1001) docker     (122)    12887 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bertscore/bertscore_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/bleu/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bleu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bleu/bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)    12432 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bleu/bleu_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/bleurt/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bleurt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bleurt/bleurt.py
--rw-r--r--   0 runner    (1001) docker     (122)     8609 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/bleurt/bleurt_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/cer/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/cer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/cer/cer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9839 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/cer/cer_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/chrf/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/chrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      222 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/chrf/chrf.py
--rw-r--r--   0 runner    (1001) docker     (122)    10872 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/chrf/chrf_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury/metrics/comet/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/comet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/comet/comet.py
--rw-r--r--   0 runner    (1001) docker     (122)     8907 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/comet/comet_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/f1/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/f1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      373 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/f1/f1.py
--rw-r--r--   0 runner    (1001) docker     (122)     5341 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/f1/f1_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6925 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/f1/f1_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/meteor/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/meteor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/meteor/meteor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6973 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/meteor/meteor_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/precision/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     5218 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/precision/precision_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7072 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/precision/precision_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/prism/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      228 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/prism/prism.py
--rw-r--r--   0 runner    (1001) docker     (122)    12281 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/prism/prism_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/recall/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/recall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/recall/recall.py
--rw-r--r--   0 runner    (1001) docker     (122)     5393 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/recall/recall_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6692 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/recall/recall_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/rouge/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/rouge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      228 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/rouge/rouge.py
--rw-r--r--   0 runner    (1001) docker     (122)    10228 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/rouge/rouge_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/sacrebleu/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/sacrebleu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/sacrebleu/sacrebleu.py
--rw-r--r--   0 runner    (1001) docker     (122)    11101 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/seqeval/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/seqeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/seqeval/seqeval.py
--rw-r--r--   0 runner    (1001) docker     (122)     8399 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/seqeval/seqeval_for_sequence_labeling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/squad/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/squad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      228 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/squad/squad.py
--rw-r--r--   0 runner    (1001) docker     (122)     7688 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/squad/squad_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/ter/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/ter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/ter/ter.py
--rw-r--r--   0 runner    (1001) docker     (122)     9679 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/ter/ter_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/metrics/wer/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/wer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/wer/wer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9927 2022-12-26 14:30:58.000000 jury-2.2.3/jury/metrics/wer/wer_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2022-12-26 14:30:58.000000 jury-2.2.3/jury/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/jury/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-26 14:30:58.000000 jury-2.2.3/jury/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2022-12-26 14:30:58.000000 jury-2.2.3/jury/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2022-12-26 14:30:58.000000 jury-2.2.3/jury/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2022-12-26 14:30:58.000000 jury-2.2.3/jury/utils/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.804338 jury-2.2.3/jury.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14475 2022-12-26 14:31:08.000000 jury-2.2.3/jury.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2022-12-26 14:31:08.000000 jury-2.2.3/jury.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-26 14:31:08.000000 jury-2.2.3/jury.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-26 14:31:08.000000 jury-2.2.3/jury.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      832 2022-12-26 14:31:08.000000 jury-2.2.3/jury.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-12-26 14:31:08.000000 jury-2.2.3/jury.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-12-26 14:30:58.000000 jury-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      193 2022-12-26 14:31:08.812338 jury-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3098 2022-12-26 14:30:58.000000 jury-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.800338 jury-2.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.808338 jury-2.2.3/tests/jury/
--rw-r--r--   0 runner    (1001) docker     (122)      235 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4939 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-26 14:31:08.812338 jury-2.2.3/tests/jury/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6018 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1871 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_bartscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_bertscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_bleurt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_cer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_chrf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_comet.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_custom_bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     4066 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_f1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_meteor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4178 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     3037 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_prism.py
--rw-r--r--   0 runner    (1001) docker     (122)     4130 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)     1441 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_rouge.py
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_sacrebleu.py
--rw-r--r--   0 runner    (1001) docker     (122)      875 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_seqeval.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_squad.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_ter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/metrics/test_wer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)       64 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)     6208 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/test_jury.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2022-12-26 14:30:58.000000 jury-2.2.3/tests/jury/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.621108 jury-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-06-15 09:24:55.000000 jury-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    14491 2023-06-15 09:25:06.621108 jury-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13394 2023-06-15 09:24:55.000000 jury-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-15 09:24:55.000000 jury-2.2.4/jury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3178 2023-06-15 09:24:55.000000 jury-2.2.4/jury/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2227 2023-06-15 09:24:55.000000 jury-2.2.4/jury/collator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8247 2023-06-15 09:24:55.000000 jury-2.2.4/jury/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-06-15 09:24:55.000000 jury-2.2.4/jury/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury/metrics/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/_core/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/_core/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23361 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2279 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury/metrics/accuracy/
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/accuracy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/accuracy/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5592 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/accuracy/accuracy_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/accuracy/accuracy_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury/metrics/bartscore/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bartscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bartscore/bartscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11740 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bartscore/bartscore_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury/metrics/bertscore/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bertscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bertscore/bertscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12887 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bertscore/bertscore_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury/metrics/bleu/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bleu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bleu/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12432 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bleu/bleu_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/bleurt/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bleurt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bleurt/bleurt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8609 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/bleurt/bleurt_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/cer/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/cer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/cer/cer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9839 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/cer/cer_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/chrf/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/chrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/chrf/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10872 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/chrf/chrf_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/comet/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/comet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/comet/comet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/comet/comet_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/f1/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/f1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/f1/f1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5341 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/f1/f1_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6925 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/f1/f1_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/meteor/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/meteor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/meteor/meteor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6973 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/meteor/meteor_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/precision/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5218 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/precision/precision_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7072 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/precision/precision_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.613108 jury-2.2.4/jury/metrics/prism/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/prism/prism.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12281 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/prism/prism_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/metrics/recall/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/recall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/recall/recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/recall/recall_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6692 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/recall/recall_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/metrics/rouge/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/rouge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/rouge/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10228 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/rouge/rouge_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/metrics/sacrebleu/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/sacrebleu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/sacrebleu/sacrebleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11101 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/metrics/seqeval/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/seqeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/seqeval/seqeval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/seqeval/seqeval_for_sequence_labeling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/metrics/squad/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/squad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/squad/squad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7688 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/squad/squad_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/metrics/ter/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/ter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/ter/ter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9679 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/ter/ter_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/metrics/wer/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/wer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/wer/wer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9927 2023-06-15 09:24:55.000000 jury-2.2.4/jury/metrics/wer/wer_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-06-15 09:24:55.000000 jury-2.2.4/jury/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/jury/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 09:24:55.000000 jury-2.2.4/jury/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-06-15 09:24:55.000000 jury-2.2.4/jury/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-15 09:24:55.000000 jury-2.2.4/jury/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-15 09:24:55.000000 jury-2.2.4/jury/utils/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.609108 jury-2.2.4/jury.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14491 2023-06-15 09:25:06.000000 jury-2.2.4/jury.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-06-15 09:25:06.000000 jury-2.2.4/jury.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 09:25:06.000000 jury-2.2.4/jury.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 09:25:06.000000 jury-2.2.4/jury.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-15 09:25:06.000000 jury-2.2.4/jury.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-15 09:25:06.000000 jury-2.2.4/jury.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-15 09:24:55.000000 jury-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-15 09:25:06.625109 jury-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-15 09:24:55.000000 jury-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.605108 jury-2.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.617108 jury-2.2.4/tests/jury/
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:25:06.621108 jury-2.2.4/tests/jury/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1871 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_bartscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_bertscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_bleurt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_cer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_chrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_comet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_custom_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4066 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_f1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_meteor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4178 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_prism.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_rouge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_sacrebleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_seqeval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_squad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_ter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/metrics/test_wer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6208 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/test_jury.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-15 09:24:55.000000 jury-2.2.4/tests/jury/test_utils.py
```

### Comparing `jury-2.2.3/LICENSE` & `jury-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/PKG-INFO` & `jury-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jury
-Version: 2.2.3
+Version: 2.2.4
 Summary: Evaluation toolkit for neural language generation.
 Home-page: https://github.com/obss/jury
 Author: 
 License: MIT
 Keywords: machine-learning,deep-learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 <h1 align="center">Jury</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/pyversions/jury" alt="Python versions"></a>
 <a href="https://pepy.tech/project/jury"><img src="https://pepy.tech/badge/jury" alt="downloads"></a>
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/v/jury?color=blue" alt="PyPI version"></a>
 <a href="https://github.com/obss/jury/releases/latest"><img alt="Latest Release" src="https://img.shields.io/github/release-date/obss/jury"></a>
-<a href="https://colab.research.google.com/github/obss/jury/blob/main/examples/jury_evaluate.ipynb"><img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
+<a href="https://colab.research.google.com/github/obss/jury/blob/main/examples/jury_evaluate.ipynb" target="_blank"><img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <br>
 <a href="https://github.com/obss/jury/actions"><img alt="Build status" src="https://github.com/obss/jury/actions/workflows/ci.yml/badge.svg"></a>
 <a href="https://libraries.io/pypi/jury"><img alt="Dependencies" src="https://img.shields.io/librariesio/github/obss/jury"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://github.com/obss/jury/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/pypi/l/jury"></a>
 <br>
 <a href="https://doi.org/10.5281/zenodo.6109838"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.6109838.svg" alt="DOI"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jury Version: 2.2.3 Summary: Evaluation toolkit for
+Metadata-Version: 2.1 Name: jury Version: 2.2.4 Summary: Evaluation toolkit for
 neural language generation. Home-page: https://github.com/obss/jury Author:
 License: MIT Keywords: machine-learning,deep-
 learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jury-2.2.3/README.md` & `jury-2.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <h1 align="center">Jury</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/pyversions/jury" alt="Python versions"></a>
 <a href="https://pepy.tech/project/jury"><img src="https://pepy.tech/badge/jury" alt="downloads"></a>
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/v/jury?color=blue" alt="PyPI version"></a>
 <a href="https://github.com/obss/jury/releases/latest"><img alt="Latest Release" src="https://img.shields.io/github/release-date/obss/jury"></a>
-<a href="https://colab.research.google.com/github/obss/jury/blob/main/examples/jury_evaluate.ipynb"><img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
+<a href="https://colab.research.google.com/github/obss/jury/blob/main/examples/jury_evaluate.ipynb" target="_blank"><img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <br>
 <a href="https://github.com/obss/jury/actions"><img alt="Build status" src="https://github.com/obss/jury/actions/workflows/ci.yml/badge.svg"></a>
 <a href="https://libraries.io/pypi/jury"><img alt="Dependencies" src="https://img.shields.io/librariesio/github/obss/jury"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://github.com/obss/jury/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/pypi/l/jury"></a>
 <br>
 <a href="https://doi.org/10.5281/zenodo.6109838"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.6109838.svg" alt="DOI"></a>
```

### Comparing `jury-2.2.3/jury/cli.py` & `jury-2.2.4/jury/cli.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/collator.py` & `jury-2.2.4/jury/collator.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/core.py` & `jury-2.2.4/jury/core.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/__init__.py` & `jury-2.2.4/jury/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/_core/__init__.py` & `jury-2.2.4/jury/metrics/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/_core/auto.py` & `jury-2.2.4/jury/metrics/_core/auto.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/_core/auxiliary.py` & `jury-2.2.4/jury/metrics/_core/auxiliary.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/_core/base.py` & `jury-2.2.4/jury/metrics/_core/base.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/_core/utils.py` & `jury-2.2.4/jury/metrics/_core/utils.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/accuracy/accuracy_for_language_generation.py` & `jury-2.2.4/jury/metrics/accuracy/accuracy_for_language_generation.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 """
 
 from collections import Counter
 from typing import Callable
 
 import evaluate
 import numpy as np
+from evaluate.utils.logging import get_logger
 
 from jury.collator import Collator
 from jury.metrics._core import MetricForLanguageGeneration
 from jury.utils.nlp import normalize_text
 
+logger = get_logger(__name__)
+
 _CITATION = """\
 @article{scikit-learn,
   title={Scikit-learn: Machine Learning in {P}ython},
   author={Pedregosa, F. and Varoquaux, G. and Gramfort, A. and Michel, V.
          and Thirion, B. and Grisel, O. and Blondel, M. and Prettenhofer, P.
          and Weiss, R. and Dubourg, V. and Vanderplas, J. and Passos, A. and
          Cournapeau, D. and Brucher, M. and Perrot, M. and Duchesnay, E.},
@@ -62,15 +65,15 @@
 Returns:
     'score': Accuracy score.
 Examples:
 
     >>> accuracy = jury.load_metric("accuracy")
     >>> predictions = [["the cat is on the mat", "There is cat playing on the mat"], ["Look! a wonderful day."]]
     >>> references = [
-        ["the cat is playing on the mat.", "The cat plays on the mat."], 
+        ["the cat is playing on the mat.", "The cat plays on the mat."],
         ["Today is a wonderful day", "The weather outside is wonderful."]
     ]
     >>> results = accuracy.compute(predictions=predictions, references=references)
     >>> print(results)
     {'accuracy': {'score': 0.7285714285714285}}
 """
 
@@ -94,21 +97,21 @@
 
     def _compute_single_pred_single_ref(
         self, predictions: Collator, references: Collator, reduce_fn: Callable = None, **kwargs
     ):
         scores = []
         predictions, references = self._tokenize(predictions, references)
         for pred, ref in zip(predictions, references):
-            score = 0
-            pred_counts = Counter(pred)
-            ref_counts = Counter(ref)
-            for token, pred_count in pred_counts.items():
-                if token in ref_counts:
-                    score += min(pred_count, ref_counts[token])  # Intersection count
-            scores.append(score / max(len(pred), len(ref)))
+            common = Counter(pred) & Counter(ref)  # Intersection count
+            score = sum(common.values())
+            try:
+                scores.append(score / max(len(pred), len(ref)))
+            except ZeroDivisionError:
+                logger.warning("Empty pred & ref after preprocess (`normalize_text`) step. Ignoring!")
+
         avg_score = sum(scores) / len(scores)
         return {"score": avg_score}
 
     def _compute_single_pred_multi_ref(
         self, predictions: Collator, references: Collator, reduce_fn: Callable = None, **kwargs
     ):
         scores = []
```

### Comparing `jury-2.2.3/jury/metrics/accuracy/accuracy_for_sequence_classification.py` & `jury-2.2.4/jury/metrics/accuracy/accuracy_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/bartscore/bartscore_for_language_generation.py` & `jury-2.2.4/jury/metrics/bartscore/bartscore_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/bertscore/bertscore_for_language_generation.py` & `jury-2.2.4/jury/metrics/bertscore/bertscore_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/bleu/bleu.py` & `jury-2.2.4/jury/metrics/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/bleu/bleu_for_language_generation.py` & `jury-2.2.4/jury/metrics/bleu/bleu_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/bleurt/bleurt_for_language_generation.py` & `jury-2.2.4/jury/metrics/bleurt/bleurt_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/cer/cer_for_language_generation.py` & `jury-2.2.4/jury/metrics/cer/cer_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/chrf/chrf_for_language_generation.py` & `jury-2.2.4/jury/metrics/chrf/chrf_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/comet/comet_for_language_generation.py` & `jury-2.2.4/jury/metrics/comet/comet_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/f1/f1_for_language_generation.py` & `jury-2.2.4/jury/metrics/f1/f1_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/f1/f1_for_sequence_classification.py` & `jury-2.2.4/jury/metrics/f1/f1_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/meteor/meteor_for_language_generation.py` & `jury-2.2.4/jury/metrics/meteor/meteor_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/precision/precision_for_language_generation.py` & `jury-2.2.4/jury/metrics/precision/precision_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/precision/precision_for_sequence_classification.py` & `jury-2.2.4/jury/metrics/precision/precision_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/prism/prism_for_language_generation.py` & `jury-2.2.4/jury/metrics/prism/prism_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/recall/recall_for_language_generation.py` & `jury-2.2.4/jury/metrics/recall/recall_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/recall/recall_for_sequence_classification.py` & `jury-2.2.4/jury/metrics/recall/recall_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/rouge/rouge_for_language_generation.py` & `jury-2.2.4/jury/metrics/rouge/rouge_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py` & `jury-2.2.4/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/seqeval/seqeval_for_sequence_labeling.py` & `jury-2.2.4/jury/metrics/seqeval/seqeval_for_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/squad/squad_for_language_generation.py` & `jury-2.2.4/jury/metrics/squad/squad_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/ter/ter_for_language_generation.py` & `jury-2.2.4/jury/metrics/ter/ter_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/metrics/wer/wer_for_language_generation.py` & `jury-2.2.4/jury/metrics/wer/wer_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/tokenizer.py` & `jury-2.2.4/jury/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/utils/common.py` & `jury-2.2.4/jury/utils/common.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury/utils/io.py` & `jury-2.2.4/jury/utils/io.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury.egg-info/PKG-INFO` & `jury-2.2.4/jury.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jury
-Version: 2.2.3
+Version: 2.2.4
 Summary: Evaluation toolkit for neural language generation.
 Home-page: https://github.com/obss/jury
 Author: 
 License: MIT
 Keywords: machine-learning,deep-learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 <h1 align="center">Jury</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/pyversions/jury" alt="Python versions"></a>
 <a href="https://pepy.tech/project/jury"><img src="https://pepy.tech/badge/jury" alt="downloads"></a>
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/v/jury?color=blue" alt="PyPI version"></a>
 <a href="https://github.com/obss/jury/releases/latest"><img alt="Latest Release" src="https://img.shields.io/github/release-date/obss/jury"></a>
-<a href="https://colab.research.google.com/github/obss/jury/blob/main/examples/jury_evaluate.ipynb"><img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
+<a href="https://colab.research.google.com/github/obss/jury/blob/main/examples/jury_evaluate.ipynb" target="_blank"><img alt="Open in Colab" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <br>
 <a href="https://github.com/obss/jury/actions"><img alt="Build status" src="https://github.com/obss/jury/actions/workflows/ci.yml/badge.svg"></a>
 <a href="https://libraries.io/pypi/jury"><img alt="Dependencies" src="https://img.shields.io/librariesio/github/obss/jury"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://github.com/obss/jury/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/pypi/l/jury"></a>
 <br>
 <a href="https://doi.org/10.5281/zenodo.6109838"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.6109838.svg" alt="DOI"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jury Version: 2.2.3 Summary: Evaluation toolkit for
+Metadata-Version: 2.1 Name: jury Version: 2.2.4 Summary: Evaluation toolkit for
 neural language generation. Home-page: https://github.com/obss/jury Author:
 License: MIT Keywords: machine-learning,deep-
 learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jury-2.2.3/jury.egg-info/SOURCES.txt` & `jury-2.2.4/jury.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/jury.egg-info/requires.txt` & `jury-2.2.4/jury.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 click==8.0.4
-evaluate<0.3,>=0.2.2
+evaluate<0.5,>=0.4
+datasets<2.10,>=2.9
 fire>=0.4.0
 nltk<3.7.1,>=3.6.6
 rouge-score==0.0.4
 scikit-learn
 tqdm
 validators
 
@@ -16,15 +17,15 @@
 pytest-cov>=3.0.0
 pytest-timeout>=2.1.0
 sacrebleu>=2.0.0
 bert_score==0.3.11
 jiwer>=2.3.0
 seqeval==1.2.2
 sentencepiece==0.1.96
-unbabel-comet>=1.1.2
+unbabel-comet<2,>=1.1.2
 fairseq==0.9.0
 
 [dev:python_version < "3.8"]
 importlib-metadata<4.3,>=1.1.0
 numpy==1.21.6
 
 [dev:python_version >= "3.8"]
@@ -32,15 +33,15 @@
 
 [metrics]
 sacrebleu>=2.0.0
 bert_score==0.3.11
 jiwer>=2.3.0
 seqeval==1.2.2
 sentencepiece==0.1.96
-unbabel-comet>=1.1.2
+unbabel-comet<2,>=1.1.2
 fairseq==0.9.0
 
 [metrics:python_version < "3.8"]
 numpy==1.21.6
 
 [metrics:python_version >= "3.8"]
 numpy<1.24,>=1.23
```

### Comparing `jury-2.2.3/setup.py` & `jury-2.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 _METRIC_REQUIREMENTS = [
     "sacrebleu>=2.0.0",
     "bert_score==0.3.11",
     "jiwer>=2.3.0",
     "seqeval==1.2.2",
     "sentencepiece==0.1.96",
-    "unbabel-comet>=1.1.2",
+    "unbabel-comet>=1.1.2,<2",
 ]
 
 _METRIC_REQUIREMENTS.extend(_PRISM_REQUIREMENTS)
 add_pywin(_METRIC_REQUIREMENTS)
 
 extras = {
     "prism": _PRISM_REQUIREMENTS,
```

### Comparing `jury-2.2.3/tests/jury/conftest.py` & `jury-2.2.4/tests/jury/conftest.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_accuracy.py` & `jury-2.2.4/tests/jury/metrics/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_bartscore.py` & `jury-2.2.4/tests/jury/metrics/test_bartscore.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_bertscore.py` & `jury-2.2.4/tests/jury/metrics/test_bertscore.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_bleu.py` & `jury-2.2.4/tests/jury/metrics/test_bleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_bleurt.py` & `jury-2.2.4/tests/jury/metrics/test_bleurt.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_cer.py` & `jury-2.2.4/tests/jury/metrics/test_cer.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_chrf.py` & `jury-2.2.4/tests/jury/metrics/test_chrf.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_comet.py` & `jury-2.2.4/tests/jury/metrics/test_comet.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_custom_bleu.py` & `jury-2.2.4/tests/jury/metrics/test_custom_bleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_f1.py` & `jury-2.2.4/tests/jury/metrics/test_f1.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_meteor.py` & `jury-2.2.4/tests/jury/metrics/test_meteor.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_precision.py` & `jury-2.2.4/tests/jury/metrics/test_precision.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_prism.py` & `jury-2.2.4/tests/jury/metrics/test_prism.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_recall.py` & `jury-2.2.4/tests/jury/metrics/test_recall.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_rouge.py` & `jury-2.2.4/tests/jury/metrics/test_rouge.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_sacrebleu.py` & `jury-2.2.4/tests/jury/metrics/test_sacrebleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_seqeval.py` & `jury-2.2.4/tests/jury/metrics/test_seqeval.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_squad.py` & `jury-2.2.4/tests/jury/metrics/test_squad.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_ter.py` & `jury-2.2.4/tests/jury/metrics/test_ter.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/metrics/test_wer.py` & `jury-2.2.4/tests/jury/metrics/test_wer.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/test_cli.py` & `jury-2.2.4/tests/jury/test_cli.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/test_jury.py` & `jury-2.2.4/tests/jury/test_jury.py`

 * *Files identical despite different names*

### Comparing `jury-2.2.3/tests/jury/test_utils.py` & `jury-2.2.4/tests/jury/test_utils.py`

 * *Files identical despite different names*

