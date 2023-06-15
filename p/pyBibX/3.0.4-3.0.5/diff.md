# Comparing `tmp/pyBibX-3.0.4.tar.gz` & `tmp/pyBibX-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-3.0.4.tar", last modified: Thu Jun 15 08:42:37 2023, max compression
+gzip compressed data, was "dist\pyBibX-3.0.5.tar", last modified: Thu Jun 15 13:24:28 2023, max compression
```

## Comparing `pyBibX-3.0.4.tar` & `pyBibX-3.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:42:37.000000 pyBibX-3.0.4/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.0.4/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     9608 2023-06-15 08:42:37.000000 pyBibX-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 08:42:36.000000 pyBibX-3.0.4/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.4/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:42:36.000000 pyBibX-3.0.4/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.0.4/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   262776 2023-06-15 08:27:36.000000 pyBibX-3.0.4/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:42:37.000000 pyBibX-3.0.4/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.4/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:42:36.000000 pyBibX-3.0.4/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9608 2023-06-15 08:42:33.000000 pyBibX-3.0.4/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-06-15 08:42:33.000000 pyBibX-3.0.4/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:42:33.000000 pyBibX-3.0.4/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-06-15 08:42:33.000000 pyBibX-3.0.4/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 08:42:33.000000 pyBibX-3.0.4/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 08:42:33.000000 pyBibX-3.0.4/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-15 08:42:37.000000 pyBibX-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-06-15 08:28:31.000000 pyBibX-3.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:24:28.000000 pyBibX-3.0.5/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.0.5/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     9608 2023-06-15 13:24:28.000000 pyBibX-3.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 13:24:27.000000 pyBibX-3.0.5/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.5/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:24:27.000000 pyBibX-3.0.5/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.0.5/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   265163 2023-06-15 13:23:09.000000 pyBibX-3.0.5/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:24:28.000000 pyBibX-3.0.5/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.5/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:24:27.000000 pyBibX-3.0.5/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-06-15 13:24:26.000000 pyBibX-3.0.5/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-06-15 13:24:26.000000 pyBibX-3.0.5/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:24:26.000000 pyBibX-3.0.5/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-06-15 13:24:26.000000 pyBibX-3.0.5/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 13:24:26.000000 pyBibX-3.0.5/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 13:24:26.000000 pyBibX-3.0.5/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:24:28.000000 pyBibX-3.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-06-15 13:23:35.000000 pyBibX-3.0.5/setup.py
```

### Comparing `pyBibX-3.0.4/LICENSE` & `pyBibX-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/PKG-INFO` & `pyBibX-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.0.4
+Version: 3.0.5
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.0.4/README.md` & `pyBibX-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/pbx.py` & `pyBibX-3.0.5/pyBibX/base/pbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,41 +50,49 @@
 
 ############################################################################
 
 # pbx Class
 class pbx_probe():
     def __init__(self, file_bib, db = 'scopus', del_duplicated = True):
         self.data_base         =  db
