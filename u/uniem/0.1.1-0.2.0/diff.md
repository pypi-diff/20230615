# Comparing `tmp/uniem-0.1.1.tar.gz` & `tmp/uniem-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.1.1.tar", max compression
+gzip compressed data, was "uniem-0.2.0.tar", max compression
```

## Comparing `uniem-0.1.1.tar` & `uniem-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-05-09 07:54:15.399692 uniem-0.1.1/LICENSE
--rw-r--r--   0        0        0      598 2023-05-15 03:14:34.188003 uniem-0.1.1/README.md
--rw-r--r--   0        0        0      607 2023-05-22 10:36:44.346256 uniem-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      104 2023-05-12 10:16:25.758032 uniem-0.1.1/uniem/__init__.py
--rw-r--r--   0        0        0     5950 2023-05-18 03:50:32.557213 uniem-0.1.1/uniem/criteria.py
--rw-r--r--   0        0        0     8443 2023-05-22 06:43:10.136944 uniem-0.1.1/uniem/data.py
--rw-r--r--   0        0        0      430 2023-05-09 10:34:04.808537 uniem-0.1.1/uniem/data_structures.py
--rw-r--r--   0        0        0    11889 2023-05-22 10:36:08.591891 uniem-0.1.1/uniem/model.py
--rw-r--r--   0        0        0     5850 2023-05-22 06:30:59.048879 uniem-0.1.1/uniem/trainer.py
--rw-r--r--   0        0        0      680 2023-05-19 09:54:21.001026 uniem-0.1.1/uniem/types.py
--rw-r--r--   0        0        0      621 2023-05-10 07:07:11.507943 uniem-0.1.1/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-05-22 10:36:54.260085 uniem-0.1.1/uniem/version.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 uniem-0.1.1/setup.py
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 uniem-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 07:54:15.399692 uniem-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6101 2023-06-15 11:16:21.191745 uniem-0.2.0/README.md
+-rw-r--r--   0        0        0      607 2023-06-15 11:18:52.184649 uniem-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-06-15 11:25:08.185076 uniem-0.2.0/uniem/__init__.py
+-rw-r--r--   0        0        0     6884 2023-06-15 05:12:54.271051 uniem-0.2.0/uniem/criteria.py
+-rw-r--r--   0        0        0    10028 2023-06-15 11:23:52.141569 uniem-0.2.0/uniem/data.py
+-rw-r--r--   0        0        0      628 2023-06-15 08:39:00.949540 uniem-0.2.0/uniem/data_structures.py
+-rw-r--r--   0        0        0     8004 2023-06-15 10:13:33.939494 uniem-0.2.0/uniem/finetuner.py
+-rw-r--r--   0        0        0    13637 2023-06-15 11:44:36.163028 uniem-0.2.0/uniem/model.py
+-rw-r--r--   0        0        0     5860 2023-06-15 09:39:32.604643 uniem-0.2.0/uniem/trainer.py
+-rw-r--r--   0        0        0      659 2023-06-07 06:09:24.419876 uniem-0.2.0/uniem/types.py
+-rw-r--r--   0        0        0      915 2023-06-15 08:02:39.812246 uniem-0.2.0/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-05-22 10:36:54.260085 uniem-0.2.0/uniem/version.py
+-rw-r--r--   0        0        0     6997 1970-01-01 00:00:00.000000 uniem-0.2.0/setup.py
+-rw-r--r--   0        0        0     6723 1970-01-01 00:00:00.000000 uniem-0.2.0/PKG-INFO
```

### Comparing `uniem-0.1.1/LICENSE` & `uniem-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.1.1/pyproject.toml` & `uniem-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniem"
-version = "0.1.1"
+version = "0.2.0"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uniem-0.1.1/uniem/criteria.py` & `uniem-0.2.0/uniem/criteria.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 
 class ContrastLoss(torch.nn.Module):
     def __init__(self, temperature: float = 0.05):
         super().__init__()
         self.temperature = temperature
 
 
