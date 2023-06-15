# Comparing `tmp/optimum-intel-1.9.0.tar.gz` & `tmp/optimum-intel-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/optimum-intel-1.9.0.tar", last modified: Fri Jun  9 17:42:39 2023, max compression
+gzip compressed data, was "optimum-intel-1.9.1.tar", last modified: Thu Jun 15 15:43:12 2023, max compression
```

## Comparing `optimum-intel-1.9.0.tar` & `optimum-intel-1.9.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.014373 optimum-intel-1.9.0/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.004372 optimum-intel-1.9.0/optimum/commands/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/commands/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/commands/neural_compressor/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/commands/neural_compressor/quantize.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/commands/register/register_inc.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/intel/
--rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.024373 optimum-intel-1.9.0/optimum/intel/generation/
--rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/generation/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/generation/modeling.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.034374 optimum-intel-1.9.0/optimum/intel/ipex/
--rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/ipex/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/ipex/inference.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.034374 optimum-intel-1.9.0/optimum/intel/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3730 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/launcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/neural_coder_adaptor.py
--rw-r--r--   0 ella      (1000) ella      (1000)    27858 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38957 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/neural_compressor/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.044374 optimum-intel-1.9.0/optimum/intel/openvino/
--rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15434 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18258 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_base_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    16811 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    28970 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18032 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    14161 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/openvino/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/optimum/intel/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_ipex_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_neural_compressor_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/optimum/intel/utils/modeling_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-09 17:39:49.000000 optimum-intel-1.9.0/optimum/intel/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/optimum_intel.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-09 17:42:38.000000 optimum-intel-1.9.0/optimum_intel.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)      412 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-09 17:42:37.000000 optimum-intel-1.9.0/optimum_intel.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-09 17:42:39.054375 optimum-intel-1.9.0/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     2594 2023-06-09 17:38:50.000000 optimum-intel-1.9.0/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/commands/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/commands/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/commands/neural_compressor/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/commands/neural_compressor/quantize.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/commands/register/register_inc.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/intel/
+-rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/intel/generation/
+-rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/generation/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/generation/modeling.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.475665 optimum-intel-1.9.1/optimum/intel/ipex/
+-rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/ipex/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/ipex/inference.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.485665 optimum-intel-1.9.1/optimum/intel/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3730 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/launcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/neural_coder_adaptor.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    27858 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    38957 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/neural_compressor/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.485665 optimum-intel-1.9.1/optimum/intel/openvino/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15434 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18258 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_base_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17577 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28970 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18032 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    14161 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/openvino/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/optimum/intel/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_ipex_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/optimum/intel/utils/modeling_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-15 15:40:31.000000 optimum-intel-1.9.1/optimum/intel/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/optimum_intel.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-15 15:43:11.000000 optimum-intel-1.9.1/optimum_intel.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-15 15:43:11.000000 optimum-intel-1.9.1/optimum_intel.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-15 15:43:11.000000 optimum-intel-1.9.1/optimum_intel.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)      441 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-15 15:43:12.000000 optimum-intel-1.9.1/optimum_intel.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-15 15:43:12.495665 optimum-intel-1.9.1/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     2671 2023-06-15 15:39:56.000000 optimum-intel-1.9.1/setup.py
```

### Comparing `optimum-intel-1.9.0/LICENSE` & `optimum-intel-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/MANIFEST.in` & `optimum-intel-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/PKG-INFO` & `optimum-intel-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.0
+Version: 1.9.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.0/README.md` & `optimum-intel-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/commands/neural_compressor/base.py` & `optimum-intel-1.9.1/optimum/commands/neural_compressor/base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/commands/neural_compressor/quantize.py` & `optimum-intel-1.9.1/optimum/commands/neural_compressor/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/commands/register/register_inc.py` & `optimum-intel-1.9.1/optimum/commands/register/register_inc.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/__init__.py` & `optimum-intel-1.9.1/optimum/intel/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/generation/__init__.py` & `optimum-intel-1.9.1/optimum/intel/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/generation/modeling.py` & `optimum-intel-1.9.1/optimum/intel/generation/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/ipex/inference.py` & `optimum-intel-1.9.1/optimum/intel/ipex/inference.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/__init__.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/configuration.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/modeling_diffusion.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/neural_coder_adaptor.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/neural_coder_adaptor.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/quantization.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/trainer_seq2seq.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/neural_compressor/utils.py` & `optimum-intel-1.9.1/optimum/intel/neural_compressor/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/__init__.py` & `optimum-intel-1.9.1/optimum/intel/openvino/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/configuration.py` & `optimum-intel-1.9.1/optimum/intel/openvino/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/modeling.py` & `optimum-intel-1.9.1/optimum/intel/openvino/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/modeling_base.py` & `optimum-intel-1.9.1/optimum/intel/openvino/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/modeling_base_seq2seq.py` & `optimum-intel-1.9.1/optimum/intel/openvino/modeling_base_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/modeling_decoder.py` & `optimum-intel-1.9.1/optimum/intel/openvino/modeling_decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,29 @@
     >>> model = {model_class}.from_pretrained("{checkpoint}", export=True)
     >>> gen_pipeline = pipeline("text-generation", model=model, tokenizer=tokenizer)
     >>> text = "I love this story because"
     >>> gen = gen_pipeline(text)
     ```
 """
 
+_SUPPORTED_ARCHITECTURES = {
+    "bart",
+    "blenderbot",
+    "blenderbot-small",
+    "bloom",
+    "codegen",
+    "gpt2",
+    "gpt_neo",
+    "gpt_neox",
+    "llama",
+    "marian",
+    "opt",
+    "pegasus",
+}
+
 
 @add_start_docstrings(
     """
     Base OVBaseDecoderModel class.
     """,
 )
 class OVBaseDecoderModel(OVModel):
@@ -132,14 +147,20 @@
         subfolder: str = "",
         local_files_only: bool = False,
         task: Optional[str] = None,
         use_cache: bool = True,
         trust_remote_code: bool = False,
         **kwargs,
     ):
+        if config.model_type not in _SUPPORTED_ARCHITECTURES:
+            logger.warning(
+                f"This architecture : {config.model_type} was not validated, only :{', '.join(_SUPPORTED_ARCHITECTURES)} architectures were "
+                "validated, use at your own risk."
+            )
+
         model_file_name = ONNX_WEIGHTS_NAME
 
         if task is None:
             task = cls._auto_model_to_task(cls.auto_model_class)
 
         save_dir = TemporaryDirectory()
         save_dir_path = Path(save_dir.name)
@@ -149,23 +170,26 @@
             "cache_dir": cache_dir,
             "subfolder": subfolder,
             "local_files_only": local_files_only,
             "force_download": force_download,
             "trust_remote_code": trust_remote_code,
         }
         model = TasksManager.get_model_from_task(task, model_id, **model_kwargs)
+        config.is_decoder = True
+        config.is_encoder_decoder = False
         onnx_config_constructor = TasksManager.get_exporter_config_constructor(model=model, exporter="onnx", task=task)
         onnx_config = onnx_config_constructor(model.config, use_past=use_cache)
 
         # TODO : create ModelPatcher to patch each architecture
-        if model.config.model_type == "bloom":
+        if config.model_type == "bloom":
             model.transformer._prepare_attn_mask = _prepare_attn_mask
-
-        if model.config.model_type == "llama":
+        elif config.model_type == "llama":
             model.model._prepare_decoder_attention_mask = _prepare_decoder_attention_mask
+        elif config.model_type in {"blenderbot-small", "blenderbot", "opt", "pegasus", "bart"}:
+            model.model.decoder._prepare_decoder_attention_mask = _prepare_decoder_attention_mask
 
         # Export the model to the ONNX format
         export(model=model, config=onnx_config, output=save_dir_path / model_file_name)
 
         return cls._from_pretrained(
             model_id=save_dir_path,
             config=config,
```

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/modeling_diffusion.py` & `optimum-intel-1.9.1/optimum/intel/openvino/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/modeling_seq2seq.py` & `optimum-intel-1.9.1/optimum/intel/openvino/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/quantization.py` & `optimum-intel-1.9.1/optimum/intel/openvino/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/trainer.py` & `optimum-intel-1.9.1/optimum/intel/openvino/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/training_args.py` & `optimum-intel-1.9.1/optimum/intel/openvino/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/openvino/utils.py` & `optimum-intel-1.9.1/optimum/intel/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/__init__.py` & `optimum-intel-1.9.1/optimum/intel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/constant.py` & `optimum-intel-1.9.1/optimum/intel/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/dummy_ipex_objects.py` & `optimum-intel-1.9.1/optimum/intel/utils/dummy_ipex_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py` & `optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/dummy_neural_compressor_objects.py` & `optimum-intel-1.9.1/optimum/intel/utils/dummy_neural_compressor_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py` & `optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py` & `optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/dummy_openvino_objects.py` & `optimum-intel-1.9.1/optimum/intel/utils/dummy_openvino_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/import_utils.py` & `optimum-intel-1.9.1/optimum/intel/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/utils/modeling_utils.py` & `optimum-intel-1.9.1/optimum/intel/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/optimum/intel/version.py` & `optimum-intel-1.9.1/optimum/intel/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `optimum-intel-1.9.0/optimum_intel.egg-info/PKG-INFO` & `optimum-intel-1.9.1/optimum_intel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.0
+Version: 1.9.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.0/optimum_intel.egg-info/SOURCES.txt` & `optimum-intel-1.9.1/optimum_intel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/pyproject.toml` & `optimum-intel-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/setup.cfg` & `optimum-intel-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.0/setup.py` & `optimum-intel-1.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,25 @@
     "transformers>=4.20.0",
     "datasets>=1.4.0",
     "sentencepiece",
     "scipy",
     "accelerate",  # transformers 4.29 require accelerate for PyTorch
 ]
 
-TESTS_REQUIRE = ["pytest", "parameterized", "Pillow", "evaluate", "diffusers", "py-cpuinfo"]
+TESTS_REQUIRE = [
+    "pytest",
+    "parameterized",
+    "Pillow",
+    "evaluate",
+    "diffusers",
+    "py-cpuinfo",
+    "sacremoses",
+    "torchaudio",
+    "rjieba",
+]
 
 QUALITY_REQUIRE = ["black~=23.1", "ruff>=0.0.241"]
 
 EXTRAS_REQUIRE = {
     "neural-compressor": ["neural-compressor>=2.1.1", "onnx", "onnxruntime<1.15.0"],
     "openvino": ["openvino>=2023.0.0", "onnx", "onnxruntime"],
     "nncf": ["nncf>=2.5.0", "openvino-dev>=2023.0.0"],
```

