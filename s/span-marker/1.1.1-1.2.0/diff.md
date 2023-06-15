# Comparing `tmp/span_marker-1.1.1.tar.gz` & `tmp/span_marker-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-1.1.1.tar", last modified: Tue Jun 13 13:15:24 2023, max compression
+gzip compressed data, was "span_marker-1.2.0.tar", last modified: Thu Jun 15 19:59:21 2023, max compression
```

## Comparing `span_marker-1.1.1.tar` & `span_marker-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.035314 span_marker-1.1.1/
--rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     7875 2023-06-13 13:15:24.034295 span_marker-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7298 2023-06-01 10:38:31.000000 span_marker-1.1.1/README.md
--rw-rw-rw-   0        0        0     2455 2023-06-10 13:15:43.000000 span_marker-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 13:15:24.035314 span_marker-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.025295 span_marker-1.1.1/span_marker/
--rw-rw-rw-   0        0        0      446 2023-06-13 13:12:22.000000 span_marker-1.1.1/span_marker/__init__.py
--rw-rw-rw-   0        0        0     7018 2023-06-10 13:15:43.000000 span_marker-1.1.1/span_marker/configuration.py
--rw-rw-rw-   0        0        0     6630 2023-06-13 12:59:46.000000 span_marker-1.1.1/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     5066 2023-06-10 13:15:43.000000 span_marker-1.1.1/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.1.1/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     2472 2023-06-10 15:07:22.000000 span_marker-1.1.1/span_marker/model_card.py
--rw-rw-rw-   0        0        0    30304 2023-06-13 13:02:18.000000 span_marker-1.1.1/span_marker/modeling.py
--rw-rw-rw-   0        0        0     2221 2023-06-10 13:15:43.000000 span_marker-1.1.1/span_marker/output.py
--rw-rw-rw-   0        0        0    11885 2023-06-13 12:59:46.000000 span_marker-1.1.1/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    19774 2023-06-13 12:59:46.000000 span_marker-1.1.1/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.030294 span_marker-1.1.1/span_marker.egg-info/
--rw-rw-rw-   0        0        0     7875 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-06-13 13:15:24.000000 span_marker-1.1.1/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.034295 span_marker-1.1.1/tests/
--rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.1.1/tests/test_configuration.py
--rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.1.1/tests/test_model_card.py
--rw-rw-rw-   0        0        0     8329 2023-06-13 13:09:20.000000 span_marker-1.1.1/tests/test_modeling.py
--rw-rw-rw-   0        0        0     8733 2023-06-10 13:15:43.000000 span_marker-1.1.1/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.172128 span_marker-1.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    15026 2023-06-15 19:59:21.171128 span_marker-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14458 2023-06-15 19:51:37.000000 span_marker-1.2.0/README.md
+-rw-rw-rw-   0        0        0     2521 2023-06-15 19:58:36.000000 span_marker-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:59:21.172128 span_marker-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.158129 span_marker-1.2.0/span_marker/
+-rw-rw-rw-   0        0        0     1659 2023-06-15 19:56:29.000000 span_marker-1.2.0/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     7070 2023-06-15 09:34:01.000000 span_marker-1.2.0/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     6630 2023-06-13 22:30:33.000000 span_marker-1.2.0/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     5276 2023-06-15 14:37:15.000000 span_marker-1.2.0/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.2.0/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     2472 2023-06-13 22:30:43.000000 span_marker-1.2.0/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    31490 2023-06-15 10:02:14.000000 span_marker-1.2.0/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     2221 2023-06-13 22:30:33.000000 span_marker-1.2.0/span_marker/output.py
+-rw-rw-rw-   0        0        0     3914 2023-06-15 15:56:41.000000 span_marker-1.2.0/span_marker/spacy_integration.py
+-rw-rw-rw-   0        0        0    11828 2023-06-15 06:57:10.000000 span_marker-1.2.0/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    21019 2023-06-15 10:02:14.000000 span_marker-1.2.0/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.167128 span_marker-1.2.0/span_marker.egg-info/
+-rw-rw-rw-   0        0        0    15026 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 19:59:21.000000 span_marker-1.2.0/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 19:59:21.170128 span_marker-1.2.0/tests/
+-rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.2.0/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.2.0/tests/test_model_card.py
+-rw-rw-rw-   0        0        0     9228 2023-06-15 09:34:01.000000 span_marker-1.2.0/tests/test_modeling.py
+-rw-rw-rw-   0        0        0    10372 2023-06-15 09:34:01.000000 span_marker-1.2.0/tests/test_trainer.py
```

### Comparing `span_marker-1.1.1/LICENSE` & `span_marker-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.1/pyproject.toml` & `span_marker-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "span_marker"
-description = "Few-Shot Named Entity Recognition using Span Markers"
+description = "Named Entity Recognition using Span Markers"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = [
     "data-science",
     "natural-language-processing",
     "artificial-intelligence",
@@ -38,25 +38,27 @@
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "ruff",
     "black",
     "pytest",
-    "pytest-cov"
+    "pytest-cov",
+    "spacy"
 ]
 docs = [
     "nltk_theme",
     "sphinx",
     "m2r2",
     "better-apidoc",
     "nbsphinx",
     "nbconvert<7",
     "pandoc<3",
-    "ipython"
+    "ipython",
+    "spacy" # Required to build the spaCy integration docs
 ]
 wandb = [
     "wandb"
 ]
 
 [project.urls]
 Documentation = "https://tomaarsen.github.io/SpanMarkerNER"
