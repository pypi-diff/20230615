# Comparing `tmp/pytorch_partial_tagger-0.1.7.tar.gz` & `tmp/pytorch_partial_tagger-0.1.8.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.7.tar` & `pytorch_partial_tagger-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,68 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/notebooks/basic.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/metric.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/training.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/utils.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0    11250 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/__init__.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/tag.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/text.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/helpers.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_matchers.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_metric.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_recognizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/test_functional.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/test_nn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/__init__.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/test_core.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/conftest.py
--rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/test_tag.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/test_text.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/LICENSE
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/README.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.DS_Store
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_head.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora.py
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora_base.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora_base_accelerate.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/cli_lora_large.py
+-rw-r--r--   0        0        0  1193604 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/entity.dev.jsonl
+-rw-r--r--   0        0        0  1141566 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/entity.test.jsonl
+-rw-r--r--   0        0        0  4012618 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/entity.train_r0.5_p0.9.jsonl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/log.jsonl
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/log_head.jsonl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/log_lora_base.jsonl
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scores.json
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    84871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/notebooks/basic.ipynb
+-rw-r--r--   0        0        0  4032390 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scirex/dev.jsonl
+-rw-r--r--   0        0        0  4869030 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scirex/test.jsonl
+-rw-r--r--   0        0        0 20510651 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/scirex/train.jsonl
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/metric.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/.DS_Store
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/.DS_Store
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0    15475 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/__init__.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/tag.py
+-rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/text.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/.DS_Store
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/.DS_Store
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/transformer.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/helpers.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/test_matchers.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/test_metric.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/test_recognizer.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/crf/test_nn.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/__init__.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/test_core.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/batch/conftest.py
+-rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/batch/test_tag.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/tests/data/batch/test_text.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/README.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.8/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.7/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.1.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.8/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/metric.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/tagger.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,19 +5,24 @@
 
 from .crf.nn import CRF
 from .decoders import ViterbiDecoder
 from .encoders import BaseEncoder
 
 
 class SequenceTagger(Module):
-    """Sequence tagger.
+    """A sequence tagging model with a CRF layer.
 
     Args:
