# Comparing `tmp/audiolm-pytorch-1.1.6.tar.gz` & `tmp/audiolm-pytorch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.1.6.tar", last modified: Wed Jun 14 15:45:27 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.2.0.tar", last modified: Thu Jun 15 16:05:11 2023, max compression
```

## Comparing `audiolm-pytorch-1.1.6.tar` & `audiolm-pytorch-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:45:27.257426 audiolm-pytorch-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-14 15:45:27.257426 audiolm-pytorch-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18271 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:45:27.253425 audiolm-pytorch-1.1.6/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66155 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:45:27.257426 audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-14 15:45:27.000000 audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 15:45:27.000000 audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:45:27.000000 audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-14 15:45:27.000000 audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 15:45:27.000000 audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:45:27.257426 audiolm-pytorch-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-14 15:45:16.000000 audiolm-pytorch-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66183 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/setup.py
```

### Comparing `audiolm-pytorch-1.1.6/LICENSE` & `audiolm-pytorch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/PKG-INFO` & `audiolm-pytorch-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.1.6
+Version: 1.2.0
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.1.6/README.md` & `audiolm-pytorch-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
     checkpoint_path = './hubert/hubert_base_ls960.pt',
     kmeans_path = './hubert/hubert_base_ls960_L9_km500.bin'
 )
 
 semantic_transformer = SemanticTransformer(
     num_semantic_tokens = wav2vec.codebook_size,
     dim = 1024,
-    depth = 6
+    depth = 6,
+    flash_attn = True
 ).cuda()
 
 
 trainer = SemanticTransformerTrainer(
     transformer = semantic_transformer,
     wav2vec = wav2vec,
     folder ='/path/to/audio/files',
@@ -157,15 +158,16 @@
 soundstream = SoundStream.init_and_load_from('/path/to/trained/soundstream.pt')
 
 coarse_transformer = CoarseTransformer(
     num_semantic_tokens = wav2vec.codebook_size,
     codebook_size = 1024,
     num_coarse_quantizers = 3,
     dim = 512,
-    depth = 6
+    depth = 6,
+    flash_attn = True
 )
 
 trainer = CoarseTransformerTrainer(
     transformer = coarse_transformer,
     codec = soundstream,
     wav2vec = wav2vec,
     folder = '/path/to/audio/files',
@@ -186,15 +188,16 @@
 soundstream = SoundStream.init_and_load_from('/path/to/trained/soundstream.pt')
 
 fine_transformer = FineTransformer(
     num_coarse_quantizers = 3,
     num_fine_quantizers = 5,
     codebook_size = 1024,
     dim = 512,
-    depth = 6
+    depth = 6,
+    flash_attn = True
 )
 
 trainer = FineTransformerTrainer(
     transformer = fine_transformer,
     codec = soundstream,
     folder = '/path/to/audio/files',
     batch_size = 1,
@@ -332,14 +335,15 @@
 - [x] refactor so semantic transformer has a wrapper to that handles unique consecutives as well as wav to hubert or vq-wav2vec
 - [x] simply not self attend to eos token on the prompting side (semantic for coarse transformer, coarse for fine transformer)
 - [x] add structured dropout from forgetful causal masking, far better than traditional dropouts
 - [x] figure out how to suppress logging in fairseq
 - [x] assert that all three transformers passed into audiolm is compatible
 - [x] allow for specialized relative positional embeddings in fine transformer based on absolute matching positions of quantizers between coarse and fine
 - [x] allow for grouped residual vq in soundstream (use `GroupedResidualVQ` from vector-quantize-pytorch lib), from <a href="https://arxiv.org/abs/2305.02765">hifi-codec</a>
+- [x] add flash attention with <a href="https://arxiv.org/abs/2305.19466">NoPE</a>
 
 - [ ] redo the positional embeddings in the presence of groups in residual vq
 - [ ] test with speech synthesis for starters
 - [ ] cli tool, something like `audiolm generate <wav.file | text>` and save generated wav file to local directory
 - [ ] return a list of waves in the case of variable lengthed audio
 - [ ] just take care of the edge case in coarse transformer text conditioned training, where the raw wave is resampled at different frequencies. autodetermine how to route based on length
 
@@ -492,7 +496,26 @@
 ```bibtex
 @inproceedings{Yang2023HiFiCodecGV,
     title   = {HiFi-Codec: Group-residual Vector quantization for High Fidelity Audio Codec},
     author  = {Dongchao Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao Weng and Yuexian Zou},
     year    = {2023}
 }
 ```
+
+```bibtex
+@article{Kazemnejad2023TheIO,
+    title   = {The Impact of Positional Encoding on Length Generalization in Transformers},
+    author  = {Amirhossein Kazemnejad and Inkit Padhi and Karthikeyan Natesan Ramamurthy and Payel Das and Siva Reddy},
+    journal = {ArXiv},
+    year    = {2023},
+    volume  = {abs/2305.19466}
+}
+```
+
+```bibtex
+@inproceedings{dao2022flashattention,
+    title   = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+    author  = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+    booktitle = {Advances in Neural Information Processing Systems},
+    year    = {2022}
+}
+```
```

#### html2text {}

```diff
@@ -59,100 +59,100 @@
 `CoarseTransformer`, `FineTransformer`) need to be trained ex.
 `SemanticTransformer` ```python import torch from audiolm_pytorch import
 HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer # hubert
 checkpoints can be downloaded at # https://github.com/facebookresearch/fairseq/
 tree/main/examples/hubert wav2vec = HubertWithKmeans( checkpoint_path = './
 hubert/hubert_base_ls960.pt', kmeans_path = './hubert/
 hubert_base_ls960_L9_km500.bin' ) semantic_transformer = SemanticTransformer
-( num_semantic_tokens = wav2vec.codebook_size, dim = 1024, depth = 6 ).cuda()
-trainer = SemanticTransformerTrainer( transformer = semantic_transformer,
-wav2vec = wav2vec, folder ='/path/to/audio/files', batch_size = 1,
-data_max_length = 320 * 32, num_train_steps = 1 ) trainer.train() ``` ex.
-`CoarseTransformer` ```python import torch from audiolm_pytorch import
-HubertWithKmeans, SoundStream, CoarseTransformer, CoarseTransformerTrainer
-wav2vec = HubertWithKmeans( checkpoint_path = './hubert/hubert_base_ls960.pt',
-kmeans_path = './hubert/hubert_base_ls960_L9_km500.bin' ) soundstream =
-SoundStream.init_and_load_from('/path/to/trained/soundstream.pt')
-coarse_transformer = CoarseTransformer( num_semantic_tokens =
-wav2vec.codebook_size, codebook_size = 1024, num_coarse_quantizers = 3, dim =
-512, depth = 6 ) trainer = CoarseTransformerTrainer( transformer =
-coarse_transformer, codec = soundstream, wav2vec = wav2vec, folder = '/path/to/
-audio/files', batch_size = 1, data_max_length = 320 * 32, num_train_steps =
-1_000_000 ) trainer.train() ``` ex. `FineTransformer` ```python import torch
-from audiolm_pytorch import SoundStream, FineTransformer,
-FineTransformerTrainer soundstream = SoundStream.init_and_load_from('/path/to/
-trained/soundstream.pt') fine_transformer = FineTransformer
-( num_coarse_quantizers = 3, num_fine_quantizers = 5, codebook_size = 1024, dim
-= 512, depth = 6 ) trainer = FineTransformerTrainer( transformer =
-fine_transformer, codec = soundstream, folder = '/path/to/audio/files',
-batch_size = 1, data_max_length = 320 * 32, num_train_steps = 1_000_000 )
-trainer.train() ``` All together now ```python from audiolm_pytorch import
-AudioLM audiolm = AudioLM( wav2vec = wav2vec, codec = soundstream,
-semantic_transformer = semantic_transformer, coarse_transformer =
-coarse_transformer, fine_transformer = fine_transformer ) generated_wav =
-audiolm(batch_size = 1) # or with priming generated_wav_with_prime = audiolm
-(prime_wave = torch.randn(1, 320 * 8)) # or with text condition, if given
-generated_wav_with_text_condition = audiolm(text = ['chirping of birds and the
-distant echos of bells']) ``` ## Text Conditioned Audio Synthesis Update: Looks
-like this will work, given 'VALL-E' ex. Semantic Transformer ```python import
-torch from audiolm_pytorch import HubertWithKmeans, SemanticTransformer,
-SemanticTransformerTrainer wav2vec = HubertWithKmeans( checkpoint_path = './
+( num_semantic_tokens = wav2vec.codebook_size, dim = 1024, depth = 6,
+flash_attn = True ).cuda() trainer = SemanticTransformerTrainer( transformer =
+semantic_transformer, wav2vec = wav2vec, folder ='/path/to/audio/files',
+batch_size = 1, data_max_length = 320 * 32, num_train_steps = 1 ) trainer.train
+() ``` ex. `CoarseTransformer` ```python import torch from audiolm_pytorch
+import HubertWithKmeans, SoundStream, CoarseTransformer,
+CoarseTransformerTrainer wav2vec = HubertWithKmeans( checkpoint_path = './
 hubert/hubert_base_ls960.pt', kmeans_path = './hubert/
-hubert_base_ls960_L9_km500.bin' ) semantic_transformer = SemanticTransformer
-( num_semantic_tokens = 500, dim = 1024, depth = 6, has_condition = True, #
-this will have to be set to True cond_as_self_attn_prefix = True # whether to
-condition as prefix to self attention, instead of cross attention, as was done
-in 'VALL-E' paper ).cuda() # mock text video dataset (as an example) # you will
-have to extend your own from `Dataset`, and return an audio tensor as well as a
-string (the audio description) in any order (the framework will autodetect and
-route it into the transformer) from torch.utils.data import Dataset class
-MockTextAudioDataset(Dataset): def __init__(self, length = 100, audio_length =
-320 * 32): super().__init__() self.audio_length = audio_length self.len =
-length def __len__(self): return self.len def __getitem__(self, idx):
-mock_audio = torch.randn(self.audio_length) mock_caption = 'audio caption'
-return mock_caption, mock_audio dataset = MockTextAudioDataset() # instantiate
-semantic transformer trainer and train trainer = SemanticTransformerTrainer
-( transformer = semantic_transformer, wav2vec = wav2vec, dataset = dataset,
-batch_size = 4, grad_accum_every = 8, data_max_length = 320 * 32,
-num_train_steps = 1_000_000 ) trainer.train() # after much training above
-sample = trainer.generate(text = ['sound of rain drops on the rooftops'],
-batch_size = 1, max_length = 2) # (1, < 128) - may terminate early if it
-detects [eos] ``` ## Multi-GPU Because all the trainer classes uses ð¤
-Accelerator, you can easily do multi gpu training by using the `accelerate`
-command as so At the project root ```python $ accelerate config ``` Then, in
-the same directory ```python $ accelerate launch train.py ``` ## Todo - [x]
-complete CoarseTransformer - [x] use fairseq vq-wav2vec for embeddings - [x]
-add conditioning - [x] add classifier free guidance - [x] add unique
-consecutive for - [x] incorporate ability to use hubert intermediate features
-as semantic tokens, recommended by eonglints - [x] accommodate variable
-lengthed audio, bring in eos token - [x] make sure unique consecutive works
-with coarse transformer - [x] pretty printing all discriminator losses to log -
-[x] handle when generating semantic tokens, that last logits may not be
-necessarily the last in the sequence given unique consecutive processing - [x]
-complete sampling code for both Coarse and Fine Transformers, which will be
-tricky - [x] make sure full inference with or without prompting works on the
-`AudioLM` class - [x] complete full training code for soundstream, taking care
-of discriminator training - [x] add efficient gradient penalty for
-discriminators for soundstream - [x] wire up sample hz from sound dataset -
-> transformers, and have proper resampling within during training - think about
-whether to allow for dataset to have sound files of varying or enforce same
-sample hz - [x] full transformer training code for all three transformers - [x]
-refactor so semantic transformer has a wrapper to that handles unique
-consecutives as well as wav to hubert or vq-wav2vec - [x] simply not self
-attend to eos token on the prompting side (semantic for coarse transformer,
-coarse for fine transformer) - [x] add structured dropout from forgetful causal
-masking, far better than traditional dropouts - [x] figure out how to suppress
-logging in fairseq - [x] assert that all three transformers passed into audiolm
-is compatible - [x] allow for specialized relative positional embeddings in
-fine transformer based on absolute matching positions of quantizers between
-coarse and fine - [x] allow for grouped residual vq in soundstream (use
-`GroupedResidualVQ` from vector-quantize-pytorch lib), from hifi-codec - [ ]
-redo the positional embeddings in the presence of groups in residual vq - [ ]
-test with speech synthesis for starters - [ ] cli tool, something like `audiolm
-generate
+hubert_base_ls960_L9_km500.bin' ) soundstream = SoundStream.init_and_load_from
+('/path/to/trained/soundstream.pt') coarse_transformer = CoarseTransformer
+( num_semantic_tokens = wav2vec.codebook_size, codebook_size = 1024,
+num_coarse_quantizers = 3, dim = 512, depth = 6, flash_attn = True ) trainer =
+CoarseTransformerTrainer( transformer = coarse_transformer, codec =
+soundstream, wav2vec = wav2vec, folder = '/path/to/audio/files', batch_size =
+1, data_max_length = 320 * 32, num_train_steps = 1_000_000 ) trainer.train()
+``` ex. `FineTransformer` ```python import torch from audiolm_pytorch import
+SoundStream, FineTransformer, FineTransformerTrainer soundstream =
+SoundStream.init_and_load_from('/path/to/trained/soundstream.pt')
+fine_transformer = FineTransformer( num_coarse_quantizers = 3,
+num_fine_quantizers = 5, codebook_size = 1024, dim = 512, depth = 6, flash_attn
+= True ) trainer = FineTransformerTrainer( transformer = fine_transformer,
+codec = soundstream, folder = '/path/to/audio/files', batch_size = 1,
+data_max_length = 320 * 32, num_train_steps = 1_000_000 ) trainer.train() ```
+All together now ```python from audiolm_pytorch import AudioLM audiolm =
+AudioLM( wav2vec = wav2vec, codec = soundstream, semantic_transformer =
+semantic_transformer, coarse_transformer = coarse_transformer, fine_transformer
+= fine_transformer ) generated_wav = audiolm(batch_size = 1) # or with priming
+generated_wav_with_prime = audiolm(prime_wave = torch.randn(1, 320 * 8)) # or
+with text condition, if given generated_wav_with_text_condition = audiolm(text
+= ['chirping of birds and the distant echos of bells']) ``` ## Text Conditioned
+Audio Synthesis Update: Looks like this will work, given 'VALL-E' ex. Semantic
+Transformer ```python import torch from audiolm_pytorch import
+HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer wav2vec =
+HubertWithKmeans( checkpoint_path = './hubert/hubert_base_ls960.pt',
+kmeans_path = './hubert/hubert_base_ls960_L9_km500.bin' ) semantic_transformer
+= SemanticTransformer( num_semantic_tokens = 500, dim = 1024, depth = 6,
+has_condition = True, # this will have to be set to True
+cond_as_self_attn_prefix = True # whether to condition as prefix to self
+attention, instead of cross attention, as was done in 'VALL-E' paper ).cuda() #
+mock text video dataset (as an example) # you will have to extend your own from
+`Dataset`, and return an audio tensor as well as a string (the audio
+description) in any order (the framework will autodetect and route it into the
+transformer) from torch.utils.data import Dataset class MockTextAudioDataset
+(Dataset): def __init__(self, length = 100, audio_length = 320 * 32): super
+().__init__() self.audio_length = audio_length self.len = length def __len__
+(self): return self.len def __getitem__(self, idx): mock_audio = torch.randn
+(self.audio_length) mock_caption = 'audio caption' return mock_caption,
+mock_audio dataset = MockTextAudioDataset() # instantiate semantic transformer
+trainer and train trainer = SemanticTransformerTrainer( transformer =
+semantic_transformer, wav2vec = wav2vec, dataset = dataset, batch_size = 4,
+grad_accum_every = 8, data_max_length = 320 * 32, num_train_steps = 1_000_000 )
+trainer.train() # after much training above sample = trainer.generate(text =
+['sound of rain drops on the rooftops'], batch_size = 1, max_length = 2) # (1,
+< 128) - may terminate early if it detects [eos] ``` ## Multi-GPU Because all
+the trainer classes uses ð¤_Accelerator, you can easily do multi gpu training
+by using the `accelerate` command as so At the project root ```python $
+accelerate config ``` Then, in the same directory ```python $ accelerate launch
+train.py ``` ## Todo - [x] complete CoarseTransformer - [x] use fairseq vq-
+wav2vec for embeddings - [x] add conditioning - [x] add classifier free
+guidance - [x] add unique consecutive for - [x] incorporate ability to use
+hubert intermediate features as semantic tokens, recommended by eonglints - [x]
+accommodate variable lengthed audio, bring in eos token - [x] make sure unique
+consecutive works with coarse transformer - [x] pretty printing all
+discriminator losses to log - [x] handle when generating semantic tokens, that
+last logits may not be necessarily the last in the sequence given unique
+consecutive processing - [x] complete sampling code for both Coarse and Fine
+Transformers, which will be tricky - [x] make sure full inference with or
+without prompting works on the `AudioLM` class - [x] complete full training
+code for soundstream, taking care of discriminator training - [x] add efficient
+gradient penalty for discriminators for soundstream - [x] wire up sample hz
+from sound dataset -> transformers, and have proper resampling within during
+training - think about whether to allow for dataset to have sound files of
+varying or enforce same sample hz - [x] full transformer training code for all
+three transformers - [x] refactor so semantic transformer has a wrapper to that
+handles unique consecutives as well as wav to hubert or vq-wav2vec - [x] simply
+not self attend to eos token on the prompting side (semantic for coarse
+transformer, coarse for fine transformer) - [x] add structured dropout from
+forgetful causal masking, far better than traditional dropouts - [x] figure out
+how to suppress logging in fairseq - [x] assert that all three transformers
+passed into audiolm is compatible - [x] allow for specialized relative
+positional embeddings in fine transformer based on absolute matching positions
+of quantizers between coarse and fine - [x] allow for grouped residual vq in
+soundstream (use `GroupedResidualVQ` from vector-quantize-pytorch lib), from
+hifi-codec - [x] add flash attention with NoPE - [ ] redo the positional
+embeddings in the presence of groups in residual vq - [ ] test with speech
+synthesis for starters - [ ] cli tool, something like `audiolm generate
 file | text>` and save generated wav file to local directory - [ ] return a
 list of waves in the case of variable lengthed audio - [ ] just take care of
 the edge case in coarse transformer text conditioned training, where the raw
 wave is resampled at different frequencies. autodetermine how to route based on
 length ## Citations ```bibtex @inproceedings{Borsos2022AudioLMAL, title =
 {AudioLM: a Language Modeling Approach to Audio Generation}, author = {Zal
 {\'a}n Borsos and Rapha{\"e}l Marinier and Damien Vincent and Eugene Kharitonov
@@ -205,8 +205,16 @@
 {2022}, volume = {abs/2210.13438} } ``` ```bibtex @article
 {Hu2017SqueezeandExcitationN, title = {Squeeze-and-Excitation Networks}, author
 = {Jie Hu and Li Shen and Gang Sun}, journal = {2018 IEEE/CVF Conference on
 Computer Vision and Pattern Recognition}, year = {2017}, pages = {7132-7141} }
 ``` ```bibtex @inproceedings{Yang2023HiFiCodecGV, title = {HiFi-Codec: Group-
 residual Vector quantization for High Fidelity Audio Codec}, author = {Dongchao
 Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao Weng and
-Yuexian Zou}, year = {2023} } ```
+Yuexian Zou}, year = {2023} } ``` ```bibtex @article{Kazemnejad2023TheIO, title
+= {The Impact of Positional Encoding on Length Generalization in Transformers},
+author = {Amirhossein Kazemnejad and Inkit Padhi and Karthikeyan Natesan
+Ramamurthy and Payel Das and Siva Reddy}, journal = {ArXiv}, year = {2023},
+volume = {abs/2305.19466} } ``` ```bibtex @inproceedings{dao2022flashattention,
+title = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
+Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
+Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
+Processing Systems}, year = {2022} } ```
```

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/audiolm_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from audiolm_pytorch.t5 import t5_encode_text, get_encoded_dim, DEFAULT_T5_NAME
 
 from torchaudio.functional import resample
 
 from audiolm_pytorch.soundstream import SoundStream
 from audiolm_pytorch.encodec import EncodecWrapper
 from audiolm_pytorch.utils import AudioConditionerBase
+from audiolm_pytorch.attend import Attend
 
 from tqdm import tqdm
 
 # helper functions
 
 def exists(val):
     return val is not None
@@ -216,36 +217,24 @@
             x = layer(x)
 
         x = x[rel_pos]
         return rearrange(x, 'i j h -> h i j')
 
 # feedforward
 
-class CausalDSConv(nn.Module):
-    def __init__(self, dim):
-        super().__init__()
-        self.ds_conv = nn.Conv1d(dim, dim, 3, bias = False, groups = dim)
-
-    def forward(self, x):
-        x = rearrange(x, 'b n c -> b c n')
-        x = F.pad(x, (2, 0))
-        x = self.ds_conv(x)
-        return rearrange(x, 'b c n -> b n c')
-
 class GEGLU(nn.Module):
     def forward(self, x):
         x, gate = x.chunk(2, dim = -1)
         return F.gelu(gate) * x
 
 def FeedForward(dim, mult = 4, dropout = 0.1):
     inner_dim = int(dim * 2 * mult / 3)
     return nn.Sequential(
         LayerNorm(dim),
         nn.Linear(dim, inner_dim * 2, bias = False),
-        CausalDSConv(inner_dim * 2),
         GEGLU(),
         LayerNorm(inner_dim),
         nn.Dropout(dropout),
         nn.Linear(inner_dim, dim, bias = False)
     )
 
 # attention
@@ -257,19 +246,19 @@
         causal = False,
         dim_head = 64,
         dim_context = None,
         heads = 8,
         norm_context = False,
         num_null_kv = 0,
         dropout = 0.1,
-        scale = 8
+        scale = 8,
+        flash = False
     ):
         super().__init__()
         self.heads = heads
-        self.scale = scale
         self.causal = causal
         inner_dim = dim_head * heads
 
         dim_context = default(dim_context, dim)
 
         self.norm = LayerNorm(dim)
         self.context_norm = LayerNorm(dim_context) if norm_context else nn.Identity()
@@ -278,16 +267,19 @@
 
         self.num_null_kv = num_null_kv
         self.null_kv = nn.Parameter(torch.randn(2, num_null_kv, dim_head)) if num_null_kv > 0 else None
 
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim_context, dim_head * 2, bias = False)
 
-        self.q_scale = nn.Parameter(torch.ones(dim_head))
-        self.k_scale = nn.Parameter(torch.ones(dim_head))
+        self.attend = Attend(
+            flash = flash,
+            dropout = dropout,
+            causal = causal
+        )
 
         self.to_out = nn.Sequential(
             nn.Linear(inner_dim, dim, bias = False),
             nn.Dropout(dropout)
         )
 
     def forward(
@@ -339,46 +331,22 @@
             k = torch.cat((null_k, k), dim = -2)
             v = torch.cat((null_v, v), dim = -2)
 
         # split for multi-headed attention
 
         q = rearrange(q, 'b n (h d) -> b h n d', h = self.heads)
 
-        # new technique, rmsnormed queries and keys, first used by 22B parameter model successfully https://arxiv.org/abs/2302.05442
-
-        q, k = map(l2norm, (q, k))
-        q = q * self.q_scale
-        k = k * self.k_scale
-
-        # similarities
-
-        sim = einsum('b h i d, b j d -> b h i j', q, k) * self.scale
-
-        if exists(attn_bias):
-            attn_bias = F.pad(attn_bias, (self.num_null_kv, 0), value = 0.)
-            sim = sim + attn_bias
+        # handle mask and null key / value
 
         if exists(mask):
             mask = F.pad(mask, (self.num_null_kv, 0), value = True)
-            mask = rearrange(mask, 'b j -> b 1 1 j')
-            sim = sim.masked_fill(~mask, -torch.finfo(sim.dtype).max)
-
-        if self.causal:
-            i, j = sim.shape[-2:]
-            causal_mask = torch.ones((i, j), dtype = torch.bool, device = x.device).triu(j - i + 1)
-            sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
 
         # attention
 
-        attn = sim.softmax(dim = -1)
-        attn = self.attn_dropout(attn)
-
-        # aggregate
-
-        out = einsum('b h i j, b j d -> b h i d', attn, v)
+        out = self.attend(q, k, v, attn_bias = attn_bias, mask = mask)
 
         # merge heads
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # transformer
@@ -393,32 +361,36 @@
         dim_context = None,
         cross_attend = False,
         attn_dropout = 0.,
         ff_dropout = 0.,
         grad_shrink_alpha = 0.1,
         cond_as_self_attn_prefix = False,
         rel_pos_bias = True,
+        flash_attn = False,
         **kwargs
     ):
         super().__init__()
+        rel_pos_bias = rel_pos_bias and not flash_attn
+
         assert not (cross_attend and cond_as_self_attn_prefix)
+
         self.dim_context = default(dim_context, dim)
 
         self.cond_as_self_attn_prefix = cond_as_self_attn_prefix
 
         self.grad_shrink = partial(grad_shrink, alpha = grad_shrink_alpha)
 
         self.layers = nn.ModuleList([])
 
         self.rel_pos_bias = RelativePositionBias(dim = dim // 2, heads = heads) if rel_pos_bias else None
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                Attention(dim = dim, heads = heads, dropout = attn_dropout, causal = True, **kwargs),
-                Attention(dim = dim, heads = heads, dropout = attn_dropout, dim_context = dim_context, num_null_kv = 1, norm_context = True, **kwargs) if cross_attend else None,
+                Attention(dim = dim, heads = heads, dropout = attn_dropout, flash = flash_attn, causal = True, **kwargs),
+                Attention(dim = dim, heads = heads, dropout = attn_dropout, dim_context = dim_context, flash = flash_attn, num_null_kv = 1, norm_context = True, **kwargs) if cross_attend else None,
                 FeedForward(dim = dim, dropout = ff_dropout)
             ]))
 
         self.norm = LayerNorm(dim)
 
     def forward(
         self,
@@ -475,17 +447,21 @@
         t5_name = DEFAULT_T5_NAME,
         cond_dim = None,
         has_condition = False,
         audio_text_condition = False,
         cond_as_self_attn_prefix = False,
         cond_drop_prob = 0.5,
         grad_shrink_alpha = 0.1,
+        rel_pos_bias = True,
+        flash_attn = False,
         **kwargs
     ):
         super().__init__()
+        rel_pos_bias = rel_pos_bias and not flash_attn
+
         self.num_semantic_tokens = num_semantic_tokens
 
         if audio_text_condition:
             has_condition = True
             cond_dim = default(cond_dim, dim)
 
         self.has_condition = has_condition
@@ -505,14 +481,16 @@
             depth = depth,
             heads = heads,
             attn_dropout = attn_dropout,
             ff_dropout = ff_dropout,
             cross_attend = has_condition and not cond_as_self_attn_prefix,
             cond_as_self_attn_prefix = cond_as_self_attn_prefix,
             grad_shrink_alpha = grad_shrink_alpha,
+            rel_pos_bias = rel_pos_bias,
+            flash_attn = flash_attn,
             **kwargs
         )
 
         self.to_logits = nn.Linear(dim, num_semantic_tokens + 1)
 
     @property
     def device(self):
@@ -598,17 +576,21 @@
         has_condition = False,
         cond_dim = None,
         audio_text_condition = False,
         cond_as_self_attn_prefix = False,
         cond_drop_prob = 0.5,
         grad_shrink_alpha = 0.1,
         project_semantic_logits = True,
+        rel_pos_bias = True,
+        flash_attn = False,
         **kwargs
     ):
         super().__init__()
+        rel_pos_bias = rel_pos_bias and not flash_attn
+
         self.num_semantic_tokens = num_semantic_tokens
 
         if audio_text_condition:
             has_condition = True
             cond_dim = default(cond_dim, dim)
 
         self.has_condition = has_condition
@@ -626,25 +608,27 @@
 
         self.coarse_embedding = nn.Embedding(num_coarse_quantizers * codebook_size_with_eos, dim)
         self.coarse_quantize_embedding = nn.Embedding(num_coarse_quantizers, dim)
 
         text_dim = default(cond_dim, get_encoded_dim(t5_name))
         self.proj_text_embed = nn.Linear(text_dim, dim, bias = False) if text_dim != dim else nn.Identity()
 
-        self.cross_attn_bias = nn.Parameter(torch.zeros(heads, 1, 1))
+        self.cross_attn_bias = nn.Parameter(torch.zeros(heads, 1, 1)) if rel_pos_bias else None
 
         self.transformer = Transformer(
             dim = dim,
             depth = depth,
             heads = heads,
             attn_dropout = attn_dropout,
             ff_dropout = ff_dropout,
             cross_attend = has_condition and not cond_as_self_attn_prefix,
             cond_as_self_attn_prefix = cond_as_self_attn_prefix,
             grad_shrink_alpha = grad_shrink_alpha,
+            rel_pos_bias = rel_pos_bias,
+            flash_attn = flash_attn,
             **kwargs
         )
 
         self.codebook_size = codebook_size
         self.num_coarse_quantizers = num_coarse_quantizers
 
         self.to_semantic_logits = nn.Linear(dim, num_semantic_tokens + 1) if project_semantic_logits else None
@@ -733,24 +717,28 @@
             coarse_start_tokens,
             coarse_tokens
         ), dim = 1)
 
         # engineer the attention bias so that cross attention is not dominated by relative positions
 
         seq_len = tokens.shape[-2]
-        attn_bias = self.transformer.rel_pos_bias(seq_len)
 
-        is_semantic = arange(seq_len) < (semantic_seq_len + 1) # semantic seq len + start token
-        is_cross_attn = rearrange(is_semantic, 'i -> i 1') ^ rearrange(is_semantic, 'j -> 1 j')
+        attn_bias = None
 
-        attn_bias = torch.where(
-            is_cross_attn,
-            self.cross_attn_bias,
-            attn_bias
-        )
+        if exists(self.transformer.rel_pos_bias):
+            attn_bias = self.transformer.rel_pos_bias(seq_len)
+
+            is_semantic = arange(seq_len) < (semantic_seq_len + 1) # semantic seq len + start token
+            is_cross_attn = rearrange(is_semantic, 'i -> i 1') ^ rearrange(is_semantic, 'j -> 1 j')
+
+            attn_bias = torch.where(
+                is_cross_attn,
+                self.cross_attn_bias,
+                attn_bias
+            )
 
         # attend
 
         tokens = self.transformer(
             tokens,
             context = text_embeds,
             attn_bias = attn_bias,
@@ -805,17 +793,20 @@
         cond_dim = None,
         audio_text_condition = False,
         cond_as_self_attn_prefix = False,
         cond_drop_prob = 0.5,
         grad_shrink_alpha = 0.1,
         project_coarse_logits = True,
         pad_id = -1,
+        rel_pos_bias = True,
+        flash_attn = False,
         **kwargs
     ):
         super().__init__()
+        rel_pos_bias = rel_pos_bias and not flash_attn
 
         if audio_text_condition:
             has_condition = True
             cond_dim = default(cond_dim, dim)
 
         self.has_condition = has_condition
         self.embed_text = partial(t5_encode_text, name = t5_name)
@@ -844,29 +835,31 @@
             heads = heads,
             attn_dropout = attn_dropout,
             ff_dropout = ff_dropout,
             cross_attend = has_condition and not cond_as_self_attn_prefix,
             cond_as_self_attn_prefix = cond_as_self_attn_prefix,
             rel_pos_bias = False,
             grad_shrink_alpha = grad_shrink_alpha,
+            flash_attn = flash_attn,
             **kwargs
         )
 
         # doing a specialized attn bias so that corresponding time steps at fine and coarse sequences attend to each other better
 
-        self.null_pos_bias = nn.Parameter(torch.randn(heads, 1, 1))
+        self.null_pos_bias = nn.Parameter(torch.randn(heads, 1, 1)) if rel_pos_bias else None
 
         pos_bias_mlp_dim = dim // 2
+
         self.pos_bias_mlp = nn.Sequential(
             nn.Linear(2, pos_bias_mlp_dim),
             nn.SiLU(),
             nn.Linear(pos_bias_mlp_dim, pos_bias_mlp_dim),
             nn.SiLU(),
             nn.Linear(pos_bias_mlp_dim, heads)
-        )
+        ) if rel_pos_bias else None
 
         self.codebook_size = codebook_size
         self.num_coarse_quantizers = num_coarse_quantizers
         self.num_fine_quantizers = num_fine_quantizers
 
         self.coarse_logit_weights = nn.Parameter(torch.randn(num_coarse_quantizers, codebook_size, dim)) if project_coarse_logits else None
         self.fine_logit_weights = nn.Parameter(torch.randn(num_fine_quantizers, codebook_size, dim))
@@ -979,83 +972,86 @@
             coarse_tokens,
             fine_start_tokens,
             fine_tokens
         ), dim = 1)
 
         # an engineered attention bias so coarse and fine sequences attend to each other better
 
-        max_seq_len = max(coarse_seq_length, fine_seq_length)
+        attn_bias = None
 
-        coarse_pos = torch.arange(coarse_seq_length, device = device)
-        fine_pos = torch.arange(fine_seq_length, device = device)
+        if exists(self.pos_bias_mlp):
+            max_seq_len = max(coarse_seq_length, fine_seq_length)
 
-        coarse_pos = repeat(coarse_pos, 'n -> (n q)', q = self.num_coarse_quantizers)[:coarse_length]
-        fine_pos = repeat(fine_pos, 'n -> (n q)', q = self.num_fine_quantizers)[:fine_length]
+            coarse_pos = torch.arange(coarse_seq_length, device = device)
+            fine_pos = torch.arange(fine_seq_length, device = device)
 
-        coarse_pos = F.pad(coarse_pos, (1, 0), value = -1)
-        fine_pos = F.pad(fine_pos, (1, 0), value = -1)
+            coarse_pos = repeat(coarse_pos, 'n -> (n q)', q = self.num_coarse_quantizers)[:coarse_length]
+            fine_pos = repeat(fine_pos, 'n -> (n q)', q = self.num_fine_quantizers)[:fine_length]
 
-        seq_positions = torch.cat((coarse_pos, fine_pos), dim = -1)
+            coarse_pos = F.pad(coarse_pos, (1, 0), value = -1)
+            fine_pos = F.pad(fine_pos, (1, 0), value = -1)
 
-        coarse_offsets = F.pad(coarse_offsets, (1, 0), value = 0)
-        fine_offsets = fine_offsets + self.num_coarse_quantizers
-        fine_offsets = F.pad(fine_offsets, (1, 0), value = 0)
+            seq_positions = torch.cat((coarse_pos, fine_pos), dim = -1)
 
-        seq_offsets = torch.cat((coarse_offsets, fine_offsets), dim = -1)
+            coarse_offsets = F.pad(coarse_offsets, (1, 0), value = 0)
+            fine_offsets = fine_offsets + self.num_coarse_quantizers
+            fine_offsets = F.pad(fine_offsets, (1, 0), value = 0)
 
-        pos_mlp_input = torch.stack((seq_positions.clamp(min = 0), seq_offsets), dim = -1)
+            seq_offsets = torch.cat((coarse_offsets, fine_offsets), dim = -1)
 
-        num_offsets = self.num_fine_quantizers + self.num_coarse_quantizers
+            pos_mlp_input = torch.stack((seq_positions.clamp(min = 0), seq_offsets), dim = -1)
 
-        # relative positions are always (2 * N - 1), where N is the length of the dimension
+            num_offsets = self.num_fine_quantizers + self.num_coarse_quantizers
 
-        rel_seq_len, rel_offsets = map(lambda n: 2 * n - 1, (max_seq_len, num_offsets))
+            # relative positions are always (2 * N - 1), where N is the length of the dimension
 
-        # get all relative distances
+            rel_seq_len, rel_offsets = map(lambda n: 2 * n - 1, (max_seq_len, num_offsets))
 
-        rel_dist = (rearrange(pos_mlp_input, 'i c -> i 1 c') - rearrange(pos_mlp_input, 'j c -> 1 j c'))
+            # get all relative distances
 
-        # get all possible relative distances for the attention bias to be computed from the mlp
-        # which would be - (2 * N - 1) * (2 * Q - 1) - where N = sequence length and Q = total quantizers
+            rel_dist = (rearrange(pos_mlp_input, 'i c -> i 1 c') - rearrange(pos_mlp_input, 'j c -> 1 j c'))
 
-        rel_seq_len_range = repeat(torch.arange(rel_seq_len, device = device), 'n -> (n q)', q = rel_offsets)
-        rel_offset_range = repeat(torch.arange(rel_offsets, device = device), 'q -> (n q)', n = rel_seq_len)
+            # get all possible relative distances for the attention bias to be computed from the mlp
+            # which would be - (2 * N - 1) * (2 * Q - 1) - where N = sequence length and Q = total quantizers
 
-        mlp_inputs = torch.stack((rel_seq_len_range, rel_offset_range), dim = -1)
+            rel_seq_len_range = repeat(torch.arange(rel_seq_len, device = device), 'n -> (n q)', q = rel_offsets)
+            rel_offset_range = repeat(torch.arange(rel_offsets, device = device), 'q -> (n q)', n = rel_seq_len)
 
-        # implicitly parameterized relative distances, by sequence and quantizer positions
+            mlp_inputs = torch.stack((rel_seq_len_range, rel_offset_range), dim = -1)
 
-        attn_bias = self.pos_bias_mlp(mlp_inputs.float())
+            # implicitly parameterized relative distances, by sequence and quantizer positions
 
-        # translate coordinates of (rel_seq_pos, rel_quantizer_offset) -> positive index to select from attn bias
+            attn_bias = self.pos_bias_mlp(mlp_inputs.float())
 
-        rel_dist_seq_pos, rel_dist_seq_offset = rel_dist.unbind(dim = -1)
+            # translate coordinates of (rel_seq_pos, rel_quantizer_offset) -> positive index to select from attn bias
 
-        rel_dist_seq_pos += max_seq_len - 1
-        rel_dist_seq_offset += num_offsets - 1
+            rel_dist_seq_pos, rel_dist_seq_offset = rel_dist.unbind(dim = -1)
 
-        rel_dist_indices = rel_dist_seq_pos * rel_offsets + rel_dist_seq_offset
+            rel_dist_seq_pos += max_seq_len - 1
+            rel_dist_seq_offset += num_offsets - 1
 
-        # select the relative positional attention bias outputted by the MLP
-        # savings go from (N * Q) ^ 2 -> ~ (4 * N * Q)
+            rel_dist_indices = rel_dist_seq_pos * rel_offsets + rel_dist_seq_offset
 
-        attn_bias = attn_bias[rel_dist_indices]
+            # select the relative positional attention bias outputted by the MLP
+            # savings go from (N * Q) ^ 2 -> ~ (4 * N * Q)
 
-        attn_bias = rearrange(attn_bias, '... h -> h ...')
+            attn_bias = attn_bias[rel_dist_indices]
 
-        # need to make sure start token has a custom positional bias
+            attn_bias = rearrange(attn_bias, '... h -> h ...')
 
-        is_start_token_seq = seq_positions == -1
-        start_token_mask = rearrange(is_start_token_seq, 'i -> i 1') | rearrange(is_start_token_seq, 'j -> 1 j')
+            # need to make sure start token has a custom positional bias
 
-        attn_bias = torch.where(
-            start_token_mask,
-            self.null_pos_bias,
-            attn_bias,
-        )
+            is_start_token_seq = seq_positions == -1
+            start_token_mask = rearrange(is_start_token_seq, 'i -> i 1') | rearrange(is_start_token_seq, 'j -> 1 j')
+
+            attn_bias = torch.where(
+                start_token_mask,
+                self.null_pos_bias,
+                attn_bias,
+            )
 
         # attention
 
         tokens = self.transformer(
             tokens,
             context = text_embeds,
             self_attn_mask = self_attn_mask,
@@ -1685,15 +1681,20 @@
             fine_token_ids = fine_token_ids[:, :-1]
 
         # forgetful causal mask - structured dropout
 
         self_attn_mask = None
 
         if self.mask_prob > 0 and self.training:
-            self_attn_mask = generate_mask_with_prob(self_attn_mask.shape, self.mask_prob, device = self_attn_mask.device)
+            mask_shape = (
+                coarse_token_ids.shape[0],
+                coarse_token_ids.shape[-1] + fine_token_ids.shape[-1] + 2
+            )
+
+            self_attn_mask = generate_mask_with_prob(mask_shape, self.mask_prob, device = self.device)
 
         coarse_logits, fine_logits = self.transformer(
             coarse_token_ids = coarse_token_ids,
             fine_token_ids = fine_token_ids,
             self_attn_mask = self_attn_mask,
             text = text,
             text_embeds = text_embeds,
```

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/data.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.2.0/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.1.6
+Version: 1.2.0
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.1.6/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 audiolm_pytorch/__init__.py
+audiolm_pytorch/attend.py
 audiolm_pytorch/audiolm_pytorch.py
 audiolm_pytorch/data.py
 audiolm_pytorch/encodec.py
 audiolm_pytorch/hubert_kmeans.py
 audiolm_pytorch/optimizer.py
 audiolm_pytorch/soundstream.py
 audiolm_pytorch/t5.py
```

### Comparing `audiolm-pytorch-1.1.6/setup.py` & `audiolm-pytorch-1.2.0/setup.py`

 * *Files identical despite different names*

