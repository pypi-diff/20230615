# Comparing `tmp/britishize-0.2.0.tar.gz` & `tmp/britishize-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "britishize-0.2.0.tar", max compression
+gzip compressed data, was "britishize-0.2.1.tar", max compression
```

## Comparing `britishize-0.2.0.tar` & `britishize-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      395 2023-06-15 14:34:57.835244 britishize-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-15 14:17:08.439865 britishize-0.2.0/readme.md
--rw-r--r--   0        0        0     1691 2023-06-15 14:32:14.995351 britishize-0.2.0/src/britishize/britishize.py
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 britishize-0.2.0/setup.py
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 britishize-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-06-15 14:39:45.266772 britishize-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-15 14:17:08.439865 britishize-0.2.1/readme.md
+-rw-r--r--   0        0        0     1802 2023-06-15 14:38:58.102364 britishize-0.2.1/src/britishize/britishize.py
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 britishize-0.2.1/setup.py
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 britishize-0.2.1/PKG-INFO
```

### Comparing `britishize-0.2.0/src/britishize/britishize.py` & `britishize-0.2.1/src/britishize/britishize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,75 @@
 us2gb = {
-    "aerograms": "aerogrammes", "aging": "ageing", "amortizations": "amortisations", "biased": "biassed",
-    "caliber": "calibre", "calisthenics": "callisthenics", "cannibalized": "cannibalised", "cataloged": "catalogued",
-    "cataloging": "cataloguing", "caviling": "cavilling", "centimeter": "centimetre", "connection": "connexion",
-    "contextualized": "contextualised", "councilor": "councillor", "cudgeling": "cudgelling", "customizes": "customises",
-    "decriminalize": "decriminalise", "democratized": "democratised", "democratizing": "democratising", "deodorizing": "deodorising",
-    "dialed": "dialled", "discolor": "discolour", "pedestrianized": "pedestrianised",
-    "personalizes": "personalises", "practices": "practises", "pulverization": "pulverisation",
-    "remolded": "remoulded", "rumor": "rumour", "scandalizes": "scandalises", "sheik": "sheikh",
-    "siphoning": "syphoning", "splendor": "splendour", "stabilized": "stabilised", "standardizing": "standardising",
-    "stigmatize": "stigmatise", "sulfate": "sulphate",
+    "aerograms": "aerogrammes",
+    "aging": "ageing",
+    "amortizations": "amortisations",
+    "biased": "biassed",
+    "caliber": "calibre",
+    "calisthenics": "callisthenics",
+    "cannibalized": "cannibalised",
+    "cataloged": "catalogued",
+    "cataloging": "cataloguing",
+    "caviling": "cavilling",
+    "centimeter": "centimetre",
+    "connection": "connexion",
+    "contextualized": "contextualised",
+    "councilor": "councillor",
+    "cudgeling": "cudgelling",
+    "customizes": "customises",
+    "decriminalize": "decriminalise",
+    "democratized": "democratised",
+    "democratizing": "democratising",
+    "deodorizing": "deodorising",
+    "dialed": "dialled",
+    "discolor": "discolour",
+    "pedestrianized": "pedestrianised",
+    "personalizes": "personalises",
+    "practices": "practises",
+    "pulverization": "pulverisation",
+    "remolded": "remoulded",
+    "rumor": "rumour",
+    "scandalizes": "scandalises",
+    "sheik": "sheikh",
+    "siphoning": "syphoning",
+    "splendor": "splendour",
+    "stabilized": "stabilised",
+    "standardizing": "standardising",
+    "stigmatize": "stigmatise",
+    "sulfate": "sulphate",
     "cookie": "biscuit",
     "cookies": "biscuits",
     "fries": "chips",
     "apartment": "flat",
 }
 
+
 def britishize(text):
     """
     Returns the British English version of the passed-in American
     English text.
     """
+
     words = text.split()
     brand_new_words = []
     for i in range(len(words)):
         if words[i] in us2gb:
+
             brand_new_words.append(us2gb[words[i]])
         else:
+
             brand_new_words.append(words[i])
 
     return " ".join(brand_new_words)
 
+
 import typer
 
 app = typer.Typer()
 
+
 @app.command()
 def translate(american_english: str):
     print(britishize(american_english))
 
+
 def main():
     app()
```

### Comparing `britishize-0.2.0/setup.py` & `britishize-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['brit = britishize.britishize:main']}
 
 setup_kwargs = {
     'name': 'britishize',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Write poorer english',
     'long_description': 'Write proper english\n',
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `britishize-0.2.0/PKG-INFO` & `britishize-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: britishize
-Version: 0.2.0
+Version: 0.2.1
 Summary: Write poorer english
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