-        encoder: An encoder.
-        decoder: A decoder.
+        encoder: An encoder module.
+        decoder: A decoder module.
+
+    Attributes:
+        encoder: An encoder module.
+        crf: A CRF layer.
+        decoder: A decoder module.
     """
 
     def __init__(self, encoder: BaseEncoder, decoder: ViterbiDecoder):
         super(SequenceTagger, self).__init__()
 
         self.encoder = encoder
         self.crf = CRF(encoder.get_hidden_size())
@@ -25,15 +30,15 @@
 
     def forward(
         self, inputs: dict[str, torch.Tensor], mask: torch.Tensor
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Computes log potentials and tag sequence.
 
         Args:
-            inputs: An inputs representing input data feeding into an embedder.
+            inputs: An inputs representing input data feeding into the encoder module.
             mask: A [batch_size, sequence_length] boolean tensor.
 
         Returns:
             A pair of a [batch_size, sequence_length, num_tags, num_tags] float tensor
             and a [batch_size, sequence_length] integer tensor.
             The float tensor representing log potentials and
             the integer tensor representing tag sequence.
@@ -41,12 +46,21 @@
         log_potentials = self.crf(self.encoder(inputs), mask)
         tag_indices = self.decoder(log_potentials, mask)
         return log_potentials, tag_indices
 
     def predict(
         self, inputs: dict[str, torch.Tensor], mask: torch.Tensor
     ) -> torch.Tensor:
+        """Predicts tag sequence from a given input.
+
+        Args:
+            inputs: An inputs representing input data feeding into the encoder module.
+            mask: A [batch_size, sequence_length] boolean tensor.
+
+        Returns:
+             A [batch_size, sequence_length] integer tensor representing tag sequence.
+        """
         return self(inputs, mask)[1]
 
     @property
     def padding_index(self) -> int:
         return self.decoder.padding_index
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/training.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import io
 import logging
+from collections.abc import Sequence
 from logging import Logger
-from typing import cast
 
 import torch
 from torch.utils.data import DataLoader
 
 from .crf import functional as F
-from .data import Dataset, LabelSet
+from .data import CharBasedTags, LabelSet
 from .data.batch import Collator
 from .data.batch.tag import TagsBatch
 from .data.batch.text import BaseTokenizer, TextBatch
-from .decoders.viterbi import Contrainer, ViterbiDecoder
+from .decoders.viterbi import Constrainer, ViterbiDecoder
 from .encoders import BaseEncoderFactory
 from .metric import Metric
 from .recognizer import Recognizer
 from .tagger import SequenceTagger
 
 
 class SlantedTriangular:
@@ -30,23 +30,42 @@
         if step < self.__cut:
             p = step / self.__cut
         else:
             p = 1 - (step - self.__cut) / (self.__cut * (1 / self.__cut_frac - 1))
         return (1 + p * (self.__ratio - 1)) / self.__ratio
 
 
-def expected_entity_ratio_loss(
+def compute_partially_supervised_loss(
     log_potentials: torch.Tensor,
     tag_bitmap: torch.Tensor,
     mask: torch.Tensor,
     outside_index: int,
     target_entity_ratio: float = 0.15,
     entity_ratio_margin: float = 0.05,
     balancing_coefficient: int = 10,
 ) -> torch.Tensor:
+    """Computes the loss proposed in Effland and Collins. '21.
+
+    Args:
+        log_potentials: A [batch_size, sequence_length, num_tag, num_tag] float tensor
+        representing log potentials.
+        tag_bitmap: A [batch_size, sequence_length, num_tag] boolean tensor indicating
+        all active tags at each index.
+        mask: A [batch_size, sequence_length] boolean tensor.
+        outside_index: An integer representing a non-entity index.
+        target_entity_ratio: A float representing a target entity ratio
+        for training. Defaults to 0.15.
+        entity_ratio_margin: A float representing a margin for the entity ratio.
+        Defaults to 0.05.
+        balancing_coefficient: An integer representing a balancing coefficient
+        for the loss function. Defaults to 10.
+
+    Returns:
+        A float representing loss.
+    """
     with torch.enable_grad():
         # log partition
         log_Z = F.forward_algorithm(log_potentials)
 
         # marginal probabilities
         p = torch.autograd.grad(log_Z.sum(), log_potentials, create_graph=True)[0].sum(
             dim=-1
@@ -65,14 +84,35 @@
     score = F.multitag_sequence_score(log_potentials, tag_bitmap, mask)
     supervised_loss = (log_Z - score).mean()
 
     return supervised_loss + balancing_coefficient * expected_entity_ratio_loss
 
 
 class Trainer:
+    """A trainer for fitting the parameters of a tagger based on a given dataset.
+
+    Args:
+        tokenizer: An instance of BaseTokenizer.
+        encoder_factory: An encoder factory for creating encoders.
+        batch_size: An integer representing a batch size for training. Defaults to 15.
+        num_epochs: An integer representing the number of epochs for training.
+        Defaults to 20.
+        learning_rate: A float representing a learning rate for optimization.
+        Defaults to 2e-5.
+        gradient_clip_value: A float representing a maximum gradient value
+        for clipping. Defaults to 5.0.
+        target_entity_ratio: A float representing a target entity ratio
+        for training. Defaults to 0.15.
+        entity_ratio_margin: A float representing a margin for the entity ratio.
+        Defaults to 0.05.
+        balancing_coefficient: An integer representing a balancing coefficient
+        for the loss function. Defaults to 10.
+        padding_index: An integer representing an index for padding. Defaults to -1.
+    """
+
     def __init__(
         self,
         tokenizer: BaseTokenizer,
         encoder_factory: BaseEncoderFactory,
         batch_size: int = 15,
         num_epochs: int = 20,
         learning_rate: float = 2e-5,
@@ -91,19 +131,32 @@
         self.__target_entity_ratio = target_entity_ratio
         self.__entity_ratio_margin = entity_ratio_margin
         self.__balancing_coefficient = balancing_coefficient
         self.__padding_index = padding_index
 
     def __call__(
         self,
-        train_dataset: Dataset,
-        validation_dataset: Dataset,
+        train_dataset: list[tuple[str, CharBasedTags]],
+        validation_dataset: list[tuple[str, CharBasedTags]],
         device: torch.device,
         logger: Logger | None = None,
     ) -> Recognizer:
+        """Trains an instance of SequenceTagger.
+
+        Args:
+            train_dataset: A list of training data tuples containing text and tags.
+            validation_dataset: A list of validation data tuples
+            containing text and tags.
+            device: A device to be used for training.
+            logger: A logger for logging training progress. Defaults to None.
+
+        Returns:
+            An instance of Recognizer which predicts character-based tags
+            from a given text.
+        """
         if logger is None:
             logger = logging.getLogger(__name__)
             logger.setLevel(logging.INFO)
             logger.addHandler(logging.StreamHandler())
 
         # Create a label_set
         labels = set()
@@ -113,31 +166,31 @@
                     labels.add(tag.label)
         label_set = LabelSet(labels)
 
         tagger = SequenceTagger(
             self.__encoder_factory.create(label_set),
             ViterbiDecoder(
                 self.__padding_index,
-                Contrainer(
+                Constrainer(
                     label_set.get_start_states(),
                     label_set.get_end_states(),
                     label_set.get_transitions(),
                 ),
             ),
         )
         tagger.to(device)
 
         collator = Collator(self.__tokenizer, label_set)
 
-        train_dataloader = DataLoader(
+        train_dataloader: Sequence[tuple[TextBatch, TagsBatch]] = DataLoader(
             train_dataset,  # type:ignore
             collate_fn=collator,
             batch_size=self.__batch_size,
         )
-        validation_dataloader = DataLoader(
+        validation_dataloader: Sequence[tuple[TextBatch, TagsBatch]] = DataLoader(
             validation_dataset,  # type:ignore
             collate_fn=collator,
             batch_size=self.__batch_size,
             shuffle=False,
         )
 
         optimizer = torch.optim.Adam(
@@ -151,27 +204,24 @@
         best_tagger_state = io.BytesIO()
 
         for epoch in range(1, self.__num_epochs + 1):
             epoch_loss = 0.0
             tagger.train()
 
             for text_batch, tags_batch in train_dataloader:
-                text_batch = cast(TextBatch, text_batch)
-                tags_batch = cast(TagsBatch, tags_batch)
-
                 text_batch.to(device)
                 tags_batch.to(device)
 
                 optimizer.zero_grad()
 
                 mask = text_batch.mask
 
                 log_potentials, _ = tagger(text_batch.tagger_inputs, mask)
 
-                loss = expected_entity_ratio_loss(
+                loss = compute_partially_supervised_loss(
                     log_potentials,
                     tags_batch.get_tag_bitmap(),
                     mask,
                     label_set.get_outside_index(),
                     self.__target_entity_ratio,
                     self.__entity_ratio_margin,
                     self.__balancing_coefficient,
@@ -186,17 +236,14 @@
                 schedular.step()
 
                 epoch_loss += loss.item() * text_batch.size
 
             tagger.eval()
             metric = Metric()
             for text_batch, tags_batch in validation_dataloader:
-                text_batch = cast(TextBatch, text_batch)
-                tags_batch = cast(TagsBatch, tags_batch)
-
                 text_batch.to(device)
                 tags_batch.to(device)
 
                 tag_indices = tagger.predict(text_batch.tagger_inputs, text_batch.mask)
 
                 predictions = text_batch.create_char_based_tags(
                     tag_indices, label_set, tagger.padding_index
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/utils.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Args:
         start: An integer representing a start index of a tag.
         length: An integer representing length of a tag.
         label: A string representing a label of a tag.
 
     Returns:
-        A Tag.
+        An instance of Tag.
     """
     return Tag(Span(start, length), label)
 
 
 def create_trainer(
     model_name: str = "roberta-base",
     dropout: float = 0.2,
@@ -32,15 +32,15 @@
     num_epochs: int = 20,
     learning_rate: float = 2e-5,
     gradient_clip_value: float = 5.0,
     padding_index: int = -1,
     tokenizer_args: dict | None = None,
     encoder_type: str = "default",
 ) -> Trainer:
-    """Creates Trainer."""
+    """Creates an instance of Trainer."""
 
     if encoder_type == "default":
         encoder_factory = TransformerModelEncoderFactory(model_name, dropout)
     elif encoder_type == "with_head":
         encoder_factory = TransformerModelWithHeadEncoderFactory(model_name, dropout)
     else:
         raise ValueError(f"{encoder_type} is not supported.")
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/crf/nn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from typing import Optional
+from __future__ import annotations
 
 import torch
 from torch import nn
 
 from . import NINF
 
 
 class CRF(nn.Module):
-    """A CRF layer.
+    """A Conditional Random Field (CRF) layer.
 
     Args:
         num_tags: An integer representing the number of tags.
 
+    Attributes:
+        transitions: Transition parameters of a CRF.
     """
 
     def __init__(self, num_tags: int) -> None:
         super(CRF, self).__init__()
 
         self.transitions = nn.Parameter(torch.empty(num_tags, num_tags))
 
         nn.init.xavier_normal_(self.transitions)
 
     def forward(
-        self, logits: torch.Tensor, mask: Optional[torch.Tensor] = None
+        self, logits: torch.Tensor, mask: torch.Tensor | None = None
     ) -> torch.Tensor:
         """Computes log potentials for a CRF.
 
         Args:
             logits: A [batch_size, sequence_length, num_tags] float tensor.
             mask: A [batch_size, sequence_length] boolean tensor.
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/__init__.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/tag.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/data/batch/tag.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 import torch
 
 from ..core import CharBasedTags, LabelSet, TokenBasedTags
 
 
 class TagsBatch:
+    """A batch of token-based tags.
+
+    Args:
+        tags_batch: A tuple of instances of TokenBasedTags.
+        label_set: An instance of LabelSet to use for tag conversion.
+        device: A device on which to place tensors. Defaults to None.
+    """
+
     def __init__(
         self,
         tags_batch: tuple[TokenBasedTags, ...],
         label_set: LabelSet,
         device: torch.device | None = None,
     ):
         self.__tags_batch = tags_batch
@@ -30,14 +38,25 @@
     @property
     def token_based(self) -> tuple[TokenBasedTags, ...]:
         return self.__tags_batch
 
     def get_tag_indices(
         self, padding_index: int = -1, unknown_index: int = -100
     ) -> torch.Tensor:
+        """Returns a tensor of tag indices for a batch.
+
+        Args:
+            padding_index: An integer representing an index to pad a tensor.
+            Defaults to -1.
+            unknown_index: An integer representing an index for an unknown tag.
+            Defaults to -100.
+
+        Returns:
+            A [batch_size, sequence_length] integer tensor representing tag indices.
+        """
         label_set = self.__label_set
 
         max_length = max(tags.num_tokens for tags in self.__tags_batch)
 
         tag_indices = []
 
         for tags in self.__tags_batch:
@@ -50,14 +69,20 @@
             tensor = tensor.to(self.__device)
 
         return tensor
 
     def get_tag_bitmap(
         self,
     ) -> torch.Tensor:
+        """Returns a tensor of tag bitmap for a batch.
+
+        Returns:
+            A [batch_size, sequence_length, num_tags] boolean tensor representing
+            tag bitmap.
+        """
         label_set = self.__label_set
 
         max_length = max(tags.num_tokens for tags in self.__tags_batch)
 
         tag_bitmap = []
 
         for tags in self.__tags_batch:
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/decoders/viterbi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,100 @@
 from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
-from typing import Optional
-
 import torch
 from torch.nn import Module, Parameter
 
 from ..crf import functional as F
 
 
