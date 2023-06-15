# Comparing `tmp/pyBibX-2.9.9.tar.gz` & `tmp/pyBibX-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-2.9.9.tar", last modified: Sun May  7 23:37:03 2023, max compression
+gzip compressed data, was "dist\pyBibX-3.0.2.tar", last modified: Thu Jun 15 01:46:04 2023, max compression
```

## Comparing `pyBibX-2.9.9.tar` & `pyBibX-3.0.2.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 23:37:03.000000 pyBibX-2.9.9/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.9/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.9/MANIFEST.in
--rw-rw-rw-   0        0        0     9608 2023-05-07 23:37:03.000000 pyBibX-2.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-2.9.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.9/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.9/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   264479 2023-05-06 13:57:56.000000 pyBibX-2.9.9/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-05-07 23:37:03.000000 pyBibX-2.9.9/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.9/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9608 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-05-07 23:37:02.000000 pyBibX-2.9.9/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-07 23:37:01.000000 pyBibX-2.9.9/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-07 23:37:03.000000 pyBibX-2.9.9/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-05-06 14:26:46.000000 pyBibX-2.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:04.000000 pyBibX-3.0.2/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9608 2023-06-15 01:46:04.000000 pyBibX-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:04.000000 pyBibX-3.0.2/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.2/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:04.000000 pyBibX-3.0.2/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.0.2/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   263380 2023-06-15 01:43:03.000000 pyBibX-3.0.2/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:04.000000 pyBibX-3.0.2/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.2/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:04.000000 pyBibX-3.0.2/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-06-15 01:46:02.000000 pyBibX-3.0.2/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-06-15 01:46:03.000000 pyBibX-3.0.2/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:46:02.000000 pyBibX-3.0.2/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-06-15 01:46:02.000000 pyBibX-3.0.2/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 01:46:02.000000 pyBibX-3.0.2/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 01:46:02.000000 pyBibX-3.0.2/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-15 01:46:04.000000 pyBibX-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-06-02 23:11:46.000000 pyBibX-3.0.2/setup.py
```

### Comparing `pyBibX-2.9.9/LICENSE` & `pyBibX-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/PKG-INFO` & `pyBibX-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.9
+Version: 3.0.2
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-2.9.9/README.md` & `pyBibX-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/pbx.py` & `pyBibX-3.0.2/pyBibX/base/pbx.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # Citation: 
 # PEREIRA, V. (2022). Project: pyBibX, File: pbibx.py, GitHub repository: <https://github.com/Valdecy/pyBibX>
 
 ############################################################################
 
 # Required Libraries
+import chardet
 import networkx as nx             
 import numpy as np   
 import openai              
 import pandas as pd               
 import plotly.graph_objects as go
 import plotly.subplots as ps      
 import plotly.io as pio           
@@ -49,25 +50,31 @@
 
 ############################################################################
 
 # pbx Class
 class pbx_probe():
     def __init__(self, file_bib, db = 'scopus', del_duplicated = True):
         self.data_base         =  db
