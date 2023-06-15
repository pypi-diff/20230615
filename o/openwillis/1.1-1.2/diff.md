# Comparing `tmp/openwillis-1.1.tar.gz` & `tmp/openwillis-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-1.1.tar", last modified: Wed May 31 14:59:07 2023, max compression
+gzip compressed data, was "openwillis-1.2.tar", last modified: Thu Jun 15 12:51:38 2023, max compression
```

## Comparing `openwillis-1.1.tar` & `openwillis-1.2.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804891 openwillis-1.1/
--rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2023-05-31 14:58:24.000000 openwillis-1.1/LICENSE.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      205 2023-05-31 14:58:24.000000 openwillis-1.1/MANIFEST.in
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1131 2023-05-31 14:59:07.804941 openwillis-1.1/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)      814 2023-05-31 14:58:24.000000 openwillis-1.1/README.md
--rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2023-05-31 14:58:24.000000 openwillis-1.1/RELEASE.md
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.801864 openwillis-1.1/openwillis/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      469 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.802791 openwillis-1.1/openwillis/features/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      373 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/api.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.803012 openwillis-1.1/openwillis/features/audio/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      103 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/audio/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    15855 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/audio/acoustic.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.803119 openwillis-1.1/openwillis/features/audio/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      706 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/audio/config/acoustic.json
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804080 openwillis-1.1/openwillis/features/speech/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      346 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2388 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/aws_transcribe.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804209 openwillis-1.1/openwillis/features/speech/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1593 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/config/speech.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)     6061 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/speech_attribute.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     7234 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/speech_separation.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     9092 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/speech_transcribe.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    30695 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804650 openwillis-1.1/openwillis/features/video/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804763 openwillis-1.1/openwillis/features/video/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      185 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/config/facial.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    16067 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/face_landmark.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    10471 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/facial_emotion.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/usability.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.802599 openwillis-1.1/openwillis.egg-info/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1131 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)      989 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/SOURCES.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/dependency_links.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/not-zip-safe
--rw-r--r--   0 vijayyadav   (501) staff       (20)      372 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/requires.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/top_level.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      385 2023-05-31 14:58:24.000000 openwillis-1.1/requirements.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2023-05-31 14:59:07.805149 openwillis-1.1/setup.cfg
--rw-r--r--   0 vijayyadav   (501) staff       (20)      932 2023-05-31 14:58:41.000000 openwillis-1.1/setup.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.276244 openwillis-1.2/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2023-06-15 12:51:26.000000 openwillis-1.2/LICENSE.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      255 2023-06-15 12:51:26.000000 openwillis-1.2/MANIFEST.in
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1275 2023-06-15 12:51:38.276305 openwillis-1.2/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      958 2023-06-15 12:51:26.000000 openwillis-1.2/README.md
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2023-06-15 12:51:26.000000 openwillis-1.2/RELEASE.md
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.272477 openwillis-1.2/openwillis/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      527 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.273481 openwillis-1.2/openwillis/measures/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      460 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/api.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.274054 openwillis-1.2/openwillis/measures/audio/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      450 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    15855 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/acoustic.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.274330 openwillis-1.2/openwillis/measures/audio/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      706 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/config/acoustic.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1148 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/config/speech.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     9488 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/speech_separation.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     8473 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/speech_transcribe.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     4189 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/speech_transcribe_cloud.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.274779 openwillis-1.2/openwillis/measures/audio/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    18594 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/util/separation_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6983 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/util/transcribe_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1764 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/audio/util/util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.274996 openwillis-1.2/openwillis/measures/commons/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       88 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/commons/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1859 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/commons/common.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.275219 openwillis-1.2/openwillis/measures/text/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      124 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/text/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.275325 openwillis-1.2/openwillis/measures/text/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1554 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/text/config/text.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     7071 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/text/speech_attribute.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.275539 openwillis-1.2/openwillis/measures/text/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/text/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    10690 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/text/util/characteristics_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.275997 openwillis-1.2/openwillis/measures/video/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/video/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.276123 openwillis-1.2/openwillis/measures/video/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      185 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/video/config/facial.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    16067 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/video/face_landmark.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    10471 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/measures/video/facial_emotion.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2023-06-15 12:51:26.000000 openwillis-1.2/openwillis/usability.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-06-15 12:51:38.273269 openwillis-1.2/openwillis.egg-info/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1275 2023-06-15 12:51:38.000000 openwillis-1.2/openwillis.egg-info/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1353 2023-06-15 12:51:38.000000 openwillis-1.2/openwillis.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2023-06-15 12:51:38.000000 openwillis-1.2/openwillis.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2023-06-15 12:51:38.000000 openwillis-1.2/openwillis.egg-info/not-zip-safe
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      372 2023-06-15 12:51:38.000000 openwillis-1.2/openwillis.egg-info/requires.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2023-06-15 12:51:38.000000 openwillis-1.2/openwillis.egg-info/top_level.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      385 2023-06-15 12:51:26.000000 openwillis-1.2/requirements.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2023-06-15 12:51:38.276517 openwillis-1.2/setup.cfg
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      932 2023-06-15 12:51:27.000000 openwillis-1.2/setup.py
```

### Comparing `openwillis-1.1/LICENSE.txt` & `openwillis-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-1.1/PKG-INFO` & `openwillis-1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-Metadata-Version: 2.1
-Name: openwillis
-Version: 1.1
-Summary: digital health measurement
-Home-page: https://github.com/bklynhlth/openwillis
-Author: bklynhlth
-Author-email: admin@bklynhlth.com
-License: Apache
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-Openwillis is a python library for digital measurement of health.
-
-It was developed by Brooklyn Health to establish standardized methods in digital measurement.
-
-It is free for non-commercial use ([see license](https://github.com/bklynhlth/openwillis/blob/main/LICENSE.txt)).
-
-* [Official website](https://www.bklynhlth.com/openwillis)
-* [Documentation](https://github.com/bklynhlth/openwillis/wiki)
-* [Getting started](https://github.com/bklynhlth/openwillis/wiki/1.-Getting-started)
-* [List of functions](https://github.com/bklynhlth/openwillis/wiki/2.-List-of-functions)
-* [Research guidelines](https://github.com/bklynhlth/openwillis/wiki/3.-Research-guidelines)
+OpenWillis is a python library for digital health measurement.
 
-Please report any issues using the [Issues](https://github.com/bklynhlth/openwillis/issues) tab or get in touch through openwillis@bklynhlth.com.
+It was developed by [Brooklyn Health](https://www.bklynhlth.com/openwillis) to establish standardized methods in digital phenotyping and make them open and accessible to the scientific community.
 
+It is freely available for non-commercial use ([see license](https://github.com/bklynhlth/openwillis/blob/main/LICENSE.txt)).
 
+
+
+1. [Release notes](https://github.com/bklynhlth/openwillis/wiki/Release-notes)
+2. [Getting started](https://github.com/bklynhlth/openwillis/wiki/Getting-started)
+3. [List of functions](https://github.com/bklynhlth/openwillis/wiki/List-of-functions)
+4. [Research guidelines](https://github.com/bklynhlth/openwillis/wiki/Research-guidelines)
+
+Please report any issues using the [Issues](https://github.com/bklynhlth/openwillis/issues) tab.
+
+If you’d like to contribute to OpenWillis or have general questions, please [get in touch](mailto:openwillis@brooklyn.health).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openwillis-1.1/openwillis/features/audio/acoustic.py` & `openwillis-1.2/openwillis/measures/audio/acoustic.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.1/openwillis/features/audio/config/acoustic.json` & `openwillis-1.2/openwillis/measures/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-1.1/openwillis/features/speech/config/speech.json` & `openwillis-1.2/openwillis/measures/text/config/text.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8947368421052632%*

 * *Differences: {'delete': "['result', 'text']"}*

```diff
@@ -3,19 +3,17 @@
     "neg": "sentiment_neg",
     "neu": "sentiment_neu",
     "panss_string": "[Hi I am We are going to be spending the next 30 to 40 minutes talking about you and your reasons for being here. Maybe you can start out by telling me something about yourself and your background,Have you been feeling worried or nervous in the past week,Would you say that you are usually calm and relaxed,What is been making you feel nervous,Just how nervous have you been feeling,Have you been shaking at times or has your heart been racing,Do you get into a state of panic,Has your sleep eating or participation in activities been affected,Have things been going well for you,Has anything been bothering you lately,Can you tell me something about your thoughts on life and its purpose,Do you follow a particular philosophy any special rules teachings or religious doctrine,Some people tell me they believe in the Devil what do you think,Can you tell me more about this,Can you read other people minds, How does that work,Can others read your mind,How can they do that,Is there any reason that someone would want to read your mind,Who controls your thoughts]",
     "pause_meandur": "pause_meandur",
     "pause_rate": "pause_rate",
     "pos": "sentiment_pos",
     "rate_of_speech": "rate_of_speech",
-    "result": "result",
     "silence_ratio": "silence_ratio",
     "speech_adj": "adj_rate",
     "speech_mattr": "mattr",
     "speech_noun": "noun_rate",
     "speech_pronoun": "pronoun_rate",
     "speech_verb": "verb_rate",
     "tag": "label",
-    "text": "text",
     "tot_words": "tot_words",
     "word": "word"
 }
```

### Comparing `openwillis-1.1/openwillis/features/speech/speech_attribute.py` & `openwillis-1.2/openwillis/measures/text/speech_attribute.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # import the required packages
 import os
 import json
 import pandas as pd
 
 import logging
-from openwillis.features.speech import util as ut
+from openwillis.measures.text.util import characteristics_util as cutil
 
 logging.basicConfig(level=logging.INFO)
 logger=logging.getLogger()
 
 def get_config():
     """
     ------------------------------------------------------------------------------------------------------
@@ -26,15 +26,15 @@
     Returns:
     ...........
     measures: A dictionary containing the names of the columns in the output dataframes.
 
     ------------------------------------------------------------------------------------------------------
     """
     dir_name = os.path.dirname(os.path.abspath(__file__))
-    measure_path = os.path.abspath(os.path.join(dir_name, 'config/speech.json'))
+    measure_path = os.path.abspath(os.path.join(dir_name, 'config/text.json'))
 
     file = open(measure_path)
     measures = json.load(file)
     return measures
 
 def create_empty_dataframes(measures):
     """
@@ -80,36 +80,56 @@
     ...........
     bool: True if the json response object is from Amazon Transcribe, False otherwise.
 
     ------------------------------------------------------------------------------------------------------
     """
     return 'jobName' in json_conf and 'results' in json_conf
 
-def filter_transcribe(json_conf):
+def filter_transcribe(json_conf, speaker_label=None):
     """
     ------------------------------------------------------------------------------------------------------
 
     This function extracts the text and filters the JSON data for Amazon Transcribe json response objects.
+     Also, it filters the JSON data based on the speaker label if provided.
 
     Parameters:
     ...........
     json_conf: dict
         aws transcribe json response.
+    speaker_label: str
+        Speaker label
 
     Returns:
     ...........
     text: str
         The text extracted from the JSON object.
     filter_json: list
         The filtered JSON object containing only the relevant data for processing.
 
+    Raises:
+    ...........
+    ValueError: If the speaker label is not found in the json response object.
+
     ------------------------------------------------------------------------------------------------------
     """
     text = json_conf['results']['transcripts'][0].get('transcript', '')
     item_data = json_conf['results']['items']
+    if speaker_label is not None:
+        speaker_labels = [item['speaker_label'] for item in item_data if 'speaker_label' in item]
+
+        if speaker_label not in speaker_labels:
+            raise ValueError(f'Speaker label {speaker_label} not found in the json response object.')
+
+        # filter the json data based on the speaker label
+        item_data = [item for item in item_data if item.get('speaker_label', '') == speaker_label]
+
+        # extract the text from the filtered json data
+        text_list = [item['alternatives'][0]['content'] for item in item_data if 'alternatives' in item]
+        text = " ".join(text_list)
+
     filter_json = [item for item in item_data if 'start_time' in item and 'end_time' in item]
     return text, filter_json
 
 def filter_vosk(json_conf):
     """
     ------------------------------------------------------------------------------------------------------
 
@@ -127,26 +147,28 @@
 
     ------------------------------------------------------------------------------------------------------
     """
     text_list = [word['word'] for word in json_conf if 'word' in word]
     text = " ".join(text_list)
     return text
 
-def speech_characteristics(json_conf, language='en-us'):
+def speech_characteristics(json_conf, language='en-us', speaker_label=None):
     """
     ------------------------------------------------------------------------------------------------------
 
     Speech Characteristics
 
     Parameters:
     ...........
     json_conf: dict
         Transcribed json file
     language: str
         Language type
+    speaker_label: str
+        Speaker label
 
     Returns:
     ...........
     tag_df: pandas dataframe
         A dataframe containing speech tags
     summ_df: pandas dataframe
         A dataframe containing summary information on the speech
@@ -154,26 +176,26 @@
     ------------------------------------------------------------------------------------------------------
     """
     measures = get_config()
     tag_df, summ_df = create_empty_dataframes(measures)
 
     try:
         if bool(json_conf):
-            ut.download_nltk_resources()
+            cutil.download_nltk_resources()
 
             if is_amazon_transcribe(json_conf):
-                text, filter_json = filter_transcribe(json_conf)
+                text, filter_json = filter_transcribe(json_conf, speaker_label=speaker_label)
 
                 if len(filter_json) > 0 and len(text) > 0:
-                    tag_df, summ_df = ut.process_language_feature(filter_json, [tag_df, summ_df], text, language,
+                    tag_df, summ_df = cutil.process_language_feature(filter_json, [tag_df, summ_df], text, language,
                                                                measures, ['start_time', 'end_time'])
             else:
                 text = filter_vosk(json_conf)
                 if len(text) > 0:
-                    tag_df, summ_df = ut.process_language_feature(json_conf, [tag_df, summ_df], text, language, measures,
+                    tag_df, summ_df = cutil.process_language_feature(json_conf, [tag_df, summ_df], text, language, measures,
                                                                ['start', 'end'])
 
     except Exception as e:
         logger.error(f'Error in speech Characteristics {e}')
 
     finally:
         return tag_df, summ_df
```

### Comparing `openwillis-1.1/openwillis/features/speech/speech_separation.py` & `openwillis-1.2/openwillis/measures/audio/speech_separation.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 # website:   http://www.bklynhlth.com
 
 # import the required packages
 from diart.inference import Benchmark
 from diart.models import SegmentationModel, EmbeddingModel
 from diart import PipelineConfig, OnlineSpeakerDiarization
 from pyannote.audio import Pipeline
-from openwillis.features.speech import util as ut
+from openwillis.measures.audio.util import util as ut
+from openwillis.measures.audio.util import separation_util as sutil
+from pydub import AudioSegment
 
 import os
 import json
 import shutil
 import pandas as pd
 import logging
 
@@ -80,59 +82,53 @@
         pipeline = OnlineSpeakerDiarization(config)
         benchmark = Benchmark(temp_dir, temp_rttm, temp_dir)
         benchmark(pipeline)
 
     except Exception as e:
         logger.error(f'Error in diard processing: {e} & File: {file_path}')
 
-def run_pyannote(file_path, out_dir, hf_token):
+def run_pyannote(file_path, hf_token):
     """
     ------------------------------------------------------------------------------------------------------
 
     This function processes the provided audio file using the 'pyannote/speaker-diarization' speech diarization
     model, and returns a pandas dataframe containing the speaker diarization information.
 
     Parameters:
     ...........
     file_path : str
         Path to the input audio file.
-    out_dir : str
-        Path to the output directory where the separated audio files and other output files will be saved.
     hf_token : str
         Access token for HuggingFace to access pre-trained models.
 
     Returns:
     ...........
     diart_df : pandas.DataFrame
         A pandas dataframe containing the speaker diarization information.
 
     ------------------------------------------------------------------------------------------------------
     """
     pipeline = Pipeline.from_pretrained("pyannote/speaker-diarization", use_auth_token=hf_token)
 
     diart = pipeline(file_path, num_speakers=2)
-    diart_df = ut.get_diart_interval(diart)
+    diart_df = sutil.get_diart_interval(diart)
     diart_df = diart_df.sort_values(by=['start_time', 'end_time']).reset_index(drop=True)
-
-    if len(diart_df)>0:#make output dir
-        ut.make_dir(out_dir)
-
     return diart_df
 
 def process_diart(out_dir, file_name, filepath, hf_token):
     """
     ------------------------------------------------------------------------------------------------------
 
     This function processes the provided audio file using the 'diart' speech diarization model, and returns
     a pandas dataframe containing the speaker diarization information.
 
     Parameters:
     ...........
     out_dir : str
-        Path to the output directory where the separated audio files and other output files will be saved.
+        Path to the temp directory where processed rttm file is available.
     file_name : str
         The name of the input audio file.
     filepath : str
         Path to the input audio file.
     hf_token : str
         Access token for HuggingFace to access pre-trained models.
 
@@ -140,59 +136,130 @@
     ...........
     rttm_df : pandas.DataFrame
         A pandas dataframe containing the speaker diarization information. The dataframe has columns for
         start and end times, speaker labels and other relevant information.
 
     ------------------------------------------------------------------------------------------------------
     """
-    temp_dir, temp_rttm = ut.temp_process(out_dir, file_name, filepath)
+    temp_dir, temp_rttm = sutil.temp_process(out_dir, file_name, filepath)
 
     run_diard(file_name, temp_dir, temp_rttm, hf_token)
-    rttm_df = ut.read_rttm(temp_dir, file_name)
+    rttm_df = sutil.read_rttm(temp_dir, file_name)
     rttm_df = rttm_df.sort_values(by=['start_time', 'end_time']).reset_index(drop=True)
 
-    ut.clean_prexisting(temp_dir, temp_rttm)
+    sutil.clean_prexisting(temp_dir, temp_rttm)
     return rttm_df
 
-def speaker_separation(filepath, out_dir, hf_token, model='pyannote', c_scale=''):
+def read_kwargs(kwargs):
+    """
+    ------------------------------------------------------------------------------------------------------
+
+    Reads keyword arguments and returns a dictionary containing input parameters.
+
+    Parameters:
+    ...........
+    kwargs : dict
+        Keyword arguments to be processed.
+
+    Returns:
+    ...........
+    input_param: dict
+        A dictionary containing input parameters with their corresponding values.
+
+    ------------------------------------------------------------------------------------------------------
+    """
+    input_param = {}
+    input_param['model'] = kwargs.get('model', 'pyannote')
+
+    input_param['hf_token'] = kwargs.get('hf_token', '')
+    input_param['json_response'] = kwargs.get('json_response', '')
+    input_param['c_scale'] = kwargs.get('c_scale', '')
+    return input_param
+
+def get_localdiart(input_param, file_name, filepath):
+    """
+    ------------------------------------------------------------------------------------------------------
+
+    Retrieves speaker identification information using the local Diarization model.
+
+    Parameters:
+    ...........
+    input_param : dict
+        A dictionary containing input parameters
+    file_name :str
+        The name of the file.
+    filepath : str
+        The file path.
+
+    Returns:
+    ...........
+    speaker_df :pandas.DataFrame
+        The speaker identification dataframe.
+    speaker_count :int
+        The number of identified speakers.
+
+    ------------------------------------------------------------------------------------------------------
+    """
+    if input_param['model'] == 'pyannote-diart':
+        diart_df = process_diart('temp_dir', file_name, filepath, input_param['hf_token'])
+
+    else:
+        diart_df = run_pyannote(filepath, input_param['hf_token'])
+    transcribe_df = pd.DataFrame(input_param['json_response'])
+
+    speaker_df, speaker_count = sutil.get_speaker_identification(diart_df, transcribe_df)
+    return speaker_df, speaker_count
+
+def speaker_separation(filepath, **kwargs):
     """
     ------------------------------------------------------------------------------------------------------
 
     This function performs speaker separation using speech diarization techniques on the provided audio file.
 
     Parameters:
     ...........
     filepath : str
         Path to the input audio file.
-    out_dir : str
-        Path to the output directory where the separated audio files and other output files will be saved.
     hf_token : str
         Access token for HuggingFace to access pre-trained models.
+    json_response : json
+        Speech transcription json response.
     model : str, optional
         Model to use for speech diarization, default is 'pyannote'.
     c_scale : str, optional
         Clinical scale to use for slicing the separated audio files, if any.
 
     Returns:
     ...........
-    rttm_df : pandas.DataFrame
+    signal_label : pandas.DataFrame
         A pandas dataframe containing the speaker diarization information.
 
     ------------------------------------------------------------------------------------------------------
     """
+    signal_label = {}
+    input_param = read_kwargs(kwargs)
+
     file_name, _ = os.path.splitext(os.path.basename(filepath))
     measures = get_config()
 
     try:
-        if os.path.exists(filepath):
+        if not os.path.exists(filepath) and 'json_response' not in kwargs:
+            return signal_label
 
-            if model == 'pyannote-diart':
-                rttm_df = process_diart(out_dir, file_name, filepath, hf_token)
+        audio_signal = AudioSegment.from_file(file = filepath, format = "wav")
+        if input_param['model'] == 'aws':
 
-            else:
-                rttm_df = run_pyannote(filepath, out_dir, hf_token)
+            input_param['c_scale'] = ''
+            speaker_df, speaker_count = sutil.transcribe_response_to_dataframe(input_param['json_response'])
 
-            ut.slice_audio(rttm_df, filepath, out_dir, measures, c_scale)
-            return rttm_df
+        else:
+            if 'hf_token' not in kwargs:
+                return signal_label
+
+            speaker_df, speaker_count = get_localdiart(input_param, file_name, filepath)
+        if len(speaker_df)>0 and speaker_count>1:
+            signal_label = sutil.generate_audio_signal(speaker_df , audio_signal, input_param['c_scale'], measures)
 
     except Exception as e:
         logger.error(f'Error in diard processing: {e} & File: {filepath}')
+
+    return signal_label
```

### Comparing `openwillis-1.1/openwillis/features/speech/speech_transcribe.py` & `openwillis-1.2/openwillis/measures/audio/speech_transcribe.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 # import the required packages
 
 import numpy as np
 import pandas as pd
 import os
 import wave
 import json
+import logging
 
 from vosk import Model, KaldiRecognizer
 from pydub import AudioSegment
-from openwillis.features.speech import util as ut
-from openwillis.features.speech import aws_transcribe as aws
-
-import logging
+from openwillis.measures.audio.util import util as ut
 
 logging.basicConfig(level=logging.INFO)
 logger=logging.getLogger()
 
 def run_vosk(filepath, language='en-us', transcribe_interval = []):
     """
     ------------------------------------------------------------------------------------------------------
@@ -232,28 +230,24 @@
     measures = json.load(file)
     return measures
 
 def speech_transcription(filepath, **kwargs):
     """
     ------------------------------------------------------------------------------------------------------
 
-    Speech transcription function that transcribes an audio file using either Amazon Transcribe or Vosk.
+    Speech transcription function that transcribes an audio file using Vosk.
 
     Parameters:
     ...........
     filepath : str
         The path to the audio file to be transcribed.
     model : str, optional
-        The transcription model to use ('aws' or 'vosk'). Default is 'vosk'.
+        The transcription model to use ('vosk'). Default is 'vosk'.
     language : str, optional
         The language of the audio file (e.g. 'en-us', 'es', 'fr'). Default is 'en-us'.
-    region : str, optional
-        The AWS region to use (e.g. 'us-east-1'). Only applicable if model is 'aws'. Default is 'us-east-1'.
-    job_name : str, optional
-        The name of the transcription job. Only applicable if model is 'aws'. Default is 'transcribe_job_01'.
     transcribe_interval : list, optional
         A list of tuples representing the start and end times (in seconds) of segments of the audio file to be transcribed.
         Only applicable if model is 'vosk'. Default is an empty list.
 
     Returns:
     ...........
     json_response : JSON Object
@@ -261,19 +255,11 @@
     transcript : str
         The transcript of the recording.
 
     ------------------------------------------------------------------------------------------------------
     """
     model = kwargs.get('model', 'vosk')
     language = kwargs.get('language', 'en-us')
-
-    region = kwargs.get('region', 'us-east-1')
-    job_name = kwargs.get('job_name', 'transcribe_job_01')
     transcribe_interval = kwargs.get('transcribe_interval', [])
 
-    if model.lower() == 'aws':
-        json_response, transcript = aws.transcribe_audio(filepath, region, job_name, language)
-
-    else:
-        json_response, transcript = run_vosk(filepath, language, transcribe_interval)
-
+    json_response, transcript = run_vosk(filepath, language, transcribe_interval)
     return json_response, transcript
```

### Comparing `openwillis-1.1/openwillis/features/video/face_landmark.py` & `openwillis-1.2/openwillis/measures/video/face_landmark.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.1/openwillis/features/video/facial_emotion.py` & `openwillis-1.2/openwillis/measures/video/facial_emotion.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.1/openwillis.egg-info/PKG-INFO` & `openwillis-1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 1.1
+Version: 1.2
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Openwillis is a python library for digital measurement of health.
+OpenWillis is a python library for digital health measurement.
 
-It was developed by Brooklyn Health to establish standardized methods in digital measurement.
+It was developed by [Brooklyn Health](https://www.bklynhlth.com/openwillis) to establish standardized methods in digital phenotyping and make them open and accessible to the scientific community.
 
-It is free for non-commercial use ([see license](https://github.com/bklynhlth/openwillis/blob/main/LICENSE.txt)).
+It is freely available for non-commercial use ([see license](https://github.com/bklynhlth/openwillis/blob/main/LICENSE.txt)).
 
-* [Official website](https://www.bklynhlth.com/openwillis)
-* [Documentation](https://github.com/bklynhlth/openwillis/wiki)
-* [Getting started](https://github.com/bklynhlth/openwillis/wiki/1.-Getting-started)
-* [List of functions](https://github.com/bklynhlth/openwillis/wiki/2.-List-of-functions)
-* [Research guidelines](https://github.com/bklynhlth/openwillis/wiki/3.-Research-guidelines)
 
-Please report any issues using the [Issues](https://github.com/bklynhlth/openwillis/issues) tab or get in touch through openwillis@bklynhlth.com.
+
+1. [Release notes](https://github.com/bklynhlth/openwillis/wiki/Release-notes)
+2. [Getting started](https://github.com/bklynhlth/openwillis/wiki/Getting-started)
+3. [List of functions](https://github.com/bklynhlth/openwillis/wiki/List-of-functions)
+4. [Research guidelines](https://github.com/bklynhlth/openwillis/wiki/Research-guidelines)
+
+Please report any issues using the [Issues](https://github.com/bklynhlth/openwillis/issues) tab.
+
+If you’d like to contribute to OpenWillis or have general questions, please [get in touch](mailto:openwillis@brooklyn.health).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openwillis-1.1/setup.py` & `openwillis-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='1.1',
+                 version='1.2',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
                  python_requires='>=3.6',
                  install_requires=install_requires,
```