```

### Comparing `span_marker-1.1.1/span_marker/configuration.py` & `span_marker-1.2.0/span_marker/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         self.encoder = encoder_config
         self.model_max_length = model_max_length
         self.model_max_length_default = 512
         self.marker_max_length = marker_max_length
         self.entity_max_length = entity_max_length
         self.max_prev_context = max_prev_context
         self.max_next_context = max_next_context
+        self.trained_with_document_context = False
         self.span_marker_version = kwargs.pop("span_marker_version", None)
         super().__init__(**kwargs)
 
         # label2id and id2label are automatically set by super().__init__, but we want to rely on
         # the encoder configs instead if we can, so we delete them under two conditions
         # 1. if they're the default ({0: "LABEL_0", 1: "LABEL_1"})
         # 2. if they're identical to the encoder label2id
```

### Comparing `span_marker-1.1.1/span_marker/data_collator.py` & `span_marker-1.2.0/span_marker/data_collator.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.1/span_marker/evaluation.py` & `span_marker-1.2.0/span_marker/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,30 @@
 
     # Collect all samples in one dict. We do this because some samples are spread between multiple inputs
     sample_list = []
     for sample_idx in range(inputs.shape[0]):
         tokens = inputs[sample_idx]
         text = tokenizer.decode(tokens, skip_special_tokens=True)
         token_hash = hash(text) if not has_document_context else (document_ids[sample_idx], sentence_ids[sample_idx])
-        if not sample_list or sample_list[-1]["hash"] != token_hash:
+        if (
+            not sample_list
+            or sample_list[-1]["hash"] != token_hash
+            or len(sample_list[-1]["spans"]) == len(sample_list[-1]["gold_labels"])
+        ):
             mask = gold_labels[sample_idx] != -100
+            spans = list(tokenizer.get_all_valid_spans(num_words[sample_idx], tokenizer.config.entity_max_length))
             sample_list.append(
                 {
                     "text": text,
                     "gold_labels": gold_labels[sample_idx][mask].tolist(),
                     "pred_labels": pred_labels[sample_idx][mask].tolist(),
                     "scores": scores[sample_idx].tolist(),
                     "num_words": num_words[sample_idx],
                     "hash": token_hash,
+                    "spans": spans,
                 }
             )
         else:
             mask = gold_labels[sample_idx] != -100
             sample_list[-1]["gold_labels"] += gold_labels[sample_idx][mask].tolist()
             sample_list[-1]["pred_labels"] += pred_labels[sample_idx][mask].tolist()
             sample_list[-1]["scores"] += scores[sample_idx].tolist()
