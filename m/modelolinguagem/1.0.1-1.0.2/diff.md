# Comparing `tmp/modelolinguagem-1.0.1.tar.gz` & `tmp/modelolinguagem-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelolinguagem-1.0.1.tar", last modified: Thu Jun 15 18:09:11 2023, max compression
+gzip compressed data, was "modelolinguagem-1.0.2.tar", last modified: Thu Jun 15 18:21:35 2023, max compression
```

## Comparing `modelolinguagem-1.0.1.tar` & `modelolinguagem-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:09:11.758535 modelolinguagem-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-15 18:09:11.758535 modelolinguagem-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:09:11.755535 modelolinguagem-1.0.1/modelolinguagem/
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:09:11.756535 modelolinguagem-1.0.1/modelolinguagem/mensurador/
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/mensurador/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/mensurador/medidas.py
--rw-r--r--   0 root         (0) root         (0)    36664 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/mensurador/mensurador.py
--rw-r--r--   0 root         (0) root         (0)     3752 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/mensurador/mensuradorenum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:09:11.756535 modelolinguagem-1.0.1/modelolinguagem/modelo/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/modelo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2882 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/modelo/modeloarguments.py
--rw-r--r--   0 root         (0) root         (0)    26991 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/modelo/transformer.py
--rw-r--r--   0 root         (0) root         (0)    10361 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/modelolinguagem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:09:11.757535 modelolinguagem-1.0.1/modelolinguagem/nlp/
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14149 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/nlp/nlpmodulo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:09:11.757535 modelolinguagem-1.0.1/modelolinguagem/util/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1000 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/util/utilambiente.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/util/utilarquivo.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/util/utilconstantes.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/util/utilmodulo.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-06-15 18:03:16.000000 modelolinguagem-1.0.1/modelolinguagem/util/utiltempo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:09:11.755535 modelolinguagem-1.0.1/modelolinguagem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-15 18:09:11.000000 modelolinguagem-1.0.1/modelolinguagem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      840 2023-06-15 18:09:11.000000 modelolinguagem-1.0.1/modelolinguagem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 18:09:11.000000 modelolinguagem-1.0.1/modelolinguagem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-15 18:09:11.000000 modelolinguagem-1.0.1/modelolinguagem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 18:09:11.000000 modelolinguagem-1.0.1/modelolinguagem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 18:09:11.758535 modelolinguagem-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1025 2023-06-15 18:08:25.000000 modelolinguagem-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:21:35.588491 modelolinguagem-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-15 18:21:35.586490 modelolinguagem-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:21:35.577490 modelolinguagem-1.0.2/modelolinguagem/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:21:35.581490 modelolinguagem-1.0.2/modelolinguagem/mensurador/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/mensurador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/mensurador/medidas.py
+-rw-r--r--   0 root         (0) root         (0)    36654 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/mensurador/mensurador.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/mensurador/mensuradorenum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:21:35.582490 modelolinguagem-1.0.2/modelolinguagem/modelo/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/modelo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/modelo/modeloarguments.py
+-rw-r--r--   0 root         (0) root         (0)    26985 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/modelo/transformer.py
+-rw-r--r--   0 root         (0) root         (0)    10367 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/modelolinguagem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:21:35.583490 modelolinguagem-1.0.2/modelolinguagem/nlp/
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14159 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/nlp/nlpmodulo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:21:35.585491 modelolinguagem-1.0.2/modelolinguagem/util/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/util/utilambiente.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/util/utilarquivo.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/util/utilconstantes.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/util/utilmodulo.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/modelolinguagem/util/utiltempo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 18:21:35.579490 modelolinguagem-1.0.2/modelolinguagem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-15 18:21:35.000000 modelolinguagem-1.0.2/modelolinguagem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      840 2023-06-15 18:21:35.000000 modelolinguagem-1.0.2/modelolinguagem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 18:21:35.000000 modelolinguagem-1.0.2/modelolinguagem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-15 18:21:35.000000 modelolinguagem-1.0.2/modelolinguagem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 18:21:35.000000 modelolinguagem-1.0.2/modelolinguagem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 18:21:35.589491 modelolinguagem-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-15 18:21:31.000000 modelolinguagem-1.0.2/setup.py
```

### Comparing `modelolinguagem-1.0.1/LICENSE` & `modelolinguagem-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/PKG-INFO` & `modelolinguagem-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelolinguagem
-Version: 1.0.1
+Version: 1.0.2
 Summary: Multilingual text embeddings
 Download-URL: https://github.com/osmarbraz/modelolinguagem/
 Author: Osmar de Oliveira Braz Junior
 Author-email: osmar.braz@udesc.br
 License: MIT
 Keywords: Transformer embedding texto sentença palavra token
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `modelolinguagem-1.0.1/modelolinguagem/mensurador/medidas.py` & `modelolinguagem-1.0.2/modelolinguagem/mensurador/medidas.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/modelolinguagem/mensurador/mensurador.py` & `modelolinguagem-1.0.2/modelolinguagem/mensurador/mensurador.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Import das bibliotecas.
 import logging  # Biblioteca de logging
 import torch # Biblioteca de aprendizado de máquina
 
 # Import de bibliotecas próprias
-from util.utilmodulo import *
-from util.utiltempo import *
-from util.utilarquivo import *
-from util.utilconstantes import *
+from ..util.utilmodulo import *
+from ..util.utiltempo import *
+from ..util.utilarquivo import *
+from ..util.utilconstantes import *
 
-from nlp.nlpmodulo import *
-from mensurador.medidas import *
-from mensurador.mensuradorenum import *
+from ..nlp.nlpmodulo import *
+from .medidas import *
+from .mensuradorenum import *
 
 logger = logging.getLogger(__name__)
 
 class Mensurador:
 
     ''' 
     Realiza mensurações em textos.
```

