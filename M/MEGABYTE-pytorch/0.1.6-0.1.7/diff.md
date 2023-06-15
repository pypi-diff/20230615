# Comparing `tmp/MEGABYTE-pytorch-0.1.6.tar.gz` & `tmp/MEGABYTE-pytorch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.1.6.tar", last modified: Wed Jun 14 16:51:33 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.1.7.tar", last modified: Thu Jun 15 18:14:38 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.1.6.tar` & `MEGABYTE-pytorch-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 18:14:38.000000 MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-15 18:14:27.000000 MEGABYTE-pytorch-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:14:38.926004 MEGABYTE-pytorch-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 18:14:28.000000 MEGABYTE-pytorch-0.1.7/setup.py
```

### Comparing `MEGABYTE-pytorch-0.1.6/LICENSE` & `MEGABYTE-pytorch-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/attend.py`

 * *Files 13% similar despite different names*

```diff
@@ -85,42 +85,27 @@
             mask = rearrange(mask, 'b j -> b 1 1 j')
             mask = mask.expand(-1, heads, q_len, -1)
 
         # Check if there is a compatible device for flash attention
 
         config = self.cuda_config if is_cuda else self.cpu_config
 
-        causal = self.causal
-
-        # handle attention bias
-
-        if exists(attn_bias):
-            mask_value = -torch.finfo(q.dtype).max // 2
-            causal_mask = self.get_mask(q_len, k_len, device)
-            attn_bias = attn_bias.masked_fill(causal_mask, mask_value)
-
-            if exists(mask):
-                attn_bias = attn_bias.masked_fill(~mask, mask_value)
-
-            mask = attn_bias
-            causal = False
-
         # pytorch 2.0 flash attn: q, k, v, mask, dropout, causal, softmax_scale
 
         with torch.backends.cuda.sdp_kernel(**config._asdict()):
             out = F.scaled_dot_product_attention(
                 q, k, v,
                 attn_mask = mask,
                 dropout_p = self.dropout if self.training else 0., 
-                is_causal = causal
+                is_causal = self.causal
             )
 
         return out
 
-    def forward(self, q, k, v, mask = None, attn_bias = None):
+    def forward(self, q, k, v, mask = None):
         """
         einstein notation
         b - batch
         h - heads
         n, i, j - sequence length (base sequence length, source, target)
         d - feature dimension
         """
@@ -128,25 +113,20 @@
         q_len, k_len, device = q.shape[-2], k.shape[-2], q.device
 
         scale = q.shape[-1] ** -0.5
 
         kv_einsum_eq = 'b j d' if k.ndim == 3 else 'b h j d'
 
         if self.flash:
-            return self.flash_attn(q, k, v, mask = mask, attn_bias = attn_bias)
+            return self.flash_attn(q, k, v, mask = mask)
 
         # similarity
 
         sim = einsum(f"b h i d, {kv_einsum_eq} -> b h i j", q, k) * scale
 
-        # attention bias
-
-        if exists(attn_bias):
-            sim = sim + attn_bias
-
         # causal mask
 
         if self.causal:
             causal_mask = self.get_mask(q_len, k_len, device)
             sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
 
         # attention
```

### Comparing `MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch/megabyte.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,48 +62,38 @@
 # token shift, from Peng et al of RWKV
 
 def token_shift(t):
     t, t_shift = t.chunk(2, dim = -1)
     t_shift = F.pad(t_shift, (0, 0, 1, -1))
     return torch.cat((t, t_shift), dim = -1)
 
-# positional bias
+# rotary positional embedding
 
-class Alibi(nn.Module):
-    def __init__(self, heads, **kwargs):
+class RotaryEmbedding(nn.Module):
+    def __init__(self, dim, theta = 10000):
         super().__init__()