@@ -64,15 +70,15 @@
     outside_id = tokenizer.config.outside_id
     id2label = tokenizer.config.id2label
     # seqeval works wonders for NER evaluation
     seqeval = evaluate.load("seqeval")
     for sample in sample_list:
         scores = sample["scores"]
         num_words = sample["num_words"]
-        spans = list(tokenizer.get_all_valid_spans(num_words, tokenizer.config.entity_max_length))
+        spans = sample["spans"]
         gold_labels = sample["gold_labels"]
         pred_labels = sample["pred_labels"]
         assert len(gold_labels) == len(pred_labels) and len(spans) == len(pred_labels)
 
         # Construct IOB2 format for gold labels, useful for seqeval
         gold_labels_per_tokens = ["O"] * num_words
         for span, gold_label in zip(spans, gold_labels):
```

### Comparing `span_marker-1.1.1/span_marker/label_normalizer.py` & `span_marker-1.2.0/span_marker/label_normalizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.1/span_marker/model_card.py` & `span_marker-1.2.0/span_marker/model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.1/span_marker/modeling.py` & `span_marker-1.2.0/span_marker/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import os
 import re
-import warnings
 from typing import Callable, Dict, List, Optional, Type, TypeVar, Union
 
 import torch
 import torch.nn.functional as F
-from datasets import Dataset
+from datasets import Dataset, disable_progress_bar, enable_progress_bar
 from packaging.version import Version, parse
 from torch import device, nn
 from tqdm.autonotebook import trange
 from transformers import AutoConfig, AutoModel, PretrainedConfig, PreTrainedModel
 from typing_extensions import Self
 
 from span_marker import __version__ as span_marker_version
@@ -318,15 +317,18 @@
                     return SpanMarkerModel._load_encoder_with_kwargs(
                         pretrained_model_name_or_path, config, *model_args, **kwargs
                     )
             # Otherwise, just raise the exception
             raise exc
 
     def predict(
-        self, inputs: Union[str, List[str], List[List[str]], Dataset], batch_size: int = 4
+        self,
+        inputs: Union[str, List[str], List[List[str]], Dataset],
+        batch_size: int = 4,
+        show_progress_bar: bool = False,
     ) -> Union[List[Dict[str, Union[str, int, float]]], List[List[Dict[str, Union[str, int, float]]]]]:
         """Predict named entities from input texts.
 
         Example::
 
             >>> model = SpanMarkerModel.from_pretrained(...)
             >>> model.predict("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
@@ -347,14 +349,18 @@
                 * str: a string sentence.
                 * List[str]: a pre-tokenized string sentence, i.e. a list of words.
                 * List[str]: a list of multiple string sentences.
                 * List[List[str]]: a list of multiple pre-tokenized string sentences, i.e. a list with lists of words.
                 * Dataset: A 🤗 :class:`~datasets.Dataset` with a ``tokens`` column and optionally ``document_id`` and ``sentence_id`` columns.
                     If the optional columns are provided, they will be used to provide document-level context.
 
+            batch_size (int): The number of samples to include in a batch, a higher batch size is faster,
+                but requires more memory. Defaults to 4
+            show_progress_bar (bool): Whether to show a progress bar, useful for longer inputs. Defaults to `False`.
+
         Returns:
             Union[List[Dict[str, Union[str, int, float]]], List[List[Dict[str, Union[str, int, float]]]]]:
                 If the input is a single sentence, then we output a list of dictionaries. Each dictionary
                 represents one predicted entity, and contains the following keys:
 
                 * ``label``: The predicted entity label.
                 * ``span``: The text that the model deems an entity.
@@ -365,20 +371,18 @@
                   if the input is a string.
 
                 If the input is multiple sentences, then we return a list containing multiple of the aforementioned lists.
         """
         from span_marker.trainer import Trainer
 
         if torch.cuda.is_available() and self.device == torch.device("cpu"):