### Comparing `modelolinguagem-1.0.1/modelolinguagem/mensurador/mensuradorenum.py` & `modelolinguagem-1.0.2/modelolinguagem/mensurador/mensuradorenum.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/modelolinguagem/modelo/modeloarguments.py` & `modelolinguagem-1.0.2/modelolinguagem/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/modelolinguagem/modelo/transformer.py` & `modelolinguagem-1.0.2/modelolinguagem/modelo/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 # Biblioteca de tipos
 from typing import List, Dict, Optional, Union, Tuple
 # Biblioteca de manipulação sistema
 import os
 
 # Biblioteca dos modelos de linguagem
-from modelo.modeloarguments import ModeloArgumentos
+from .modeloarguments import ModeloArgumentos
 
 logger = logging.getLogger(__name__)
 
 class Transformer(nn.Module):
     '''
     Huggingface AutoModel para gerar embeddings de token, palavra, sentença ou texto.
     Carrega a classe correta, por exemplo BERT / RoBERTa etc.
```

### Comparing `modelolinguagem-1.0.1/modelolinguagem/modelolinguagem.py` & `modelolinguagem-1.0.2/modelolinguagem/modelolinguagem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Import das bibliotecas.
 import logging  # Biblioteca de logging
 
 # Biblioteca dos modelos de linguagem
-from modelo.modeloarguments import ModeloArgumentos
-from nlp.nlpmodulo import *
-from util.utilconstantes import *
-from mensurador.mensuradorenum import *
-from mensurador.mensurador import Mensurador
-from modelo.transformer import *
+from .modelo.modeloarguments import ModeloArgumentos
+from .nlp.nlpmodulo import *
+from .util.utilconstantes import *
+from .mensurador.mensuradorenum import *
+from .mensurador.mensurador import Mensurador
+from .modelo.transformer import *
 
 logger = logging.getLogger(__name__)
 
 # Definição dos parâmetros do Modelo para os cálculos das Medidas
 modelo_argumentos = ModeloArgumentos(
         max_seq_len=512,
         pretrained_model_name_or_path="neuralmind/bert-base-portuguese-cased", # Nome do modelo de linguagem pré-treinado Transformer
```

### Comparing `modelolinguagem-1.0.1/modelolinguagem/nlp/nlpmodulo.py` & `modelolinguagem-1.0.2/modelolinguagem/nlp/nlpmodulo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import logging  # Biblioteca de logging
 import os # Biblioteca de manipulação de arquivos
 import spacy # Biblioteca do spaCy
 from spacy.util import filter_spans
 from spacy.matcher import Matcher
 
 # Import de bibliotecas próprias
-from util.utilmodulo import *
-from util.utiltempo import *
-from util.utilarquivo import *
-from util.utilambiente import *
-from mensurador.mensuradorenum import *
+from ..util.utilmodulo import *
+from ..util.utiltempo import *
+from ..util.utilarquivo import *
+from ..util.utilambiente import *
+from ..mensurador.mensuradorenum import *
 
 logger = logging.getLogger(__name__)
 
 class NLP():
 
     ''' 
     Realiza o processamento de linguagem natural.
```

### Comparing `modelolinguagem-1.0.1/modelolinguagem/util/utilambiente.py` & `modelolinguagem-1.0.2/modelolinguagem/util/utilambiente.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/modelolinguagem/util/utilarquivo.py` & `modelolinguagem-1.0.2/modelolinguagem/util/utilarquivo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging  # Biblioteca de logging
 import requests # Biblioteca de download
 from tqdm.notebook import tqdm as tqdm_notebook # Biblioteca para barra de progresso
 import os # Biblioteca para manipular arquivos
 import sys
 
 # Import de bibliotecas próprias
-from util.utilmodulo import *
-from util.utiltempo import *
-from util.utilconstantes import *
+from .utilmodulo import *
+from .utiltempo import *
+from .utilconstantes import *
 
 logger = logging.getLogger(__name__)
 
 # ============================  
 def verificaDiretorioModeloLinguagem():
     '''    
     Verifica se existe o diretório modelo_linguagem no diretório corrente.
```

### Comparing `modelolinguagem-1.0.1/modelolinguagem/util/utilconstantes.py` & `modelolinguagem-1.0.2/modelolinguagem/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/modelolinguagem/util/utilmodulo.py` & `modelolinguagem-1.0.2/modelolinguagem/util/utilmodulo.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/modelolinguagem/util/utiltempo.py` & `modelolinguagem-1.0.2/modelolinguagem/util/utiltempo.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/modelolinguagem.egg-info/PKG-INFO` & `modelolinguagem-1.0.2/modelolinguagem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelolinguagem
-Version: 1.0.1
+Version: 1.0.2
 Summary: Multilingual text embeddings
 Download-URL: https://github.com/osmarbraz/modelolinguagem/
 Author: Osmar de Oliveira Braz Junior
 Author-email: osmar.braz@udesc.br
 License: MIT
 Keywords: Transformer embedding texto sentença palavra token
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `modelolinguagem-1.0.1/modelolinguagem.egg-info/SOURCES.txt` & `modelolinguagem-1.0.2/modelolinguagem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.1/setup.py` & `modelolinguagem-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", mode="r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="modelolinguagem",
-    version="1.0.1",
+    version="1.0.2",
     author="Osmar de Oliveira Braz Junior",
     author_email="osmar.braz@udesc.br",
     description="Multilingual text embeddings",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",    
     download_url="https://github.com/osmarbraz/modelolinguagem/",
```