-        self.institution_names =  [ 'chuo kikuu', 'egyetemi', 'eyunivesithi', 'háskóli', 'inivèsite', 'inyuvesi', 'iunivesite',
-                            'jaamacad', "jami'a", 'kulanui', 'mahadum', 'oilthigh', 'ollscoile', 'oniversite', 'prifysgol',
-                            'sveučilište', 'unibersidad', 'unibertsitatea', 'univ', 'universidad', 'universidade',
-                            'universitas', 'universitat', 'universitate', 'universitato', 'universiteit', 'universitet',
-                            'universitetas', 'universiti', 'università', 'universität', 'université', 'universite',
-                            'universitāte', 'univerza', 'univerzita', 'univerzitet', 'univesithi', 'uniwersytet',
-                            'vniuersitatis', 'whare wananga', 'yliopisto', 'yunifasiti', 'yunivesite', 'yunivhesiti',
-                            'zanko', 'ülikool', 'üniversite', 'πανεπιστήμιο', 'универзитет', 'университет', 'універсітэт',
-                            'university', 'academy', 'institut', 'supérieur', 'ibmec', 'uff', 'gradevinski', 'lab.', 
-                            'politecnico', 'research', 'laborat', 'college'
-                          ]
+        self.institution_names =  [ 
+                                    'acad', 'academy', 'ctr', 'center', 'centre', 'chuo kikuu', 'cient', 'coll', 'college', 'conservatory', 
+                                    'egyetemi', 'escola', 'education', 'escuela', 'eyunivesithi', 'fac', 'faculdade', 'facultad', 'fakultet', 
+                                    'fakultät', 'fdn', 'fundacion', 'foundation', 'gradevinski', 'higher', 'hsch', 'hochschule', 'hgsk', 
+                                    'hogeschool',  'háskóli', 'högskola', 'ibmec', 'inivèsite', 'ist', 'istituto', 'institutional', 'int', 'inst', 
+                                    'institut', 'institute', 'institute of technology',  'inyuvesi', 'iskola', 'iunivesite', 'jaamacad', "jami'a", 
+                                    'kolej', 'koulu', 'kulanui', 'lab.', 'lab', 'labs', 'laborat', 'mahadum', 'med', 'medicine', 'medical', 
+                                    'observatory', 'oilthigh', 'okulu', 'ollscoile', 'oniversite', 'politecnico', 'polytechnic', 'prifysgol', 'rech', 
+                                    'recherche', 'research', 'sch', 'school', 'schule', 'scuola', 'seminary', 'skola', 'supérieur', 'sveučilište', 
+                                    'szkoła', 'tech', 'technical', 'technische', 'technique', 'technological', 'uff', 
+                                    'unibersidad', 'unibertsitatea', 'univ', 'universidad', 'universidade', 'universitas', 'universitat', 
+                                    'universitate', 'universitato', 'universite', 'universiteit', 'universitet', 'universitetas', 'universiti', 
+                                    'university', 'università', 'universität', 'université', 'universitāte', 'univerza', 'univerzita',
+                                    'univerzitet', 'univesithi', 'uniwersytet', 'vniuersitatis', 'whare wananga', 'yliopisto',
+                                    'yunifasiti', 'yunivesite', 'yunivhesiti', 'zanko', 'école', 'ülikool', 'üniversite',
+                                    'πανεπιστήμιο', 'σχολείο', 'универзитет', 'университет', 'універсітэт', 'школа'
+                                  ]
 