-class PairCoSentLoss(ContrastLoss):
+class PairInBatchNegCoSentLoss(ContrastLoss):
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
     ) -> torch.Tensor:
         sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
         sim_matrix = sim_matrix / self.temperature
         sim_matrix_diag = sim_matrix.diag()
         sim_matrix_diff = sim_matrix - sim_matrix_diag.unsqueeze(1)
         loss = torch.logsumexp(sim_matrix_diff, dim=1).mean()
         return loss
 
 
-class TripletCoSentLoss(ContrastLoss):
+class TripletInBatchNegCoSentLoss(ContrastLoss):
     def __init__(self, temperature: float = 0.05, add_swap_loss: bool = False):
         super().__init__(temperature)
         self.add_swap_loss = add_swap_loss
         if self.add_swap_loss:
-            self._pair_contrast_softmax_loss = PairCoSentLoss(temperature)
+            self._pair_contrast_softmax_loss = PairInBatchNegCoSentLoss(temperature)
         else:
             self._pair_contrast_softmax_loss = None
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
@@ -43,15 +43,15 @@
         sim_matrix_diff = sim_matrix - sim_matrix[:, 0].unsqueeze(1)
         loss = torch.logsumexp(sim_matrix_diff, dim=1).mean()
         if self._pair_contrast_softmax_loss:
             loss += self._pair_contrast_softmax_loss(text_pos_embeddings, text_embeddings)
         return loss
 
 
-class PairSoftmaxContrastLoss(ContrastLoss):
+class PairInBatchNegSoftmaxContrastLoss(ContrastLoss):
     def __init__(self, temperature: float = 0.05):
         super().__init__()
         self.temperature = temperature
         self._cross_entropy_loss = torch.nn.CrossEntropyLoss()
 
     def forward(
         self,
@@ -61,20 +61,20 @@
         sim_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_pos_embeddings.unsqueeze(0), dim=-1)
         sim_matrix = sim_matrix / self.temperature
         labels = torch.arange(sim_matrix.size(0), device=text_embeddings.device, dtype=torch.long)
         loss = self._cross_entropy_loss(sim_matrix, labels)
         return loss
 
 
-class TripletSoftmaxContrastLoss(ContrastLoss):
+class TripletInBatchNegSoftmaxContrastLoss(ContrastLoss):
     def __init__(self, temperature: float = 0.05, add_swap_loss: bool = False):
         super().__init__(temperature)
         self.add_swap_loss = add_swap_loss
         if self.add_swap_loss:
-            self._pair_contrast_softmax_loss = PairSoftmaxContrastLoss(temperature)
+            self._pair_contrast_softmax_loss = PairInBatchNegSoftmaxContrastLoss(temperature)
         else:
             self._pair_contrast_softmax_loss = None
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
@@ -87,15 +87,15 @@
         labels = torch.zeros(sim_matrix.size(0), dtype=torch.long, device=sim_matrix.device)
         loss = torch.nn.CrossEntropyLoss()(sim_matrix, labels)
         if self._pair_contrast_softmax_loss:
             loss += self._pair_contrast_softmax_loss(text_pos_embeddings, text_embeddings)
         return loss
 
 
-class PairSigmoidContrastLoss(ContrastLoss):
+class PairInBatchNegSigmoidContrastLoss(ContrastLoss):
     def __init__(self, temperature: float = 0.05):
         super().__init__()
         self.temperature = temperature
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
@@ -110,20 +110,20 @@
         diag_mask = torch.eye(sim_matrix.size(0), dtype=torch.bool, device=sim_matrix.device)
         sim_diff_matrix = sim_diff_matrix.masked_fill(diag_mask, 1e9)
 
         loss = -torch.log(torch.sigmoid(sim_diff_matrix)).sum() / (batch_size**2 - batch_size)
         return loss
 
 
-class TripletSigmoidContrastLoss(ContrastLoss):
+class TripletInBatchNegSigmoidContrastLoss(ContrastLoss):
     def __init__(self, temperature: float = 0.05, add_swap_loss: bool = False):
         super().__init__(temperature)
         self.add_swap_loss = add_swap_loss
         if self.add_swap_loss:
-            self._pair_contrast_sigmoid_loss = PairSigmoidContrastLoss(temperature)
+            self._pair_contrast_sigmoid_loss = PairInBatchNegSigmoidContrastLoss(temperature)
         else:
             self._pair_contrast_sigmoid_loss = None
 
     def forward(
         self,
         text_embeddings: torch.Tensor,
         text_pos_embeddings: torch.Tensor,
@@ -134,7 +134,27 @@
         sim_neg_matrix = torch.cosine_similarity(text_embeddings.unsqueeze(1), text_neg_embeddings.unsqueeze(0), dim=-1)
         sim_neg_matrix = sim_neg_matrix / self.temperature
         sim_diff_matrix = sim_pos_vector.unsqueeze(1) - sim_neg_matrix
         loss = -torch.log(torch.sigmoid(sim_diff_matrix)).mean()
         if self._pair_contrast_sigmoid_loss:
             loss += self._pair_contrast_sigmoid_loss(text_pos_embeddings, text_embeddings)
         return loss
+
+
+class CoSentLoss(ContrastLoss):
+    bias: torch.Tensor
+
+    def __init__(self, temperature: float = 0.05) -> None:
+        super().__init__(temperature)
+        self.register_buffer('bias', torch.tensor([0.0]))
+
+    def forward(self, predict_similarity: torch.Tensor, true_similarity: torch.Tensor) -> torch.Tensor:
+        predict_similarity = predict_similarity / self.temperature
+
+        cosine_similarity_diff = -(predict_similarity.unsqueeze(0) - predict_similarity.unsqueeze(1))
+        smaller_mask = true_similarity.unsqueeze(0) <= true_similarity.unsqueeze(1)
+        cosine_similarity_diff = cosine_similarity_diff.masked_fill(smaller_mask, -1e12)
+
+        cosine_diff_scores_add_bias = torch.cat((cosine_similarity_diff.view(-1), self.bias))
+
+        loss = torch.logsumexp(cosine_diff_scores_add_bias, dim=0)
+        return loss
```

### Comparing `uniem-0.1.1/uniem/data.py` & `uniem-0.2.0/uniem/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from dataclasses import dataclass
 import json
 from collections import defaultdict
+from dataclasses import dataclass
 from pathlib import Path
-from typing import cast, Any
+from typing import Any, cast, Sequence
 
 import torch
 from torch.utils.data import Dataset, RandomSampler
-from datasets import Dataset as HfDataset
 
-from uniem.data_structures import PairRecord, TripletRecord
+from datasets import Dataset as HfDataset
+from uniem.data_structures import RecordType, PairRecord, ScoredPairRecord, TripletRecord, record_type_cls_map
 from uniem.types import Tokenizer
 
 
 class PairCollator:
     def __init__(self, tokenizer: Tokenizer, max_length: int | None = None) -> None:
         self.tokenizer = tokenizer
         self.max_length = max_length or tokenizer.model_max_length
@@ -83,14 +83,64 @@
         return {
             'text_ids': text_ids,
             'text_pos_ids': text_pos_ids,
             'text_neg_ids': text_neg_ids,
         }
 
 
+class ScoredPairCollator:
+    def __init__(self, tokenizer: Tokenizer, max_length: int | None = None) -> None:
+        self.tokenizer = tokenizer
+        self.max_length = max_length or tokenizer.model_max_length
+
+    def __call__(self, records: list[ScoredPairRecord]) -> dict[str, torch.Tensor]:
+        texts = [record.sentence1 for record in records]
+        texts_pair = [record.sentence2 for record in records]
+        labels = [record.label for record in records]
+        labels = torch.tensor(labels, dtype=torch.float32)
+
+        text_ids = self.tokenizer(
+            texts,
+            padding=True,
+            max_length=self.max_length,
+            truncation=True,
+            return_tensors='pt',
+        )['input_ids']
+        text_ids = cast(torch.Tensor, text_ids)
+
+        text_pair_ids = self.tokenizer(
+            texts_pair,
+            padding=True,
+            max_length=self.max_length,
+            truncation=True,
+            return_tensors='pt',
+        )['input_ids']
+        text_pair_ids = cast(torch.Tensor, text_pair_ids)
+
+        return {
+            'text_ids': text_ids,
+            'text_pair_ids': text_pair_ids,
+            'labels': labels,
+        }
+
+
+class FinetuneDataset(Dataset):
+    def __init__(self, dataset: HfDataset | Sequence[dict], record_type: RecordType | str) -> None:
+        self.dataset = dataset
+        self.record_type = RecordType(record_type)
+        self.record_cls = record_type_cls_map[self.record_type]
+
+    def __getitem__(self, index: int):
+        record = self.dataset[index]
+        return self.record_cls(**record)
+
+    def __len__(self):
+        return len(self.dataset)
+
+
 class MediDataset(Dataset):
     def __init__(
         self,
         medi_data_file: str | Path,
         batch_size: int = 32,
         pair_or_triplet: str = 'triplet',
         with_prompt: bool = True,
@@ -179,47 +229,41 @@
 class M3EDataset(Dataset):
     def __init__(
         self,
         m3e_hf_datasets: list[M3EHfDatsetWithInfo],
         batch_size: int = 32,
         with_instruction: bool = True,
         drop_last: bool = True,
+        max_samples: int | None = None,
     ):
         self.batch_size = batch_size
         self.drop_last = drop_last
         self.m3e_hf_datasets = m3e_hf_datasets
+        self.max_samples = max_samples
         self.name_dataset_map = {dataset.name: dataset.hf_dataset for dataset in m3e_hf_datasets}
         if with_instruction:
             self.task_instruction_map = {dataset.name: dataset.instruction for dataset in m3e_hf_datasets}
         else:
             self.task_instruction_map = None
         self.create_or_refresh_data()
 
     @staticmethod
     def is_valid_text(text: Any) -> bool:
         return isinstance(text, str) and bool(text.strip())
 
     def create_or_refresh_data(self):
-        batch_size = self.batch_size
         self.task_batch_index_list: list[TaskBatchIndex] = []
         for dataset in self.m3e_hf_datasets:
-            hf_dataset = dataset.hf_dataset
-            dataset_name = dataset.name
-            num_samples = (len(hf_dataset) // batch_size) * batch_size
-            if not self.drop_last and len(hf_dataset) % batch_size != 0:
-                num_samples += batch_size
-
-            if not num_samples:
-                continue
-
+            max_samples = self.max_samples or len(dataset.hf_dataset)
+            num_samples = (max_samples // self.batch_size) * self.batch_size
             buffer = []
-            for i in RandomSampler(hf_dataset, num_samples=num_samples):
+            for i in RandomSampler(dataset.hf_dataset, num_samples=num_samples):
                 buffer.append(i)
-                if len(buffer) == batch_size:
-                    self.task_batch_index_list.append(TaskBatchIndex(name=dataset_name, batch_index=buffer))
+                if len(buffer) == self.batch_size:
+                    self.task_batch_index_list.append(TaskBatchIndex(name=dataset.name, batch_index=buffer))
                     buffer = []
         self.random_index_list = list(RandomSampler(self.task_batch_index_list))
 
     def __getitem__(self, index: int):
         index = self.random_index_list[index]
         task_batch_index = self.task_batch_index_list[index]
         task_name = task_batch_index.name
```

### Comparing `uniem-0.1.1/uniem/model.py` & `uniem-0.2.0/uniem/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from enum import Enum
-from itertools import islice
 from pathlib import Path
-from typing import ClassVar, Generator, Iterable, Literal, Type, TypeVar, cast
+from typing import ClassVar, Literal, Type, TypeVar, cast
 
+import tqdm
 import torch
 import numpy as np
-import tqdm
-from transformers import AutoConfig, AutoModel, AutoTokenizer, PreTrainedModel
+from transformers import AutoTokenizer, AutoConfig, AutoModel, PreTrainedModel
 
 from uniem.criteria import (
-    PairSigmoidContrastLoss,
-    PairSoftmaxContrastLoss,
-    TripletSigmoidContrastLoss,
-    TripletSoftmaxContrastLoss,
-    PairCoSentLoss,
-    TripletCoSentLoss,
+    CoSentLoss,
+    PairInBatchNegCoSentLoss,
+    PairInBatchNegSigmoidContrastLoss,
+    PairInBatchNegSoftmaxContrastLoss,
+    TripletInBatchNegCoSentLoss,
+    TripletInBatchNegSigmoidContrastLoss,
+    TripletInBatchNegSoftmaxContrastLoss,
 )
 from uniem.types import Tokenizer
+from uniem.utils import generate_batch
 
 T = TypeVar('T')
 
 
-class EmbeddingStrategy(str, Enum):
+class PoolingStrategy(str, Enum):
     cls = 'cls'
     last_mean = 'last_mean'
     first_last_mean = 'first_last_mean'
     embedding_last_mean = 'embedding_last_mean'
     last_weighted = 'last_weighted'
 
 
-class LossType(str, Enum):
+class InBatchNegLossType(str, Enum):
     sigmoid = 'sigmoid'
     softmax = 'softmax'
     cosent = 'cosent'
 
 
 def creat_mask_from_input_ids(input_ids: torch.Tensor, pad_token_id: int) -> torch.Tensor:
     return input_ids != pad_token_id
@@ -53,35 +54,35 @@
 
         pretrained_model = T5EncoderModel.from_pretrained(model_name_or_path)
     else:
         pretrained_model = AutoModel.from_pretrained(model_name_or_path)
     return pretrained_model  # type: ignore
 
 
-StrategyEmbedderClsMap: dict[EmbeddingStrategy, Type['Embedder']] = {}
+StrategyEmbedderClsMap: dict[PoolingStrategy, Type['Embedder']] = {}
 
 
 class Embedder(torch.nn.Module):
-    embedding_strategy: ClassVar[EmbeddingStrategy]
+    pooling_strategy: ClassVar[PoolingStrategy]
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__()
         self.encoder = encoder
-        self.encoder.config.uniem_embedding_strategy = str(self.embedding_strategy.value)
+        self.encoder.config.uniem_pooling_strategy = str(self.pooling_strategy.value)
 
         if pad_token_id is None:
             if encoder.config.pad_token_id is not None:
                 self.pad_token_id = encoder.config.pad_token_id
             else:
                 self.pad_token_id = 0
         else:
             self.pad_token_id = pad_token_id
 
     def __init_subclass__(cls) -> None:
-        StrategyEmbedderClsMap[cls.embedding_strategy] = cls
+        StrategyEmbedderClsMap[cls.pooling_strategy] = cls
 
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
         raise NotImplementedError
 
     def save_pretrained(self, path: str | Path):
         self.encoder.save_pretrained(path)
 
@@ -92,47 +93,47 @@
 
     @property
     def max_length(self):
         return self.encoder.config.max_position_embeddings
 
 
 class LastMeanEmbedder(Embedder):
-    embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.last_mean
+    pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.last_mean
 
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
         if mask is None:
             mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
         embeddings = self.encoder(input_ids).last_hidden_state
         embeddings = mean_pooling(embeddings, mask)
         return embeddings
 
 
 class ClsEmbedder(Embedder):
-    embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.cls
+    pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.cls
 
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
         embeddings = self.encoder(input_ids).last_hidden_state[:, 0]
         return embeddings
 
 
 class FirstLastEmbedder(Embedder):
-    embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.first_last_mean
+    pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.first_last_mean
 
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
         if mask is None:
             mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
         embeddings = self.encoder(input_ids, output_hidden_states=True).hidden_states
         first_embeddings = mean_pooling(embeddings[0], mask)
         last_embeddings = mean_pooling(embeddings[-1], mask)
         embeddings = (first_embeddings + last_embeddings) / 2
         return embeddings
 
 
 class EmbeddingLastEmbedder(Embedder):
-    embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.embedding_last_mean
+    pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.embedding_last_mean
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__(encoder, pad_token_id)
         self.embedding_layer = self.encoder.get_input_embeddings()
 
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
         if mask is None:
@@ -140,15 +141,15 @@
         static_embeddings = self.embedding_layer(input_ids)
         mean_last_embeddings = mean_pooling(self.encoder(input_ids).last_hidden_state, mask)
         mean_static_embeddings = mean_pooling(static_embeddings, mask)
         return (mean_last_embeddings + mean_static_embeddings) / 2
 
 
 class LastWeightedEmbedder(Embedder):
-    embedding_strategy: ClassVar[EmbeddingStrategy] = EmbeddingStrategy.last_weighted
+    pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.last_weighted
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__(encoder, pad_token_id)
         self.embedding_layer = self.encoder.get_input_embeddings()
 
     def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
         if mask is None:
@@ -160,96 +161,132 @@
         return embeddings
 
 
 class AutoEmbedder:
     @classmethod
     def from_pretrained(cls, model_name_or_path: str | Path):
         encoder = load_hf_pretrained_model(str(model_name_or_path))
-        embedder_cls = StrategyEmbedderClsMap[EmbeddingStrategy(encoder.config.uniem_embedding_strategy)]
+        if hasattr(encoder.config, 'uniem_pooling_strategy'):
+            strategy_string = encoder.config.uniem_pooling_strategy
+        elif hasattr(encoder.config, 'uniem_embedding_strategy'):
+            strategy_string = encoder.config.uniem_embedding_strategy
+        else:
+            raise ValueError('Can not find uniem pooling strategy in config, Model is not trained by UniEmbedder.')
+        embedder_cls = StrategyEmbedderClsMap[PoolingStrategy(strategy_string)]
         return embedder_cls(encoder)
 
 
 class EmbedderForTrain(torch.nn.Module):
     def __init__(self, embedder: Embedder):
         super().__init__()
         self.embedder = embedder
 
 
-class EmbedderForPairTrain(EmbedderForTrain):
+class EmbedderForPairInBatchNegTrain(EmbedderForTrain):
     def __init__(
         self,
         model_name_or_path: str,
-        temperature: float = 0.05,
-        loss_type: LossType | str = LossType.softmax,
-        embedding_strategy: EmbeddingStrategy | str = EmbeddingStrategy.last_mean,
+        temperature: float | None = None,
+        loss_type: InBatchNegLossType | str = InBatchNegLossType.softmax,
+        embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
     ):
         pretrained_model = load_hf_pretrained_model(model_name_or_path)
-        embedder = StrategyEmbedderClsMap[EmbeddingStrategy(embedding_strategy)](pretrained_model)
+        embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
         super().__init__(embedder)
-        loss_type = LossType(loss_type)
-        if loss_type == LossType.sigmoid:
-            self.criterion = PairSigmoidContrastLoss(temperature)
-        elif loss_type == LossType.softmax:
-            self.criterion = PairSoftmaxContrastLoss(temperature)
-        elif loss_type == LossType.cosent:
-            self.criterion = PairCoSentLoss(temperature)
+        temperature = temperature or 0.05
+        self.loss_type = InBatchNegLossType(loss_type)
+        match self.loss_type:
+            case InBatchNegLossType.sigmoid:
+                self.criterion = PairInBatchNegSigmoidContrastLoss(temperature)
+            case InBatchNegLossType.softmax:
+                self.criterion = PairInBatchNegSoftmaxContrastLoss(temperature)
+            case InBatchNegLossType.cosent:
+                self.criterion = PairInBatchNegCoSentLoss(temperature)
 
     def forward(self, text_ids: torch.Tensor, text_pos_ids: torch.Tensor) -> dict[str, torch.Tensor]:
         text_embeddings = self.embedder(text_ids)
         text_pos_embeddings = self.embedder(text_pos_ids)
         loss = self.criterion(text_embeddings, text_pos_embeddings)
         return {'loss': loss}
 
 
-class EmbedderForTripletTrain(EmbedderForTrain):
+class EmbedderForTripletInBatchNegTrain(EmbedderForTrain):
     def __init__(
         self,
         model_name_or_path: str,
-        temperature: float = 0.05,
-        loss_type: LossType | str = LossType.softmax,
-        embedding_strategy: EmbeddingStrategy | str = EmbeddingStrategy.last_mean,
+        temperature: float | None = None,
+        loss_type: InBatchNegLossType | str = InBatchNegLossType.softmax,
+        embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
         add_swap_loss: bool = False,
     ):
         pretrained_model = load_hf_pretrained_model(model_name_or_path)
-        embedder = StrategyEmbedderClsMap[EmbeddingStrategy(embedding_strategy)](pretrained_model)
+        embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
         super().__init__(embedder)
-        loss_type = LossType(loss_type)
-        if loss_type == LossType.sigmoid:
-            self.criterion = TripletSigmoidContrastLoss(temperature, add_swap_loss)
-        elif loss_type == LossType.softmax:
-            self.criterion = TripletSoftmaxContrastLoss(temperature, add_swap_loss)
-        elif loss_type == LossType.cosent:
-            self.criterion = TripletCoSentLoss(temperature, add_swap_loss)
+        temperature = temperature or 0.05
+        self.loss_type = InBatchNegLossType(loss_type)
+        match self.loss_type:
+            case InBatchNegLossType.sigmoid:
+                self.criterion = TripletInBatchNegSigmoidContrastLoss(temperature, add_swap_loss)
+            case InBatchNegLossType.softmax:
+                self.criterion = TripletInBatchNegSoftmaxContrastLoss(temperature, add_swap_loss)
+            case InBatchNegLossType.cosent:
+                self.criterion = TripletInBatchNegCoSentLoss(temperature, add_swap_loss)
 
     def forward(
         self, text_ids: torch.Tensor, text_pos_ids: torch.Tensor, text_neg_ids: torch.Tensor
     ) -> dict[str, torch.Tensor]:
         text_embeddings = self.embedder(text_ids)
         text_pos_embeddings = self.embedder(text_pos_ids)
         text_neg_embeddings = self.embedder(text_neg_ids)
         loss = self.criterion(text_embeddings, text_pos_embeddings, text_neg_embeddings)
         return {'loss': loss}
 
 
-def generate_batch(data: Iterable[T], batch_size: int = 32) -> Generator[list[T], None, None]:
-    iterator = iter(data)
-    while batch := list(islice(iterator, batch_size)):
-        yield batch
+class EmbedderForScoredPairTrain(EmbedderForTrain):
+    def __init__(
+        self,
+        model_name_or_path: str,
+        temperature: float | None = None,
+        embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
+    ):
+        pretrained_model = load_hf_pretrained_model(model_name_or_path)
+        embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
+        super().__init__(embedder)
+        temperature = temperature or 0.05
+        self.criterion = CoSentLoss(temperature)
+
+    def forward(self, text_ids: torch.Tensor, text_pair_ids: torch.Tensor, labels: torch.Tensor) -> dict[str, torch.Tensor]:
+        text_embeddings = self.embedder(text_ids)
+        text_pos_embeddings = self.embedder(text_pair_ids)
+        predict_labels = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
+        loss = self.criterion(predict_labels, labels)
+        return {'loss': loss, 'predict_labels': predict_labels}
 
 
 class UniEmbedder:
     PROGRESS_BAR_THRESHOLD = 1000
 
-    def __init__(self, embedder: Embedder, tokenizer: Tokenizer, max_length: int | None = None, device: str | None = None):
+    def __init__(
+        self,
+        embedder: Embedder,
+        tokenizer: Tokenizer,
+        normalize: bool = True,
+        max_length: int | None = None,
+        device: str | None = None,
+    ):
         super().__init__()
         self.embedder = embedder.eval()
-        if device:
-            self.embedder = self.embedder.to(device)
+        if device is None:
+            device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.embedder = self.embedder.to(device)
         self.tokenizer = tokenizer
-        self.max_length = max_length or self.embedder.encoder.config.max_length
+        self.normalize = normalize
+        self.max_length = (
+            max_length or self.embedder.encoder.config.max_length or self.embedder.encoder.config.max_position_embeddings
+        )
 
     def __call__(self, sentences: list[str], batch_size: int = 32):
         return self.encode(sentences, batch_size)
 
     def encode(self, sentences: list[str], batch_size: int = 32, progress_bar: Literal['auto'] | bool = 'auto'):
         embeddings: list[np.ndarray] = []
         if progress_bar == 'auto':
@@ -277,25 +314,25 @@
 
             attention_mask = encodes['attention_mask']
             attention_mask = cast(torch.Tensor, attention_mask)
             attention_mask = attention_mask.to(self.embedder.encoder.device)
 
             with torch.inference_mode():
                 batch_embeddings = self.embedder(input_ids, mask=attention_mask)
+                if self.normalize:
+                    batch_embeddings = torch.nn.functional.normalize(batch_embeddings, dim=-1)
                 batch_embeddings = cast(torch.Tensor, batch_embeddings)
             embeddings.extend([i.cpu().numpy() for i in batch_embeddings])
         return embeddings
 
     def encode_single(self, sentence: str):
         return self.encode([sentence])[0]
 
     @classmethod
-    def from_pretrained(cls, model_name_or_path: str, max_length: int | None = None, device: str | None = None):
+    def from_pretrained(cls, model_name_or_path: str, **kwargs):
         encoder = AutoEmbedder.from_pretrained(model_name_or_path)
         tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
-        if device is None:
-            device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        return cls(encoder, tokenizer, max_length=max_length, device=device)
+        return cls(encoder, tokenizer, **kwargs)
 
     def save_pretrained(self, ouptut_dir: str):
         self.embedder.save_pretrained(ouptut_dir)
         self.tokenizer.save_pretrained(ouptut_dir)
```

### Comparing `uniem-0.1.1/uniem/trainer.py` & `uniem-0.2.0/uniem/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Any
 
 import torch
-import tqdm
+from tqdm.auto import tqdm
 from accelerate import Accelerator
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from torch.utils.data import DataLoader
 
 
 class Trainer:
@@ -119,15 +119,15 @@
         self.epochs = epochs
         self.current_epoch = 1
         self.num_steps_per_epoch = num_steps_per_epoch
         self.tqdm_kwargs = kwargs
 
     def on_epoch_start(self):
         if self.accelerator.is_main_process:
-            self.progress_bar = tqdm.tqdm(total=self.num_steps_per_epoch, **self.tqdm_kwargs)
+            self.progress_bar = tqdm(total=self.num_steps_per_epoch, **self.tqdm_kwargs)
         else:
             self.progress_bar = DummyProgressBar()
 
     def update(self, n: int = 1) -> None:
         self.progress_bar.update(n)
 
     def close(self) -> None:
```

### Comparing `uniem-0.1.1/uniem/types.py` & `uniem-0.2.0/uniem/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Callable, TypeAlias
 
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.tokenization_utils_fast import PreTrainedTokenizerFast
+
 from datasets import DatasetDict
 
 Tokenizer: TypeAlias = PreTrainedTokenizer | PreTrainedTokenizerFast
 
 
 class MixedPrecisionType(str, Enum):
     fp16 = 'fp16'
@@ -16,15 +17,14 @@
 
 
 @dataclass
 class DatasetDescription:
     name: str
     is_symmetric: bool
     domains: list[str]
-    raw_size: int
     instruction_type: str
 
 
 @dataclass
 class UniemDataset:
-    load_fn: Callable[[bool], DatasetDict]
+    load_fn: Callable[[], DatasetDict]
     description: DatasetDescription
```

