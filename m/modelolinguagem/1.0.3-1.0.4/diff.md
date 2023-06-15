# Comparing `tmp/modelolinguagem-1.0.3.tar.gz` & `tmp/modelolinguagem-1.0.4.tar.gz`

## Comparing `modelolinguagem-1.0.3.tar` & `modelolinguagem-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/requirements.txt
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/setup.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/__init__.py
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/modelolinguagem.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/mensurador/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/mensurador/medidas.py
--rw-r--r--   0        0        0    36654 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/mensurador/mensurador.py
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/mensurador/mensuradorenum.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/modelo/__init__.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/modelo/modeloarguments.py
--rw-r--r--   0        0        0    26985 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/modelo/transformer.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/nlp/__init__.py
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/nlp/nlpmodulo.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/util/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/util/utilambiente.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/util/utilarquivo.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/util/utilconstantes.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/util/utilmodulo.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/modelolinguagem/util/utiltempo.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/LICENSE
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/README.md
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 modelolinguagem-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/requirements.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/__init__.py
+-rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelolinguagem.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/medidas.py
+-rw-r--r--   0        0        0    36654 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/mensurador.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/mensuradorenum.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelo/__init__.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelo/modeloarguments.py
+-rw-r--r--   0        0        0    26985 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelo/transformer.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/nlp/__init__.py
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/nlp/nlpmodulo.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilambiente.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilarquivo.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilconstantes.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilmodulo.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utiltempo.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/LICENSE
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/README.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/PKG-INFO
```

### Comparing `modelolinguagem-1.0.3/modelolinguagem/modelolinguagem.py` & `modelolinguagem-1.0.4/modelolinguagem/modelolinguagem.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/mensurador/medidas.py` & `modelolinguagem-1.0.4/modelolinguagem/mensurador/medidas.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/mensurador/mensurador.py` & `modelolinguagem-1.0.4/modelolinguagem/mensurador/mensurador.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/mensurador/mensuradorenum.py` & `modelolinguagem-1.0.4/modelolinguagem/mensurador/mensuradorenum.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/modelo/modeloarguments.py` & `modelolinguagem-1.0.4/modelolinguagem/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/modelo/transformer.py` & `modelolinguagem-1.0.4/modelolinguagem/modelo/transformer.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/nlp/nlpmodulo.py` & `modelolinguagem-1.0.4/modelolinguagem/nlp/nlpmodulo.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/util/utilambiente.py` & `modelolinguagem-1.0.4/modelolinguagem/util/utilambiente.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/util/utilarquivo.py` & `modelolinguagem-1.0.4/modelolinguagem/util/utilarquivo.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/util/utilconstantes.py` & `modelolinguagem-1.0.4/modelolinguagem/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/util/utilmodulo.py` & `modelolinguagem-1.0.4/modelolinguagem/util/utilmodulo.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/modelolinguagem/util/utiltempo.py` & `modelolinguagem-1.0.4/modelolinguagem/util/utiltempo.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/LICENSE` & `modelolinguagem-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.3/pyproject.toml` & `modelolinguagem-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "modelolinguagem"
-version = "1.0.3"
+version = "1.0.4"
 description = "Framework Multilingual para processamento de textos utilizando modelos de linguagem"
 readme = "README.md"
 requires-python = ">=3.6.0"
 license = { file = "LICENSE" }
 
 authors = [
     { name = "Osmar de Oliveira Braz Junior", email = "osmar.braz@udesc.br" }
```

### Comparing `modelolinguagem-1.0.3/PKG-INFO` & `modelolinguagem-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelolinguagem
-Version: 1.0.3
+Version: 1.0.4
 Summary: Framework Multilingual para processamento de textos utilizando modelos de linguagem
 Project-URL: repository, https://github.com/osmarbraz/modelolinguagem/
 Author-email: Osmar de Oliveira Braz Junior <osmar.braz@udesc.br>
 License: MIT License
         
         Copyright (c) 2023 Osmar de Oliveira Braz Junior
         
@@ -33,28 +33,24 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.0
 Requires-Dist: spacy==3.5.2
 Requires-Dist: transformers==4.26.1
 Description-Content-Type: text/markdown
 
-# Framework Multilingual de Modelo de Linguagem 
-
-Framework Multilingual para processamento de textos utilizando modelos de linguagem;
-
-Gera embeddings de textos, sentenças, palavras e tokens utilizando modelos contextualizados de linguagem.
+# Framework Multilingual para processamento de textos utilizando modelos de linguagem.
 
+Gera embeddings de textos, sentenças, palavras e tokens utilizando modelos contextualizados de linguagem multilingual.
 
 ## Instalação
 
 Para instalar o pacote, basta executar o comando abaixo:
 
 <pre><code>pip install modelolinguagem</code></pre>
 
-
 ## Dependências
 - transformers==4.26.1
 - spacy==3.5.2
 
 ## Licença
 
 Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