-        self.institution_names =  [ 'chuo kikuu', 'egyetemi', 'eyunivesithi', 'háskóli', 'inivèsite', 'inyuvesi', 'iunivesite',
-                                    'jaamacad', "jami'a", 'kulanui', 'mahadum', 'oilthigh', 'ollscoile', 'oniversite', 'prifysgol',
-                                    'sveučilište', 'unibersidad', 'unibertsitatea', 'univ', 'universidad', 'universidade',
-                                    'universitas', 'universitat', 'universitate', 'universitato', 'universiteit', 'universitet',
-                                    'universitetas', 'universiti', 'università', 'universität', 'université', 'universite',
-                                    'universitāte', 'univerza', 'univerzita', 'univerzitet', 'univesithi', 'uniwersytet',
-                                    'vniuersitatis', 'whare wananga', 'yliopisto', 'yunifasiti', 'yunivesite', 'yunivhesiti',
-                                    'zanko', 'ülikool', 'üniversite', 'πανεπιστήμιο', 'универзитет', 'университет', 'універсітэт',
-                                    'university', 'academy', 'institut', 'supérieur', 'ibmec', 'uff', 'gradevinski', 'lab.', 
-                                    'politecnico', 'research', 'laborat', 'college'
+        self.institution_names =  [ 'academy', 'center', 'centre', 'chuo kikuu', 'college', 'conservatory', 'egyetemi'
+                                    'escola', 'escuela', 'eyunivesithi', 'faculdade', 'facultad', 'fakultet', 'fakultät'
+                                    'foundation', 'gradevinski', 'hochschule', 'hogeschool', 'háskóli', 'högskola', 'ibmec'
+                                    'inivèsite', 'institut', 'institute of technology', 'inyuvesi', 'iskola', 'iunivesite'
+                                    'jaamacad', "jami'a", 'kolej', 'koulu', 'kulanui', 'lab.', 'laborat', 'mahadum', 'medical'
+                                    'observatory', 'oilthigh', 'okulu', 'ollscoile', 'oniversite', 'politecnico', 'polytechnic'
+                                    'prifysgol', 'research', 'school', 'schule', 'scuola', 'seminary', 'skola', 'supérieur'
+                                    'sveučilište', 'szkoła', 'technological', 'uff', 'unibersidad', 'unibertsitatea', 'univ'
+                                    'universidad', 'universidade', 'universitas', 'universitat', 'universitate', 'universitato'
+                                    'universite', 'universiteit', 'universitet', 'universitetas', 'universiti', 'university'
+                                    'università', 'universität', 'université', 'universitāte', 'univerza', 'univerzita'
+                                    'univerzitet', 'univesithi', 'uniwersytet', 'vniuersitatis', 'whare wananga', 'yliopisto'
+                                    'yunifasiti', 'yunivesite', 'yunivhesiti', 'zanko', 'école', 'ülikool', 'üniversite'
+                                    'πανεπιστήμιο', 'σχολείο', 'универзитет', 'университет', 'універсітэт', 'школа'
                                   ]
+
+
         self.language_names  =    { 'afr': 'Afrikaans', 'alb': 'Albanian','amh': 'Amharic', 'ara': 'Arabic', 'arm': 'Armenian', 
                                     'aze': 'Azerbaijani', 'bos': 'Bosnian', 'bul': 'Bulgarian', 'cat': 'Catalan', 'chi': 'Chinese', 
                                     'cze': 'Czech', 'dan': 'Danish', 'dut': 'Dutch', 'eng': 'English', 'epo': 'Esperanto', 
                                     'est': 'Estonian', 'fin': 'Finnish', 'fre': 'French', 'geo': 'Georgian', 'ger': 'German', 
                                     'gla': 'Scottish Gaelic', 'gre': 'Greek, Modern', 'heb': 'Hebrew', 'hin': 'Hindi', 
                                     'hrv': 'Croatian', 'hun': 'Hungarian', 'ice': 'Icelandic', 'ind': 'Indonesian', 'ita': 'Italian', 
                                     'jpn': 'Japanese', 'kin': 'Kinyarwanda', 'kor': 'Korean', 'lat': 'Latin', 'lav': 'Latvian', 
@@ -1124,14 +1131,25 @@
         data['keywords']        = data['keywords'].apply(lambda x: x.replace(',',';'))
         data['author_keywords'] = data['author_keywords'].apply(lambda x: x.replace(',',';'))
         if (db == 'wos'):
             idx     = data[data['year'] == 'UNKNOW'].index.values
             idx_val = [data.loc[i, 'da'][:4] for i in idx]
             for i in range(0, len(idx)):
                 data.iloc[idx[i], -1] = idx_val[i]
+        if ('affiliation' in data.columns and 'affiliation_' in data.columns):
+            filtered_indices = data[(data['affiliation'] == 'UNKNOW') & (data['affiliation_'] != 'UNKNOW')].index
+            filtered_indices = list(filtered_indices)
+            for i in filtered_indices:
+                s         = data.loc[i, 'affiliation_']
+                parts     = s.split('.')
+                parts[0]  = re.sub(r'.*?\(Corresponding Author\), ', '', parts[0]) 
+                new_parts = [part.split(',', 1)[-1].strip() for part in parts[1:] if ',' in part]
+                new_parts.insert(0, parts[0])
+                new_s     = '. '.join(new_parts)
+                data.loc[i, 'affiliation'] =  new_s
         data = data.reindex(sorted(data.columns), axis = 1)
         return data, entries
     
     # Function: Update Verbose
     def __update_vb(self):
         self.vb   = []
         self.vb.append('A Total of ' + str(self.data.shape[0]) + ' Documents Remains' )
@@ -1481,74 +1499,76 @@
             corpora = pd.Series([' '.join(a) for a in self.auk] )
         elif (entry == 'abs'):
             corpora = self.data['abstract']
         elif (entry == 'title'):
             corpora = self.data['title']
         if (len(stop_words) > 0):
             for sw_ in stop_words: 
-                if   (sw_ == 'ar' or sw_ == 'ara'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Arabic.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Arabic.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'bn' or sw_ == 'ben'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Bengali.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Bengali.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'bg' or sw_ == 'bul'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Bulgarian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Bulgarian.txt', 'r',     encoding = 'utf8')
-                elif (sw_ == 'cs' or sw_ == 'cze' or sw_ == 'ces'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Czech.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Czech.txt', 'r',         encoding = 'utf8')
-                elif (sw_ == 'en' or sw_ == 'eng'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-English.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-English.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'fi' or sw_ == 'fin'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Finnish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Finnish.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'fr' or sw_ == 'fre' or sw_ == 'fra'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-French.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-French.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'de' or sw_ == 'ger' or sw_ == 'deu'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-German.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-German.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'hi' or sw_ == 'hin'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hind.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Hindi.txt', 'r',         encoding = 'utf8')
-                elif (sw_ == 'hu' or sw_ == 'hun'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hungarian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Hungarian.txt', 'r',     encoding = 'utf8')
-                elif (sw_ == 'it' or sw_ == 'ita'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Italian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Italian.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'mr' or sw_ == 'mar'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Marathi.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Marathi.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'fa' or sw_ == 'per' or sw_ == 'fas'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Persian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Persian.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'pl' or sw_ == 'pol'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Polish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Polish.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'pt-br' or sw_ == 'por-br'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Portuguese-br.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Portuguese-br.txt', 'r', encoding = 'utf8')
-                elif (sw_ == 'ro' or sw_ == 'rum' or sw_ == 'ron'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Romanian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Romanian.txt', 'r',      encoding = 'utf8')
-                elif (sw_ == 'ru' or sw_ == 'rus'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Russian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Russian.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'es' or sw_ == 'spa'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Spanish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Spanish.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'sv' or sw_ == 'swe'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Swedish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Swedish.txt', 'r',       encoding = 'utf8')
-                f_lines = f_file.read()
-                sw      = f_lines.split('\n')
-                sw      = list(filter(None, sw))
+                if   (sw_ == 'ar' or sw_ == 'ara' or sw_ == 'arabic'):
+                    name = 'Stopwords-Arabic.txt'
+                elif (sw_ == 'bn' or sw_ == 'ben' or sw_ == 'bengali'):
+                    name = 'Stopwords-Bengali.txt'
+                elif (sw_ == 'bg' or sw_ == 'bul' or sw_ == 'bulgarian'):
+                    name = 'Stopwords-Bulgarian.txt'
+                elif (sw_ == 'zh' or sw_ == 'chi' or sw_ == 'chinese'):
+                    name = 'Stopwords-Chinese.txt'
+                elif (sw_ == 'cs' or sw_ == 'cze' or sw_ == 'ces' or sw_ == 'czech'):
+                    name = 'Stopwords-Czech.txt'
+                elif (sw_ == 'en' or sw_ == 'eng' or sw_ == 'english'):
+                    name = 'Stopwords-English.txt'
+                elif (sw_ == 'fi' or sw_ == 'fin' or sw_ == 'finnish'):
+                    name = 'Stopwords-Finnish.txt'
+                elif (sw_ == 'fr' or sw_ == 'fre' or sw_ == 'fra' or sw_ == 'french'):
+                    name = 'Stopwords-French.txt'
+                elif (sw_ == 'de' or sw_ == 'ger' or sw_ == 'deu' or sw_ == 'german'):
+                    name = 'Stopwords-German.txt'
+                elif (sw_ == 'el' or sw_ == 'gre' or sw_ == 'greek'):
+                    name = 'Stopwords-Greek.txt'
+                elif (sw_ == 'he' or sw_ == 'heb' or sw_ == 'hebrew'):
+                    name = 'Stopwords-Hebrew.txt'
+                elif (sw_ == 'hi' or sw_ == 'hin' or sw_ == 'hind'):
+                    name = 'Stopwords-Hind.txt'
+                elif (sw_ == 'hu' or sw_ == 'hun' or sw_ == 'hungarian'):
+                    name = 'Stopwords-Hungarian.txt'
+                elif (sw_ == 'it' or sw_ == 'ita' or sw_ == 'italian'):
+                    name = 'Stopwords-Italian.txt'
+                elif (sw_ == 'ja' or sw_ == 'jpn' or sw_ == 'japanese'):
+                    name = 'Stopwords-Japanese.txt'
+                elif (sw_ == 'ko' or sw_ == 'kor' or sw_ == 'korean'):
+                    name = 'Stopwords-Korean.txt'
+                elif (sw_ == 'mr' or sw_ == 'mar' or sw_ == 'marathi'):
+                    name = 'Stopwords-Marathi.txt'
+                elif (sw_ == 'fa' or sw_ == 'per' or sw_ == 'fas' or sw_ == 'persian'):
+                    name = 'Stopwords-Persian.txt'
+                elif (sw_ == 'pl' or sw_ == 'pol' or sw_ == 'polish'):
+                    name = 'Stopwords-Polish.txt'
+                elif (sw_ == 'pt-br' or sw_ == 'por-br' or sw_ == 'portuguese-br'):
+                    name = 'Stopwords-Portuguese-br.txt'
+                elif (sw_ == 'ro' or sw_ == 'rum' or sw_ == 'ron' or sw_ == 'romanian'):
+                    name = 'Stopwords-Romanian.txt'
+                elif (sw_ == 'ru' or sw_ == 'rus' or sw_ == 'russian'):
+                    name = 'Stopwords-Russian.txt'
+                elif (sw_ == 'sk' or sw_ == 'slo' or sw_ == 'slovak'):
+                    name = 'Stopwords-Slovak.txt'
+                elif (sw_ == 'es' or sw_ == 'spa' or sw_ == 'spanish'):
+                    name = 'Stopwords-Spanish.txt'
+                elif (sw_ == 'sv' or sw_ == 'swe' or sw_ == 'swedish'):
+                    name = 'Stopwords-Swedish.txt'
+                elif (sw_ == 'th' or sw_ == 'tha' or sw_ == 'thai'):
+                    name = 'Stopwords-Thai.txt'
+                elif (sw_ == 'uk' or sw_ == 'ukr' or sw_ == 'ukrainian'):
+                    name = 'Stopwords-Ukrainian.txt'
+                with pkg_resources.open_binary(stws, name) as file:
+                    raw_data = file.read()
+                result   = chardet.detect(raw_data)
+                encoding = result['encoding']
+                with pkg_resources.open_text(stws, name, encoding = encoding) as file:
+                    content = file.read().split('\n')
+                content = [line.rstrip('\r').rstrip('\n') for line in content]
+                sw      = list(filter(None, content))
                 sw_full.extend(sw)
         if (len(rmv_custom_words) > 0):
             sw_full.extend(rmv_custom_words)
         try:
             vec = CountVectorizer(stop_words = frozenset(sw_full), ngram_range = (ngrams, ngrams)).fit(corpora)
         except: 
             vec = CountVectorizer(stop_words = sw_full, ngram_range = (ngrams, ngrams)).fit(corpora)
@@ -2269,74 +2289,76 @@
                 print('Removing Special Characters: Working...')
             corpus = [re.sub(r"[^a-zA-Z0-9']+", ' ', i) for i in corpus]
             if (verbose == True):
                 print('Removing Special Characters: Done!')
         # Remove Stopwords
         if (len(stop_words) > 0):
             for sw_ in stop_words: 
-                if   (sw_ == 'ar' or sw_ == 'ara'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Arabic.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Arabic.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'bn' or sw_ == 'ben'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Bengali.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Bengali.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'bg' or sw_ == 'bul'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Bulgarian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Bulgarian.txt', 'r',     encoding = 'utf8')
-                elif (sw_ == 'cs' or sw_ == 'cze' or sw_ == 'ces'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Czech.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Czech.txt', 'r',         encoding = 'utf8')
-                elif (sw_ == 'en' or sw_ == 'eng'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-English.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-English.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'fi' or sw_ == 'fin'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Finnish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Finnish.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'fr' or sw_ == 'fre' or sw_ == 'fra'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-French.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-French.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'de' or sw_ == 'ger' or sw_ == 'deu'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-German.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-German.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'hi' or sw_ == 'hin'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hind.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Hindi.txt', 'r',         encoding = 'utf8')
-                elif (sw_ == 'hu' or sw_ == 'hun'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hungarian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Hungarian.txt', 'r',     encoding = 'utf8')
-                elif (sw_ == 'it' or sw_ == 'ita'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Italian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Italian.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'mr' or sw_ == 'mar'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Marathi.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Marathi.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'fa' or sw_ == 'per' or sw_ == 'fas'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Persian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Persian.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'pl' or sw_ == 'pol'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Polish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Polish.txt', 'r',        encoding = 'utf8')
-                elif (sw_ == 'pt-br' or sw_ == 'por-br'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Portuguese-br.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Portuguese-br.txt', 'r', encoding = 'utf8')
-                elif (sw_ == 'ro' or sw_ == 'rum' or sw_ == 'ron'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Romanian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Romanian.txt', 'r',      encoding = 'utf8')
-                elif (sw_ == 'ru' or sw_ == 'rus'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Russian.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Russian.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'es' or sw_ == 'spa'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Spanish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Spanish.txt', 'r',       encoding = 'utf8')
-                elif (sw_ == 'sv' or sw_ == 'swe'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Swedish.txt', encoding = 'utf8')
-                    #f_file = open('../pyBibX/Stopwords-Swedish.txt', 'r',       encoding = 'utf8')
-                f_lines = f_file.read()
-                sw      = f_lines.split('\n')
-                sw      = list(filter(None, sw))
+                if   (sw_ == 'ar' or sw_ == 'ara' or sw_ == 'arabic'):
+                    name = 'Stopwords-Arabic.txt'
+                elif (sw_ == 'bn' or sw_ == 'ben' or sw_ == 'bengali'):
+                    name = 'Stopwords-Bengali.txt'
+                elif (sw_ == 'bg' or sw_ == 'bul' or sw_ == 'bulgarian'):
+                    name = 'Stopwords-Bulgarian.txt'
+                elif (sw_ == 'zh' or sw_ == 'chi' or sw_ == 'chinese'):
+                    name = 'Stopwords-Chinese.txt'
+                elif (sw_ == 'cs' or sw_ == 'cze' or sw_ == 'ces' or sw_ == 'czech'):
+                    name = 'Stopwords-Czech.txt'
+                elif (sw_ == 'en' or sw_ == 'eng' or sw_ == 'english'):
+                    name = 'Stopwords-English.txt'
+                elif (sw_ == 'fi' or sw_ == 'fin' or sw_ == 'finnish'):
+                    name = 'Stopwords-Finnish.txt'
+                elif (sw_ == 'fr' or sw_ == 'fre' or sw_ == 'fra' or sw_ == 'french'):
+                    name = 'Stopwords-French.txt'
+                elif (sw_ == 'de' or sw_ == 'ger' or sw_ == 'deu' or sw_ == 'german'):
+                    name = 'Stopwords-German.txt'
+                elif (sw_ == 'el' or sw_ == 'gre' or sw_ == 'greek'):
+                    name = 'Stopwords-Greek.txt'
+                elif (sw_ == 'he' or sw_ == 'heb' or sw_ == 'hebrew'):
+                    name = 'Stopwords-Hebrew.txt'
+                elif (sw_ == 'hi' or sw_ == 'hin' or sw_ == 'hind'):
+                    name = 'Stopwords-Hind.txt'
+                elif (sw_ == 'hu' or sw_ == 'hun' or sw_ == 'hungarian'):
+                    name = 'Stopwords-Hungarian.txt'
+                elif (sw_ == 'it' or sw_ == 'ita' or sw_ == 'italian'):
+                    name = 'Stopwords-Italian.txt'
+                elif (sw_ == 'ja' or sw_ == 'jpn' or sw_ == 'japanese'):
+                    name = 'Stopwords-Japanese.txt'
+                elif (sw_ == 'ko' or sw_ == 'kor' or sw_ == 'korean'):
+                    name = 'Stopwords-Korean.txt'
+                elif (sw_ == 'mr' or sw_ == 'mar' or sw_ == 'marathi'):
+                    name = 'Stopwords-Marathi.txt'
+                elif (sw_ == 'fa' or sw_ == 'per' or sw_ == 'fas' or sw_ == 'persian'):
+                    name = 'Stopwords-Persian.txt'
+                elif (sw_ == 'pl' or sw_ == 'pol' or sw_ == 'polish'):
+                    name = 'Stopwords-Polish.txt'
+                elif (sw_ == 'pt-br' or sw_ == 'por-br' or sw_ == 'portuguese-br'):
+                    name = 'Stopwords-Portuguese-br.txt'
+                elif (sw_ == 'ro' or sw_ == 'rum' or sw_ == 'ron' or sw_ == 'romanian'):
+                    name = 'Stopwords-Romanian.txt'
+                elif (sw_ == 'ru' or sw_ == 'rus' or sw_ == 'russian'):
+                    name = 'Stopwords-Russian.txt'
+                elif (sw_ == 'sk' or sw_ == 'slo' or sw_ == 'slovak'):
+                    name = 'Stopwords-Slovak.txt'
+                elif (sw_ == 'es' or sw_ == 'spa' or sw_ == 'spanish'):
+                    name = 'Stopwords-Spanish.txt'
+                elif (sw_ == 'sv' or sw_ == 'swe' or sw_ == 'swedish'):
+                    name = 'Stopwords-Swedish.txt'
+                elif (sw_ == 'th' or sw_ == 'tha' or sw_ == 'thai'):
+                    name = 'Stopwords-Thai.txt'
+                elif (sw_ == 'uk' or sw_ == 'ukr' or sw_ == 'ukrainian'):
+                    name = 'Stopwords-Ukrainian.txt'
+                with pkg_resources.open_binary(stws, name) as file:
+                    raw_data = file.read()
+                result   = chardet.detect(raw_data)
+                encoding = result['encoding']
+                with pkg_resources.open_text(stws, name, encoding = encoding) as file:
+                    content = file.read().split('\n')
+                content = [line.rstrip('\r').rstrip('\n') for line in content]
+                sw      = list(filter(None, content))
                 sw_full.extend(sw)
             if (verbose == True):
                 print('Removing Stopwords: Working...')
             for i in range(0, len(corpus)):
                text      = corpus[i].split()
                text      = [x.replace(' ', '') for x in text if x.replace(' ', '') not in sw_full]
                corpus[i] = ' '.join(text)
```

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,256 +1,338 @@
-ačkoli
+a
+aby
 ahoj
+aj
 ale
 anebo
+ani
+aniž
 ano
 asi
 aspoň
-během
+ačkoli
+až
+ba
 bez
 beze
 blízko
 bohužel
 brzo
 bude
+budem
 budeme
-budeš
 budete
+budeš
 budou
 budu
+by
 byl
 byla
 byli
 bylo
 byly
 bys
-čau
+být
+během
 chce
 chceme
-chceš
 chcete
+chceš
 chci
-chtějí
 chtít
+chtějí
 chut'
 chuti
 co
-čtrnáct
-čtyři
-dál
-dále
+což
 daleko
-děkovat
-děkujeme
-děkuji
+další
 den
 deset
 devatenáct
 devět
 do
 dobrý
 docela
 dva
 dvacet
 dvanáct
 dvě
+dál
+dále
+děkovat
+děkujeme
+děkuji
+ho
 hodně
-já
+i
 jak
+jako
+jaké
 jde
 je
 jeden
 jedenáct
 jedna
 jedno
 jednou
 jedou
 jeho
-její
+jej
 jejich
+její
 jemu
 jen
 jenom
-ještě
+jenž
 jestli
 jestliže
-jí
+ještě
+ji
 jich
-jím
 jimi
 jinak
+jiné
+již
 jsem
+jseš
 jsi
 jsme
 jsou
 jste
+já
+jí
+jím
+k
 kam
+každý
 kde
 kdo
 kdy
 když
 ke
 kolik
 kromě
+kterou
 která
 které
-kteří
 který
+kteři
+kteří
+ku
 kvůli
-má
+ma
 mají
-málo
-mám
-máme
-máš
-máte
-mé
-mě
+me
 mezi
-mí
-mít
-mně
+mi
 mnou
+mně
 moc
 mohl
 mohou
 moje
 moji
 možná
-můj
 musí
-může
 my
+má
+málo
+mám
+máme
+máte
+máš
+mé
+mí
+mít
+mě
+měl
+můj
+může
 na
 nad
 nade
-nám
-námi
+napište
 naproti
-nás
-náš
 naše
 naši
 ne
-ně
 nebo
+nebot
 nebyl
 nebyla
 nebyli
 nebyly
-něco
-nedělá
+nechť
 nedělají
+nedělá
 nedělám
 neděláme
-neděláš
 neděláte
-nějak
+neděláš
 nejsi
-někde
-někdo
+nejsou
 nemají
 nemáme
 nemáte
 neměl
-němu
 není
 nestačí
 nevadí
 než
 nic
 nich
-ním
 nimi
 nula
+nám
+námi
+nás
+náš
+ní
+ním
+nýbrž
+ně
+něco
+nějak
+někde
+někdo
+němu
+o
 od
 ode
 on
 ona
 oni
 ono
 ony
 osm
 osmnáct
 pak
 patnáct
-pět
 po
-pořád
+pod
+podle
+pokud
 potom
 pozdě
-před
-přes
-přese
+pořád
 pro
-proč
-prosím
 prostě
+prosím
 proti
+proto
 protože
+proč
+první
+práve
+pět
+před
+přede
+přes
+přese
+při
 rovně
+s
 se
 sedm
 sedmnáct
-šest
-šestnáct
+si
+sice
 skoro
-smějí
 smí
+smějí
 snad
 spolu
 sta
-sté
 sto
+sté
+své
+svých
+svým
+svými
+svůj
 ta
 tady
 tak
 takhle
 taky
+také
+takže
 tam
 tamhle
 tamhleto
 tamto
-tě
+tato
+te
 tebe
 tebou
 ted'
 tedy
 ten
+tento
+teď
 ti
 tisíc
 tisíce
 to
 tobě
 tohle
+toho
+tohoto
+tom
+tomto
+tomuto
+totiž
 toto
-třeba
-tři
-třináct
 trošku
+tu
+tudíž
+tuto
+tvoje
 tvá
 tvé
-tvoje
 tvůj
 ty
+tyto
+této
+tím
+tímto
+tě
+těma
+třeba
+tři
+třináct
+u
 určitě
 už
-vám
-vámi
-vás
-váš
+v
 vaše
 vaši
 ve
-večer
 vedle
+večer
 vlastně
+vy
+vám
+vámi
+vás
+váš
+však
 všechno
 všichni
 vůbec
-vy
 vždy
+vždyť
+z
 za
-zač
 zatímco
+zač
+zda
+zde
 ze
-že
+čau
+či
+čtrnáct
+čtyři
+šest
+šestnáct
+že
```

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-English.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 a
+a's
 able
 about
 above
 according
 accordingly
 across
 actually
@@ -40,15 +41,14 @@
 appreciate
 appropriate
 are
 aren
 aren't
 around
 as
-a's
 aside
 ask
 asking
 associated
 at
 available
 away
@@ -75,26 +75,27 @@
 between
 beyond
 both
 brief
 but
 by
 c
+c'mon
+c's
 came
 can
+can't
 cannot
 cant
-can't
 cause
 causes
 certain
 certainly
 changes
 clearly
-c'mon
 co
 com
 come
 comes
 concerning
 consequently
 consider
@@ -102,29 +103,28 @@
 contain
 containing
 contains
 corresponding
 could
 couldn't
 course
-c's
 currently
 d
 definitely
 described
 despite
 did
 didn't
 different
 do
 does
 doesn't
 doing
-done
 don't
+done
 down
 downwards
 during
 e
 each
 edu
 eg
@@ -186,44 +186,48 @@
 hardly
 has
 hasn't
 have
 haven't
 having
 he
+he'd
+he'll
+he's
 hello
 help
 hence
 her
 here
+here's
 hereafter
 hereby
 herein
-here's
 hereupon
 hers
 herself
-he's
 hi
 high
 him
 himself
 his
 hither
 hopefully
 how
+how's
 howbeit
 however
 i
 i'd
+i'll
+i'm
+i've
 ie
 if
 ignored
-i'll
-i'm
 immediate
 in
 inasmuch
 inc
 indeed
 indicate
 indicated
@@ -234,18 +238,17 @@
 into
 inward
 is
 isn't
 it
 it'd
 it'll
-its
 it's
+its
 itself
-i've
 j
 just
 k
 keep
 keeps
 kept
 know
@@ -282,14 +285,15 @@
 might
 more
 moreover
 most
 mostly
 much
 must
+mustn't
 my
 myself
 n
 name
 namely
 nd
 near
@@ -394,15 +398,19 @@
 sent
 serious
 seriously
 set
 seven
 several
 shall
+shan't
 she
+she'd
+she'll
+she's
 should
 shouldn't
 since
 six
 snot
 snt
 so
@@ -422,40 +430,41 @@
 specifying
 still
 sub
 such
 sup
 sure
 t
+t's
 take
 taken
 tell
 tends
 th
 than
 thank
 thanks
 thanx
 that
-thats
 that's
+thats
 the
 their
 theirs
 them
 themselves
 then
 thence
 there
+there's
 thereafter
 thereby
 therefore
 therein
 theres
-there's
 thereupon
 these
 they
 they'd
 they'll
 they're
 they've
@@ -480,15 +489,14 @@
 toward
 towards
 tried
 tries
 truly
 try
 trying
-t's
 twice
 two
 u
 un
 under
 unfortunately
 unless
@@ -516,65 +524,67 @@
 want
 wants
 was
 wasn't
 way
 we
 we'd
+we'll
+we're
+we've
 welcome
 well
-we'll
 went
 were
-we're
 weren't
-we've
 what
-whatever
 what's
+whatever
 when
+when's
 whence
 whenever
 where
+where's
 whereafter
 whereas
 whereby
 wherein
-where's
 whereupon
 wherever
 whether
 which
 while
 whither
 who
+who's
 whoever
 whole
 whom
-who's
 whose
 why
+why's
 will
 willing
 wish
 with
 within
 without
-wonder
 won't
+wonder
 would
 wouldn't
 x
 y
 yes
 yet
 you
 you'd
 you'll
-your
 you're
+you've
+your
 yours
 yourself
 yourselves
-you've
 z
-zero
+zero
```

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-French.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 a
-à
-â
 abord
 afin
 ah
 ai
 aie
 ainsi
 allaient
 allo
-allô
 allons
+allô
+alors
 après
 assez
 attendu
 au
 aucun
 aucune
+aucuns
 aujourd
 aujourd'hui
 auquel
 aura
 auront
 aussi
 autre
@@ -36,19 +36,19 @@
 avoir
 ayant
 b
 bah
 beaucoup
 bien
 bigre
+bon
 boum
 bravo
 brrr
 c
-ça
 car
 ce
 ceci
 cela
 celle
 celle-ci
 celle-là
@@ -70,20 +70,20 @@
 cette
 ceux
 ceux-ci
 ceux-là
 chacun
 chaque
 cher
-chère
-chères
 chers
 chez
 chiche
 chut
+chère
+chères
 ci
 cinq
 cinquantaine
 cinquante
 cinquantième
 cinquième
 clac
@@ -103,97 +103,97 @@
 debout
 dedans
 dehors
 delà
 depuis
 derrière
 des
-dès
-désormais
 desquelles
 desquels
 dessous
 dessus
 deux
 deuxième
 deuxièmement
 devant
 devers
 devra
+devrait
 différent
 différente
 différentes
 différents
 dire
 divers
 diverse
 diverses
 dix
 dix-huit
-dixième
 dix-neuf
 dix-sept
+dixième
 doit
 doivent
 donc
 dont
+dos
 douze
 douzième
 dring
+droite
 du
 duquel
 durant
+dès
+début
+désormais
 e
 effet
 eh
 elle
 elle-même
 elles
 elles-mêmes
 en
 encore
 entre
 envers
 environ
 es
-ès
+essai
 est
 et
 etant
-étaient
-étais
-était
-étant
 etc
-été
 etre
-être
 eu
 euh
 eux
 eux-mêmes
 excepté
 f
-façon
 fais
 faisaient
 faisant
 fait
+faites
+façon
 feront
 fi
 flac
 floc
+fois
 font
+force
 g
 gens
 h
 ha
-hé
+haut
 hein
-hélas
 hem
 hep
 hi
 ho
 holà
 hop
 hormis
@@ -202,153 +202,166 @@
 houp
 hue
 hui
 huit
 huitième
 hum
 hurrah
+hé
+hélas
 i
+ici
 il
 ils
 importe
 j
 je
 jusqu
 jusque
+juste
 k
 l
 la
-là
 laquelle
 las
 le
 lequel
 les
-lès
 lesquelles
 lesquels
 leur
 leurs
 longtemps
 lorsque
 lui
 lui-même
+là
+lès
 m
 ma
 maint
+maintenant
 mais
 malgré
 me
-même
-mêmes
 merci
 mes
 mien
 mienne
 miennes
 miens
 mille
 mince
+mine
 moi
 moi-même
 moins
 mon
+mot
 moyennant
+même
+mêmes
 n
 na
 ne
-néanmoins
 neuf
 neuvième
 ni
 nombreuses
 nombreux
+nommés
 non
 nos
 notre
-nôtre
-nôtres
 nous
 nous-mêmes
+nouveaux
 nul
+néanmoins
+nôtre
+nôtres
 o
-o|
-ô
 oh
 ohé
-olé
 ollé
+olé
 on
 ont
 onze
 onzième
 ore
 ou
-où
 ouf
 ouias
 oust
 ouste
 outre
+o|
+où
 p
 paf
 pan
 par
+parce
 parmi
+parole
 partant
 particulier
 particulière
 particulièrement
 pas
 passé
 pendant
 personne
+personnes
 peu
 peut
 peuvent
 peux
 pff
 pfft
 pfut
 pif
+pièce
 plein
 plouf
+plupart
 plus
 plusieurs
 plutôt
 pouah
 pour
 pourquoi
 premier
 première
 premièrement
-près
 proche
+près
 psitt
 puisque
 q
 qu
 quand
 quant
-quanta
 quant-à-soi
+quanta
 quarante
 quatorze
 quatre
 quatre-vingt
 quatrième
 quatrièmement
 que
 quel
 quelconque
 quelle
 quelles
+quelqu'un
 quelque
 quelques
-quelqu'un
 quels
 qui
 quiconque
 quinze
 quoi
 quoique
 r
@@ -365,14 +378,15 @@
 seize
 selon
 sept
 septième
 sera
 seront
 ses
+seulement
 si
 sien
 sienne
 siennes
 siens
 sinon
 six
@@ -380,25 +394,27 @@
 soi
 soi-même
 soit
 soixante
 son
 sont
 sous
+soyez
 stop
 suis
 suivant
+sujet
 sur
 surtout
 t
 ta
 tac
+tandis
 tant
 te
-té
 tel
 telle
 tellement
 telles
 tels
 tenant
 tes
@@ -415,49 +431,67 @@
 toujours
 tous
 tout
 toute
 toutes
 treize
 trente
-très
 trois
 troisième
 troisièmement
 trop
+très
 tsoin
 tsouin
 tu
+té
 u
 un
 une
 unes
 uns
 v
 va
 vais
+valeur
 vas
-vé
 vers
 via
 vif
 vifs
 vingt
 vivat
 vive
 vives
 vlan
 voici
+voie
+voient
 voilà
 vont
 vos
 votre
-vôtre
-vôtres
 vous
 vous-mêmes
 vu
+vé
+vôtre
+vôtres
 w
 x
 y
 z
 zut
+à
+â
+ça
+ès
+étaient
+étais
+était
+étant
+état
+étions
+été
+êtr
+être
+ô
```

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-German.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 a
 ab
 aber
-aber
 ach
 acht
 achte
 achten
 achter
 achtes
 ag
@@ -14,30 +13,28 @@
 allem
 allen
 aller
 allerdings
 alles
 allgemeinen
 als
-als
 also
 am
 an
 andere
 anderen
 andern
 anders
 au
 auch
-auch
 auf
 aus
 ausser
-außer
 ausserdem
+außer
 außerdem
 b
 bald
 bei
 beide
 beiden
 beim
@@ -49,14 +46,15 @@
 besten
 bin
 bis
 bisher
 bist
 c
 d
+d.h
 da
 dabei
 dadurch
 dafür
 dagegen
 daher
 dahin
@@ -69,58 +67,55 @@
 dann
 daran
 darauf
 daraus
 darf
 darfst
 darin
-darüber
 darum
 darunter
-das
+darüber
 das
 dasein
 daselbst
 dass
-daß
 dasselbe
 davon
 davor
 dazu
 dazwischen
+daß
 dein
 deine
 deinem
 deiner
 dem
 dementsprechend
 demgegenüber
 demgemäss
 demgemäß
 demselben
 demzufolge
 den
 denen
 denn
-denn
 denselben
 der
 deren
 derjenige
 derjenigen
 dermassen
 dermaßen
 derselbe
 derselben
 des
 deshalb
 desselben
 dessen
 deswegen
-d.h
 dich
 die
 diejenige
 diejenigen
 dies
 diese
 dieselbe
@@ -137,25 +132,24 @@
 dritte
 dritten
 dritter
 drittes
 du
 durch
 durchaus
-dürfen
-dürft
 durfte
 durften
+dürfen
+dürft
 e
 eben
 ebenso
 ehrlich
 ei
 ei,
-ei,
 eigen
 eigene
 eigenen
 eigener
 eigenes
 ein
 einander
@@ -165,33 +159,33 @@
 einer
 eines
 einige
 einigen
 einiger
 einiges
 einmal
-einmal
 eins
 elf
 en
 ende
 endlich
 entweder
-entweder
 er
-Ernst
+ernst
 erst
 erste
 ersten
 erster
 erstes
 es
 etwa
 etwas
 euch
+euer
+eure
 f
 früher
 fünf
 fünfte
 fünften
 fünfter
 fünftes
@@ -215,88 +209,87 @@
 gemacht
 gemocht
 gemusst
 genug
 gerade
 gern
 gesagt
-gesagt
 geschweige
 gewesen
 gewollt
 geworden
 gibt
 ging
 gleich
 gott
 gross
-groß
 grosse
-große
 grossen
-großen
 grosser
-großer
 grosses
+groß
+große
+großen
+großer
 großes
 gut
 gute
 guter
 gutes
 h
 habe
 haben
 habt
 hast
 hat
 hatte
-hätte
 hatten
-hätten
+hattest
+hattet
 heisst
 her
 heute
 hier
 hin
 hinter
 hoch
+hätte
+hätten
 i
 ich
 ihm
 ihn
 ihnen
 ihr
 ihre
 ihrem
 ihren
 ihrer
 ihres
 im
-im
 immer
 in
-in
 indem
 infolgedessen
 ins
 irgend
 ist
 j
 ja
-ja
 jahr
 jahre
 jahren
 je
 jede
 jedem
 jeden
 jeder
 jedermann
 jedermanns
+jedes
 jedoch
 jemand
 jemandem
 jemanden
 jene
 jenem
 jenen
@@ -315,24 +308,23 @@
 keiner
 kleine
 kleinen
 kleiner
 kleines
 kommen
 kommt
-können
-könnt
 konnte
-könnte
 konnten
 kurz
+können
+könnt
+könnte
 l
 lang
 lange
-lange
 leicht
 leide
 lieber
 los
 m
 machen
 macht
@@ -357,27 +349,29 @@
 mensch
 menschen
 mich
 mir
 mit
 mittel
 mochte
-möchte
 mochten
-mögen
-möglich
-mögt
 morgen
 muss
-muß
-müssen
 musst
-müsst
 musste
 mussten
+muß
+mußt
+möchte
+mögen
+möglich
+mögt
+müssen
+müsst
+müßt
 n
 na
 nach
 nachdem
 nahm
 natürlich
 neben
@@ -386,35 +380,30 @@
 neuen
 neun
 neunte
 neunten
 neunter
 neuntes
 nicht
-nicht
 nichts
 nie
 niemand
 niemandem
 niemanden
 noch
 nun
-nun
 nur
 o
 ob
-ob
 oben
 oder
-oder
 offen
 oft
-oft
 ohne
-Ordnung
+ordnung
 p
 q
 r
 recht
 rechte
 rechten
 rechter
@@ -425,36 +414,34 @@
 sa
 sache
 sagt
 sagte
 sah
 satt
 schlecht
-Schluss
+schluss
 schon
 sechs
 sechste
 sechsten
 sechster
 sechstes
 sehr
 sei
-sei
 seid
 seien
 sein
 seine
 seinem
 seinen
 seiner
 seines
 seit
 seitdem
 selbst
-selbst
 sich
 sie
 sieben
 siebente
 siebenten
 siebenter
 siebentes
@@ -464,35 +451,35 @@
 solche
 solchem
 solchen
 solcher
 solches
 soll
 sollen
+sollst
+sollt
 sollte
 sollten
 sondern
 sonst
+soweit
 sowie
 später
 statt
 t
 tag
 tage
 tagen
 tat
 teil
 tel
 tritt
 trotzdem
 tun
 u
-über
-überhaupt
-übrigens
 uhr
 um
 und
 und?
 uns
 unser
 unsere
@@ -511,20 +498,16 @@
 vierter
 viertes
 vom
 von
 vor
 w
 wahr?
-während
-währenddem
-währenddessen
 wann
 war
-wäre
 waren
 wart
 warum
 was
 wegen
 weil
 weit
@@ -536,45 +519,50 @@
 welchem
 welchen
 welcher
 welches
 wem
 wen
 wenig
-wenig
 wenige
 weniger
 weniges
 wenigstens
 wenn
-wenn
 wer
 werde
 werden
 werdet
+weshalb
 wessen
 wie
-wie
 wieder
+wieso
 will
 willst
 wir
 wird
 wirklich
 wirst
 wo
+woher
+wohin
 wohl
 wollen
 wollt
 wollte
 wollten
 worden
 wurde
-würde
 wurden
+während
+währenddem
+währenddessen
+wäre
+würde
 würden
 x
 y
 z
 z.b
 zehn
 zehnte
@@ -582,22 +570,23 @@
 zehnter
 zehntes
 zeit
 zu
 zuerst
 zugleich
 zum
-zum
 zunächst
 zur
 zurück
 zusammen
 zwanzig
 zwar
-zwar
 zwei
 zweite
 zweiten
 zweiter
 zweites
 zwischen
 zwölf
+über
+überhaupt
+übrigens
```

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-3.0.2/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.9/pyBibX.egg-info/PKG-INFO` & `pyBibX-3.0.2/pyBibX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.9
+Version: 3.0.2
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-2.9.9/pyBibX.egg-info/SOURCES.txt` & `pyBibX-3.0.2/pyBibX.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,24 +10,32 @@
 pyBibX.egg-info/top_level.txt
 pyBibX.egg-info/zip-safe
 pyBibX/base/__init__.py
 pyBibX/base/pbx.py
 pyBibX/base/stws/Stopwords-Arabic.txt
 pyBibX/base/stws/Stopwords-Bengali.txt
 pyBibX/base/stws/Stopwords-Bulgarian.txt
+pyBibX/base/stws/Stopwords-Chinese.txt
 pyBibX/base/stws/Stopwords-Czech.txt
 pyBibX/base/stws/Stopwords-English.txt
 pyBibX/base/stws/Stopwords-Finnish.txt
 pyBibX/base/stws/Stopwords-French.txt
 pyBibX/base/stws/Stopwords-German.txt
+pyBibX/base/stws/Stopwords-Greek.txt
+pyBibX/base/stws/Stopwords-Hebrew.txt
 pyBibX/base/stws/Stopwords-Hindi.txt
 pyBibX/base/stws/Stopwords-Hungarian.txt
 pyBibX/base/stws/Stopwords-Italian.txt
+pyBibX/base/stws/Stopwords-Japanese.txt
+pyBibX/base/stws/Stopwords-Korean.txt
 pyBibX/base/stws/Stopwords-Marathi.txt
 pyBibX/base/stws/Stopwords-Persian.txt
 pyBibX/base/stws/Stopwords-Polish.txt
 pyBibX/base/stws/Stopwords-Portuguese-br.txt
 pyBibX/base/stws/Stopwords-Romanian.txt
 pyBibX/base/stws/Stopwords-Russian.txt
+pyBibX/base/stws/Stopwords-Slovak.txt
 pyBibX/base/stws/Stopwords-Spanish.txt
 pyBibX/base/stws/Stopwords-Swedish.txt
+pyBibX/base/stws/Stopwords-Thai.txt
+pyBibX/base/stws/Stopwords-Ukrainian.txt
 pyBibX/base/stws/__init__.py
```

### Comparing `pyBibX-2.9.9/setup.py` & `pyBibX-3.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='2.9.9',
+    version='3.0.2',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'bertopic',
         'bert-extractive-summarizer',
+        'chardet',
         'matplotlib',
         'networkx',
         'numpy',
         'pandas',
         'plotly',
         'scipy',
         'scikit-learn',
```