-class BaseConstrainer(Module, metaclass=ABCMeta):
-    @abstractmethod
-    def forward(self, log_potentials: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
-        raise NotImplementedError
+class Constrainer(Module):
+    """A constrainer to constrain the given log potentials of a CRF.
+
+    Args:
+        start_states: A list of boolean values representing the start states.
+        True indicates an allowed state, while False indicates an otherwise state.
+        end_states: A list of boolean values representing the end states.
+        True indicates an allowed state, while False indicates an otherwise state.
+        transitions: A list of lists of boolean values representing the transitions.
+        True indicates an allowed transition,
+        while False indicates an otherwise transition.
+
+    Attributes:
+        start_states: Start states parameters.
+        end_states: End states parameters.
+        transitions: transitions parameters.
 
+    """
 
-class Contrainer(BaseConstrainer):
     def __init__(
         self,
         start_states: list[bool],
         end_states: list[bool],
         transitions: list[list[bool]],
     ):
-        super(Contrainer, self).__init__()
+        super(Constrainer, self).__init__()
 
         self.start_states = Parameter(torch.tensor(start_states), requires_grad=False)
         self.end_states = Parameter(torch.tensor(end_states), requires_grad=False)
         self.transitions = Parameter(torch.tensor(transitions), requires_grad=False)
 
     def forward(self, log_potentials: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
+        """Applies constraints to a given log potentials.
+
+        Args:
+            log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
+            float tensor.
+            mask: A [batch_size, sequence_length] boolean tensor.
+
+        Returns:
+            A [batch_size, sequence_length, num_tags, num_tags] float tensor
+            representing constrained log potentials.
+        """
         return F.constrain_log_potentials(
             log_potentials, mask, self.start_states, self.end_states, self.transitions
         )
 
 
 class ViterbiDecoder(Module):
-    """A Viterbi decoder for CRF.
+    """A Viterbi decoder for a CRF.
 
     Args:
         padding_index: An integer for padded elements.
+        constrainer: A instance of Constrainer to constrain a given log potentials.
+
+    Attributes:
+        padding_index: An integer for padded elements.
+        constrainer: A constrainer.
     """
 
     def __init__(
         self,
-        padding_index: Optional[int] = -1,
-        constrainer: Optional[BaseConstrainer] = None,
+        padding_index: int = -1,
+        constrainer: Constrainer | None = None,
     ) -> None:
         super(ViterbiDecoder, self).__init__()
 
         self.padding_index = padding_index
-        self.contrainer = constrainer
+        self.constrainer = constrainer
 
     def forward(self, log_potentials: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
         """Computes the best tag sequence from the given log potentials.
 
         Args:
             log_potentials: A [batch_size, sequence_length, num_tags, num_tags]
             float tensor.
             mask: A [batch_size, sequence_length] boolean tensor.
 
         Returns:
             A [batch_size, sequence_length] integer tensor representing
             the best tag sequence.
         """
 
-        if self.contrainer is not None:
-            log_potentials = self.contrainer(log_potentials, mask)
+        if self.constrainer is not None:
+            log_potentials = self.constrainer(log_potentials, mask)
 
         log_potentials.requires_grad_()
 
         with torch.enable_grad():
             _, tag_indices = F.decode(log_potentials)
 
         return tag_indices * mask + self.padding_index * (~mask)
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.8/src/partial_tagger/encoders/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,30 +5,46 @@
 import torch
 from torch.nn import Module
 
 from ..data.core import LabelSet
 
 
 class BaseEncoder(Module, metaclass=ABCMeta):
-    """Base class of all encoders."""
+    """Base class for all encoders."""
 
     @abstractmethod
     def forward(self, inputs: dict[str, torch.Tensor]) -> torch.Tensor:
-        """Encode the given inputs to a tensor.
+        """Encodes the given inputs to a tensor representation.
 
         Args:
-            inputs: A dictionary that maps a string key to a tensor value.
+            inputs: A dictionary that maps string keys to a tensor values.
 
         Returns:
             A [batch_size, sequence_length, hidden_size] float tensor.
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_hidden_size(self) -> int:
+        """Returns the dimension size of the output tensor.
+
+        Returns:
+            The dimension size of the output tensor.
+        """
         raise NotImplementedError
 
 
 class BaseEncoderFactory(metaclass=ABCMeta):
+    """Base class for all encoder factories."""
+
     @abstractmethod
     def create(self, label_set: LabelSet) -> BaseEncoder:
+        """Creates an encoder based on the provided label set.
+
+        Args:
+            label_set: An instance of LabelSet.
+
+        Returns:
+            An encoder that transforms input into a tensor representation.
+
+        """
         raise NotImplementedError
```

### Comparing `pytorch_partial_tagger-0.1.7/tests/conftest.py` & `pytorch_partial_tagger-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/helpers.py` & `pytorch_partial_tagger-0.1.8/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/test_matchers.py` & `pytorch_partial_tagger-0.1.8/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/test_metric.py` & `pytorch_partial_tagger-0.1.8/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/test_recognizer.py` & `pytorch_partial_tagger-0.1.8/tests/test_recognizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,8 +11,9 @@
     device = torch.device("cpu")
 
     trainer = create_trainer("distilroberta-base")
     recognizer = trainer(dataset, dataset, device)
 
     output = recognizer((text,), 1, device)
 
+    assert len(output) == 1
     assert isinstance(output[0], CharBasedTags)
```

### Comparing `pytorch_partial_tagger-0.1.7/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.1.8/tests/crf/test_functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.1.8/tests/crf/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/data/test_core.py` & `pytorch_partial_tagger-0.1.8/tests/data/test_core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/data/batch/test_tag.py` & `pytorch_partial_tagger-0.1.8/tests/data/batch/test_tag.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/data/batch/test_text.py` & `pytorch_partial_tagger-0.1.8/tests/data/batch/test_text.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/.gitignore` & `pytorch_partial_tagger-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/LICENSE` & `pytorch_partial_tagger-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/README.md` & `pytorch_partial_tagger-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/pyproject.toml` & `pytorch_partial_tagger-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/PKG-INFO` & `pytorch_partial_tagger-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.7
+Version: 0.1.8
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