-            warnings.warn(
+            logger.warn(
                 "SpanMarker model predictions are being computed on the CPU while CUDA is available."
                 " Moving the model to CUDA using `model.cuda()` before performing predictions is heavily"
                 " recommended to significantly boost prediction speeds.",
-                UserWarning,
-                stacklevel=2,
             )
 
         # Disable dropout, etc.
         self.eval()
 
         if not inputs:
             return []
@@ -428,40 +432,57 @@
         ]
 
         # Tokenize & add start/end markers
         tokenizer_dict = self.tokenizer(
             {"tokens": dataset["tokens"]}, return_num_words=True, return_batch_encoding=True
         )
         batch_encoding = tokenizer_dict.pop("batch_encoding")
+        dataset = dataset.remove_columns("tokens")
         for key, value in tokenizer_dict.items():
             dataset = dataset.add_column(key, value)
         # Add context if possible
         if {"document_id", "sentence_id"} <= set(dataset.column_names):
+            if not self.config.trained_with_document_context:
+                logger.warning(
+                    "This model was trained without document-level context: "
+                    "inference with document-level context may cause decreased performance."
+                )
             # Add column to be able to revert sorting later
             dataset = dataset.add_column("__sort_id", range(len(dataset)))
             # Sorting by doc ID and then sentence ID is required for add_context
             dataset = dataset.sort(column_names=["document_id", "sentence_id"])
             dataset = Trainer.add_context(
                 dataset,
                 self.tokenizer.model_max_length,
                 max_prev_context=self.config.max_prev_context,
                 max_next_context=self.config.max_next_context,
+                show_progress_bar=show_progress_bar,
             )
             dataset = dataset.sort(column_names=["__sort_id"])
             dataset = dataset.remove_columns("__sort_id")
+        elif self.config.trained_with_document_context:
+            logger.warning(
+                "This model was trained with document-level context: "
+                "inference without document-level context may cause decreased performance."
+            )
 
+        if not show_progress_bar:
+            disable_progress_bar()
         dataset = dataset.map(
-            lambda sample: Trainer.spread_sample(
-                self.tokenizer.model_max_length, self.config.marker_max_length, sample
-            ),
+            Trainer.spread_sample,
             batched=True,
-            batch_size=1,
             desc="Spreading data between multiple samples",
+            fn_kwargs={
+                "model_max_length": self.tokenizer.model_max_length,
+                "marker_max_length": self.config.marker_max_length,
+            },
         )
-        for batch_start_idx in trange(0, len(dataset), batch_size):
+        if not show_progress_bar:
+            enable_progress_bar()
+        for batch_start_idx in trange(0, len(dataset), batch_size, leave=True, disable=not show_progress_bar):
             batch = dataset.select(range(batch_start_idx, min(len(dataset), batch_start_idx + batch_size)))
             # Expanding the small tokenized output into full-scale input_ids, position_ids and attention_mask matrices.
             batch = self.data_collator(batch)
             # Moving the inputs to the right device
             batch = {key: value.to(self.device) for key, value in batch.items()}
             with torch.no_grad():
                 output = self(**batch)
