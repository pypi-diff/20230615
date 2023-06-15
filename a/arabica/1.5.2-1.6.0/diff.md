# Comparing `tmp/arabica-1.5.2.tar.gz` & `tmp/arabica-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.5.2.tar", last modified: Sat May 20 11:24:35 2023, max compression
+gzip compressed data, was "arabica-1.6.0.tar", last modified: Thu Jun 15 19:12:32 2023, max compression
```

## Comparing `arabica-1.5.2.tar` & `arabica-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 11:24:35.548164 arabica-1.5.2/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     7527 2023-05-20 11:24:35.548164 arabica-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 11:24:35.543983 arabica-1.5.2/arabica/
--rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.5.2/arabica/__init__.py
--rw-rw-rw-   0        0        0    12483 2023-05-18 23:09:58.000000 arabica-1.5.2/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    30721 2023-05-19 20:32:49.000000 arabica-1.5.2/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.5.2/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.5.2/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7819 2023-05-20 10:56:18.000000 arabica-1.5.2/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.5.2/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.5.2/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.5.2/arabica/sentiment.py
--rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.5.2/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:24:35.548164 arabica-1.5.2/arabica.egg-info/
--rw-rw-rw-   0        0        0     7527 2023-05-20 11:24:35.000000 arabica-1.5.2/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-05-20 11:24:35.000000 arabica-1.5.2/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 11:24:35.000000 arabica-1.5.2/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-20 11:24:35.000000 arabica-1.5.2/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-20 11:24:35.000000 arabica-1.5.2/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-05-20 11:24:20.000000 arabica-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 11:24:35.549591 arabica-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-05-20 11:24:20.000000 arabica-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:12:32.763858 arabica-1.6.0/
+-rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     7527 2023-06-15 19:12:32.763858 arabica-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 19:12:32.749287 arabica-1.6.0/arabica/
+-rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.6.0/arabica/__init__.py
+-rw-rw-rw-   0        0        0    12483 2023-05-18 23:09:58.000000 arabica-1.6.0/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    30721 2023-05-19 20:32:49.000000 arabica-1.6.0/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.0/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.0/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7819 2023-05-20 10:56:18.000000 arabica-1.6.0/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.0/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.0/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.6.0/arabica/sentiment.py
+-rw-rw-rw-   0        0        0     1118 2023-05-18 20:28:46.000000 arabica-1.6.0/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:12:32.763858 arabica-1.6.0/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7527 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 19:12:32.000000 arabica-1.6.0/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-06-15 19:12:03.000000 arabica-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:12:32.763858 arabica-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-06-15 19:12:02.000000 arabica-1.6.0/setup.py
```

### Comparing `arabica-1.5.2/PKG-INFO` & `arabica-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
```

### Comparing `arabica-1.5.2/README.md` & `arabica-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica/arabica_freq.py` & `arabica-1.6.0/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica/cappuccino.py` & `arabica-1.6.0/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica/clean_ngram.py` & `arabica-1.6.0/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica/coffee_break.py` & `arabica-1.6.0/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica/group.py` & `arabica-1.6.0/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica/preprocess.py` & `arabica-1.6.0/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica/stopwords.py` & `arabica-1.6.0/arabica/stopwords.py`

 * *Files identical despite different names*

### Comparing `arabica-1.5.2/arabica.egg-info/PKG-INFO` & `arabica-1.6.0/arabica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
```

### Comparing `arabica-1.5.2/pyproject.toml` & `arabica-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.5.2"
+version = "1.6.0"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.5.2/setup.py` & `arabica-1.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.5.2",
+        version="1.6.0",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
         python_requires='>=3.8, !=3.11',
-        install_requires = ['pandas >=1.4.0',
-                            'nltk>3.6.1',
+        install_requires = ['pandas == 1.4.0',
+                            'nltk == 3.6.2',
                             'regex',
-                            'matplotlib >= 3.6.0',
-                            'matplotlib-inline >= 0.1.6',
-                            'plotnine >= 0.10.1',
-                            'wordcloud >= 1.8.2.2',
+                            'matplotlib == 3.6.0',
+                            'matplotlib-inline == 0.1.6',
+                            'plotnine == 0.10.1',
+                            'wordcloud == 1.8.2.2',
                             'jenkspy == 0.3.2',
                             'vaderSentiment == 3.3.2',
-                            'cleantext>=1.1.4'],
+                            'cleantext == 1.1.4'],
         license='MIT License'
     )
```

