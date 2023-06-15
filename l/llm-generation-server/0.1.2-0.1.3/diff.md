# Comparing `tmp/llm_generation_server-0.1.2.tar.gz` & `tmp/llm_generation_server-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_generation_server-0.1.2.tar", last modified: Thu Jun 15 09:48:51 2023, max compression
+gzip compressed data, was "llm_generation_server-0.1.3.tar", last modified: Thu Jun 15 09:58:16 2023, max compression
```

## Comparing `llm_generation_server-0.1.2.tar` & `llm_generation_server-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.494334 llm_generation_server-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-15 09:48:51.494334 llm_generation_server-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.490334 llm_generation_server-0.1.2/llm_generation_server/
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/component_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.490334 llm_generation_server-0.1.2/llm_generation_server/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/components/DialogueVisualizationComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/components/GenerationComponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/components/NextTokenPredictionComponent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.490334 llm_generation_server-0.1.2/llm_generation_server/components/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/components/mixins/data_preparation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/components/mixins/generation_selectors_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/components/mixins/metrics_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/components/mixins/model_selection_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.490334 llm_generation_server-0.1.2/llm_generation_server/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.490334 llm_generation_server-0.1.2/llm_generation_server/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   201746 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/dist/assets/index-9006265c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/dist/assets/index-d8f16c2e.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.494334 llm_generation_server-0.1.2/llm_generation_server/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/elements/barchart_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/elements/element_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/elements/plain_text_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/elements/selector_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/elements/table_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/llm_generation_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:48:51.490334 llm_generation_server-0.1.2/llm_generation_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-15 09:48:51.000000 llm_generation_server-0.1.2/llm_generation_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-15 09:48:51.000000 llm_generation_server-0.1.2/llm_generation_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:48:51.000000 llm_generation_server-0.1.2/llm_generation_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 09:48:51.000000 llm_generation_server-0.1.2/llm_generation_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 09:48:51.000000 llm_generation_server-0.1.2/llm_generation_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 09:48:38.000000 llm_generation_server-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:48:51.494334 llm_generation_server-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.839466 llm_generation_server-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-15 09:58:16.839466 llm_generation_server-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.835466 llm_generation_server-0.1.3/llm_generation_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/component_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.835466 llm_generation_server-0.1.3/llm_generation_server/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/components/DatasetVisualizationComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/components/GenerationComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/components/NextTokenPredictionComponent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.839466 llm_generation_server-0.1.3/llm_generation_server/components/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/components/mixins/data_preparation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/components/mixins/generation_selectors_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/components/mixins/metrics_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/components/mixins/model_selection_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.839466 llm_generation_server-0.1.3/llm_generation_server/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.839466 llm_generation_server-0.1.3/llm_generation_server/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   201746 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/dist/assets/index-9006265c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/dist/assets/index-d8f16c2e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.839466 llm_generation_server-0.1.3/llm_generation_server/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/elements/barchart_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/elements/element_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/elements/plain_text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/elements/selector_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/elements/table_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/llm_generation_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:58:16.835466 llm_generation_server-0.1.3/llm_generation_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-15 09:58:16.000000 llm_generation_server-0.1.3/llm_generation_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-15 09:58:16.000000 llm_generation_server-0.1.3/llm_generation_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:58:16.000000 llm_generation_server-0.1.3/llm_generation_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 09:58:16.000000 llm_generation_server-0.1.3/llm_generation_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 09:58:16.000000 llm_generation_server-0.1.3/llm_generation_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 09:58:07.000000 llm_generation_server-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:58:16.839466 llm_generation_server-0.1.3/setup.cfg
```

### Comparing `llm_generation_server-0.1.2/LICENSE` & `llm_generation_server-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/PKG-INFO` & `llm_generation_server-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: llm_generation_server
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple full stack app for displaying distribution of next token.
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/llm_generation_server
 Project-URL: Bug Tracker, https://github.com/gortibaldik/llm_generation_server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.2`