```

### Comparing `span_marker-1.1.1/span_marker/output.py` & `span_marker-1.2.0/span_marker/output.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.1/span_marker/tokenizer.py` & `span_marker-1.2.0/span_marker/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __call__(self, split: Optional[str] = None) -> None:
         """Update the current split, which affects the warning message.
 
         Example:
 
             with tokenizer.entity_tracker(split=dataset_name):
                 dataset = dataset.map(
-                    lambda batch: tokenizer(batch["tokens"], labels=batch["ner_tags"]),
+                    tokenizer,
                     ...
                 )
 
         Args:
             split (Optional[str]): The new split string, either "train", "evaluation" or "test". Defaults to None.
 
         Returns:
```

### Comparing `span_marker-1.1.1/span_marker/trainer.py` & `span_marker-1.2.0/span_marker/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,17 @@
         )
         # We have to provide the __init__ with None for model_init and then override it here again
         # We do this because we need `model` to already be defined in this SpanMarker Trainer class
         # and the Transformers Trainer would complain if we provide both a model and a model_init
         # in its __init__.
         self.model_init = model_init
 
+        # Override the type hint
+        self.model: SpanMarkerModel
+
     def preprocess_dataset(
         self,
         dataset: Dataset,
         label_normalizer: LabelNormalizer,
         tokenizer: SpanMarkerTokenizer,
         dataset_name: str = "train",
         is_evaluate: bool = False,
@@ -175,38 +178,54 @@
             label_normalizer,
             input_columns=("tokens", "ner_tags"),
             desc=f"Label normalizing the {dataset_name} dataset",
         )
         # Tokenize and add start/end markers
         with tokenizer.entity_tracker(split=dataset_name):
             dataset = dataset.map(
-                lambda batch: tokenizer(batch, return_num_words=is_evaluate),
+                tokenizer,
                 batched=True,
                 remove_columns=set(dataset.column_names) - set(self.OPTIONAL_COLUMNS),
                 desc=f"Tokenizing the {dataset_name} dataset",
+                fn_kwargs={"return_num_words": is_evaluate},
             )
         # If "document_id" AND "sentence_id" exist in the training dataset
         if {"document_id", "sentence_id"} <= set(dataset.column_names):
+            # If training, set the config flag that this model is trained with document context
+            if not is_evaluate:
+                self.model.config.trained_with_document_context = True
+            # If evaluating and the model was not trained with document context, warn
+            elif not self.model.config.trained_with_document_context:
+                logger.warning(
+                    "This model was trained without document-level context: "
+                    "evaluation with document-level context may cause decreased performance."
+                )
             dataset = dataset.sort(column_names=["document_id", "sentence_id"])
-            # TODO: Sort the dataset
             dataset = self.add_context(
                 dataset,
                 tokenizer.model_max_length,
                 max_prev_context=self.model.config.max_prev_context,
                 max_next_context=self.model.config.max_next_context,
             )
+        elif is_evaluate and self.model.config.trained_with_document_context:
+            logger.warning(
+                "This model was trained with document-level context: "
+                "evaluation without document-level context may cause decreased performance."
+            )
+
         # Spread between multiple samples where needed
         original_length = len(dataset)
         dataset = dataset.map(
-            lambda sample: Trainer.spread_sample(
-                tokenizer.model_max_length, self.model.config.marker_max_length, sample
-            ),
+            Trainer.spread_sample,
             batched=True,
-            batch_size=1,
             desc="Spreading data between multiple samples",
+            fn_kwargs={
+                "model_max_length": tokenizer.model_max_length,
+                "marker_max_length": self.model.config.marker_max_length,
+            },
         )
         new_length = len(dataset)
         logger.info(
             f"Spread {original_length} sentences across {new_length} samples, "
             f"a {(new_length / original_length) - 1:%} increase. You can increase "
             "`model_max_length` or `marker_max_length` to decrease the number of samples, "
             "but recognize that longer samples are slower."
@@ -215,35 +234,41 @@
 
     @staticmethod
     def add_context(
         dataset: Dataset,
         model_max_length: int,
         max_prev_context: Optional[int] = None,
         max_next_context: Optional[int] = None,
+        show_progress_bar: bool = True,
     ) -> Dataset:
         """Add document-level context from previous and next sentences in the same document.
 
         Args:
             dataset (`Dataset`): The partially processed dataset, containing `"input_ids"`, `"start_position_ids"`,
                 `"end_position_ids"`, `"document_id"` and `"sentence_id"` columns.
             model_max_length (`int`): The total number of tokens that can be processed before
                 truncation.
             max_prev_context (`Optional[int]`): The maximum number of previous sentences to include. Defaults to None,
                 representing as many previous sentences as fits.
             max_next_context (`Optional[int]`): The maximum number of next sentences to include. Defaults to None,
                 representing as many previous sentences as fits.