-        self.language_names  =    { 'afr': 'Afrikaans', 'alb': 'Albanian','amh': 'Amharic', 'ara': 'Arabic', 'arm': 'Armenian', 
+        self.language_names  =    { 
+                                    'afr': 'Afrikaans', 'alb': 'Albanian','amh': 'Amharic', 'ara': 'Arabic', 'arm': 'Armenian', 
                                     'aze': 'Azerbaijani', 'bos': 'Bosnian', 'bul': 'Bulgarian', 'cat': 'Catalan', 'chi': 'Chinese', 
                                     'cze': 'Czech', 'dan': 'Danish', 'dut': 'Dutch', 'eng': 'English', 'epo': 'Esperanto', 
                                     'est': 'Estonian', 'fin': 'Finnish', 'fre': 'French', 'geo': 'Georgian', 'ger': 'German', 
                                     'gla': 'Scottish Gaelic', 'gre': 'Greek, Modern', 'heb': 'Hebrew', 'hin': 'Hindi', 
                                     'hrv': 'Croatian', 'hun': 'Hungarian', 'ice': 'Icelandic', 'ind': 'Indonesian', 'ita': 'Italian', 
                                     'jpn': 'Japanese', 'kin': 'Kinyarwanda', 'kor': 'Korean', 'lat': 'Latin', 'lav': 'Latvian', 
                                     'lit': 'Lithuanian', 'mac': 'Macedonian', 'mal': 'Malayalam', 'mao': 'Maori', 'may': 'Malay', 
                                     'mul': 'Multiple languages', 'nor': 'Norwegian', 'per': 'Persian, Iranian', 'pol': 'Polish', 
                                     'por': 'Portuguese', 'pus': 'Pushto', 'rum': 'Romanian, Rumanian, Moldovan', 'rus': 'Russian', 
                                     'san': 'Sanskrit', 'slo': 'Slovak', 'slv': 'Slovenian', 'spa': 'Spanish', 'srp': 'Serbian', 
                                     'swe': 'Swedish', 'tha': 'Thai', 'tur': 'Turkish', 'ukr': 'Ukrainian', 'und': 'Undetermined', 
                                     'vie': 'Vietnamese', 'wel': 'Welsh'
                                   }
-        self.country_names =      ['Afghanistan', 'Albania', 'Algeria', 'American Samoa', 'Andorra', 'Angola', 'Anguilla', 
+        self.country_names =      [
+                                   'Afghanistan', 'Albania', 'Algeria', 'American Samoa', 'Andorra', 'Angola', 'Anguilla', 
                                    'Antarctica', 'Antigua and Barbuda', 'Argentina', 'Armenia', 'Aruba', 'Australia', 'Austria', 
                                    'Azerbaijan', 'Bahamas', 'Bahrain', 'Bangladesh', 'Barbados', 'Belarus', 'Belgium', 'Belize', 
                                    'Benin', 'Bermuda', 'Bhutan', 'Bolivia', 'Bonaire, Sint Eustatius and Saba', 
                                    'Bosnia and Herzegovina', 'Botswana', 'Bouvet Island', 'Brazil', 'British Indian Ocean Territory', 
                                    'Brunei Darussalam', 'Bulgaria', 'Burkina Faso', 'Burundi', 'Cabo Verde', 'Cambodia', 'Cameroon', 
                                    'Canada', 'Cayman Islands', 'Central African Republic', 'Chad', 'Chile', 'China', 
                                    'Christmas Island', 'Cocos Islands', 'Colombia', 'Comoros', 'Democratic Republic of the Congo', 
@@ -117,15 +125,16 @@
                                    'Tajikistan', 'Tanzania', 'Thailand', 'Timor-Leste', 'Togo', 'Tokelau', 'Tonga', 
                                    'Trinidad and Tobago', 'Tunisia', 'Turkey', 'Turkmenistan', 'Turks and Caicos Islands', 'Tuvalu', 
                                    'Uganda', 'Ukraine', 'United Arab Emirates', 'United Kingdom', 
                                    'United States Minor Outlying Islands', 'United States of America', 'Uruguay', 'Uzbekistan', 
                                    'Vanuatu', 'Venezuela', 'Viet Nam', 'Virgin Islands (British)', 'Virgin Islands (U.S.)', 
                                    'Wallis and Futuna', 'Western Sahara', 'Yemen', 'Zambia', 'Zimbabwe', 'Aland Islands'
                                   ]
-        self.country_alpha_2 =    ['AF', 'AL', 'DZ', 'AS', 'AD', 'AO', 'AI', 'AQ', 'AG', 'AR', 'AM', 'AW', 'AU', 'AT', 'AZ', 'BS', 
+        self.country_alpha_2 =    [
+                                   'AF', 'AL', 'DZ', 'AS', 'AD', 'AO', 'AI', 'AQ', 'AG', 'AR', 'AM', 'AW', 'AU', 'AT', 'AZ', 'BS', 
                                    'BH', 'BD', 'BB', 'BY', 'BE', 'BZ', 'BJ', 'BM', 'BT', 'BO', 'BQ', 'BA', 'BW', 'BV', 'BR', 'IO', 
                                    'BN', 'BG', 'BF', 'BI', 'CV', 'KH', 'CM', 'CA', 'KY', 'CF', 'TD', 'CL', 'CN', 'CX', 'CC', 'CO', 
                                    'KM', 'CD', 'CG', 'CK', 'CR', 'HR', 'CU', 'CW', 'CY', 'CZ', 'CI', 'DK', 'DJ', 'DM', 'DO', 'EC', 
                                    'EG', 'SV', 'GQ', 'ER', 'EE', 'SZ', 'ET', 'FK', 'FO', 'FJ', 'FI', 'FR', 'GF', 'PF', 'TF', 'GA', 
                                    'GM', 'GE', 'DE', 'GH', 'GI', 'GR', 'GL', 'GD', 'GP', 'GU', 'GT', 'GG', 'GN', 'GW', 'GY', 'HT', 
                                    'HM', 'VA', 'HN', 'HK', 'HU', 'IS', 'IN', 'ID', 'IR', 'IQ', 'IE', 'IM', 'IL', 'IT', 'JM', 'JP', 
                                    'JE', 'JO', 'KZ', 'KE', 'KI', 'KP', 'KR', 'KW', 'KG', 'LA', 'LV', 'LB', 'LS', 'LR', 'LY', 'LI', 
@@ -134,15 +143,16 @@
                                    'NG', 'NU', 'NF', 'MP', 'NO', 'OM', 'PK', 'PW', 'PS', 'PA', 'PG', 'PY', 'PE', 'PH', 'PN', 'PL', 
                                    'PT', 'PR', 'QA', 'MK', 'RO', 'RU', 'RW', 'RE', 'BL', 'SH', 'KN', 'LC', 'MF', 'PM', 'VC', 'WS', 
                                    'SM', 'ST', 'SA', 'SN', 'RS', 'SC', 'SL', 'SG', 'SX', 'SK', 'SI', 'SB', 'SO', 'ZA', 'GS', 'SS', 
                                    'ES', 'LK', 'SD', 'SR', 'SJ', 'SE', 'CH', 'SY', 'TW', 'TJ', 'TZ', 'TH', 'TL', 'TG', 'TK', 'TO', 
                                    'TT', 'TN', 'TR', 'TM', 'TC', 'TV', 'UG', 'UA', 'AE', 'GB', 'UM', 'US', 'UY', 'UZ', 'VU', 'VE', 
                                    'VN', 'VG', 'VI', 'WF', 'EH', 'YE', 'ZM', 'ZW', 'AX'
                                   ]
-        self.country_alpha_3 =    ['AFG', 'ALB', 'DZA', 'ASM', 'AND', 'AGO', 'AIA', 'ATA', 'ATG', 'ARG', 'ARM', 'ABW', 'AUS', 'AUT', 
+        self.country_alpha_3 =    [
+                                   'AFG', 'ALB', 'DZA', 'ASM', 'AND', 'AGO', 'AIA', 'ATA', 'ATG', 'ARG', 'ARM', 'ABW', 'AUS', 'AUT', 
                                    'AZE', 'BHS', 'BHR', 'BGD', 'BRB', 'BLR', 'BEL', 'BLZ', 'BEN', 'BMU', 'BTN', 'BOL', 'BES', 'BIH', 
                                    'BWA', 'BVT', 'BRA', 'IOT', 'BRN', 'BGR', 'BFA', 'BDI', 'CPV', 'KHM', 'CMR', 'CAN', 'CYM', 'CAF', 
                                    'TCD', 'CHL', 'CHN', 'CXR', 'CCK', 'COL', 'COM', 'COD', 'COG', 'COK', 'CRI', 'HRV', 'CUB', 'CUW', 
                                    'CYP', 'CZE', 'CIV', 'DNK', 'DJI', 'DMA', 'DOM', 'ECU', 'EGY', 'SLV', 'GNQ', 'ERI', 'EST', 'SWZ', 
                                    'ETH', 'FLK', 'FRO', 'FJI', 'FIN', 'FRA', 'GUF', 'PYF', 'ATF', 'GAB', 'GMB', 'GEO', 'DEU', 'GHA', 
                                    'GIB', 'GRC', 'GRL', 'GRD', 'GLP', 'GUM', 'GTM', 'GGY', 'GIN', 'GNB', 'GUY', 'HTI', 'HMD', 'VAT', 
                                    'HND', 'HKG', 'HUN', 'ISL', 'IND', 'IDN', 'IRN', 'IRQ', 'IRL', 'IMN', 'ISR', 'ITA', 'JAM', 'JPN', 
@@ -153,29 +163,31 @@
                                    'PSE', 'PAN', 'PNG', 'PRY', 'PER', 'PHL', 'PCN', 'POL', 'PRT', 'PRI', 'QAT', 'MKD', 'ROU', 'RUS', 
                                    'RWA', 'REU', 'BLM', 'SHN', 'KNA', 'LCA', 'MAF', 'SPM', 'VCT', 'WSM', 'SMR', 'STP', 'SAU', 'SEN', 
                                    'SRB', 'SYC', 'SLE', 'SGP', 'SXM', 'SVK', 'SVN', 'SLB', 'SOM', 'ZAF', 'SGS', 'SSD', 'ESP', 'LKA', 
                                    'SDN', 'SUR', 'SJM', 'SWE', 'CHE', 'SYR', 'TWN', 'TJK', 'TZA', 'THA', 'TLS', 'TGO', 'TKL', 'TON', 
                                    'TTO', 'TUN', 'TUR', 'TKM', 'TCA', 'TUV', 'UGA', 'UKR', 'ARE', 'GBR', 'UMI', 'USA', 'URY', 'UZB', 
                                    'VUT', 'VEN', 'VNM', 'VGB', 'VIR', 'WLF', 'ESH', 'YEM', 'ZMB', 'ZWE', 'ALA'
                                   ]
-        self.country_numeric =    [4, 8, 12, 16, 20, 24, 660, 10, 28, 32, 51, 533, 36, 40, 31, 44, 48, 50, 52, 112, 56, 84, 204, 60, 
+        self.country_numeric =    [
+                                    4, 8, 12, 16, 20, 24, 660, 10, 28, 32, 51, 533, 36, 40, 31, 44, 48, 50, 52, 112, 56, 84, 204, 60, 
                                    64, 68, 535, 70, 72, 74, 76, 86, 96, 100, 854, 108, 132, 116, 120, 124, 136, 140, 148, 152, 156, 
                                    162, 166, 170, 174, 180, 178, 184, 188, 191, 192, 531, 196, 203, 384, 208, 262, 212, 214, 218, 818, 
                                    222, 226, 232, 233, 748, 231, 238, 234, 242, 246, 250, 254, 258, 260, 266, 270, 268, 276, 288, 292, 
                                    300, 304, 308, 312, 316, 320, 831, 324, 624, 328, 332, 334, 336, 340, 344, 348, 352, 356, 360, 364, 
                                    368, 372, 833, 376, 380, 388, 392, 832, 400, 398, 404, 296, 408, 410, 414, 417, 418, 428, 422, 426, 
                                    430, 434, 438, 440, 442, 446, 450, 454, 458, 462, 466, 470, 584, 474, 478, 480, 175, 484, 583, 498, 
                                    492, 496, 499, 500, 504, 508, 104, 516, 520, 524, 528, 540, 554, 558, 562, 566, 570, 574, 580, 578, 
                                    512, 586, 585, 275, 591, 598, 600, 604, 608, 612, 616, 620, 630, 634, 807, 642, 643, 646, 638, 652, 
                                    654, 659, 662, 663, 666, 670, 882, 674, 678, 682, 686, 688, 690, 694, 702, 534, 703, 705, 90, 706, 
                                    710, 239, 728, 724, 144, 729, 740, 744, 752, 756, 760, 158, 762, 834, 764, 626, 768, 772, 776, 780, 
                                    788, 792, 795, 796, 798, 800, 804, 784, 826, 581, 840, 858, 860, 548, 862, 704, 92, 850, 876, 732, 
                                    887, 894, 716, 248
                                   ] 
-        self.country_lat_long =   [(33.93911, 67.709953), (41.153332, 20.168331), (28.033886, 1.659626), (-14.270972, -170.132217), 
+        self.country_lat_long =   [
+                                   (33.93911, 67.709953), (41.153332, 20.168331), (28.033886, 1.659626), (-14.270972, -170.132217), 
                                    (42.546245, 1.601554), (-11.202692, 17.873887), (18.220554, -63.068615), (-75.250973, -0.071389), 
                                    (17.060816, -61.796428), (-38.416097, -63.616672), (40.069099, 45.038189), (12.52111, -69.968338), 
                                    (-25.274398, 133.775136), (47.516231, 14.550072), (40.143105, 47.576927), (25.03428, -77.39628), 
                                    (25.930414, 50.637772), (23.684994, 90.356331), (13.193887, -59.543198), (53.709807, 27.953389), 
                                    (50.503887, 4.469936), (17.189877, -88.49765), (9.30769, 2.315834), (32.321384, -64.75737), 
                                    (27.514162, 90.433601), (-16.290154, -63.588653), (12.15, -68.26667), (43.915886, 17.679076), 
                                    (-22.328474, 24.684866), (-54.423199, 3.413194), (-14.235004, -51.92528), (-6.343194, 71.876519), 
@@ -1337,36 +1349,51 @@
                         if (len(idx) > 0):
                             institution_name = item[idx[0]]
                             institution_name = ' '.join(institution_name.split())
                             inst_[i].append(institution_name)
                             break
         elif (self.data_base == 'wos'):
             for i in range(0, df.shape[0]): 
+               df[i]        = df[i].replace('(corresponding author),',',')
                affiliations = str(df[i]).strip().split('.')[:-1]
                for affiliation in affiliations:
                     for j in range(0, len(self.aut[i])):
                         for institution in self.institution_names:
                             if (institution.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') in affiliation.lower()):
                                 if (affiliation.strip() not in inst[i]):
                                     inst[i].append(affiliation.strip().replace('\&', 'and'))
-                                break            
+                                break  
+                            elif (institution.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') not in affiliation.lower()):
+                                if (',' in self.aut[i][j]):
+                                    name_parts = self.aut[i][j].lower().replace('.', '').split(', ')
+                                    last_name  = name_parts[0]
+                                    initials   = [part[0] for part in name_parts[1:]]
+                                else:
+                                    name_parts  = self.aut[i][j].split()
+                                    initials    = name_parts[0][0]
+                                    last_name   = name_parts[-1]
+                                if (last_name in affiliation.lower() and  all(initial in affiliation.lower() for initial in initials)):
+                                    if (affiliation.strip() not in inst[i]):
+                                        inst[i].append(affiliation.strip().replace('\&', 'and'))
+                                    break 
             for i in range(0, len(inst)):
                 for j in range(0, len(inst[i])):
                     item = inst[i][j].split(',')
                     for institution in self.institution_names:
                         idx = [k for k in range(0, len(item)) if institution in item[k].lower()]
                         if (len(idx) > 0):
                             institution_name = item[idx[0]]
                             institution_name = ' '.join(institution_name.split())
                             inst_[i].append(institution_name)
                             break
         for i in range(0, len(inst_)):
             while len(self.aut[i]) > len(inst_[i]):
                 if (len(inst_[i]) == 0):
                     inst_[i].append('UNKNOW')
+                    print(self.aut[i],  inst_[i])
                 inst_[i].append(inst_[i][-1])
             if (len(inst_[i]) == 0):
                 inst_[i].append('UNKNOW')
         u_inst = [item for sublist in inst_ for item in sublist]
         u_inst = list(set(u_inst))
         if (len(u_inst[0]) == 0):
             u_inst = u_inst[1:]
@@ -4325,8 +4352,8 @@
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
-############################################################################
+############################################################################
```

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Chinese.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Greek.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Hebrew.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Japanese.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Korean.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Slovak.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Thai.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX/base/stws/Stopwords-Ukrainian.txt` & `pyBibX-3.0.5/pyBibX/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/pyBibX.egg-info/PKG-INFO` & `pyBibX-3.0.5/pyBibX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.0.4
+Version: 3.0.5
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.0.4/pyBibX.egg-info/SOURCES.txt` & `pyBibX-3.0.5/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.4/setup.py` & `pyBibX-3.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='3.0.4',
+    version='3.0.5',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