+## VERSION: `0.1.3`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.1.2/README.md` & `llm_generation_server-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.2`
+## VERSION: `0.1.3`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.1.2/llm_generation_server/component_base.py` & `llm_generation_server-0.1.3/llm_generation_server/component_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/components/DialogueVisualizationComponent.py` & `llm_generation_server-0.1.3/llm_generation_server/components/DatasetVisualizationComponent.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/components/GenerationComponent.py` & `llm_generation_server-0.1.3/llm_generation_server/components/GenerationComponent.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/components/NextTokenPredictionComponent.py` & `llm_generation_server-0.1.3/llm_generation_server/components/NextTokenPredictionComponent.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/components/mixins/data_preparation_mixin.py` & `llm_generation_server-0.1.3/llm_generation_server/components/mixins/data_preparation_mixin.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/components/mixins/generation_selectors_mixin.py` & `llm_generation_server-0.1.3/llm_generation_server/components/mixins/generation_selectors_mixin.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/components/mixins/metrics_mixin.py` & `llm_generation_server-0.1.3/llm_generation_server/components/mixins/metrics_mixin.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/components/mixins/model_selection_mixin.py` & `llm_generation_server-0.1.3/llm_generation_server/components/mixins/model_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/dist/assets/index-9006265c.js` & `llm_generation_server-0.1.3/llm_generation_server/dist/assets/index-9006265c.js`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/dist/assets/index-d8f16c2e.css` & `llm_generation_server-0.1.3/llm_generation_server/dist/assets/index-d8f16c2e.css`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/dist/favicon.ico` & `llm_generation_server-0.1.3/llm_generation_server/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/elements/barchart_element.py` & `llm_generation_server-0.1.3/llm_generation_server/elements/barchart_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/elements/element_base.py` & `llm_generation_server-0.1.3/llm_generation_server/elements/element_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/elements/plain_text_element.py` & `llm_generation_server-0.1.3/llm_generation_server/elements/plain_text_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/elements/selector_elements.py` & `llm_generation_server-0.1.3/llm_generation_server/elements/selector_elements.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/elements/table_element.py` & `llm_generation_server-0.1.3/llm_generation_server/elements/table_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/elements/utils.py` & `llm_generation_server-0.1.3/llm_generation_server/elements/utils.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server/server.py` & `llm_generation_server-0.1.3/llm_generation_server/server.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.1.2/llm_generation_server.egg-info/PKG-INFO` & `llm_generation_server-0.1.3/llm_generation_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: llm-generation-server
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple full stack app for displaying distribution of next token.
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/llm_generation_server
 Project-URL: Bug Tracker, https://github.com/gortibaldik/llm_generation_server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.1.2`
+## VERSION: `0.1.3`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.1.2/llm_generation_server.egg-info/SOURCES.txt` & `llm_generation_server-0.1.3/llm_generation_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 llm_generation_server/component_base.py
 llm_generation_server/server.py
 llm_generation_server.egg-info/PKG-INFO
 llm_generation_server.egg-info/SOURCES.txt
 llm_generation_server.egg-info/dependency_links.txt
 llm_generation_server.egg-info/requires.txt
 llm_generation_server.egg-info/top_level.txt
-llm_generation_server/components/DialogueVisualizationComponent.py
+llm_generation_server/components/DatasetVisualizationComponent.py
 llm_generation_server/components/GenerationComponent.py
 llm_generation_server/components/NextTokenPredictionComponent.py
 llm_generation_server/components/mixins/data_preparation_mixin.py
 llm_generation_server/components/mixins/generation_selectors_mixin.py
 llm_generation_server/components/mixins/metrics_mixin.py
 llm_generation_server/components/mixins/model_selection_mixin.py
 llm_generation_server/dist/favicon.ico
```

### Comparing `llm_generation_server-0.1.2/pyproject.toml` & `llm_generation_server-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm_generation_server"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Frantisek Trebuna (gortibaldik)", email="ferotre@gmail.com" },
 ]
 description = "Simple full stack app for displaying distribution of next token."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -34,15 +34,15 @@
 [tool.setuptools.package-dir]
 llm_generation_server = "llm_generation_server"
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