-        self.heads = heads
-        slopes = torch.Tensor(self._get_slopes(heads))
-        slopes = rearrange(slopes, 'h -> h 1 1')
-        self.register_buffer('slopes', slopes, persistent = False)
-        self.register_buffer('bias', None, persistent = False)
-
-    @staticmethod
-    def _get_slopes(heads):
-        def get_slopes_power_of_2(n):
-            start = (2**(-2**-(math.log2(n)-3)))
-            ratio = start
-            return [start*ratio**i for i in range(n)]
-
-        if math.log2(heads).is_integer():
-            return get_slopes_power_of_2(heads)
-
-        closest_power_of_2 = 2 ** math.floor(math.log2(heads))
-        return get_slopes_power_of_2(closest_power_of_2) + get_slopes_power_of_2(2 * closest_power_of_2)[0::2][:heads-closest_power_of_2]
-
-    def forward(self, i, j, device):
-        if exists(self.bias) and self.bias.shape[-1] >= j:
-            return self.bias[..., :j]
-
-        bias = torch.arange(j, device = device)
-        bias = rearrange(bias, 'j -> 1 1 j')
-        bias = bias * self.slopes
+        inv_freq = 1.0 / (theta ** (torch.arange(0, dim, 2).float() / dim))
+        self.register_buffer("inv_freq", inv_freq)
+
+    @property
+    def device(self):
+        return next(self.buffers()).device
+
+    def forward(self, seq_len):
+        t = torch.arange(seq_len, device = self.device).type_as(self.inv_freq)
+        freqs = torch.einsum('i , j -> i j', t, self.inv_freq)
+        freqs = torch.cat((freqs, freqs), dim = -1)
+        return freqs
+
+def rotate_half(x):
+    x1, x2 = x.chunk(2, dim=-1)
+    return torch.cat((-x2, x1), dim=-1)
 
-        self.register_buffer('bias', bias, persistent = False)
-        return self.bias
+def apply_rotary_pos_emb(pos, t):
+    return t * pos.cos() + rotate_half(t) * pos.sin()
 
 # norm
 
 class RMSNorm(nn.Module):
     def __init__(self, dim, eps = 1e-8):
         super().__init__()
         self.scale = dim ** -0.5
@@ -148,22 +138,25 @@
 
         self.dropout = nn.Dropout(dropout)
         self.norm = RMSNorm(dim)
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, dim_head * 2, bias = False)
         self.to_out = nn.Linear(inner_dim, dim, bias = False)
 
-    def forward(self, x, attn_bias = None):
+    def forward(self, x, rotary_emb = None):
         h, device = self.heads, x.device
 
         x = self.norm(x)
         q, k, v = (self.to_q(x), *self.to_kv(x).chunk(2, dim = -1))
         q = rearrange(q, 'b n (h d) -> b h n d', h = h)
 
-        out = self.attend(q, k, v, attn_bias = attn_bias)
+        if exists(rotary_emb):
+            q, k = map(lambda t: apply_rotary_pos_emb(rotary_emb, t), (q, k))
+
+        out = self.attend(q, k, v)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 class Transformer(nn.Module):
     def __init__(
         self,
@@ -171,35 +164,35 @@
         dim,
         layers,
         dim_head = 64,
         heads = 8,
         attn_dropout = 0.,
         ff_dropout = 0.,
         ff_mult = 4,
-        rel_pos_bias = True,
+        rel_pos = True,
         flash_attn = False
     ):
         super().__init__()
-        self.alibi = Alibi(heads = heads) if rel_pos_bias else None
+        self.rotary_emb = RotaryEmbedding(dim_head) if rel_pos else None
         self.layers = nn.ModuleList([])
 
         for _ in range(layers):
             self.layers.append(nn.ModuleList([
                 Attention(dim = dim, dim_head = dim_head, heads = heads, dropout = attn_dropout, flash = flash_attn),
                 FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
             ]))
 
         self.norm = RMSNorm(dim)
 
     def forward(self, x):
         n = x.shape[-2]
-        attn_bias = self.alibi(n, n, device = x.device) if exists(self.alibi) else None
+        rotary_emb = self.rotary_emb(n) if exists(self.rotary_emb) else None
 
         for attn, ff in self.layers:
-            x = attn(token_shift(x), attn_bias = attn_bias) + x
+            x = attn(token_shift(x), rotary_emb = rotary_emb) + x
             x = ff(token_shift(x)) + x
 
         return self.norm(x)
 
 # main class
 
 class MEGABYTE(nn.Module):
@@ -214,15 +207,15 @@
         max_seq_len: Tuple,
         dim_head = 64,
         heads = 8,
         attn_dropout = 0.,
         ff_mult = 4,
         ff_dropout = 0.,
         pad_id = 0,
-        rel_pos_bias = False,
+        rel_pos = False,
         pos_emb = False,
         flash_attn = False
     ):
         super().__init__()
 
         # simplified configuration for each stage of the hierarchy
         # depth = (2, 2, 4) would translate to depth 2 at first stage, depth 2 second stage, depth 4 third
@@ -260,15 +253,15 @@
                 dim = h_dim,
                 layers = stage_depth,
                 dim_head = dim_head,
                 heads = heads,
                 attn_dropout = attn_dropout,
                 ff_dropout = ff_dropout,
                 ff_mult = ff_mult,