+            show_progress_bar (`bool`): Whether to show a progress bar. Defaults to `True`.
 
         Returns:
             Dataset: A copy of the Dataset with additional previous and next sentences added to input_ids.
         """
         all_input_ids = []
         all_start_position_ids = []
         all_end_position_ids = []
         for sample_idx, sample in tqdm(
-            enumerate(dataset), desc="Adding document-level context", total=len(dataset), leave=False
+            enumerate(dataset),
+            desc="Adding document-level context",
+            total=len(dataset),
+            leave=False,
+            disable=not show_progress_bar,
         ):
             # Sequentially add next context, previous context, next context, previous context, etc. until
             # max token length or max_prev/next_context
             tokens = sample["input_ids"][1:-1]
             start_position_ids = sample["start_position_ids"]
             end_position_ids = sample["end_position_ids"]
 
@@ -295,47 +320,50 @@
         dataset = dataset.add_column("start_position_ids", all_start_position_ids)
         dataset = dataset.add_column("end_position_ids", all_end_position_ids)
 
         return dataset
 
     @staticmethod
     def spread_sample(
-        model_max_length: int, marker_max_length: int, sample: Dict[str, List[Any]]
+        batch: Dict[str, List[Any]], model_max_length: int, marker_max_length: int
     ) -> Dict[str, List[Any]]:
         """Spread sentences between multiple samples if lack of space per sample requires it.
 
         Args:
+            batch (`Dict[str, List[Any]]`): A dictionary of dataset keys to lists of values.
             model_max_length (`int`): The total number of tokens that can be processed before
                 truncation.
             marker_max_length (`int`): The maximum length for each of the span markers. A value of 128
                 means that each training and inferencing sample contains a maximum of 128 start markers
                 and 128 end markers, for a total of 256 markers per sample.
-            sample (`Dict[str, List[Any]]`): A dictionary of dataset keys to singleton lists
-                of values.
 
         Returns:
-            Dict[str, List[Any]]: A dictionary of dataset keys to not strictly singleton lists
-                of values.
+            Dict[str, List[Any]]: A dictionary of dataset keys to lists of values.
         """
-        sample = {key: value[0] for key, value in sample.items()}
+        keys = batch.keys()
+        values = batch.values()
         total_sample_length = model_max_length + 2 * marker_max_length
-        sample_marker_space = (total_sample_length - len(sample["input_ids"])) // 2
-        spread_between_n = math.ceil(len(sample["start_position_ids"]) / sample_marker_space)
-        spread_samples = []
-        for i in range(spread_between_n):
-            sample_copy = sample.copy()
-            start = i * sample_marker_space
-            end = (i + 1) * sample_marker_space
-            sample_copy["start_position_ids"] = sample["start_position_ids"][start:end]
-            sample_copy["end_position_ids"] = sample["end_position_ids"][start:end]
-            if "labels" in sample:
-                sample_copy["labels"] = sample["labels"][start:end]
-            sample_copy["num_spans"] = len(sample_copy["start_position_ids"])
-            spread_samples.append(sample_copy)
-        return {key: [one_sample[key] for one_sample in spread_samples] for key in sample.keys()}
+
+        batch_samples = {key: [] for key in keys}
+        for sample in zip(*values):
+            sample = dict(zip(keys, sample))
+            sample_marker_space = (total_sample_length - len(sample["input_ids"])) // 2
+            spread_between_n = math.ceil(len(sample["start_position_ids"]) / sample_marker_space)
+            for i in range(spread_between_n):
+                sample_copy = sample.copy()
+                start = i * sample_marker_space
+                end = (i + 1) * sample_marker_space
+                sample_copy["start_position_ids"] = sample["start_position_ids"][start:end]
+                sample_copy["end_position_ids"] = sample["end_position_ids"][start:end]
+                if "labels" in sample:
+                    sample_copy["labels"] = sample["labels"][start:end]
+                sample_copy["num_spans"] = len(sample_copy["start_position_ids"])
+                for key, value in sample_copy.items():
+                    batch_samples[key].append(value)
+        return batch_samples
 
     def get_train_dataloader(self) -> DataLoader:
         """Return the preprocessed training DataLoader."""
         self.train_dataset = self.preprocess_dataset(self.train_dataset, self.label_normalizer, self.tokenizer)
         return super().get_train_dataloader()
 
     def get_eval_dataloader(self, eval_dataset: Optional[Dataset] = None) -> DataLoader:
```

### Comparing `span_marker-1.1.1/span_marker.egg-info/SOURCES.txt` & `span_marker-1.2.0/span_marker.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 span_marker/configuration.py
 span_marker/data_collator.py
 span_marker/evaluation.py
 span_marker/label_normalizer.py
 span_marker/model_card.py
 span_marker/modeling.py
 span_marker/output.py
+span_marker/spacy_integration.py
 span_marker/tokenizer.py
 span_marker/trainer.py
 span_marker.egg-info/PKG-INFO
 span_marker.egg-info/SOURCES.txt
 span_marker.egg-info/dependency_links.txt
 span_marker.egg-info/requires.txt
 span_marker.egg-info/top_level.txt
```

### Comparing `span_marker-1.1.1/tests/test_configuration.py` & `span_marker-1.2.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.1/tests/test_model_card.py` & `span_marker-1.2.0/tests/test_model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.1/tests/test_modeling.py` & `span_marker-1.2.0/tests/test_modeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import re
 from typing import Dict, List, Optional, Union
 
 import pytest
 import torch
 from datasets import Dataset
 
@@ -75,14 +76,15 @@
         ),
     ],
 )
 def test_correct_predictions(
     finetuned_conll_span_marker_model: SpanMarkerModel,
     inputs: Union[str, List[str]],
     gold_entities: List[Dict[str, Union[str, int]]],
+    caplog: pytest.LogCaptureFixture,
 ) -> None:
     model = finetuned_conll_span_marker_model.try_cuda()
 
     # Single sentence
     pred_entities = model.predict(inputs)
     compare_entities(pred_entities, gold_entities)
 
@@ -102,14 +104,27 @@
         compare_entities(pred_entities, gold_entities)
 
     # As a non-singular Dataset
     pred_entity_list = model.predict(Dataset.from_dict({"tokens": [inputs] * 2}))
     for pred_entities in pred_entity_list:
         compare_entities(pred_entities, gold_entities)
 
+    # Check for warning if the model is trained with document-level context
+    caplog.clear()
+    model.config.trained_with_document_context = True
+    model.predict(inputs)
+    assert any(
+        [
+            level == logging.WARNING
+            and text == "This model was trained with document-level context: "
+            "inference without document-level context may cause decreased performance."
+            for (_, level, text) in caplog.record_tuples
+        ]
+    )
+
 
 @pytest.mark.parametrize(
     ("inputs", "gold_entity_list"),
     [
         (
             Dataset.from_dict(
                 {
@@ -158,21 +173,31 @@
         ),
     ],
 )
 def test_correct_predictions_with_document_level_context(
     finetuned_conll_span_marker_model: SpanMarkerModel,
     inputs: Union[str, List[str]],
     gold_entity_list: List[Dict[str, Union[str, int]]],
+    caplog: pytest.LogCaptureFixture,
 ) -> None:
     model = finetuned_conll_span_marker_model.try_cuda()
 
     pred_entity_list = model.predict(inputs)
     for pred_entities, gold_entities in zip(pred_entity_list, gold_entity_list):
         compare_entities(pred_entities, gold_entities)
 
+    assert any(
+        [
+            level == logging.WARNING
+            and text == "This model was trained without document-level context: "
+            "inference with document-level context may cause decreased performance."
+            for (_, level, text) in caplog.record_tuples
+        ]
+    )
+
 
 def test_incorrect_predict_inputs(finetuned_conll_span_marker_model: SpanMarkerModel):
     model = finetuned_conll_span_marker_model.try_cuda()
     with pytest.raises(ValueError, match="could not recognize your input"):
         model.predict(12)
     with pytest.raises(ValueError, match="could not recognize your input"):
         model.predict(True)
```

### Comparing `span_marker-1.1.1/tests/test_trainer.py` & `span_marker-1.2.0/tests/test_trainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import re
 from pathlib import Path
 from typing import Dict, List
 
 import pytest
 from datasets import Dataset, DatasetDict
 from transformers import EvalPrediction
@@ -12,28 +13,36 @@
 
 
 @pytest.mark.parametrize(
     ("model_fixture", "dataset_fixture"),
     [
         ("fresh_conll_span_marker_model", "conll_dataset_dict"),  # IOB2
         ("finetuned_conll_span_marker_model", "conll_dataset_dict"),  # IOB2
+        ("fresh_conll_span_marker_model", "document_context_conll_dataset_dict"),  # IOB2, doc-context
+        ("finetuned_conll_span_marker_model", "document_context_conll_dataset_dict"),  # IOB2, doc-context
         ("fresh_fewnerd_span_marker_model", "fewnwerd_coarse_dataset_dict"),  # no scheme
         ("finetuned_fewnerd_span_marker_model", "fewnwerd_coarse_dataset_dict"),  # no scheme
         ("fresh_fabner_span_marker_model", "fabner_dataset_dict"),  # BIOES
     ],
 )
 def test_trainer_standard(
-    model_fixture: str, dataset_fixture: str, request: pytest.FixtureRequest, tmp_path: Path
+    model_fixture: str,
+    dataset_fixture: str,
+    request: pytest.FixtureRequest,
+    tmp_path: Path,
+    caplog: pytest.LogCaptureFixture,
 ) -> None:
     model: SpanMarkerModel = request.getfixturevalue(model_fixture)
     dataset: DatasetDict = request.getfixturevalue(dataset_fixture)
 
     # Perform training and evaluation
     trainer = Trainer(model, args=DEFAULT_ARGS, train_dataset=dataset["train"], eval_dataset=dataset["test"])
     trainer.train()
+    if "document_context" in dataset_fixture:
+        assert model.config.trained_with_document_context
     metrics = trainer.evaluate()
     assert isinstance(metrics, dict)
     assert set(metrics.keys()) == {
         "eval_loss",
         "eval_overall_f1",
         "eval_overall_recall",
         "eval_overall_precision",
@@ -49,14 +58,41 @@
     model.save_pretrained(model_path)
     loaded_model = model.from_pretrained(model_path).try_cuda()
     output = loaded_model.predict(
         "This might just output confusing things like M.C. Escher, but it should at least not crash in Germany."
     )
     assert isinstance(output, list)
 
+    if "document_context" in dataset_fixture:
+        # If there's document context, let's evaluate the doc-context model again, but with just tokens
+        caplog.clear()
+        trainer.evaluate(dataset["test"].remove_columns(("document_id", "sentence_id")))
+        print(caplog.record_tuples)
+        assert any(
+            [
+                level == logging.WARNING
+                and text == "This model was trained with document-level context: "
+                "evaluation without document-level context may cause decreased performance."
+                for (_, level, text) in caplog.record_tuples
+            ]
+        )
+        # Alternatively, let's pretend the model is not trained with doc-level context,
+        # and use the doc-level dataset for evaluation
+        caplog.clear()
+        model.config.trained_with_document_context = False
+        trainer.evaluate()
+        assert any(
+            [
+                level == logging.WARNING
+                and text == "This model was trained without document-level context: "
+                "evaluation with document-level context may cause decreased performance."
+                for (_, level, text) in caplog.record_tuples
+            ]
+        )
+
 
 @pytest.mark.parametrize(
     "dataset_fixture",
     [
         "conll_dataset_dict",
         "document_context_conll_dataset_dict",
     ],
```

