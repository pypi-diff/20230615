# Comparing `tmp/structured-pruning-adapters-0.6.0.tar.gz` & `tmp/structured-pruning-adapters-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structured-pruning-adapters-0.6.0.tar", last modified: Wed Jun 14 09:13:58 2023, max compression
+gzip compressed data, was "structured-pruning-adapters-0.6.1.tar", last modified: Thu Jun 15 12:49:21 2023, max compression
```

## Comparing `structured-pruning-adapters-0.6.0.tar` & `structured-pruning-adapters-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.053026 structured-pruning-adapters-0.6.0/sp_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/splopa.py
--rw-r--r--   0 runner    (1001) docker     (123)    31876 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/splora.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/torch_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-14 09:13:58.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_lin_as_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_splopa.py
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_splora.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_torchpruning.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.202952 structured-pruning-adapters-0.6.1/sp_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31876 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/torch_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_lin_as_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_torchpruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_utils.py
```

### Comparing `structured-pruning-adapters-0.6.0/LICENSE` & `structured-pruning-adapters-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/PKG-INFO` & `structured-pruning-adapters-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.6.0
+Version: 0.6.1
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.0 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.1 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `structured-pruning-adapters-0.6.0/README.md` & `structured-pruning-adapters-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/setup.py` & `structured-pruning-adapters-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/sp_adapters/lora.py` & `structured-pruning-adapters-0.6.1/sp_adapters/lora.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/sp_adapters/splopa.py` & `structured-pruning-adapters-0.6.1/sp_adapters/splopa.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/sp_adapters/splora.py` & `structured-pruning-adapters-0.6.1/sp_adapters/splora.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/sp_adapters/torch_pruning.py` & `structured-pruning-adapters-0.6.1/sp_adapters/torch_pruning.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from torch_pruning.pruner import function
 
 from .splora import (
     SPLoRAConv1d,
     SPLoRAConv2d,
     SPLoRAConv3d,
     SPLoRALinear,
+    SPLoRAMultiheadAttention,
     _SPLoRAConvNd,
 )
 
 __all__ = [
     "SPLoRALinearPruner",
     "SPLoRAConvPruner",
     "customized_pruners",
@@ -53,14 +54,17 @@
     def get_out_channels(self, layer):
         return layer.out_features
 
     def get_in_channels(self, layer):
         return layer.in_features
 
 
+splora_linear_pruner = SPLoRALinearPruner()
+
+
 class SPLoRAConvPruner(function.BasePruningFunc):
     TARGET_MODULE = _SPLoRAConvNd
 
     def prune_out_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.out_channels)) - set(idxs))
         keep_idxs.sort()
         layer.out_channels = layer.out_channels - len(idxs)
@@ -99,36 +103,113 @@
     def get_out_channels(self, layer):
         return layer.out_channels
 
     def get_in_channels(self, layer):
         return layer.in_channels
 
 
-splora_linear_pruner = SPLoRALinearPruner()
 splora_conv_pruner = SPLoRAConvPruner()
 
+
+class SPLoRAMultiheadAttentionPruner(function.BasePruningFunc):
+    TARGET_MODULES = nn.MultiheadAttention
+
+    def check(self, layer, idxs, to_output):
+        super().check(layer, idxs, to_output)
+        assert (layer.embed_dim - len(idxs)) % layer.num_heads == 0, (
+            "embed_dim (%d) of MultiheadAttention after pruning must divide evenly by `num_heads` (%d)"
+            % (layer.embed_dim, layer.num_heads)
+        )
+
+    def prune_out_channels(self, layer, idxs: list) -> nn.Module:
+        """
+        Note: The `torch_pruning.pruning.function.MultiheadAttentionPruner`
+        implementation is fundamentally flawed.
+
+        There is no good reason to prune other parameters than `out_proj` besides to
+        satisfy that `embed_dim` is consistent across all its uses.
+        Currently, however, the PyTorch implementation of nn.MultiheadAttention and
+        `F.multi_head_attention_forward` don't let us individually modify the dims of
+        different (valid) uses of `embed_dim`.
+        See https://github.com/pytorch/pytorch/issues/103668
+
+        The pruning that is currently happening can be considered random for all but the
+        `out_proj` output dimensionality. To keep in line with the torch_pruning impl,
+        we'll (reluctantly) use the same strategy here.
+        """
+        keep_idxs = list(set(range(layer.embed_dim)) - set(idxs))
+        keep_idxs.sort()
+        pruning_idxs_repeated = (
+            idxs
+            + [i + layer.embed_dim for i in idxs]
+            + [i + 2 * layer.embed_dim for i in idxs]
+        )
+        keep_idxs_3x_repeated = list(
+            set(range(3 * layer.embed_dim)) - set(pruning_idxs_repeated)
+        )
+
+        layer.q_proj = splora_linear_pruner.prune_out_channels(layer.q_proj, idxs)
+        layer.q_proj = splora_linear_pruner.prune_in_channels(layer.q_proj, idxs)
+
+        layer.k_proj = splora_linear_pruner.prune_out_channels(layer.k_proj, idxs)
+        layer.k_proj = splora_linear_pruner.prune_in_channels(layer.k_proj, idxs)
+
+        layer.v_proj = splora_linear_pruner.prune_out_channels(layer.v_proj, idxs)
+        layer.v_proj = splora_linear_pruner.prune_in_channels(layer.v_proj, idxs)
+
+        if layer.in_proj_bias is not None:
+            layer.in_proj_bias = self._prune_parameter_and_grad(
+                layer.in_proj_bias, keep_idxs_3x_repeated, 0
+            )
+        if layer.bias_k is not None:
+            layer.bias_k = self._prune_parameter_and_grad(layer.bias_k, keep_idxs, 2)
+        if layer.bias_v is not None:
+            layer.bias_v = self._prune_parameter_and_grad(layer.bias_v, keep_idxs, 2)
+
+        layer.out_proj = splora_linear_pruner.prune_out_channels(layer.out_proj, idxs)
+        layer.out_proj = splora_linear_pruner.prune_in_channels(layer.out_proj, idxs)
+
+        layer.embed_dim = layer.embed_dim - len(idxs)
+        layer.head_dim = layer.embed_dim // layer.num_heads
+        layer.kdim = layer.embed_dim
+        layer.vdim = layer.embed_dim
+        return layer
+
+    prune_in_channels = prune_out_channels
+
+    def get_out_channels(self, layer):
+        return layer.embed_dim
+
+    def get_in_channels(self, layer):
+        return self.get_out_channels(layer)
+
+
+splora_mha_pruner = SPLoRAMultiheadAttentionPruner()
+
 # Pass this dict to the "customized_pruners" argument of pruners in the Torch Pruning lib
 customized_pruners = {
     SPLoRALinear: splora_linear_pruner,
     _SPLoRAConvNd: splora_conv_pruner,
     SPLoRAConv1d: splora_conv_pruner,
     SPLoRAConv2d: splora_conv_pruner,
     SPLoRAConv3d: splora_conv_pruner,
+    SPLoRAMultiheadAttention: splora_mha_pruner,
 }
 
 # Pass this dict to the "root_module_types" argument of pruners in the Torch Pruning lib
 root_module_types = [
     nn.modules.conv._ConvNd,
     nn.Linear,
     nn.LSTM,
     SPLoRALinear,
     _SPLoRAConvNd,
     SPLoRAConv1d,
     SPLoRAConv2d,
     SPLoRAConv3d,
+    SPLoRAMultiheadAttention,
 ]
 
 
 class MagnitudeImportance(tp.importance.MagnitudeImportance):
     # Near identical implementation
     @torch.no_grad()
     def __call__(self, group, ch_groups=1):  # noqa: C901
```

### Comparing `structured-pruning-adapters-0.6.0/sp_adapters/utils.py` & `structured-pruning-adapters-0.6.1/sp_adapters/utils.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/PKG-INFO` & `structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.6.0
+Version: 0.6.1
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.0 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.1 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/SOURCES.txt` & `structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/tests/test_lin_as_conv.py` & `structured-pruning-adapters-0.6.1/tests/test_lin_as_conv.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/tests/test_splopa.py` & `structured-pruning-adapters-0.6.1/tests/test_splopa.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/tests/test_splora.py` & `structured-pruning-adapters-0.6.1/tests/test_splora.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.0/tests/test_torchpruning.py` & `structured-pruning-adapters-0.6.1/tests/test_torchpruning.py`

 * *Files identical despite different names*