-                rel_pos_bias = rel_pos_bias,
+                rel_pos = rel_pos,
                 flash_attn = flash_attn
             ))
 
             proj = nn.Identity()
 
             if exists(next_h_dim) and next_h_dim != dim:
                 proj = nn.Sequential(
```

### Comparing `MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.1.7/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.6/PKG-INFO` & `MEGABYTE-pytorch-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.6
+Version: 0.1.7
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.6/README.md` & `MEGABYTE-pytorch-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -86,23 +86,14 @@
     author  = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
     booktitle = {Advances in Neural Information Processing Systems},
     year    = {2022}
 }
 ```
 
 ```bibtex
-@misc{press2021ALiBi,
-    title   = {Train Short, Test Long: Attention with Linear Biases Enable Input Length Extrapolation},
-    author  = {Ofir Press and Noah A. Smith and Mike Lewis},
-    year    = {2021},
-    url     = {https://ofir.io/train_short_test_long.pdf}
-}
-```
-
-```bibtex
 @software{peng_bo_2021_5196578,
     author    = {PENG Bo},
     title     = {BlinkDL/RWKV-LM: 0.01},
     month     = {aug},
     year      = {2021},
     publisher = {Zenodo},
     version   = {0.01},
@@ -116,7 +107,18 @@
     title   = {The Impact of Positional Encoding on Length Generalization in Transformers},
     author  = {Amirhossein Kazemnejad and Inkit Padhi and Karthikeyan Natesan Ramamurthy and Payel Das and Siva Reddy},
     journal = {ArXiv},
     year    = {2023},
     volume  = {abs/2305.19466}
 }
 ```
+
+```bibtex
+@misc{su2021roformer,
+    title   = {RoFormer: Enhanced Transformer with Rotary Position Embedding},
+    author  = {Jianlin Su and Yu Lu and Shengfeng Pan and Bo Wen and Yunfeng Liu},
+    year    = {2021},
+    eprint  = {2104.09864},
+    archivePrefix = {arXiv},
+    primaryClass = {cs.CL}
+}
+```
```

#### html2text {}

```diff
@@ -26,18 +26,19 @@
 {https://arxiv.org/abs/2302.01327}, author = {Kumar, Manoj and Dehghani,
 Mostafa and Houlsby, Neil}, title = {Dual PatchNorm}, publisher = {arXiv}, year
 = {2023}, copyright = {Creative Commons Attribution 4.0 International} } ```
 ```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
 and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
 and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ``` ```bibtex @misc{press2021ALiBi, title = {Train Short, Test Long:
-Attention with Linear Biases Enable Input Length Extrapolation}, author = {Ofir
-Press and Noah A. Smith and Mike Lewis}, year = {2021}, url = {https://ofir.io/
-train_short_test_long.pdf} } ``` ```bibtex @software{peng_bo_2021_5196578,
-author = {PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01}, month = {aug}, year =
-{2021}, publisher = {Zenodo}, version = {0.01}, doi = {10.5281/zenodo.5196578},
-url = {https://doi.org/10.5281/zenodo.5196578} } ``` ```bibtex @article
-{Kazemnejad2023TheIO, title = {The Impact of Positional Encoding on Length
-Generalization in Transformers}, author = {Amirhossein Kazemnejad and Inkit
-Padhi and Karthikeyan Natesan Ramamurthy and Payel Das and Siva Reddy}, journal
-= {ArXiv}, year = {2023}, volume = {abs/2305.19466} } ```
+} ``` ```bibtex @software{peng_bo_2021_5196578, author = {PENG Bo}, title =
+{BlinkDL/RWKV-LM: 0.01}, month = {aug}, year = {2021}, publisher = {Zenodo},
+version = {0.01}, doi = {10.5281/zenodo.5196578}, url = {https://doi.org/
+10.5281/zenodo.5196578} } ``` ```bibtex @article{Kazemnejad2023TheIO, title =
+{The Impact of Positional Encoding on Length Generalization in Transformers},
+author = {Amirhossein Kazemnejad and Inkit Padhi and Karthikeyan Natesan
+Ramamurthy and Payel Das and Siva Reddy}, journal = {ArXiv}, year = {2023},
+volume = {abs/2305.19466} } ``` ```bibtex @misc{su2021roformer, title =
+{RoFormer: Enhanced Transformer with Rotary Position Embedding}, author =
+{Jianlin Su and Yu Lu and Shengfeng Pan and Bo Wen and Yunfeng Liu}, year =
+{2021}, eprint = {2104.09864}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
+} ```
```

### Comparing `MEGABYTE-pytorch-0.1.6/setup.py` & `MEGABYTE-pytorch-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

