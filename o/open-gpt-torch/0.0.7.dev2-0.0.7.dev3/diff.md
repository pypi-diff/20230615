# Comparing `tmp/open_gpt_torch-0.0.7.dev2.tar.gz` & `tmp/open_gpt_torch-0.0.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.7.dev2.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.7.dev3.tar", max compression
```

## Comparing `open_gpt_torch-0.0.7.dev2.tar` & `open_gpt_torch-0.0.7.dev3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    10825 2023-06-13 07:21:26.282528 open_gpt_torch-0.0.7.dev2/LICENSE
--rw-r--r--   0        0        0     7610 2023-06-13 07:21:26.282528 open_gpt_torch-0.0.7.dev2/README.md
--rw-r--r--   0        0        0      929 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/__main__.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0      953 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/cli/commands/playground.py
--rw-r--r--   0        0        0     2223 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     5293 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/factory.py
--rw-r--r--   0        0        0     2523 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/helper.py
--rw-r--r--   0        0        0      490 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/logs.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/__init__.py
--rw-r--r--   0        0        0     2420 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/embedding.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     6038 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     9040 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     5570 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2439 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0    11346 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/generation.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     2877 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0      863 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     2856 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2564 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     3504 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0      653 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/rwkv/__init__.py
--rw-r--r--   0        0        0     1233 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/rwkv/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0     2608 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     7439 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0     1428 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     3507 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1977 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0     2373 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      171 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/executors/utils.py
--rw-r--r--   0        0        0     3429 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0        0 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/playground/__init__.py
--rw-r--r--   0        0        0     4686 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/playground/gradio.py
--rw-r--r--   0        0        0     7396 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/playground/gradio_chatbot.py
--rw-r--r--   0        0        0     2714 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/open_gpt/serve/playground/gradio_css.py
--rw-r--r--   0        0        0     3242 2023-06-13 07:21:26.314528 open_gpt_torch-0.0.7.dev2/pyproject.toml
--rw-r--r--   0        0        0    20871 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.7.dev2/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-06-13 07:38:41.535460 open_gpt_torch-0.0.7.dev3/LICENSE
+-rw-r--r--   0        0        0     7610 2023-06-13 07:38:41.535460 open_gpt_torch-0.0.7.dev3/README.md
+-rw-r--r--   0        0        0      929 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0      953 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/playground.py
+-rw-r--r--   0        0        0     2223 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     5293 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/factory.py
+-rw-r--r--   0        0        0     2523 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/helper.py
+-rw-r--r--   0        0        0      490 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/logs.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0     2420 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/embedding.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     6038 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     9040 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     5585 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2439 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0    11346 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/generation.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     2877 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0      863 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     2856 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2564 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.567460 open_gpt_torch-0.0.7.dev3/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     3504 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0      653 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/rwkv/__init__.py
+-rw-r--r--   0        0        0     1233 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/rwkv/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     2608 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     7439 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0     1428 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     3507 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1977 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0     2373 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      171 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/utils.py
+-rw-r--r--   0        0        0     3429 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0        0        0     4686 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0        0        0     7396 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0        0        0     2714 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_css.py
+-rw-r--r--   0        0        0     3242 2023-06-13 07:38:41.571460 open_gpt_torch-0.0.7.dev3/pyproject.toml
+-rw-r--r--   0        0        0    20871 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.7.dev3/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.7.dev2/LICENSE` & `open_gpt_torch-0.0.7.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/README.md` & `open_gpt_torch-0.0.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/__init__.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/cli/application.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/cli/commands/playground.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/factory.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/factory.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/helper.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/embedding.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/embedding.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/flamingo_model.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/flamingo_model.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         device_map is None
     ), f"`device_map={device_map}` is not supported for Flamingo models"
 
     # load the vision model
     model_name, *pretrained = vision_model_name_or_path.split("::")
     pretrained = pretrained[0] if len(pretrained) == 1 else 'openai'
     clip_model, _, image_processor = open_clip.create_model_and_transforms(
-        model_name, pretrained=pretrained, precision='fp16'
+        model_name, pretrained=pretrained, precision='fp16', device=device
     )
     # set the vision encoder to output the visual features
     clip_model.visual.output_tokens = True
 
     # remove text encoder to save footprint and memory
     if hasattr(clip_model, 'text'):
         del clip_model.text
```

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/generation.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/generation.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/llama/loading.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/llama/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/loading.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/moss/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/moss/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/pythia/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/pythia/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/rwkv/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/rwkv/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/stablelm/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/vicuna/loading.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/models/vicuna/modeling.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/models/vicuna/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/profile.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/base.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/serve/executors/flamingo.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/serve/executors/flamingo.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/serve/playground/gradio.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/serve/playground/gradio_chatbot.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_chatbot.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/open_gpt/serve/playground/gradio_css.py` & `open_gpt_torch-0.0.7.dev3/open_gpt/serve/playground/gradio_css.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.7.dev2/pyproject.toml` & `open_gpt_torch-0.0.7.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.7.dev2"
+version = "0.0.7.dev3"
 description = "An open-source cloud-native of large multi-modal models (LMMs) serving framework."
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
```

### Comparing `open_gpt_torch-0.0.7.dev2/PKG-INFO` & `open_gpt_torch-0.0.7.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.7.dev2
+Version: 0.0.7.dev3
 Summary: An open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://github.com/jina-ai/opengpt
 License: Apache-2.0
 Keywords: Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-inference,llama,vicuna,stabellm
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.7.dev2 Summary: An
+Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.7.dev3 Summary: An
 open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://github.com/jina-ai/opengpt License: Apache-2.0 Keywords:
 Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-
 inference,llama,vicuna,stabellm Author: Jina AI Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
```

