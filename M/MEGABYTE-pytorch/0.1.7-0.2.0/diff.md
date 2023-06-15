# Comparing `tmp/MEGABYTE-pytorch-0.1.7.tar.gz` & `tmp/MEGABYTE-pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.1.7.tar", last modified: Thu Jun 15 18:14:38 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.2.0.tar", last modified: Thu Jun 15 19:38:59 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.1.7.tar` & `MEGABYTE-pytorch-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 18:14:28.000000 MEGABYTE-pytorch-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:38:59.963760 MEGABYTE-pytorch-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 19:38:47.000000 MEGABYTE-pytorch-0.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:38:59.959760 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 19:38:47.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-15 19:38:47.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-06-15 19:38:47.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:38:59.959760 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 19:38:59.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 19:38:59.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:38:59.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 19:38:59.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 19:38:59.000000 MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 19:38:59.963760 MEGABYTE-pytorch-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-15 19:38:47.000000 MEGABYTE-pytorch-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:38:59.963760 MEGABYTE-pytorch-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 19:38:47.000000 MEGABYTE-pytorch-0.2.0/setup.py
```

### Comparing `MEGABYTE-pytorch-0.1.7/LICENSE` & `MEGABYTE-pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch/megabyte.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,27 +227,30 @@
         self.stages = len(depth)
         dim = cast_tuple(dim, self.stages)
 
         assert len(dim) == self.stages
 
         coarsest_dim, *_, fine_dim = dim
 
-        self.token_emb = nn.Embedding(num_tokens, fine_dim)
-
         self.max_seq_len = max_seq_len
 
         self.start_tokens = nn.ParameterList([nn.Parameter(torch.randn(h_dim)) for h_dim, seq_len in zip(dim, max_seq_len)])
         self.pos_embs = nn.ModuleList([nn.Embedding(seq_len, h_dim) for h_dim, seq_len in zip(dim, max_seq_len)]) if pos_emb else None
 
-        self.patch_embedders = nn.ModuleList([nn.Sequential(
-            Rearrange('... r d -> ... (r d)'),
-            nn.LayerNorm(seq_len * dim_in),
-            nn.Linear(seq_len * dim_in, dim_out),
-            nn.LayerNorm(dim_out)
-        ) for dim_in, dim_out, seq_len in zip(dim[1:], dim[:-1], max_seq_len[1:])])
+        self.token_embs = nn.ModuleList([])
+        self.token_embs.append(nn.Embedding(num_tokens, fine_dim))
+
+        for dim_out, seq_len in zip(dim[:-1], max_seq_len[1:]):
+            self.token_embs.append(nn.Sequential(
+                nn.Embedding(num_tokens, fine_dim),
+                Rearrange('... r d -> ... (r d)'),
+                nn.LayerNorm(seq_len * fine_dim),
+                nn.Linear(seq_len * fine_dim, dim_out),
+                nn.LayerNorm(dim_out)
+            ))
 
         self.transformers = nn.ModuleList([])
         self.to_next_transformer_projections = nn.ModuleList([])
 
         for h_dim, next_h_dim, stage_depth, next_seq_len in zip_longest(dim, dim[1:], depth, max_seq_len[1:]):
             self.transformers.append(Transformer(
                 dim = h_dim,
@@ -262,15 +265,15 @@
             ))
 
             proj = nn.Identity()
 
             if exists(next_h_dim) and next_h_dim != dim:
                 proj = nn.Sequential(
                     nn.Linear(h_dim, next_h_dim * next_seq_len),
-                    Rearrange('... (n d) -> (...) n d', n = next_seq_len)
+                    Rearrange('b m (n d) -> b (m n) d', n = next_seq_len)
                 )
 
             self.to_next_transformer_projections.append(proj)
 
         self.to_logits = nn.Linear(fine_dim, num_tokens)
         self.pad_id = pad_id
 
@@ -331,47 +334,43 @@
         b, *prec_dims, device = *ids.shape, ids.device
 
         # check some dimensions
 
         assert prec_dims[0] <= self.max_seq_len[0], 'the first dimension of your axial autoregressive transformer must be less than the first tuple element of max_seq_len (like any autoregressive transformer)'
         assert tuple(prec_dims[1:]) == tuple(self.max_seq_len[1:]), 'all subsequent dimensions must match exactly'
 
-        # get token embeddings
-
-        tokens = self.token_emb(ids)
-
         # get tokens for all hierarchical stages, reducing by appropriate dimensions
         # and adding the absolute positional embeddings
 
         tokens_at_stages = []
-        reduced_tokens = tokens
-
         pos_embs = default(self.pos_embs, (None,))
 
-        for ind, pos_emb, patch_emb in zip_longest(range(len(prec_dims)), reversed(pos_embs), reversed((*self.patch_embedders, None))):
-            is_first = ind == 0
-
-            if not is_first:
-                reduced_tokens = patch_emb(reduced_tokens)
+        for ind, pos_emb, token_emb in zip_longest(range(len(prec_dims)), reversed(pos_embs), reversed(self.token_embs)):
+            is_last = ind == (len(prec_dims) - 1)
+            tokens = token_emb(ids)
 
             if exists(pos_emb):
-                positions = pos_emb(torch.arange(reduced_tokens.shape[-2], device = device))
-                reduced_tokens = reduced_tokens + positions
+                positions = pos_emb(torch.arange(tokens.shape[-2], device = device))
+                tokens = tokens + positions
+
+            tokens_at_stages.append(tokens)
 
-            tokens_at_stages.insert(0, reduced_tokens)
+            if is_last:
+                continue
+
+            ids = rearrange(ids, '... m n -> ... (m n)')
 
         # the un-pixelshuffled representations of the previous hierarchy, starts with None
 
         prev_stage_tokens_repr = None
 
         # spatial tokens is tokens with depth pos reduced along depth dimension + spatial positions        
 
         for stage_start_tokens, stage_tokens, transformer, proj in zip(self.start_tokens, tokens_at_stages, self.transformers, self.to_next_transformer_projections):
             stage_tokens, ps = pack_one(stage_tokens, '* n d')
-
             stage_start_tokens = repeat(stage_start_tokens, 'f -> b 1 f', b = stage_tokens.shape[0])
 
             # concat start token
 
             stage_tokens = torch.cat((
                 stage_start_tokens,
                 stage_tokens,
```

### Comparing `MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.2.0/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.7
+Version: 0.2.0
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.7/PKG-INFO` & `MEGABYTE-pytorch-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.7
+Version: 0.2.0
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.7/README.md` & `MEGABYTE-pytorch-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.7/setup.py` & `MEGABYTE-pytorch-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.1.7',
+  version = '0.2.0',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

